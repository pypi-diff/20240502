# Comparing `tmp/finbourne_access_sdk-2.1.8.tar.gz` & `tmp/finbourne_access_sdk-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finbourne_access_sdk-2.1.8.tar", max compression
+gzip compressed data, was "finbourne_access_sdk-2.1.9.tar", max compression
```

## Comparing `finbourne_access_sdk-2.1.8.tar` & `finbourne_access_sdk-2.1.9.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0    17778 2024-04-12 15:53:36.673940 finbourne_access_sdk-2.1.8/README.md
--rw-r--r--   0        0        0    10462 2024-04-12 15:53:36.655940 finbourne_access_sdk-2.1.8/finbourne_access/__init__.py
--rw-r--r--   0        0        0      498 2024-04-12 15:53:36.655940 finbourne_access_sdk-2.1.8/finbourne_access/api/__init__.py
--rw-r--r--   0        0        0     7551 2024-04-12 15:53:36.654940 finbourne_access_sdk-2.1.8/finbourne_access/api/application_metadata_api.py
--rw-r--r--   0        0        0   160687 2024-04-12 15:53:36.655940 finbourne_access_sdk-2.1.8/finbourne_access/api/policies_api.py
--rw-r--r--   0        0        0    55454 2024-04-12 15:53:36.655940 finbourne_access_sdk-2.1.8/finbourne_access/api/policy_templates_api.py
--rw-r--r--   0        0        0    68286 2024-04-12 15:53:36.655940 finbourne_access_sdk-2.1.8/finbourne_access/api/roles_api.py
--rw-r--r--   0        0        0    76101 2024-04-12 15:53:36.655940 finbourne_access_sdk-2.1.8/finbourne_access/api/user_roles_api.py
--rw-r--r--   0        0        0    30808 2024-04-12 15:53:36.665940 finbourne_access_sdk-2.1.8/finbourne_access/api_client.py
--rw-r--r--   0        0        0      852 2024-04-12 15:53:36.665940 finbourne_access_sdk-2.1.8/finbourne_access/api_response.py
--rw-r--r--   0        0        0    14461 2024-04-12 15:53:36.655940 finbourne_access_sdk-2.1.8/finbourne_access/configuration.py
--rw-r--r--   0        0        0     5348 2024-04-12 15:53:36.655940 finbourne_access_sdk-2.1.8/finbourne_access/exceptions.py
--rw-r--r--   0        0        0      593 2024-04-12 15:53:36.665940 finbourne_access_sdk-2.1.8/finbourne_access/extensions/__init__.py
--rw-r--r--   0        0        0    30677 2024-04-12 15:53:36.665940 finbourne_access_sdk-2.1.8/finbourne_access/extensions/api_client.py
--rw-r--r--   0        0        0     9882 2024-04-12 15:53:36.665940 finbourne_access_sdk-2.1.8/finbourne_access/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8107 2024-04-12 15:53:36.665940 finbourne_access_sdk-2.1.8/finbourne_access/extensions/api_configuration.py
--rw-r--r--   0        0        0     6804 2024-04-12 15:53:36.665940 finbourne_access_sdk-2.1.8/finbourne_access/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-04-12 15:53:36.665940 finbourne_access_sdk-2.1.8/finbourne_access/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-04-12 15:53:36.665940 finbourne_access_sdk-2.1.8/finbourne_access/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12709 2024-04-12 15:53:36.666940 finbourne_access_sdk-2.1.8/finbourne_access/extensions/rest.py
--rw-r--r--   0        0        0    11575 2024-04-12 15:53:36.665940 finbourne_access_sdk-2.1.8/finbourne_access/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-04-12 15:53:36.666940 finbourne_access_sdk-2.1.8/finbourne_access/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3888 2024-04-12 15:53:36.666940 finbourne_access_sdk-2.1.8/finbourne_access/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     8919 2024-04-12 15:53:36.654940 finbourne_access_sdk-2.1.8/finbourne_access/models/__init__.py
--rw-r--r--   0        0        0     3918 2024-04-12 15:53:36.644940 finbourne_access_sdk-2.1.8/finbourne_access/models/access_controlled_action.py
--rw-r--r--   0        0        0     4861 2024-04-12 15:53:36.644940 finbourne_access_sdk-2.1.8/finbourne_access/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2079 2024-04-12 15:53:36.644940 finbourne_access_sdk-2.1.8/finbourne_access/models/action_id.py
--rw-r--r--   0        0        0     2705 2024-04-12 15:53:36.644940 finbourne_access_sdk-2.1.8/finbourne_access/models/add_policy_collection_to_role_request.py
--rw-r--r--   0        0        0     2461 2024-04-12 15:53:36.644940 finbourne_access_sdk-2.1.8/finbourne_access/models/add_policy_to_role_request.py
--rw-r--r--   0        0        0     3823 2024-04-12 15:53:36.644940 finbourne_access_sdk-2.1.8/finbourne_access/models/add_to_policy_collection_request.py
--rw-r--r--   0        0        0     2563 2024-04-12 15:53:36.645940 finbourne_access_sdk-2.1.8/finbourne_access/models/as_at_predicate_contract.py
--rw-r--r--   0        0        0     2488 2024-04-12 15:53:36.645940 finbourne_access_sdk-2.1.8/finbourne_access/models/as_at_range_for_spec.py
--rw-r--r--   0        0        0     2466 2024-04-12 15:53:36.645940 finbourne_access_sdk-2.1.8/finbourne_access/models/as_at_relative.py
--rw-r--r--   0        0        0     6888 2024-04-12 15:53:36.645940 finbourne_access_sdk-2.1.8/finbourne_access/models/attached_policy_definition_response.py
--rw-r--r--   0        0        0     1096 2024-04-12 15:53:36.645940 finbourne_access_sdk-2.1.8/finbourne_access/models/date_quality.py
--rw-r--r--   0        0        0      781 2024-04-12 15:53:36.645940 finbourne_access_sdk-2.1.8/finbourne_access/models/date_unit.py
--rw-r--r--   0        0        0     1971 2024-04-12 15:53:36.645940 finbourne_access_sdk-2.1.8/finbourne_access/models/effective_date_has_quality.py
--rw-r--r--   0        0        0     2538 2024-04-12 15:53:36.645940 finbourne_access_sdk-2.1.8/finbourne_access/models/effective_date_relative.py
--rw-r--r--   0        0        0     2148 2024-04-12 15:53:36.645940 finbourne_access_sdk-2.1.8/finbourne_access/models/effective_range.py
--rw-r--r--   0        0        0     2387 2024-04-12 15:53:36.645940 finbourne_access_sdk-2.1.8/finbourne_access/models/entitlement_metadata.py
--rw-r--r--   0        0        0     2625 2024-04-12 15:53:36.645940 finbourne_access_sdk-2.1.8/finbourne_access/models/evaluation_request.py
--rw-r--r--   0        0        0     2473 2024-04-12 15:53:36.645940 finbourne_access_sdk-2.1.8/finbourne_access/models/evaluation_response.py
--rw-r--r--   0        0        0      766 2024-04-12 15:53:36.645940 finbourne_access_sdk-2.1.8/finbourne_access/models/evaluation_result.py
--rw-r--r--   0        0        0     4459 2024-04-12 15:53:36.645940 finbourne_access_sdk-2.1.8/finbourne_access/models/for_spec.py
--rw-r--r--   0        0        0     3649 2024-04-12 15:53:36.646941 finbourne_access_sdk-2.1.8/finbourne_access/models/generate_policy_from_template_request.py
--rw-r--r--   0        0        0     3731 2024-04-12 15:53:36.646941 finbourne_access_sdk-2.1.8/finbourne_access/models/generated_policy_components.py
--rw-r--r--   0        0        0      654 2024-04-12 15:53:36.646941 finbourne_access_sdk-2.1.8/finbourne_access/models/grant.py
--rw-r--r--   0        0        0     2867 2024-04-12 15:53:36.646941 finbourne_access_sdk-2.1.8/finbourne_access/models/how_spec.py
--rw-r--r--   0        0        0     3191 2024-04-12 15:53:36.646941 finbourne_access_sdk-2.1.8/finbourne_access/models/id_selector_definition.py
--rw-r--r--   0        0        0     3116 2024-04-12 15:53:36.646941 finbourne_access_sdk-2.1.8/finbourne_access/models/identifier_part_schema.py
--rw-r--r--   0        0        0     4383 2024-04-12 15:53:36.646941 finbourne_access_sdk-2.1.8/finbourne_access/models/if_expression.py
--rw-r--r--   0        0        0     2435 2024-04-12 15:53:36.646941 finbourne_access_sdk-2.1.8/finbourne_access/models/if_feature_chain_expression.py
--rw-r--r--   0        0        0     3651 2024-04-12 15:53:36.646941 finbourne_access_sdk-2.1.8/finbourne_access/models/if_identity_claim_expression.py
--rw-r--r--   0        0        0     2325 2024-04-12 15:53:36.647940 finbourne_access_sdk-2.1.8/finbourne_access/models/if_identity_scope_expression.py
--rw-r--r--   0        0        0     2496 2024-04-12 15:53:36.647940 finbourne_access_sdk-2.1.8/finbourne_access/models/if_request_header_expression.py
--rw-r--r--   0        0        0     2419 2024-04-12 15:53:36.647940 finbourne_access_sdk-2.1.8/finbourne_access/models/key_value_pair_of_string_to_string.py
--rw-r--r--   0        0        0     2271 2024-04-12 15:53:36.647940 finbourne_access_sdk-2.1.8/finbourne_access/models/link.py
--rw-r--r--   0        0        0     3866 2024-04-12 15:53:36.647940 finbourne_access_sdk-2.1.8/finbourne_access/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4702 2024-04-12 15:53:36.647940 finbourne_access_sdk-2.1.8/finbourne_access/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3115 2024-04-12 15:53:36.647940 finbourne_access_sdk-2.1.8/finbourne_access/models/match_all_selector_definition.py
--rw-r--r--   0        0        0     2448 2024-04-12 15:53:36.647940 finbourne_access_sdk-2.1.8/finbourne_access/models/metadata_expression.py
--rw-r--r--   0        0        0     3747 2024-04-12 15:53:36.647940 finbourne_access_sdk-2.1.8/finbourne_access/models/metadata_selector_definition.py
--rw-r--r--   0        0        0     2048 2024-04-12 15:53:36.647940 finbourne_access_sdk-2.1.8/finbourne_access/models/non_transitive_supervisor_role_resource.py
--rw-r--r--   0        0        0      847 2024-04-12 15:53:36.647940 finbourne_access_sdk-2.1.8/finbourne_access/models/operator.py
--rw-r--r--   0        0        0      995 2024-04-12 15:53:36.647940 finbourne_access_sdk-2.1.8/finbourne_access/models/point_in_time_specification.py
--rw-r--r--   0        0        0     6049 2024-04-12 15:53:36.647940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_collection_creation_request.py
--rw-r--r--   0        0        0     2945 2024-04-12 15:53:36.647940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_collection_id.py
--rw-r--r--   0        0        0     5205 2024-04-12 15:53:36.651940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_collection_response.py
--rw-r--r--   0        0        0     5467 2024-04-12 15:53:36.651940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_collection_update_request.py
--rw-r--r--   0        0        0     6884 2024-04-12 15:53:36.651940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_creation_request.py
--rw-r--r--   0        0        0     2865 2024-04-12 15:53:36.651940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_id.py
--rw-r--r--   0        0        0     3546 2024-04-12 15:53:36.652940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_id_role_resource.py
--rw-r--r--   0        0        0     7551 2024-04-12 15:53:36.652940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_response.py
--rw-r--r--   0        0        0     4492 2024-04-12 15:53:36.652940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_selector_definition.py
--rw-r--r--   0        0        0     3686 2024-04-12 15:53:36.652940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_template_creation_request.py
--rw-r--r--   0        0        0     5276 2024-04-12 15:53:36.652940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_template_response.py
--rw-r--r--   0        0        0     3153 2024-04-12 15:53:36.652940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_template_update_request.py
--rw-r--r--   0        0        0     2647 2024-04-12 15:53:36.652940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_templated_selector.py
--rw-r--r--   0        0        0      697 2024-04-12 15:53:36.652940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_type.py
--rw-r--r--   0        0        0     6364 2024-04-12 15:53:36.652940 finbourne_access_sdk-2.1.8/finbourne_access/models/policy_update_request.py
--rw-r--r--   0        0        0      829 2024-04-12 15:53:36.652940 finbourne_access_sdk-2.1.8/finbourne_access/models/relative_to_date_time.py
--rw-r--r--   0        0        0     3866 2024-04-12 15:53:36.652940 finbourne_access_sdk-2.1.8/finbourne_access/models/remove_from_policy_collection_request.py
--rw-r--r--   0        0        0     4251 2024-04-12 15:53:36.652940 finbourne_access_sdk-2.1.8/finbourne_access/models/request_details.py
--rw-r--r--   0        0        0     3119 2024-04-12 15:53:36.653940 finbourne_access_sdk-2.1.8/finbourne_access/models/requested_action_key.py
--rw-r--r--   0        0        0     3222 2024-04-12 15:53:36.653940 finbourne_access_sdk-2.1.8/finbourne_access/models/resource_details.py
--rw-r--r--   0        0        0     4268 2024-04-12 15:53:36.653940 finbourne_access_sdk-2.1.8/finbourne_access/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4268 2024-04-12 15:53:36.653940 finbourne_access_sdk-2.1.8/finbourne_access/models/resource_list_of_policy_collection_response.py
--rw-r--r--   0        0        0     4147 2024-04-12 15:53:36.653940 finbourne_access_sdk-2.1.8/finbourne_access/models/resource_list_of_policy_response.py
--rw-r--r--   0        0        0     4244 2024-04-12 15:53:36.653940 finbourne_access_sdk-2.1.8/finbourne_access/models/resource_list_of_policy_template_response.py
--rw-r--r--   0        0        0     4172 2024-04-12 15:53:36.653940 finbourne_access_sdk-2.1.8/finbourne_access/models/resource_list_of_user_role_response.py
--rw-r--r--   0        0        0     3486 2024-04-12 15:53:36.653940 finbourne_access_sdk-2.1.8/finbourne_access/models/role_creation_request.py
--rw-r--r--   0        0        0     2849 2024-04-12 15:53:36.653940 finbourne_access_sdk-2.1.8/finbourne_access/models/role_id.py
--rw-r--r--   0        0        0     3211 2024-04-12 15:53:36.653940 finbourne_access_sdk-2.1.8/finbourne_access/models/role_resource_request.py
--rw-r--r--   0        0        0     4782 2024-04-12 15:53:36.653940 finbourne_access_sdk-2.1.8/finbourne_access/models/role_response.py
--rw-r--r--   0        0        0     3024 2024-04-12 15:53:36.653940 finbourne_access_sdk-2.1.8/finbourne_access/models/role_update_request.py
--rw-r--r--   0        0        0     4283 2024-04-12 15:53:36.654940 finbourne_access_sdk-2.1.8/finbourne_access/models/selector_definition.py
--rw-r--r--   0        0        0     3123 2024-04-12 15:53:36.654940 finbourne_access_sdk-2.1.8/finbourne_access/models/template_metadata.py
--rw-r--r--   0        0        0     3415 2024-04-12 15:53:36.654940 finbourne_access_sdk-2.1.8/finbourne_access/models/template_selection.py
--rw-r--r--   0        0        0     1071 2024-04-12 15:53:36.654940 finbourne_access_sdk-2.1.8/finbourne_access/models/text_operator.py
--rw-r--r--   0        0        0     2816 2024-04-12 15:53:36.654940 finbourne_access_sdk-2.1.8/finbourne_access/models/user_role_creation_request.py
--rw-r--r--   0        0        0     3274 2024-04-12 15:53:36.654940 finbourne_access_sdk-2.1.8/finbourne_access/models/user_role_response.py
--rw-r--r--   0        0        0     2262 2024-04-12 15:53:36.654940 finbourne_access_sdk-2.1.8/finbourne_access/models/user_role_update_request.py
--rw-r--r--   0        0        0     2147 2024-04-12 15:53:36.654940 finbourne_access_sdk-2.1.8/finbourne_access/models/when_spec.py
--rw-r--r--   0        0        0        0 2024-04-12 15:53:36.655940 finbourne_access_sdk-2.1.8/finbourne_access/py.typed
--rw-r--r--   0        0        0    10171 2024-04-12 15:53:36.665940 finbourne_access_sdk-2.1.8/finbourne_access/rest.py
--rw-r--r--   0        0        0      889 2024-04-12 15:53:36.673940 finbourne_access_sdk-2.1.8/pyproject.toml
--rw-r--r--   0        0        0    18861 1970-01-01 00:00:00.000000 finbourne_access_sdk-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0    17313 2024-04-15 09:49:10.170837 finbourne_access_sdk-2.1.9/README.md
+-rw-r--r--   0        0        0    10462 2024-04-15 09:49:10.164837 finbourne_access_sdk-2.1.9/finbourne_access/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-15 09:49:10.164837 finbourne_access_sdk-2.1.9/finbourne_access/api/__init__.py
+-rw-r--r--   0        0        0     7521 2024-04-15 09:49:10.163837 finbourne_access_sdk-2.1.9/finbourne_access/api/application_metadata_api.py
+-rw-r--r--   0        0        0   160297 2024-04-15 09:49:10.163837 finbourne_access_sdk-2.1.9/finbourne_access/api/policies_api.py
+-rw-r--r--   0        0        0    55454 2024-04-15 09:49:10.163837 finbourne_access_sdk-2.1.9/finbourne_access/api/policy_templates_api.py
+-rw-r--r--   0        0        0    68076 2024-04-15 09:49:10.164837 finbourne_access_sdk-2.1.9/finbourne_access/api/roles_api.py
+-rw-r--r--   0        0        0    75831 2024-04-15 09:49:10.164837 finbourne_access_sdk-2.1.9/finbourne_access/api/user_roles_api.py
+-rw-r--r--   0        0        0    30808 2024-04-15 09:49:10.164837 finbourne_access_sdk-2.1.9/finbourne_access/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-15 09:49:10.164837 finbourne_access_sdk-2.1.9/finbourne_access/api_response.py
+-rw-r--r--   0        0        0    14461 2024-04-15 09:49:10.164837 finbourne_access_sdk-2.1.9/finbourne_access/configuration.py
+-rw-r--r--   0        0        0     5348 2024-04-15 09:49:10.164837 finbourne_access_sdk-2.1.9/finbourne_access/exceptions.py
+-rw-r--r--   0        0        0      593 2024-04-15 09:49:10.165837 finbourne_access_sdk-2.1.9/finbourne_access/extensions/__init__.py
+-rw-r--r--   0        0        0    30677 2024-04-15 09:49:10.165837 finbourne_access_sdk-2.1.9/finbourne_access/extensions/api_client.py
+-rw-r--r--   0        0        0     9882 2024-04-15 09:49:10.165837 finbourne_access_sdk-2.1.9/finbourne_access/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8107 2024-04-15 09:49:10.165837 finbourne_access_sdk-2.1.9/finbourne_access/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6804 2024-04-15 09:49:10.165837 finbourne_access_sdk-2.1.9/finbourne_access/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-15 09:49:10.165837 finbourne_access_sdk-2.1.9/finbourne_access/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-15 09:49:10.165837 finbourne_access_sdk-2.1.9/finbourne_access/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12709 2024-04-15 09:49:10.165837 finbourne_access_sdk-2.1.9/finbourne_access/extensions/rest.py
+-rw-r--r--   0        0        0    11575 2024-04-15 09:49:10.165837 finbourne_access_sdk-2.1.9/finbourne_access/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-15 09:49:10.165837 finbourne_access_sdk-2.1.9/finbourne_access/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3888 2024-04-15 09:49:10.165837 finbourne_access_sdk-2.1.9/finbourne_access/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     8919 2024-04-15 09:49:10.163837 finbourne_access_sdk-2.1.9/finbourne_access/models/__init__.py
+-rw-r--r--   0        0        0     3918 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4861 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2079 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/action_id.py
+-rw-r--r--   0        0        0     2705 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/add_policy_collection_to_role_request.py
+-rw-r--r--   0        0        0     2461 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/add_policy_to_role_request.py
+-rw-r--r--   0        0        0     3823 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/add_to_policy_collection_request.py
+-rw-r--r--   0        0        0     2563 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/as_at_predicate_contract.py
+-rw-r--r--   0        0        0     2488 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/as_at_range_for_spec.py
+-rw-r--r--   0        0        0     2466 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/as_at_relative.py
+-rw-r--r--   0        0        0     6888 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/attached_policy_definition_response.py
+-rw-r--r--   0        0        0     1096 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/date_quality.py
+-rw-r--r--   0        0        0      781 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/date_unit.py
+-rw-r--r--   0        0        0     1971 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/effective_date_has_quality.py
+-rw-r--r--   0        0        0     2538 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/effective_date_relative.py
+-rw-r--r--   0        0        0     2148 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/effective_range.py
+-rw-r--r--   0        0        0     2387 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/entitlement_metadata.py
+-rw-r--r--   0        0        0     2625 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/evaluation_request.py
+-rw-r--r--   0        0        0     2473 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/evaluation_response.py
+-rw-r--r--   0        0        0      766 2024-04-15 09:49:10.159837 finbourne_access_sdk-2.1.9/finbourne_access/models/evaluation_result.py
+-rw-r--r--   0        0        0     4459 2024-04-15 09:49:10.160837 finbourne_access_sdk-2.1.9/finbourne_access/models/for_spec.py
+-rw-r--r--   0        0        0     3649 2024-04-15 09:49:10.160837 finbourne_access_sdk-2.1.9/finbourne_access/models/generate_policy_from_template_request.py
+-rw-r--r--   0        0        0     3731 2024-04-15 09:49:10.160837 finbourne_access_sdk-2.1.9/finbourne_access/models/generated_policy_components.py
+-rw-r--r--   0        0        0      654 2024-04-15 09:49:10.160837 finbourne_access_sdk-2.1.9/finbourne_access/models/grant.py
+-rw-r--r--   0        0        0     2867 2024-04-15 09:49:10.160837 finbourne_access_sdk-2.1.9/finbourne_access/models/how_spec.py
+-rw-r--r--   0        0        0     3191 2024-04-15 09:49:10.160837 finbourne_access_sdk-2.1.9/finbourne_access/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3116 2024-04-15 09:49:10.160837 finbourne_access_sdk-2.1.9/finbourne_access/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     4383 2024-04-15 09:49:10.160837 finbourne_access_sdk-2.1.9/finbourne_access/models/if_expression.py
+-rw-r--r--   0        0        0     2435 2024-04-15 09:49:10.160837 finbourne_access_sdk-2.1.9/finbourne_access/models/if_feature_chain_expression.py
+-rw-r--r--   0        0        0     3651 2024-04-15 09:49:10.160837 finbourne_access_sdk-2.1.9/finbourne_access/models/if_identity_claim_expression.py
+-rw-r--r--   0        0        0     2325 2024-04-15 09:49:10.160837 finbourne_access_sdk-2.1.9/finbourne_access/models/if_identity_scope_expression.py
+-rw-r--r--   0        0        0     2496 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/if_request_header_expression.py
+-rw-r--r--   0        0        0     2419 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/key_value_pair_of_string_to_string.py
+-rw-r--r--   0        0        0     2271 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/link.py
+-rw-r--r--   0        0        0     3866 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4702 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3115 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/match_all_selector_definition.py
+-rw-r--r--   0        0        0     2448 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/metadata_expression.py
+-rw-r--r--   0        0        0     3747 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/metadata_selector_definition.py
+-rw-r--r--   0        0        0     2048 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/non_transitive_supervisor_role_resource.py
+-rw-r--r--   0        0        0      847 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/operator.py
+-rw-r--r--   0        0        0      995 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/point_in_time_specification.py
+-rw-r--r--   0        0        0     6049 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_collection_creation_request.py
+-rw-r--r--   0        0        0     2945 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_collection_id.py
+-rw-r--r--   0        0        0     5205 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_collection_response.py
+-rw-r--r--   0        0        0     5467 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_collection_update_request.py
+-rw-r--r--   0        0        0     6884 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_creation_request.py
+-rw-r--r--   0        0        0     2865 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_id.py
+-rw-r--r--   0        0        0     3546 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_id_role_resource.py
+-rw-r--r--   0        0        0     7551 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_response.py
+-rw-r--r--   0        0        0     4492 2024-04-15 09:49:10.161837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_selector_definition.py
+-rw-r--r--   0        0        0     3686 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_template_creation_request.py
+-rw-r--r--   0        0        0     5276 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_template_response.py
+-rw-r--r--   0        0        0     3153 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_template_update_request.py
+-rw-r--r--   0        0        0     2647 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_templated_selector.py
+-rw-r--r--   0        0        0      697 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_type.py
+-rw-r--r--   0        0        0     6364 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/policy_update_request.py
+-rw-r--r--   0        0        0      829 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/relative_to_date_time.py
+-rw-r--r--   0        0        0     3866 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/remove_from_policy_collection_request.py
+-rw-r--r--   0        0        0     4251 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/request_details.py
+-rw-r--r--   0        0        0     3119 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/requested_action_key.py
+-rw-r--r--   0        0        0     3222 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/resource_details.py
+-rw-r--r--   0        0        0     4268 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4268 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/resource_list_of_policy_collection_response.py
+-rw-r--r--   0        0        0     4147 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/resource_list_of_policy_response.py
+-rw-r--r--   0        0        0     4244 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/resource_list_of_policy_template_response.py
+-rw-r--r--   0        0        0     4172 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/resource_list_of_user_role_response.py
+-rw-r--r--   0        0        0     3486 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/role_creation_request.py
+-rw-r--r--   0        0        0     2849 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/role_id.py
+-rw-r--r--   0        0        0     3211 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/role_resource_request.py
+-rw-r--r--   0        0        0     4782 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/role_response.py
+-rw-r--r--   0        0        0     3024 2024-04-15 09:49:10.162837 finbourne_access_sdk-2.1.9/finbourne_access/models/role_update_request.py
+-rw-r--r--   0        0        0     4283 2024-04-15 09:49:10.163837 finbourne_access_sdk-2.1.9/finbourne_access/models/selector_definition.py
+-rw-r--r--   0        0        0     3123 2024-04-15 09:49:10.163837 finbourne_access_sdk-2.1.9/finbourne_access/models/template_metadata.py
+-rw-r--r--   0        0        0     3415 2024-04-15 09:49:10.163837 finbourne_access_sdk-2.1.9/finbourne_access/models/template_selection.py
+-rw-r--r--   0        0        0     1071 2024-04-15 09:49:10.163837 finbourne_access_sdk-2.1.9/finbourne_access/models/text_operator.py
+-rw-r--r--   0        0        0     2816 2024-04-15 09:49:10.163837 finbourne_access_sdk-2.1.9/finbourne_access/models/user_role_creation_request.py
+-rw-r--r--   0        0        0     3274 2024-04-15 09:49:10.163837 finbourne_access_sdk-2.1.9/finbourne_access/models/user_role_response.py
+-rw-r--r--   0        0        0     2262 2024-04-15 09:49:10.163837 finbourne_access_sdk-2.1.9/finbourne_access/models/user_role_update_request.py
+-rw-r--r--   0        0        0     2147 2024-04-15 09:49:10.163837 finbourne_access_sdk-2.1.9/finbourne_access/models/when_spec.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:49:10.164837 finbourne_access_sdk-2.1.9/finbourne_access/py.typed
+-rw-r--r--   0        0        0    10171 2024-04-15 09:49:10.164837 finbourne_access_sdk-2.1.9/finbourne_access/rest.py
+-rw-r--r--   0        0        0      889 2024-04-15 09:49:10.170837 finbourne_access_sdk-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0    18396 1970-01-01 00:00:00.000000 finbourne_access_sdk-2.1.9/PKG-INFO
```

### Comparing `finbourne_access_sdk-2.1.8/README.md` & `finbourne_access_sdk-2.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # finbourne-access-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.3774
-- Package version: 2.1.8
+- API version: 0.0.3775
+- Package version: 2.1.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -169,68 +169,68 @@
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
     api_instance = api_client_factory.build(ApplicationMetadataApi)
 
     try:
-        # [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
+        # ListAccessControlledResources: Get resources available for access control
         api_response = await api_instance.list_access_controlled_resources()
         print("The response of ApplicationMetadataApi->list_access_controlled_resources:\n")
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling ApplicationMetadataApi->list_access_controlled_resources: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://fbn-prd.lusid.com/access*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
-*PoliciesApi* | [**add_to_policy_collection**](docs/PoliciesApi.md#add_to_policy_collection) | **POST** /api/policycollections/{code}/add | [EARLY ACCESS] AddToPolicyCollection: Add To PolicyCollection
-*PoliciesApi* | [**create_policy**](docs/PoliciesApi.md#create_policy) | **POST** /api/policies | [EARLY ACCESS] CreatePolicy: Create Policy
-*PoliciesApi* | [**create_policy_collection**](docs/PoliciesApi.md#create_policy_collection) | **POST** /api/policycollections | [EARLY ACCESS] CreatePolicyCollection: Create PolicyCollection
-*PoliciesApi* | [**delete_policy**](docs/PoliciesApi.md#delete_policy) | **DELETE** /api/policies/{code} | [EARLY ACCESS] DeletePolicy: Delete Policy
-*PoliciesApi* | [**delete_policy_collection**](docs/PoliciesApi.md#delete_policy_collection) | **DELETE** /api/policycollections/{code} | [EARLY ACCESS] DeletePolicyCollection: Delete PolicyCollection
-*PoliciesApi* | [**evaluate**](docs/PoliciesApi.md#evaluate) | **POST** /api/me | [EARLY ACCESS] Evaluate: Run one or more evaluations
+*ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | ListAccessControlledResources: Get resources available for access control
+*PoliciesApi* | [**add_to_policy_collection**](docs/PoliciesApi.md#add_to_policy_collection) | **POST** /api/policycollections/{code}/add | AddToPolicyCollection: Add To PolicyCollection
+*PoliciesApi* | [**create_policy**](docs/PoliciesApi.md#create_policy) | **POST** /api/policies | CreatePolicy: Create Policy
+*PoliciesApi* | [**create_policy_collection**](docs/PoliciesApi.md#create_policy_collection) | **POST** /api/policycollections | CreatePolicyCollection: Create PolicyCollection
+*PoliciesApi* | [**delete_policy**](docs/PoliciesApi.md#delete_policy) | **DELETE** /api/policies/{code} | DeletePolicy: Delete Policy
+*PoliciesApi* | [**delete_policy_collection**](docs/PoliciesApi.md#delete_policy_collection) | **DELETE** /api/policycollections/{code} | DeletePolicyCollection: Delete PolicyCollection
+*PoliciesApi* | [**evaluate**](docs/PoliciesApi.md#evaluate) | **POST** /api/me | Evaluate: Run one or more evaluations
 *PoliciesApi* | [**get_own_policies**](docs/PoliciesApi.md#get_own_policies) | **GET** /api/me | GetOwnPolicies: Get policies of requesting user
-*PoliciesApi* | [**get_policy**](docs/PoliciesApi.md#get_policy) | **GET** /api/policies/{code} | [EARLY ACCESS] GetPolicy: Get Policy
-*PoliciesApi* | [**get_policy_collection**](docs/PoliciesApi.md#get_policy_collection) | **GET** /api/policycollections/{code} | [EARLY ACCESS] GetPolicyCollection: Get PolicyCollection
+*PoliciesApi* | [**get_policy**](docs/PoliciesApi.md#get_policy) | **GET** /api/policies/{code} | GetPolicy: Get Policy
+*PoliciesApi* | [**get_policy_collection**](docs/PoliciesApi.md#get_policy_collection) | **GET** /api/policycollections/{code} | GetPolicyCollection: Get PolicyCollection
 *PoliciesApi* | [**list_policies**](docs/PoliciesApi.md#list_policies) | **GET** /api/policies | [EARLY ACCESS] ListPolicies: List Policies
-*PoliciesApi* | [**list_policy_collections**](docs/PoliciesApi.md#list_policy_collections) | **GET** /api/policycollections | [EARLY ACCESS] ListPolicyCollections: List PolicyCollections
+*PoliciesApi* | [**list_policy_collections**](docs/PoliciesApi.md#list_policy_collections) | **GET** /api/policycollections | ListPolicyCollections: List PolicyCollections
 *PoliciesApi* | [**page_policies**](docs/PoliciesApi.md#page_policies) | **GET** /api/policies/page | [EARLY ACCESS] PagePolicies: Page Policies
-*PoliciesApi* | [**page_policy_collections**](docs/PoliciesApi.md#page_policy_collections) | **GET** /api/policycollections/page | [EARLY ACCESS] PagePolicyCollections: Page PolicyCollections
-*PoliciesApi* | [**remove_from_policy_collection**](docs/PoliciesApi.md#remove_from_policy_collection) | **POST** /api/policycollections/{code}/remove | [EARLY ACCESS] RemoveFromPolicyCollection: Remove From PolicyCollection
-*PoliciesApi* | [**update_policy**](docs/PoliciesApi.md#update_policy) | **PUT** /api/policies/{code} | [EARLY ACCESS] UpdatePolicy: Update Policy
-*PoliciesApi* | [**update_policy_collection**](docs/PoliciesApi.md#update_policy_collection) | **PUT** /api/policycollections/{code} | [EARLY ACCESS] UpdatePolicyCollection: Update PolicyCollection
+*PoliciesApi* | [**page_policy_collections**](docs/PoliciesApi.md#page_policy_collections) | **GET** /api/policycollections/page | PagePolicyCollections: Page PolicyCollections
+*PoliciesApi* | [**remove_from_policy_collection**](docs/PoliciesApi.md#remove_from_policy_collection) | **POST** /api/policycollections/{code}/remove | RemoveFromPolicyCollection: Remove From PolicyCollection
+*PoliciesApi* | [**update_policy**](docs/PoliciesApi.md#update_policy) | **PUT** /api/policies/{code} | UpdatePolicy: Update Policy
+*PoliciesApi* | [**update_policy_collection**](docs/PoliciesApi.md#update_policy_collection) | **PUT** /api/policycollections/{code} | UpdatePolicyCollection: Update PolicyCollection
 *PolicyTemplatesApi* | [**create_policy_template**](docs/PolicyTemplatesApi.md#create_policy_template) | **POST** /api/policytemplates | [EXPERIMENTAL] CreatePolicyTemplate: Create a Policy Template
 *PolicyTemplatesApi* | [**delete_policy_template**](docs/PolicyTemplatesApi.md#delete_policy_template) | **DELETE** /api/policytemplates/{code} | [EXPERIMENTAL] DeletePolicyTemplate: Deleting a policy template
 *PolicyTemplatesApi* | [**generate_policy_from_template**](docs/PolicyTemplatesApi.md#generate_policy_from_template) | **POST** /api/policytemplates/$generatepolicy | [EXPERIMENTAL] GeneratePolicyFromTemplate: Generate policy from template
 *PolicyTemplatesApi* | [**get_policy_template**](docs/PolicyTemplatesApi.md#get_policy_template) | **GET** /api/policytemplates/{code} | [EXPERIMENTAL] GetPolicyTemplate: Retrieving one Policy Template
 *PolicyTemplatesApi* | [**list_policy_templates**](docs/PolicyTemplatesApi.md#list_policy_templates) | **GET** /api/policytemplates | [EXPERIMENTAL] ListPolicyTemplates: List Policy Templates
 *PolicyTemplatesApi* | [**update_policy_template**](docs/PolicyTemplatesApi.md#update_policy_template) | **PUT** /api/policytemplates/{code} | [EXPERIMENTAL] UpdatePolicyTemplate: Update a Policy Template
-*RolesApi* | [**add_policy_collection_to_role**](docs/RolesApi.md#add_policy_collection_to_role) | **POST** /api/roles/{scope}/{code}/policycollections | [EARLY ACCESS] AddPolicyCollectionToRole: Add policy collections to a role
-*RolesApi* | [**create_role**](docs/RolesApi.md#create_role) | **POST** /api/roles | [EARLY ACCESS] CreateRole: Create Role
-*RolesApi* | [**delete_role**](docs/RolesApi.md#delete_role) | **DELETE** /api/roles/{code} | [EARLY ACCESS] DeleteRole: Delete Role
-*RolesApi* | [**get_role**](docs/RolesApi.md#get_role) | **GET** /api/roles/{code} | [EARLY ACCESS] GetRole: Get Role
-*RolesApi* | [**list_roles**](docs/RolesApi.md#list_roles) | **GET** /api/roles | [EARLY ACCESS] ListRoles: List Roles
-*RolesApi* | [**remove_policy_collection_from_role**](docs/RolesApi.md#remove_policy_collection_from_role) | **DELETE** /api/roles/{scope}/{code}/policycollections/{policycollectionscope}/{policycollectioncode} | [EARLY ACCESS] RemovePolicyCollectionFromRole: Remove policy collection from role
-*RolesApi* | [**update_role**](docs/RolesApi.md#update_role) | **PUT** /api/roles/{code} | [EARLY ACCESS] UpdateRole: Update Role
-*UserRolesApi* | [**add_policy_collection_to_user_role**](docs/UserRolesApi.md#add_policy_collection_to_user_role) | **POST** /api/userroles/{userid}/policycollections | [EXPERIMENTAL] AddPolicyCollectionToUserRole: Add a policy collection to a user-role
-*UserRolesApi* | [**add_policy_to_user_role**](docs/UserRolesApi.md#add_policy_to_user_role) | **POST** /api/userroles/{userid}/policies | [EXPERIMENTAL] AddPolicyToUserRole: Add a policy to a user-role
-*UserRolesApi* | [**create_user_role**](docs/UserRolesApi.md#create_user_role) | **POST** /api/userroles | [EXPERIMENTAL] CreateUserRole: Create a user-role
-*UserRolesApi* | [**delete_user_role**](docs/UserRolesApi.md#delete_user_role) | **DELETE** /api/userroles/{userid} | [EXPERIMENTAL] DeleteUserRole: Delete a user-role
-*UserRolesApi* | [**get_user_role**](docs/UserRolesApi.md#get_user_role) | **GET** /api/userroles/{userid} | [EXPERIMENTAL] GetUserRole: Get a user-role
-*UserRolesApi* | [**list_user_roles**](docs/UserRolesApi.md#list_user_roles) | **GET** /api/userroles | [EXPERIMENTAL] ListUserRoles: List user-roles
-*UserRolesApi* | [**remove_policy_collection_from_user_role**](docs/UserRolesApi.md#remove_policy_collection_from_user_role) | **DELETE** /api/userroles/{userid}/policycollections/{policyCollectionScope}/{policyCollectionCode} | [EXPERIMENTAL] RemovePolicyCollectionFromUserRole: Remove a policy collection from a user-role
-*UserRolesApi* | [**remove_policy_from_user_role**](docs/UserRolesApi.md#remove_policy_from_user_role) | **DELETE** /api/userroles/{userid}/policies/{policyScope}/{policyCode} | [EXPERIMENTAL] RemovePolicyFromUserRole: Remove a policy from a user-role
-*UserRolesApi* | [**update_user_role**](docs/UserRolesApi.md#update_user_role) | **POST** /api/userroles/{userid}/update | [EXPERIMENTAL] UpdateUserRole: Update a user-role
+*RolesApi* | [**add_policy_collection_to_role**](docs/RolesApi.md#add_policy_collection_to_role) | **POST** /api/roles/{scope}/{code}/policycollections | AddPolicyCollectionToRole: Add policy collections to a role
+*RolesApi* | [**create_role**](docs/RolesApi.md#create_role) | **POST** /api/roles | CreateRole: Create Role
+*RolesApi* | [**delete_role**](docs/RolesApi.md#delete_role) | **DELETE** /api/roles/{code} | DeleteRole: Delete Role
+*RolesApi* | [**get_role**](docs/RolesApi.md#get_role) | **GET** /api/roles/{code} | GetRole: Get Role
+*RolesApi* | [**list_roles**](docs/RolesApi.md#list_roles) | **GET** /api/roles | ListRoles: List Roles
+*RolesApi* | [**remove_policy_collection_from_role**](docs/RolesApi.md#remove_policy_collection_from_role) | **DELETE** /api/roles/{scope}/{code}/policycollections/{policycollectionscope}/{policycollectioncode} | RemovePolicyCollectionFromRole: Remove policy collection from role
+*RolesApi* | [**update_role**](docs/RolesApi.md#update_role) | **PUT** /api/roles/{code} | UpdateRole: Update Role
+*UserRolesApi* | [**add_policy_collection_to_user_role**](docs/UserRolesApi.md#add_policy_collection_to_user_role) | **POST** /api/userroles/{userid}/policycollections | AddPolicyCollectionToUserRole: Add a policy collection to a user-role
+*UserRolesApi* | [**add_policy_to_user_role**](docs/UserRolesApi.md#add_policy_to_user_role) | **POST** /api/userroles/{userid}/policies | AddPolicyToUserRole: Add a policy to a user-role
+*UserRolesApi* | [**create_user_role**](docs/UserRolesApi.md#create_user_role) | **POST** /api/userroles | CreateUserRole: Create a user-role
+*UserRolesApi* | [**delete_user_role**](docs/UserRolesApi.md#delete_user_role) | **DELETE** /api/userroles/{userid} | DeleteUserRole: Delete a user-role
+*UserRolesApi* | [**get_user_role**](docs/UserRolesApi.md#get_user_role) | **GET** /api/userroles/{userid} | GetUserRole: Get a user-role
+*UserRolesApi* | [**list_user_roles**](docs/UserRolesApi.md#list_user_roles) | **GET** /api/userroles | ListUserRoles: List user-roles
+*UserRolesApi* | [**remove_policy_collection_from_user_role**](docs/UserRolesApi.md#remove_policy_collection_from_user_role) | **DELETE** /api/userroles/{userid}/policycollections/{policyCollectionScope}/{policyCollectionCode} | RemovePolicyCollectionFromUserRole: Remove a policy collection from a user-role
+*UserRolesApi* | [**remove_policy_from_user_role**](docs/UserRolesApi.md#remove_policy_from_user_role) | **DELETE** /api/userroles/{userid}/policies/{policyScope}/{policyCode} | RemovePolicyFromUserRole: Remove a policy from a user-role
+*UserRolesApi* | [**update_user_role**](docs/UserRolesApi.md#update_user_role) | **POST** /api/userroles/{userid}/update | UpdateUserRole: Update a user-role
 
 
 ## Documentation For Models
 
  - [AccessControlledAction](docs/AccessControlledAction.md)
  - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionId](docs/ActionId.md)
```

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/__init__.py` & `finbourne_access_sdk-2.1.9/finbourne_access/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/api/application_metadata_api.py` & `finbourne_access_sdk-2.1.9/finbourne_access/api/application_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     @overload
     def list_access_controlled_resources(self, async_req: Optional[bool]=True, **kwargs) -> ResourceListOfAccessControlledResource:  # noqa: E501
         ...
 
     @validate_arguments
     def list_access_controlled_resources(self, async_req: Optional[bool]=None, **kwargs) -> Union[ResourceListOfAccessControlledResource, Awaitable[ResourceListOfAccessControlledResource]]:  # noqa: E501
-        """[EARLY ACCESS] ListAccessControlledResources: Get resources available for access control  # noqa: E501
+        """ListAccessControlledResources: Get resources available for access control  # noqa: E501
 
         Get the comprehensive set of resources that are available for access control  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_access_controlled_resources(async_req=True)
         >>> result = thread.get()
@@ -77,15 +77,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.list_access_controlled_resources_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
     def list_access_controlled_resources_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] ListAccessControlledResources: Get resources available for access control  # noqa: E501
+        """ListAccessControlledResources: Get resources available for access control  # noqa: E501
 
         Get the comprehensive set of resources that are available for access control  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_access_controlled_resources_with_http_info(async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/api/policies_api.py` & `finbourne_access_sdk-2.1.9/finbourne_access/api/policies_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     @overload
     def add_to_policy_collection(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], add_to_policy_collection_request : Annotated[AddToPolicyCollectionRequest, Field(..., description="Ids of the PolicyCollections and/or Policies to add to the PolicyCollection")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, async_req: Optional[bool]=True, **kwargs) -> PolicyCollectionResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def add_to_policy_collection(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], add_to_policy_collection_request : Annotated[AddToPolicyCollectionRequest, Field(..., description="Ids of the PolicyCollections and/or Policies to add to the PolicyCollection")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[PolicyCollectionResponse, Awaitable[PolicyCollectionResponse]]:  # noqa: E501
-        """[EARLY ACCESS] AddToPolicyCollection: Add To PolicyCollection  # noqa: E501
+        """AddToPolicyCollection: Add To PolicyCollection  # noqa: E501
 
         Add Policies and/or PolicyCollections to a PolicyCollection  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.add_to_policy_collection(code, add_to_policy_collection_request, scope, async_req=True)
         >>> result = thread.get()
@@ -102,15 +102,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.add_to_policy_collection_with_http_info(code, add_to_policy_collection_request, scope, **kwargs)  # noqa: E501
 
     @validate_arguments
     def add_to_policy_collection_with_http_info(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], add_to_policy_collection_request : Annotated[AddToPolicyCollectionRequest, Field(..., description="Ids of the PolicyCollections and/or Policies to add to the PolicyCollection")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] AddToPolicyCollection: Add To PolicyCollection  # noqa: E501
+        """AddToPolicyCollection: Add To PolicyCollection  # noqa: E501
 
         Add Policies and/or PolicyCollections to a PolicyCollection  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.add_to_policy_collection_with_http_info(code, add_to_policy_collection_request, scope, async_req=True)
         >>> result = thread.get()
@@ -240,15 +240,15 @@
 
     @overload
     def create_policy(self, policy_creation_request : Annotated[PolicyCreationRequest, Field(..., description="The definition of the Policy")], async_req: Optional[bool]=True, **kwargs) -> PolicyResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def create_policy(self, policy_creation_request : Annotated[PolicyCreationRequest, Field(..., description="The definition of the Policy")], async_req: Optional[bool]=None, **kwargs) -> Union[PolicyResponse, Awaitable[PolicyResponse]]:  # noqa: E501
-        """[EARLY ACCESS] CreatePolicy: Create Policy  # noqa: E501
+        """CreatePolicy: Create Policy  # noqa: E501
 
         Creates a Policy  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_policy(policy_creation_request, async_req=True)
         >>> result = thread.get()
@@ -272,15 +272,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.create_policy_with_http_info(policy_creation_request, **kwargs)  # noqa: E501
 
     @validate_arguments
     def create_policy_with_http_info(self, policy_creation_request : Annotated[PolicyCreationRequest, Field(..., description="The definition of the Policy")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] CreatePolicy: Create Policy  # noqa: E501
+        """CreatePolicy: Create Policy  # noqa: E501
 
         Creates a Policy  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_policy_with_http_info(policy_creation_request, async_req=True)
         >>> result = thread.get()
@@ -398,15 +398,15 @@
 
     @overload
     def create_policy_collection(self, policy_collection_creation_request : Annotated[PolicyCollectionCreationRequest, Field(..., description="The definition of the PolicyCollection")], async_req: Optional[bool]=True, **kwargs) -> PolicyCollectionResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def create_policy_collection(self, policy_collection_creation_request : Annotated[PolicyCollectionCreationRequest, Field(..., description="The definition of the PolicyCollection")], async_req: Optional[bool]=None, **kwargs) -> Union[PolicyCollectionResponse, Awaitable[PolicyCollectionResponse]]:  # noqa: E501
-        """[EARLY ACCESS] CreatePolicyCollection: Create PolicyCollection  # noqa: E501
+        """CreatePolicyCollection: Create PolicyCollection  # noqa: E501
 
         Creates a PolicyCollection  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_policy_collection(policy_collection_creation_request, async_req=True)
         >>> result = thread.get()
@@ -430,15 +430,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.create_policy_collection_with_http_info(policy_collection_creation_request, **kwargs)  # noqa: E501
 
     @validate_arguments
     def create_policy_collection_with_http_info(self, policy_collection_creation_request : Annotated[PolicyCollectionCreationRequest, Field(..., description="The definition of the PolicyCollection")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] CreatePolicyCollection: Create PolicyCollection  # noqa: E501
+        """CreatePolicyCollection: Create PolicyCollection  # noqa: E501
 
         Creates a PolicyCollection  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_policy_collection_with_http_info(policy_collection_creation_request, async_req=True)
         >>> result = thread.get()
@@ -556,15 +556,15 @@
 
     @overload
     def delete_policy(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Policy")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the Policy")] = None, async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def delete_policy(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Policy")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the Policy")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EARLY ACCESS] DeletePolicy: Delete Policy  # noqa: E501
+        """DeletePolicy: Delete Policy  # noqa: E501
 
         Deletes an identified Policy  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_policy(code, scope, async_req=True)
         >>> result = thread.get()
@@ -590,15 +590,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.delete_policy_with_http_info(code, scope, **kwargs)  # noqa: E501
 
     @validate_arguments
     def delete_policy_with_http_info(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Policy")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the Policy")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] DeletePolicy: Delete Policy  # noqa: E501
+        """DeletePolicy: Delete Policy  # noqa: E501
 
         Deletes an identified Policy  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_policy_with_http_info(code, scope, async_req=True)
         >>> result = thread.get()
@@ -712,15 +712,15 @@
 
     @overload
     def delete_policy_collection(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def delete_policy_collection(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EARLY ACCESS] DeletePolicyCollection: Delete PolicyCollection  # noqa: E501
+        """DeletePolicyCollection: Delete PolicyCollection  # noqa: E501
 
         Deletes an identified PolicyCollection  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_policy_collection(code, scope, async_req=True)
         >>> result = thread.get()
@@ -746,15 +746,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.delete_policy_collection_with_http_info(code, scope, **kwargs)  # noqa: E501
 
     @validate_arguments
     def delete_policy_collection_with_http_info(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] DeletePolicyCollection: Delete PolicyCollection  # noqa: E501
+        """DeletePolicyCollection: Delete PolicyCollection  # noqa: E501
 
         Deletes an identified PolicyCollection  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_policy_collection_with_http_info(code, scope, async_req=True)
         >>> result = thread.get()
@@ -868,15 +868,15 @@
 
     @overload
     def evaluate(self, request_body : Annotated[Dict[str, EvaluationRequest], Field(..., description="A dictionary of evaluations, keyed using any arbitrary correlation id (it will be returned with the response for that evaluation).")], applications : Annotated[Optional[conlist(StrictStr)], Field(description="Optional. The application type of the roles and policies to use when evaluating.")] = None, as_at : Annotated[Optional[datetime], Field(description="Optional. The requested AsAt date of the entitlements")] = None, async_req: Optional[bool]=True, **kwargs) -> Dict[str, EvaluationResponse]:  # noqa: E501
         ...
 
     @validate_arguments
     def evaluate(self, request_body : Annotated[Dict[str, EvaluationRequest], Field(..., description="A dictionary of evaluations, keyed using any arbitrary correlation id (it will be returned with the response for that evaluation).")], applications : Annotated[Optional[conlist(StrictStr)], Field(description="Optional. The application type of the roles and policies to use when evaluating.")] = None, as_at : Annotated[Optional[datetime], Field(description="Optional. The requested AsAt date of the entitlements")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[Dict[str, EvaluationResponse], Awaitable[Dict[str, EvaluationResponse]]]:  # noqa: E501
-        """[EARLY ACCESS] Evaluate: Run one or more evaluations  # noqa: E501
+        """Evaluate: Run one or more evaluations  # noqa: E501
 
         Given a dictionary of evaluation requests (keyed by any arbitrary correlation identifier), each will be evaluated according to the current user's policies (deduced from the provided OAuth token).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.evaluate(request_body, applications, as_at, async_req=True)
         >>> result = thread.get()
@@ -904,15 +904,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.evaluate_with_http_info(request_body, applications, as_at, **kwargs)  # noqa: E501
 
     @validate_arguments
     def evaluate_with_http_info(self, request_body : Annotated[Dict[str, EvaluationRequest], Field(..., description="A dictionary of evaluations, keyed using any arbitrary correlation id (it will be returned with the response for that evaluation).")], applications : Annotated[Optional[conlist(StrictStr)], Field(description="Optional. The application type of the roles and policies to use when evaluating.")] = None, as_at : Annotated[Optional[datetime], Field(description="Optional. The requested AsAt date of the entitlements")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] Evaluate: Run one or more evaluations  # noqa: E501
+        """Evaluate: Run one or more evaluations  # noqa: E501
 
         Given a dictionary of evaluation requests (keyed by any arbitrary correlation identifier), each will be evaluated according to the current user's policies (deduced from the provided OAuth token).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.evaluate_with_http_info(request_body, applications, as_at, async_req=True)
         >>> result = thread.get()
@@ -1242,15 +1242,15 @@
 
     @overload
     def get_policy(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Policy")], as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the Policy")] = None, async_req: Optional[bool]=True, **kwargs) -> PolicyResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def get_policy(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Policy")], as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the Policy")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[PolicyResponse, Awaitable[PolicyResponse]]:  # noqa: E501
-        """[EARLY ACCESS] GetPolicy: Get Policy  # noqa: E501
+        """GetPolicy: Get Policy  # noqa: E501
 
         Gets an identified Policy  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_policy(code, as_at, scope, async_req=True)
         >>> result = thread.get()
@@ -1278,15 +1278,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.get_policy_with_http_info(code, as_at, scope, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_policy_with_http_info(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Policy")], as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the Policy")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] GetPolicy: Get Policy  # noqa: E501
+        """GetPolicy: Get Policy  # noqa: E501
 
         Gets an identified Policy  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_policy_with_http_info(code, as_at, scope, async_req=True)
         >>> result = thread.get()
@@ -1412,15 +1412,15 @@
 
     @overload
     def get_policy_collection(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, async_req: Optional[bool]=True, **kwargs) -> PolicyCollectionResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def get_policy_collection(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[PolicyCollectionResponse, Awaitable[PolicyCollectionResponse]]:  # noqa: E501
-        """[EARLY ACCESS] GetPolicyCollection: Get PolicyCollection  # noqa: E501
+        """GetPolicyCollection: Get PolicyCollection  # noqa: E501
 
         Gets an identified PolicyCollection  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_policy_collection(code, as_at, scope, async_req=True)
         >>> result = thread.get()
@@ -1448,15 +1448,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.get_policy_collection_with_http_info(code, as_at, scope, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_policy_collection_with_http_info(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] GetPolicyCollection: Get PolicyCollection  # noqa: E501
+        """GetPolicyCollection: Get PolicyCollection  # noqa: E501
 
         Gets an identified PolicyCollection  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_policy_collection_with_http_info(code, as_at, scope, async_req=True)
         >>> result = thread.get()
@@ -1777,15 +1777,15 @@
 
     @overload
     def list_policy_collections(self, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The requested scope")] = None, as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, sort_by : Annotated[Optional[conlist(StrictStr)], Field(description="Optional. Order the results by these fields. Use use the '-' sign to denote descending order e.g. -MyFieldName")] = None, start : Annotated[Optional[StrictInt], Field(description="Optional. When paginating, skip this number of results")] = None, limit : Annotated[Optional[StrictInt], Field(description="Optional. 2000 if not provided. When paginating, limit the number of returned results to this many.")] = None, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Optional. Expression to filter the result set")] = None, async_req: Optional[bool]=True, **kwargs) -> List[PolicyCollectionResponse]:  # noqa: E501
         ...
 
     @validate_arguments
     def list_policy_collections(self, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The requested scope")] = None, as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, sort_by : Annotated[Optional[conlist(StrictStr)], Field(description="Optional. Order the results by these fields. Use use the '-' sign to denote descending order e.g. -MyFieldName")] = None, start : Annotated[Optional[StrictInt], Field(description="Optional. When paginating, skip this number of results")] = None, limit : Annotated[Optional[StrictInt], Field(description="Optional. 2000 if not provided. When paginating, limit the number of returned results to this many.")] = None, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Optional. Expression to filter the result set")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[List[PolicyCollectionResponse], Awaitable[List[PolicyCollectionResponse]]]:  # noqa: E501
-        """[EARLY ACCESS] ListPolicyCollections: List PolicyCollections  # noqa: E501
+        """ListPolicyCollections: List PolicyCollections  # noqa: E501
 
         Gets all PolicyCollections in a scope. For pagination support, use PagePolicyCollections  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_policy_collections(scope, as_at, sort_by, start, limit, filter, async_req=True)
         >>> result = thread.get()
@@ -1819,15 +1819,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.list_policy_collections_with_http_info(scope, as_at, sort_by, start, limit, filter, **kwargs)  # noqa: E501
 
     @validate_arguments
     def list_policy_collections_with_http_info(self, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The requested scope")] = None, as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, sort_by : Annotated[Optional[conlist(StrictStr)], Field(description="Optional. Order the results by these fields. Use use the '-' sign to denote descending order e.g. -MyFieldName")] = None, start : Annotated[Optional[StrictInt], Field(description="Optional. When paginating, skip this number of results")] = None, limit : Annotated[Optional[StrictInt], Field(description="Optional. 2000 if not provided. When paginating, limit the number of returned results to this many.")] = None, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Optional. Expression to filter the result set")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] ListPolicyCollections: List PolicyCollections  # noqa: E501
+        """ListPolicyCollections: List PolicyCollections  # noqa: E501
 
         Gets all PolicyCollections in a scope. For pagination support, use PagePolicyCollections  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_policy_collections_with_http_info(scope, as_at, sort_by, start, limit, filter, async_req=True)
         >>> result = thread.get()
@@ -2158,15 +2158,15 @@
 
     @overload
     def page_policy_collections(self, as_at : Annotated[Optional[datetime], Field(description="Optional. Not currently used. The AsAt date time of the data")] = None, sort_by : Annotated[Optional[constr(strict=True, max_length=16384, min_length=1)], Field(description="Optional. Order the results by these fields. Use the '-' sign to denote descending order e.g. -MyFieldName")] = None, limit : Annotated[Optional[conint(strict=True, le=5000, ge=1)], Field(description="Optional. 2000 if not provided. When paginating, limit the number of returned results to this many")] = None, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Optional. Expression to filter the result set")] = None, page : Annotated[Optional[constr(strict=True, max_length=500, min_length=1)], Field(description="Optional. Paging token returned from a previous result")] = None, async_req: Optional[bool]=True, **kwargs) -> ResourceListOfPolicyCollectionResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def page_policy_collections(self, as_at : Annotated[Optional[datetime], Field(description="Optional. Not currently used. The AsAt date time of the data")] = None, sort_by : Annotated[Optional[constr(strict=True, max_length=16384, min_length=1)], Field(description="Optional. Order the results by these fields. Use the '-' sign to denote descending order e.g. -MyFieldName")] = None, limit : Annotated[Optional[conint(strict=True, le=5000, ge=1)], Field(description="Optional. 2000 if not provided. When paginating, limit the number of returned results to this many")] = None, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Optional. Expression to filter the result set")] = None, page : Annotated[Optional[constr(strict=True, max_length=500, min_length=1)], Field(description="Optional. Paging token returned from a previous result")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[ResourceListOfPolicyCollectionResponse, Awaitable[ResourceListOfPolicyCollectionResponse]]:  # noqa: E501
-        """[EARLY ACCESS] PagePolicyCollections: Page PolicyCollections  # noqa: E501
+        """PagePolicyCollections: Page PolicyCollections  # noqa: E501
 
         Gets all PolicyCollections with pagination support.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.page_policy_collections(as_at, sort_by, limit, filter, page, async_req=True)
         >>> result = thread.get()
@@ -2198,15 +2198,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.page_policy_collections_with_http_info(as_at, sort_by, limit, filter, page, **kwargs)  # noqa: E501
 
     @validate_arguments
     def page_policy_collections_with_http_info(self, as_at : Annotated[Optional[datetime], Field(description="Optional. Not currently used. The AsAt date time of the data")] = None, sort_by : Annotated[Optional[constr(strict=True, max_length=16384, min_length=1)], Field(description="Optional. Order the results by these fields. Use the '-' sign to denote descending order e.g. -MyFieldName")] = None, limit : Annotated[Optional[conint(strict=True, le=5000, ge=1)], Field(description="Optional. 2000 if not provided. When paginating, limit the number of returned results to this many")] = None, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Optional. Expression to filter the result set")] = None, page : Annotated[Optional[constr(strict=True, max_length=500, min_length=1)], Field(description="Optional. Paging token returned from a previous result")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] PagePolicyCollections: Page PolicyCollections  # noqa: E501
+        """PagePolicyCollections: Page PolicyCollections  # noqa: E501
 
         Gets all PolicyCollections with pagination support.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.page_policy_collections_with_http_info(as_at, sort_by, limit, filter, page, async_req=True)
         >>> result = thread.get()
@@ -2344,15 +2344,15 @@
 
     @overload
     def remove_from_policy_collection(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], remove_from_policy_collection_request : Annotated[RemoveFromPolicyCollectionRequest, Field(..., description="Ids of the PolicyCollections and/or Policies to remove from the PolicyCollection")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, async_req: Optional[bool]=True, **kwargs) -> PolicyCollectionResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def remove_from_policy_collection(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], remove_from_policy_collection_request : Annotated[RemoveFromPolicyCollectionRequest, Field(..., description="Ids of the PolicyCollections and/or Policies to remove from the PolicyCollection")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[PolicyCollectionResponse, Awaitable[PolicyCollectionResponse]]:  # noqa: E501
-        """[EARLY ACCESS] RemoveFromPolicyCollection: Remove From PolicyCollection  # noqa: E501
+        """RemoveFromPolicyCollection: Remove From PolicyCollection  # noqa: E501
 
         Remove Policies and/or PolicyCollections from a PolicyCollection  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.remove_from_policy_collection(code, remove_from_policy_collection_request, scope, async_req=True)
         >>> result = thread.get()
@@ -2380,15 +2380,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.remove_from_policy_collection_with_http_info(code, remove_from_policy_collection_request, scope, **kwargs)  # noqa: E501
 
     @validate_arguments
     def remove_from_policy_collection_with_http_info(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], remove_from_policy_collection_request : Annotated[RemoveFromPolicyCollectionRequest, Field(..., description="Ids of the PolicyCollections and/or Policies to remove from the PolicyCollection")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] RemoveFromPolicyCollection: Remove From PolicyCollection  # noqa: E501
+        """RemoveFromPolicyCollection: Remove From PolicyCollection  # noqa: E501
 
         Remove Policies and/or PolicyCollections from a PolicyCollection  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.remove_from_policy_collection_with_http_info(code, remove_from_policy_collection_request, scope, async_req=True)
         >>> result = thread.get()
@@ -2518,15 +2518,15 @@
 
     @overload
     def update_policy(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Policy")], policy_update_request : Annotated[PolicyUpdateRequest, Field(..., description="The updated definition of the Policy")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the Policy")] = None, async_req: Optional[bool]=True, **kwargs) -> PolicyResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def update_policy(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Policy")], policy_update_request : Annotated[PolicyUpdateRequest, Field(..., description="The updated definition of the Policy")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the Policy")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[PolicyResponse, Awaitable[PolicyResponse]]:  # noqa: E501
-        """[EARLY ACCESS] UpdatePolicy: Update Policy  # noqa: E501
+        """UpdatePolicy: Update Policy  # noqa: E501
 
         Updates a Policy  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_policy(code, policy_update_request, scope, async_req=True)
         >>> result = thread.get()
@@ -2554,15 +2554,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.update_policy_with_http_info(code, policy_update_request, scope, **kwargs)  # noqa: E501
 
     @validate_arguments
     def update_policy_with_http_info(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Policy")], policy_update_request : Annotated[PolicyUpdateRequest, Field(..., description="The updated definition of the Policy")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the Policy")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] UpdatePolicy: Update Policy  # noqa: E501
+        """UpdatePolicy: Update Policy  # noqa: E501
 
         Updates a Policy  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_policy_with_http_info(code, policy_update_request, scope, async_req=True)
         >>> result = thread.get()
@@ -2692,15 +2692,15 @@
 
     @overload
     def update_policy_collection(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], policy_collection_update_request : Annotated[PolicyCollectionUpdateRequest, Field(..., description="The updated definition of the PolicyCollection")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, async_req: Optional[bool]=True, **kwargs) -> PolicyCollectionResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def update_policy_collection(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], policy_collection_update_request : Annotated[PolicyCollectionUpdateRequest, Field(..., description="The updated definition of the PolicyCollection")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[PolicyCollectionResponse, Awaitable[PolicyCollectionResponse]]:  # noqa: E501
-        """[EARLY ACCESS] UpdatePolicyCollection: Update PolicyCollection  # noqa: E501
+        """UpdatePolicyCollection: Update PolicyCollection  # noqa: E501
 
         Updates a PolicyCollection  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_policy_collection(code, policy_collection_update_request, scope, async_req=True)
         >>> result = thread.get()
@@ -2728,15 +2728,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.update_policy_collection_with_http_info(code, policy_collection_update_request, scope, **kwargs)  # noqa: E501
 
     @validate_arguments
     def update_policy_collection_with_http_info(self, code : Annotated[constr(strict=True), Field(..., description="The code of the PolicyCollection")], policy_collection_update_request : Annotated[PolicyCollectionUpdateRequest, Field(..., description="The updated definition of the PolicyCollection")], scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use the default scope if not provided. The scope of the PolicyCollection")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] UpdatePolicyCollection: Update PolicyCollection  # noqa: E501
+        """UpdatePolicyCollection: Update PolicyCollection  # noqa: E501
 
         Updates a PolicyCollection  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_policy_collection_with_http_info(code, policy_collection_update_request, scope, async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/api/policy_templates_api.py` & `finbourne_access_sdk-2.1.9/finbourne_access/api/policy_templates_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/api/roles_api.py` & `finbourne_access_sdk-2.1.9/finbourne_access/api/roles_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     @overload
     def add_policy_collection_to_role(self, scope : Annotated[constr(strict=True), Field(..., description="The scope of the Role")], code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], add_policy_collection_to_role_request : Annotated[AddPolicyCollectionToRoleRequest, Field(..., description="The policy collections to add")], async_req: Optional[bool]=True, **kwargs) -> RoleResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def add_policy_collection_to_role(self, scope : Annotated[constr(strict=True), Field(..., description="The scope of the Role")], code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], add_policy_collection_to_role_request : Annotated[AddPolicyCollectionToRoleRequest, Field(..., description="The policy collections to add")], async_req: Optional[bool]=None, **kwargs) -> Union[RoleResponse, Awaitable[RoleResponse]]:  # noqa: E501
-        """[EARLY ACCESS] AddPolicyCollectionToRole: Add policy collections to a role  # noqa: E501
+        """AddPolicyCollectionToRole: Add policy collections to a role  # noqa: E501
 
         Assigns policy collections to a role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.add_policy_collection_to_role(scope, code, add_policy_collection_to_role_request, async_req=True)
         >>> result = thread.get()
@@ -93,15 +93,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.add_policy_collection_to_role_with_http_info(scope, code, add_policy_collection_to_role_request, **kwargs)  # noqa: E501
 
     @validate_arguments
     def add_policy_collection_to_role_with_http_info(self, scope : Annotated[constr(strict=True), Field(..., description="The scope of the Role")], code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], add_policy_collection_to_role_request : Annotated[AddPolicyCollectionToRoleRequest, Field(..., description="The policy collections to add")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] AddPolicyCollectionToRole: Add policy collections to a role  # noqa: E501
+        """AddPolicyCollectionToRole: Add policy collections to a role  # noqa: E501
 
         Assigns policy collections to a role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.add_policy_collection_to_role_with_http_info(scope, code, add_policy_collection_to_role_request, async_req=True)
         >>> result = thread.get()
@@ -231,15 +231,15 @@
 
     @overload
     def create_role(self, role_creation_request : Annotated[RoleCreationRequest, Field(..., description="The definition of the Role")], async_req: Optional[bool]=True, **kwargs) -> RoleResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def create_role(self, role_creation_request : Annotated[RoleCreationRequest, Field(..., description="The definition of the Role")], async_req: Optional[bool]=None, **kwargs) -> Union[RoleResponse, Awaitable[RoleResponse]]:  # noqa: E501
-        """[EARLY ACCESS] CreateRole: Create Role  # noqa: E501
+        """CreateRole: Create Role  # noqa: E501
 
         Creates a Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_role(role_creation_request, async_req=True)
         >>> result = thread.get()
@@ -263,15 +263,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.create_role_with_http_info(role_creation_request, **kwargs)  # noqa: E501
 
     @validate_arguments
     def create_role_with_http_info(self, role_creation_request : Annotated[RoleCreationRequest, Field(..., description="The definition of the Role")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] CreateRole: Create Role  # noqa: E501
+        """CreateRole: Create Role  # noqa: E501
 
         Creates a Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_role_with_http_info(role_creation_request, async_req=True)
         >>> result = thread.get()
@@ -389,15 +389,15 @@
 
     @overload
     def delete_role(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], scope : Annotated[Optional[constr(strict=True)], Field(description=">Optional. Will use default scope if not supplied. The scope of the Role")] = None, async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def delete_role(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], scope : Annotated[Optional[constr(strict=True)], Field(description=">Optional. Will use default scope if not supplied. The scope of the Role")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EARLY ACCESS] DeleteRole: Delete Role  # noqa: E501
+        """DeleteRole: Delete Role  # noqa: E501
 
         Deletes an identified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_role(code, scope, async_req=True)
         >>> result = thread.get()
@@ -423,15 +423,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.delete_role_with_http_info(code, scope, **kwargs)  # noqa: E501
 
     @validate_arguments
     def delete_role_with_http_info(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], scope : Annotated[Optional[constr(strict=True)], Field(description=">Optional. Will use default scope if not supplied. The scope of the Role")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] DeleteRole: Delete Role  # noqa: E501
+        """DeleteRole: Delete Role  # noqa: E501
 
         Deletes an identified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_role_with_http_info(code, scope, async_req=True)
         >>> result = thread.get()
@@ -545,15 +545,15 @@
 
     @overload
     def get_role(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use default scope if not supplied. The scope of the Role")] = None, async_req: Optional[bool]=True, **kwargs) -> RoleResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def get_role(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use default scope if not supplied. The scope of the Role")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[RoleResponse, Awaitable[RoleResponse]]:  # noqa: E501
-        """[EARLY ACCESS] GetRole: Get Role  # noqa: E501
+        """GetRole: Get Role  # noqa: E501
 
         Gets an identified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_role(code, as_at, scope, async_req=True)
         >>> result = thread.get()
@@ -581,15 +581,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.get_role_with_http_info(code, as_at, scope, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_role_with_http_info(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use default scope if not supplied. The scope of the Role")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] GetRole: Get Role  # noqa: E501
+        """GetRole: Get Role  # noqa: E501
 
         Gets an identified Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_role_with_http_info(code, as_at, scope, async_req=True)
         >>> result = thread.get()
@@ -715,15 +715,15 @@
 
     @overload
     def list_roles(self, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use all scopes if not supplied. The requested scope")] = None, as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, sort_by : Annotated[Optional[conlist(StrictStr)], Field(description="Optional. Order the results by these fields. Use use the '-' sign to denote descending order e.g. -MyFieldName")] = None, start : Annotated[Optional[StrictInt], Field(description="Optional. When paginating, skip this number of results")] = None, limit : Annotated[Optional[StrictInt], Field(description="Optional. When paginating, limit the number of returned results to this many.")] = None, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Optional. Expression to filter the result set")] = None, async_req: Optional[bool]=True, **kwargs) -> List[RoleResponse]:  # noqa: E501
         ...
 
     @validate_arguments
     def list_roles(self, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use all scopes if not supplied. The requested scope")] = None, as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, sort_by : Annotated[Optional[conlist(StrictStr)], Field(description="Optional. Order the results by these fields. Use use the '-' sign to denote descending order e.g. -MyFieldName")] = None, start : Annotated[Optional[StrictInt], Field(description="Optional. When paginating, skip this number of results")] = None, limit : Annotated[Optional[StrictInt], Field(description="Optional. When paginating, limit the number of returned results to this many.")] = None, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Optional. Expression to filter the result set")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[List[RoleResponse], Awaitable[List[RoleResponse]]]:  # noqa: E501
-        """[EARLY ACCESS] ListRoles: List Roles  # noqa: E501
+        """ListRoles: List Roles  # noqa: E501
 
         Gets all Roles in a scope  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_roles(scope, as_at, sort_by, start, limit, filter, async_req=True)
         >>> result = thread.get()
@@ -757,15 +757,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.list_roles_with_http_info(scope, as_at, sort_by, start, limit, filter, **kwargs)  # noqa: E501
 
     @validate_arguments
     def list_roles_with_http_info(self, scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. Will use all scopes if not supplied. The requested scope")] = None, as_at : Annotated[Optional[datetime], Field(description="Optional. The AsAt date time of the data")] = None, sort_by : Annotated[Optional[conlist(StrictStr)], Field(description="Optional. Order the results by these fields. Use use the '-' sign to denote descending order e.g. -MyFieldName")] = None, start : Annotated[Optional[StrictInt], Field(description="Optional. When paginating, skip this number of results")] = None, limit : Annotated[Optional[StrictInt], Field(description="Optional. When paginating, limit the number of returned results to this many.")] = None, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Optional. Expression to filter the result set")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] ListRoles: List Roles  # noqa: E501
+        """ListRoles: List Roles  # noqa: E501
 
         Gets all Roles in a scope  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_roles_with_http_info(scope, as_at, sort_by, start, limit, filter, async_req=True)
         >>> result = thread.get()
@@ -910,15 +910,15 @@
 
     @overload
     def remove_policy_collection_from_role(self, scope : Annotated[constr(strict=True), Field(..., description="The scope of the Role")], code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], policycollectionscope : Annotated[constr(strict=True), Field(..., description="The scope of policy collection to remove from the Role")], policycollectioncode : Annotated[constr(strict=True), Field(..., description="The code of the policy collection to remove from the Role")], async_req: Optional[bool]=True, **kwargs) -> RoleResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def remove_policy_collection_from_role(self, scope : Annotated[constr(strict=True), Field(..., description="The scope of the Role")], code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], policycollectionscope : Annotated[constr(strict=True), Field(..., description="The scope of policy collection to remove from the Role")], policycollectioncode : Annotated[constr(strict=True), Field(..., description="The code of the policy collection to remove from the Role")], async_req: Optional[bool]=None, **kwargs) -> Union[RoleResponse, Awaitable[RoleResponse]]:  # noqa: E501
-        """[EARLY ACCESS] RemovePolicyCollectionFromRole: Remove policy collection from role  # noqa: E501
+        """RemovePolicyCollectionFromRole: Remove policy collection from role  # noqa: E501
 
         Removes a policy collection from a role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.remove_policy_collection_from_role(scope, code, policycollectionscope, policycollectioncode, async_req=True)
         >>> result = thread.get()
@@ -948,15 +948,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.remove_policy_collection_from_role_with_http_info(scope, code, policycollectionscope, policycollectioncode, **kwargs)  # noqa: E501
 
     @validate_arguments
     def remove_policy_collection_from_role_with_http_info(self, scope : Annotated[constr(strict=True), Field(..., description="The scope of the Role")], code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], policycollectionscope : Annotated[constr(strict=True), Field(..., description="The scope of policy collection to remove from the Role")], policycollectioncode : Annotated[constr(strict=True), Field(..., description="The code of the policy collection to remove from the Role")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] RemovePolicyCollectionFromRole: Remove policy collection from role  # noqa: E501
+        """RemovePolicyCollectionFromRole: Remove policy collection from role  # noqa: E501
 
         Removes a policy collection from a role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.remove_policy_collection_from_role_with_http_info(scope, code, policycollectionscope, policycollectioncode, async_req=True)
         >>> result = thread.get()
@@ -1085,15 +1085,15 @@
 
     @overload
     def update_role(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], role_update_request : Annotated[RoleUpdateRequest, Field(..., description="The updated definition of the Role")], scope : Annotated[Optional[constr(strict=True)], Field(description=">Optional. Will use default scope if not supplied. The scope of the Role")] = None, before_scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. The scope of the Role. Will use default scope if not supplied.")] = None, before_code : Annotated[Optional[constr(strict=True)], Field(description="Optional. The code of the Role")] = None, after_scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. The scope of the Role. Will use default scope if not supplied.")] = None, after_code : Annotated[Optional[constr(strict=True)], Field(description="Optional. The code of the Role")] = None, async_req: Optional[bool]=True, **kwargs) -> RoleResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def update_role(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], role_update_request : Annotated[RoleUpdateRequest, Field(..., description="The updated definition of the Role")], scope : Annotated[Optional[constr(strict=True)], Field(description=">Optional. Will use default scope if not supplied. The scope of the Role")] = None, before_scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. The scope of the Role. Will use default scope if not supplied.")] = None, before_code : Annotated[Optional[constr(strict=True)], Field(description="Optional. The code of the Role")] = None, after_scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. The scope of the Role. Will use default scope if not supplied.")] = None, after_code : Annotated[Optional[constr(strict=True)], Field(description="Optional. The code of the Role")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[RoleResponse, Awaitable[RoleResponse]]:  # noqa: E501
-        """[EARLY ACCESS] UpdateRole: Update Role  # noqa: E501
+        """UpdateRole: Update Role  # noqa: E501
 
         Updates a Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_role(code, role_update_request, scope, before_scope, before_code, after_scope, after_code, async_req=True)
         >>> result = thread.get()
@@ -1129,15 +1129,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.update_role_with_http_info(code, role_update_request, scope, before_scope, before_code, after_scope, after_code, **kwargs)  # noqa: E501
 
     @validate_arguments
     def update_role_with_http_info(self, code : Annotated[constr(strict=True), Field(..., description="The code of the Role")], role_update_request : Annotated[RoleUpdateRequest, Field(..., description="The updated definition of the Role")], scope : Annotated[Optional[constr(strict=True)], Field(description=">Optional. Will use default scope if not supplied. The scope of the Role")] = None, before_scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. The scope of the Role. Will use default scope if not supplied.")] = None, before_code : Annotated[Optional[constr(strict=True)], Field(description="Optional. The code of the Role")] = None, after_scope : Annotated[Optional[constr(strict=True)], Field(description="Optional. The scope of the Role. Will use default scope if not supplied.")] = None, after_code : Annotated[Optional[constr(strict=True)], Field(description="Optional. The code of the Role")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EARLY ACCESS] UpdateRole: Update Role  # noqa: E501
+        """UpdateRole: Update Role  # noqa: E501
 
         Updates a Role  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_role_with_http_info(code, role_update_request, scope, before_scope, before_code, after_scope, after_code, async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/api/user_roles_api.py` & `finbourne_access_sdk-2.1.9/finbourne_access/api/user_roles_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     @overload
     def add_policy_collection_to_user_role(self, userid : Annotated[StrictStr, Field(..., description="Id of the User Role to get")], add_policy_collection_to_role_request : Annotated[AddPolicyCollectionToRoleRequest, Field(..., description="Dto of the policy collection to be added.")], async_req: Optional[bool]=True, **kwargs) -> UserRoleResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def add_policy_collection_to_user_role(self, userid : Annotated[StrictStr, Field(..., description="Id of the User Role to get")], add_policy_collection_to_role_request : Annotated[AddPolicyCollectionToRoleRequest, Field(..., description="Dto of the policy collection to be added.")], async_req: Optional[bool]=None, **kwargs) -> Union[UserRoleResponse, Awaitable[UserRoleResponse]]:  # noqa: E501
-        """[EXPERIMENTAL] AddPolicyCollectionToUserRole: Add a policy collection to a user-role  # noqa: E501
+        """AddPolicyCollectionToUserRole: Add a policy collection to a user-role  # noqa: E501
 
         Adds a policy collection to a user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.add_policy_collection_to_user_role(userid, add_policy_collection_to_role_request, async_req=True)
         >>> result = thread.get()
@@ -91,15 +91,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.add_policy_collection_to_user_role_with_http_info(userid, add_policy_collection_to_role_request, **kwargs)  # noqa: E501
 
     @validate_arguments
     def add_policy_collection_to_user_role_with_http_info(self, userid : Annotated[StrictStr, Field(..., description="Id of the User Role to get")], add_policy_collection_to_role_request : Annotated[AddPolicyCollectionToRoleRequest, Field(..., description="Dto of the policy collection to be added.")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EXPERIMENTAL] AddPolicyCollectionToUserRole: Add a policy collection to a user-role  # noqa: E501
+        """AddPolicyCollectionToUserRole: Add a policy collection to a user-role  # noqa: E501
 
         Adds a policy collection to a user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.add_policy_collection_to_user_role_with_http_info(userid, add_policy_collection_to_role_request, async_req=True)
         >>> result = thread.get()
@@ -223,15 +223,15 @@
 
     @overload
     def add_policy_to_user_role(self, userid : Annotated[StrictStr, Field(..., description="Id of the User Role to get")], add_policy_to_role_request : Annotated[AddPolicyToRoleRequest, Field(..., description="Dto of the policy to be added.")], async_req: Optional[bool]=True, **kwargs) -> UserRoleResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def add_policy_to_user_role(self, userid : Annotated[StrictStr, Field(..., description="Id of the User Role to get")], add_policy_to_role_request : Annotated[AddPolicyToRoleRequest, Field(..., description="Dto of the policy to be added.")], async_req: Optional[bool]=None, **kwargs) -> Union[UserRoleResponse, Awaitable[UserRoleResponse]]:  # noqa: E501
-        """[EXPERIMENTAL] AddPolicyToUserRole: Add a policy to a user-role  # noqa: E501
+        """AddPolicyToUserRole: Add a policy to a user-role  # noqa: E501
 
         Adds a policy to a user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.add_policy_to_user_role(userid, add_policy_to_role_request, async_req=True)
         >>> result = thread.get()
@@ -257,15 +257,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.add_policy_to_user_role_with_http_info(userid, add_policy_to_role_request, **kwargs)  # noqa: E501
 
     @validate_arguments
     def add_policy_to_user_role_with_http_info(self, userid : Annotated[StrictStr, Field(..., description="Id of the User Role to get")], add_policy_to_role_request : Annotated[AddPolicyToRoleRequest, Field(..., description="Dto of the policy to be added.")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EXPERIMENTAL] AddPolicyToUserRole: Add a policy to a user-role  # noqa: E501
+        """AddPolicyToUserRole: Add a policy to a user-role  # noqa: E501
 
         Adds a policy to a user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.add_policy_to_user_role_with_http_info(userid, add_policy_to_role_request, async_req=True)
         >>> result = thread.get()
@@ -389,15 +389,15 @@
 
     @overload
     def create_user_role(self, user_role_creation_request : Annotated[UserRoleCreationRequest, Field(..., description="Definition of the user-role to create.")], async_req: Optional[bool]=True, **kwargs) -> UserRoleResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def create_user_role(self, user_role_creation_request : Annotated[UserRoleCreationRequest, Field(..., description="Definition of the user-role to create.")], async_req: Optional[bool]=None, **kwargs) -> Union[UserRoleResponse, Awaitable[UserRoleResponse]]:  # noqa: E501
-        """[EXPERIMENTAL] CreateUserRole: Create a user-role  # noqa: E501
+        """CreateUserRole: Create a user-role  # noqa: E501
 
         Creates a new user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_user_role(user_role_creation_request, async_req=True)
         >>> result = thread.get()
@@ -421,15 +421,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.create_user_role_with_http_info(user_role_creation_request, **kwargs)  # noqa: E501
 
     @validate_arguments
     def create_user_role_with_http_info(self, user_role_creation_request : Annotated[UserRoleCreationRequest, Field(..., description="Definition of the user-role to create.")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EXPERIMENTAL] CreateUserRole: Create a user-role  # noqa: E501
+        """CreateUserRole: Create a user-role  # noqa: E501
 
         Creates a new user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_user_role_with_http_info(user_role_creation_request, async_req=True)
         >>> result = thread.get()
@@ -547,15 +547,15 @@
 
     @overload
     def delete_user_role(self, userid : Annotated[StrictStr, Field(..., description="Id of the user-role to delete.")], async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def delete_user_role(self, userid : Annotated[StrictStr, Field(..., description="Id of the user-role to delete.")], async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EXPERIMENTAL] DeleteUserRole: Delete a user-role  # noqa: E501
+        """DeleteUserRole: Delete a user-role  # noqa: E501
 
         Deletes an identified user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_user_role(userid, async_req=True)
         >>> result = thread.get()
@@ -579,15 +579,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.delete_user_role_with_http_info(userid, **kwargs)  # noqa: E501
 
     @validate_arguments
     def delete_user_role_with_http_info(self, userid : Annotated[StrictStr, Field(..., description="Id of the user-role to delete.")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EXPERIMENTAL] DeleteUserRole: Delete a user-role  # noqa: E501
+        """DeleteUserRole: Delete a user-role  # noqa: E501
 
         Deletes an identified user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_user_role_with_http_info(userid, async_req=True)
         >>> result = thread.get()
@@ -695,15 +695,15 @@
 
     @overload
     def get_user_role(self, userid : Annotated[StrictStr, Field(..., description="Id of the user-role to get.")], async_req: Optional[bool]=True, **kwargs) -> UserRoleResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def get_user_role(self, userid : Annotated[StrictStr, Field(..., description="Id of the user-role to get.")], async_req: Optional[bool]=None, **kwargs) -> Union[UserRoleResponse, Awaitable[UserRoleResponse]]:  # noqa: E501
-        """[EXPERIMENTAL] GetUserRole: Get a user-role  # noqa: E501
+        """GetUserRole: Get a user-role  # noqa: E501
 
         Get an identified user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_user_role(userid, async_req=True)
         >>> result = thread.get()
@@ -727,15 +727,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.get_user_role_with_http_info(userid, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_user_role_with_http_info(self, userid : Annotated[StrictStr, Field(..., description="Id of the user-role to get.")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EXPERIMENTAL] GetUserRole: Get a user-role  # noqa: E501
+        """GetUserRole: Get a user-role  # noqa: E501
 
         Get an identified user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_user_role_with_http_info(userid, async_req=True)
         >>> result = thread.get()
@@ -846,15 +846,15 @@
 
     @overload
     def list_user_roles(self, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Optional. Expression to filter the result set")] = None, sort_by : Annotated[Optional[constr(strict=True, max_length=16384, min_length=1)], Field(description="Optional. Order the results by these fields. Use the '-' sign to denote descending order e.g. -MyFieldName")] = None, limit : Annotated[Optional[conint(strict=True, le=5000, ge=1)], Field(description="Optional. When paginating, limit the number of returned results to this many.")] = None, page : Annotated[Optional[constr(strict=True, max_length=500, min_length=1)], Field(description="Optional. Encoded page string returned from a previous search result that will retrieve              the next page of data.")] = None, async_req: Optional[bool]=True, **kwargs) -> ResourceListOfUserRoleResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def list_user_roles(self, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Optional. Expression to filter the result set")] = None, sort_by : Annotated[Optional[constr(strict=True, max_length=16384, min_length=1)], Field(description="Optional. Order the results by these fields. Use the '-' sign to denote descending order e.g. -MyFieldName")] = None, limit : Annotated[Optional[conint(strict=True, le=5000, ge=1)], Field(description="Optional. When paginating, limit the number of returned results to this many.")] = None, page : Annotated[Optional[constr(strict=True, max_length=500, min_length=1)], Field(description="Optional. Encoded page string returned from a previous search result that will retrieve              the next page of data.")] = None, async_req: Optional[bool]=None, **kwargs) -> Union[ResourceListOfUserRoleResponse, Awaitable[ResourceListOfUserRoleResponse]]:  # noqa: E501
-        """[EXPERIMENTAL] ListUserRoles: List user-roles  # noqa: E501
+        """ListUserRoles: List user-roles  # noqa: E501
 
         Lists all user-roles and pages.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_user_roles(filter, sort_by, limit, page, async_req=True)
         >>> result = thread.get()
@@ -884,15 +884,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.list_user_roles_with_http_info(filter, sort_by, limit, page, **kwargs)  # noqa: E501
 
     @validate_arguments
     def list_user_roles_with_http_info(self, filter : Annotated[Optional[constr(strict=True, max_length=16384, min_length=0)], Field(description="Optional. Expression to filter the result set")] = None, sort_by : Annotated[Optional[constr(strict=True, max_length=16384, min_length=1)], Field(description="Optional. Order the results by these fields. Use the '-' sign to denote descending order e.g. -MyFieldName")] = None, limit : Annotated[Optional[conint(strict=True, le=5000, ge=1)], Field(description="Optional. When paginating, limit the number of returned results to this many.")] = None, page : Annotated[Optional[constr(strict=True, max_length=500, min_length=1)], Field(description="Optional. Encoded page string returned from a previous search result that will retrieve              the next page of data.")] = None, **kwargs) -> ApiResponse:  # noqa: E501
-        """[EXPERIMENTAL] ListUserRoles: List user-roles  # noqa: E501
+        """ListUserRoles: List user-roles  # noqa: E501
 
         Lists all user-roles and pages.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.list_user_roles_with_http_info(filter, sort_by, limit, page, async_req=True)
         >>> result = thread.get()
@@ -1021,15 +1021,15 @@
 
     @overload
     def remove_policy_collection_from_user_role(self, userid : Annotated[StrictStr, Field(..., description="Id of the User Role to get")], policy_collection_scope : Annotated[constr(strict=True), Field(..., description="The scope of policy collection to remove from the User Role")], policy_collection_code : Annotated[constr(strict=True), Field(..., description="The code of the policy collection to remove from the User Role")], async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def remove_policy_collection_from_user_role(self, userid : Annotated[StrictStr, Field(..., description="Id of the User Role to get")], policy_collection_scope : Annotated[constr(strict=True), Field(..., description="The scope of policy collection to remove from the User Role")], policy_collection_code : Annotated[constr(strict=True), Field(..., description="The code of the policy collection to remove from the User Role")], async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EXPERIMENTAL] RemovePolicyCollectionFromUserRole: Remove a policy collection from a user-role  # noqa: E501
+        """RemovePolicyCollectionFromUserRole: Remove a policy collection from a user-role  # noqa: E501
 
         Removes a policy collection from a user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.remove_policy_collection_from_user_role(userid, policy_collection_scope, policy_collection_code, async_req=True)
         >>> result = thread.get()
@@ -1057,15 +1057,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.remove_policy_collection_from_user_role_with_http_info(userid, policy_collection_scope, policy_collection_code, **kwargs)  # noqa: E501
 
     @validate_arguments
     def remove_policy_collection_from_user_role_with_http_info(self, userid : Annotated[StrictStr, Field(..., description="Id of the User Role to get")], policy_collection_scope : Annotated[constr(strict=True), Field(..., description="The scope of policy collection to remove from the User Role")], policy_collection_code : Annotated[constr(strict=True), Field(..., description="The code of the policy collection to remove from the User Role")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EXPERIMENTAL] RemovePolicyCollectionFromUserRole: Remove a policy collection from a user-role  # noqa: E501
+        """RemovePolicyCollectionFromUserRole: Remove a policy collection from a user-role  # noqa: E501
 
         Removes a policy collection from a user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.remove_policy_collection_from_user_role_with_http_info(userid, policy_collection_scope, policy_collection_code, async_req=True)
         >>> result = thread.get()
@@ -1185,15 +1185,15 @@
 
     @overload
     def remove_policy_from_user_role(self, userid : Annotated[StrictStr, Field(..., description="Id of the User Role to get")], policy_scope : Annotated[constr(strict=True), Field(..., description="The scope of the policy to remove from the User Role")], policy_code : Annotated[constr(strict=True), Field(..., description="The code of the policy to remove from the User Role")], async_req: Optional[bool]=True, **kwargs) -> None:  # noqa: E501
         ...
 
     @validate_arguments
     def remove_policy_from_user_role(self, userid : Annotated[StrictStr, Field(..., description="Id of the User Role to get")], policy_scope : Annotated[constr(strict=True), Field(..., description="The scope of the policy to remove from the User Role")], policy_code : Annotated[constr(strict=True), Field(..., description="The code of the policy to remove from the User Role")], async_req: Optional[bool]=None, **kwargs) -> Union[None, Awaitable[None]]:  # noqa: E501
-        """[EXPERIMENTAL] RemovePolicyFromUserRole: Remove a policy from a user-role  # noqa: E501
+        """RemovePolicyFromUserRole: Remove a policy from a user-role  # noqa: E501
 
         Removes a policy from a user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.remove_policy_from_user_role(userid, policy_scope, policy_code, async_req=True)
         >>> result = thread.get()
@@ -1221,15 +1221,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.remove_policy_from_user_role_with_http_info(userid, policy_scope, policy_code, **kwargs)  # noqa: E501
 
     @validate_arguments
     def remove_policy_from_user_role_with_http_info(self, userid : Annotated[StrictStr, Field(..., description="Id of the User Role to get")], policy_scope : Annotated[constr(strict=True), Field(..., description="The scope of the policy to remove from the User Role")], policy_code : Annotated[constr(strict=True), Field(..., description="The code of the policy to remove from the User Role")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EXPERIMENTAL] RemovePolicyFromUserRole: Remove a policy from a user-role  # noqa: E501
+        """RemovePolicyFromUserRole: Remove a policy from a user-role  # noqa: E501
 
         Removes a policy from a user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.remove_policy_from_user_role_with_http_info(userid, policy_scope, policy_code, async_req=True)
         >>> result = thread.get()
@@ -1349,15 +1349,15 @@
 
     @overload
     def update_user_role(self, userid : Annotated[StrictStr, Field(..., description="Id of the user-role to be updated.")], user_role_update_request : Annotated[UserRoleUpdateRequest, Field(..., description="Definition of the update to apply to the user-role.")], async_req: Optional[bool]=True, **kwargs) -> UserRoleResponse:  # noqa: E501
         ...
 
     @validate_arguments
     def update_user_role(self, userid : Annotated[StrictStr, Field(..., description="Id of the user-role to be updated.")], user_role_update_request : Annotated[UserRoleUpdateRequest, Field(..., description="Definition of the update to apply to the user-role.")], async_req: Optional[bool]=None, **kwargs) -> Union[UserRoleResponse, Awaitable[UserRoleResponse]]:  # noqa: E501
-        """[EXPERIMENTAL] UpdateUserRole: Update a user-role  # noqa: E501
+        """UpdateUserRole: Update a user-role  # noqa: E501
 
         Updates an identified user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_user_role(userid, user_role_update_request, async_req=True)
         >>> result = thread.get()
@@ -1383,15 +1383,15 @@
             raise ValueError(message)
         if async_req is not None:
             kwargs['async_req'] = async_req
         return self.update_user_role_with_http_info(userid, user_role_update_request, **kwargs)  # noqa: E501
 
     @validate_arguments
     def update_user_role_with_http_info(self, userid : Annotated[StrictStr, Field(..., description="Id of the user-role to be updated.")], user_role_update_request : Annotated[UserRoleUpdateRequest, Field(..., description="Definition of the update to apply to the user-role.")], **kwargs) -> ApiResponse:  # noqa: E501
-        """[EXPERIMENTAL] UpdateUserRole: Update a user-role  # noqa: E501
+        """UpdateUserRole: Update a user-role  # noqa: E501
 
         Updates an identified user-role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_user_role_with_http_info(userid, user_role_update_request, async_req=True)
         >>> result = thread.get()
```

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/api_client.py` & `finbourne_access_sdk-2.1.9/finbourne_access/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/api_response.py` & `finbourne_access_sdk-2.1.9/finbourne_access/api_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/configuration.py` & `finbourne_access_sdk-2.1.9/finbourne_access/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("finbourne_access-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.3774\n"\
+               "Version of the API: 0.0.3775\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/exceptions.py` & `finbourne_access_sdk-2.1.9/finbourne_access/exceptions.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/extensions/__init__.py` & `finbourne_access_sdk-2.1.9/finbourne_access/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/extensions/api_client.py` & `finbourne_access_sdk-2.1.9/finbourne_access/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/extensions/api_client_factory.py` & `finbourne_access_sdk-2.1.9/finbourne_access/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/extensions/api_configuration.py` & `finbourne_access_sdk-2.1.9/finbourne_access/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/extensions/configuration_loaders.py` & `finbourne_access_sdk-2.1.9/finbourne_access/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/extensions/proxy_config.py` & `finbourne_access_sdk-2.1.9/finbourne_access/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/extensions/refreshing_token.py` & `finbourne_access_sdk-2.1.9/finbourne_access/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/extensions/rest.py` & `finbourne_access_sdk-2.1.9/finbourne_access/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/extensions/retry.py` & `finbourne_access_sdk-2.1.9/finbourne_access/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/extensions/socket_keep_alive.py` & `finbourne_access_sdk-2.1.9/finbourne_access/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/extensions/tcp_keep_alive_connector.py` & `finbourne_access_sdk-2.1.9/finbourne_access/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/__init__.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/access_controlled_action.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/access_controlled_resource.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/action_id.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/action_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/add_policy_collection_to_role_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/add_policy_collection_to_role_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/add_policy_to_role_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/add_policy_to_role_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/add_to_policy_collection_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/add_to_policy_collection_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/as_at_predicate_contract.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/as_at_predicate_contract.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/as_at_range_for_spec.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/as_at_range_for_spec.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/as_at_relative.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/as_at_relative.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/attached_policy_definition_response.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/attached_policy_definition_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/date_quality.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/date_quality.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/date_unit.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/date_unit.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/effective_date_has_quality.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/effective_date_has_quality.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/effective_date_relative.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/effective_date_relative.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/effective_range.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/effective_range.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/entitlement_metadata.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/entitlement_metadata.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/evaluation_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/evaluation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/evaluation_response.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/evaluation_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/evaluation_result.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/for_spec.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/for_spec.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/generate_policy_from_template_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/generate_policy_from_template_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/generated_policy_components.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/generated_policy_components.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/grant.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/grant.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/how_spec.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/how_spec.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/id_selector_definition.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/identifier_part_schema.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/if_expression.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/if_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/if_feature_chain_expression.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/if_feature_chain_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/if_identity_claim_expression.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/if_identity_claim_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/if_identity_scope_expression.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/if_identity_scope_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/if_request_header_expression.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/if_request_header_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/key_value_pair_of_string_to_string.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/key_value_pair_of_string_to_string.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/link.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/link.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/lusid_problem_details.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/lusid_validation_problem_details.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/match_all_selector_definition.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/match_all_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/metadata_expression.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/metadata_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/metadata_selector_definition.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/metadata_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/non_transitive_supervisor_role_resource.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/non_transitive_supervisor_role_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/operator.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/operator.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/point_in_time_specification.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/point_in_time_specification.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_collection_creation_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_collection_id.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_collection_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_collection_response.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_collection_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_collection_update_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_collection_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_creation_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_id.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_id_role_resource.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_id_role_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_response.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_selector_definition.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_template_creation_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_template_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_template_response.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_template_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_template_update_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_template_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_templated_selector.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_templated_selector.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_type.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_type.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/policy_update_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/policy_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/relative_to_date_time.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/relative_to_date_time.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/remove_from_policy_collection_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/remove_from_policy_collection_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/request_details.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/request_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/requested_action_key.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/requested_action_key.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/resource_details.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/resource_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/resource_list_of_access_controlled_resource.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/resource_list_of_policy_collection_response.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/resource_list_of_policy_collection_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/resource_list_of_policy_response.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/resource_list_of_policy_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/resource_list_of_policy_template_response.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/resource_list_of_policy_template_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/resource_list_of_user_role_response.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/resource_list_of_user_role_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/role_creation_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/role_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/role_id.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/role_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/role_resource_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/role_resource_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/role_response.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/role_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/role_update_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/role_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/selector_definition.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/template_metadata.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/template_metadata.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/template_selection.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/template_selection.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/text_operator.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/text_operator.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/user_role_creation_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/user_role_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/user_role_response.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/user_role_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/user_role_update_request.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/user_role_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/models/when_spec.py` & `finbourne_access_sdk-2.1.9/finbourne_access/models/when_spec.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/finbourne_access/rest.py` & `finbourne_access_sdk-2.1.9/finbourne_access/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.1.8/pyproject.toml` & `finbourne_access_sdk-2.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finbourne-access-sdk"
-version = "2.1.8"
+version = "2.1.9"
 description = "FINBOURNE Access Management API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/finbourne-access-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Access Management API", "finbourne-access-sdk"]
 packages = [
```

### Comparing `finbourne_access_sdk-2.1.8/PKG-INFO` & `finbourne_access_sdk-2.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finbourne-access-sdk
-Version: 2.1.8
+Version: 2.1.9
 Summary: FINBOURNE Access Management API
 Home-page: https://github.com/finbourne/finbourne-access-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Access Management API,finbourne-access-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # finbourne-access-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.3774
-- Package version: 2.1.8
+- API version: 0.0.3775
+- Package version: 2.1.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -195,68 +195,68 @@
 
 # Enter a context with an instance of the ApiClientFactory to ensure the connection pool is closed after use
 async with api_client_factory:
     # Create an instance of the API class
     api_instance = api_client_factory.build(ApplicationMetadataApi)
 
     try:
-        # [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
+        # ListAccessControlledResources: Get resources available for access control
         api_response = await api_instance.list_access_controlled_resources()
         print("The response of ApplicationMetadataApi->list_access_controlled_resources:\n")
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling ApplicationMetadataApi->list_access_controlled_resources: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://fbn-prd.lusid.com/access*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
-*PoliciesApi* | [**add_to_policy_collection**](docs/PoliciesApi.md#add_to_policy_collection) | **POST** /api/policycollections/{code}/add | [EARLY ACCESS] AddToPolicyCollection: Add To PolicyCollection
-*PoliciesApi* | [**create_policy**](docs/PoliciesApi.md#create_policy) | **POST** /api/policies | [EARLY ACCESS] CreatePolicy: Create Policy
-*PoliciesApi* | [**create_policy_collection**](docs/PoliciesApi.md#create_policy_collection) | **POST** /api/policycollections | [EARLY ACCESS] CreatePolicyCollection: Create PolicyCollection
-*PoliciesApi* | [**delete_policy**](docs/PoliciesApi.md#delete_policy) | **DELETE** /api/policies/{code} | [EARLY ACCESS] DeletePolicy: Delete Policy
-*PoliciesApi* | [**delete_policy_collection**](docs/PoliciesApi.md#delete_policy_collection) | **DELETE** /api/policycollections/{code} | [EARLY ACCESS] DeletePolicyCollection: Delete PolicyCollection
-*PoliciesApi* | [**evaluate**](docs/PoliciesApi.md#evaluate) | **POST** /api/me | [EARLY ACCESS] Evaluate: Run one or more evaluations
+*ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | ListAccessControlledResources: Get resources available for access control
+*PoliciesApi* | [**add_to_policy_collection**](docs/PoliciesApi.md#add_to_policy_collection) | **POST** /api/policycollections/{code}/add | AddToPolicyCollection: Add To PolicyCollection
+*PoliciesApi* | [**create_policy**](docs/PoliciesApi.md#create_policy) | **POST** /api/policies | CreatePolicy: Create Policy
+*PoliciesApi* | [**create_policy_collection**](docs/PoliciesApi.md#create_policy_collection) | **POST** /api/policycollections | CreatePolicyCollection: Create PolicyCollection
+*PoliciesApi* | [**delete_policy**](docs/PoliciesApi.md#delete_policy) | **DELETE** /api/policies/{code} | DeletePolicy: Delete Policy
+*PoliciesApi* | [**delete_policy_collection**](docs/PoliciesApi.md#delete_policy_collection) | **DELETE** /api/policycollections/{code} | DeletePolicyCollection: Delete PolicyCollection
+*PoliciesApi* | [**evaluate**](docs/PoliciesApi.md#evaluate) | **POST** /api/me | Evaluate: Run one or more evaluations
 *PoliciesApi* | [**get_own_policies**](docs/PoliciesApi.md#get_own_policies) | **GET** /api/me | GetOwnPolicies: Get policies of requesting user
-*PoliciesApi* | [**get_policy**](docs/PoliciesApi.md#get_policy) | **GET** /api/policies/{code} | [EARLY ACCESS] GetPolicy: Get Policy
-*PoliciesApi* | [**get_policy_collection**](docs/PoliciesApi.md#get_policy_collection) | **GET** /api/policycollections/{code} | [EARLY ACCESS] GetPolicyCollection: Get PolicyCollection
+*PoliciesApi* | [**get_policy**](docs/PoliciesApi.md#get_policy) | **GET** /api/policies/{code} | GetPolicy: Get Policy
+*PoliciesApi* | [**get_policy_collection**](docs/PoliciesApi.md#get_policy_collection) | **GET** /api/policycollections/{code} | GetPolicyCollection: Get PolicyCollection
 *PoliciesApi* | [**list_policies**](docs/PoliciesApi.md#list_policies) | **GET** /api/policies | [EARLY ACCESS] ListPolicies: List Policies
-*PoliciesApi* | [**list_policy_collections**](docs/PoliciesApi.md#list_policy_collections) | **GET** /api/policycollections | [EARLY ACCESS] ListPolicyCollections: List PolicyCollections
+*PoliciesApi* | [**list_policy_collections**](docs/PoliciesApi.md#list_policy_collections) | **GET** /api/policycollections | ListPolicyCollections: List PolicyCollections
 *PoliciesApi* | [**page_policies**](docs/PoliciesApi.md#page_policies) | **GET** /api/policies/page | [EARLY ACCESS] PagePolicies: Page Policies
-*PoliciesApi* | [**page_policy_collections**](docs/PoliciesApi.md#page_policy_collections) | **GET** /api/policycollections/page | [EARLY ACCESS] PagePolicyCollections: Page PolicyCollections
-*PoliciesApi* | [**remove_from_policy_collection**](docs/PoliciesApi.md#remove_from_policy_collection) | **POST** /api/policycollections/{code}/remove | [EARLY ACCESS] RemoveFromPolicyCollection: Remove From PolicyCollection
-*PoliciesApi* | [**update_policy**](docs/PoliciesApi.md#update_policy) | **PUT** /api/policies/{code} | [EARLY ACCESS] UpdatePolicy: Update Policy
-*PoliciesApi* | [**update_policy_collection**](docs/PoliciesApi.md#update_policy_collection) | **PUT** /api/policycollections/{code} | [EARLY ACCESS] UpdatePolicyCollection: Update PolicyCollection
+*PoliciesApi* | [**page_policy_collections**](docs/PoliciesApi.md#page_policy_collections) | **GET** /api/policycollections/page | PagePolicyCollections: Page PolicyCollections
+*PoliciesApi* | [**remove_from_policy_collection**](docs/PoliciesApi.md#remove_from_policy_collection) | **POST** /api/policycollections/{code}/remove | RemoveFromPolicyCollection: Remove From PolicyCollection
+*PoliciesApi* | [**update_policy**](docs/PoliciesApi.md#update_policy) | **PUT** /api/policies/{code} | UpdatePolicy: Update Policy
+*PoliciesApi* | [**update_policy_collection**](docs/PoliciesApi.md#update_policy_collection) | **PUT** /api/policycollections/{code} | UpdatePolicyCollection: Update PolicyCollection
 *PolicyTemplatesApi* | [**create_policy_template**](docs/PolicyTemplatesApi.md#create_policy_template) | **POST** /api/policytemplates | [EXPERIMENTAL] CreatePolicyTemplate: Create a Policy Template
 *PolicyTemplatesApi* | [**delete_policy_template**](docs/PolicyTemplatesApi.md#delete_policy_template) | **DELETE** /api/policytemplates/{code} | [EXPERIMENTAL] DeletePolicyTemplate: Deleting a policy template
 *PolicyTemplatesApi* | [**generate_policy_from_template**](docs/PolicyTemplatesApi.md#generate_policy_from_template) | **POST** /api/policytemplates/$generatepolicy | [EXPERIMENTAL] GeneratePolicyFromTemplate: Generate policy from template
 *PolicyTemplatesApi* | [**get_policy_template**](docs/PolicyTemplatesApi.md#get_policy_template) | **GET** /api/policytemplates/{code} | [EXPERIMENTAL] GetPolicyTemplate: Retrieving one Policy Template
 *PolicyTemplatesApi* | [**list_policy_templates**](docs/PolicyTemplatesApi.md#list_policy_templates) | **GET** /api/policytemplates | [EXPERIMENTAL] ListPolicyTemplates: List Policy Templates
 *PolicyTemplatesApi* | [**update_policy_template**](docs/PolicyTemplatesApi.md#update_policy_template) | **PUT** /api/policytemplates/{code} | [EXPERIMENTAL] UpdatePolicyTemplate: Update a Policy Template
-*RolesApi* | [**add_policy_collection_to_role**](docs/RolesApi.md#add_policy_collection_to_role) | **POST** /api/roles/{scope}/{code}/policycollections | [EARLY ACCESS] AddPolicyCollectionToRole: Add policy collections to a role
-*RolesApi* | [**create_role**](docs/RolesApi.md#create_role) | **POST** /api/roles | [EARLY ACCESS] CreateRole: Create Role
-*RolesApi* | [**delete_role**](docs/RolesApi.md#delete_role) | **DELETE** /api/roles/{code} | [EARLY ACCESS] DeleteRole: Delete Role
-*RolesApi* | [**get_role**](docs/RolesApi.md#get_role) | **GET** /api/roles/{code} | [EARLY ACCESS] GetRole: Get Role
-*RolesApi* | [**list_roles**](docs/RolesApi.md#list_roles) | **GET** /api/roles | [EARLY ACCESS] ListRoles: List Roles
-*RolesApi* | [**remove_policy_collection_from_role**](docs/RolesApi.md#remove_policy_collection_from_role) | **DELETE** /api/roles/{scope}/{code}/policycollections/{policycollectionscope}/{policycollectioncode} | [EARLY ACCESS] RemovePolicyCollectionFromRole: Remove policy collection from role
-*RolesApi* | [**update_role**](docs/RolesApi.md#update_role) | **PUT** /api/roles/{code} | [EARLY ACCESS] UpdateRole: Update Role
-*UserRolesApi* | [**add_policy_collection_to_user_role**](docs/UserRolesApi.md#add_policy_collection_to_user_role) | **POST** /api/userroles/{userid}/policycollections | [EXPERIMENTAL] AddPolicyCollectionToUserRole: Add a policy collection to a user-role
-*UserRolesApi* | [**add_policy_to_user_role**](docs/UserRolesApi.md#add_policy_to_user_role) | **POST** /api/userroles/{userid}/policies | [EXPERIMENTAL] AddPolicyToUserRole: Add a policy to a user-role
-*UserRolesApi* | [**create_user_role**](docs/UserRolesApi.md#create_user_role) | **POST** /api/userroles | [EXPERIMENTAL] CreateUserRole: Create a user-role
-*UserRolesApi* | [**delete_user_role**](docs/UserRolesApi.md#delete_user_role) | **DELETE** /api/userroles/{userid} | [EXPERIMENTAL] DeleteUserRole: Delete a user-role
-*UserRolesApi* | [**get_user_role**](docs/UserRolesApi.md#get_user_role) | **GET** /api/userroles/{userid} | [EXPERIMENTAL] GetUserRole: Get a user-role
-*UserRolesApi* | [**list_user_roles**](docs/UserRolesApi.md#list_user_roles) | **GET** /api/userroles | [EXPERIMENTAL] ListUserRoles: List user-roles
-*UserRolesApi* | [**remove_policy_collection_from_user_role**](docs/UserRolesApi.md#remove_policy_collection_from_user_role) | **DELETE** /api/userroles/{userid}/policycollections/{policyCollectionScope}/{policyCollectionCode} | [EXPERIMENTAL] RemovePolicyCollectionFromUserRole: Remove a policy collection from a user-role
-*UserRolesApi* | [**remove_policy_from_user_role**](docs/UserRolesApi.md#remove_policy_from_user_role) | **DELETE** /api/userroles/{userid}/policies/{policyScope}/{policyCode} | [EXPERIMENTAL] RemovePolicyFromUserRole: Remove a policy from a user-role
-*UserRolesApi* | [**update_user_role**](docs/UserRolesApi.md#update_user_role) | **POST** /api/userroles/{userid}/update | [EXPERIMENTAL] UpdateUserRole: Update a user-role
+*RolesApi* | [**add_policy_collection_to_role**](docs/RolesApi.md#add_policy_collection_to_role) | **POST** /api/roles/{scope}/{code}/policycollections | AddPolicyCollectionToRole: Add policy collections to a role
+*RolesApi* | [**create_role**](docs/RolesApi.md#create_role) | **POST** /api/roles | CreateRole: Create Role
+*RolesApi* | [**delete_role**](docs/RolesApi.md#delete_role) | **DELETE** /api/roles/{code} | DeleteRole: Delete Role
+*RolesApi* | [**get_role**](docs/RolesApi.md#get_role) | **GET** /api/roles/{code} | GetRole: Get Role
+*RolesApi* | [**list_roles**](docs/RolesApi.md#list_roles) | **GET** /api/roles | ListRoles: List Roles
+*RolesApi* | [**remove_policy_collection_from_role**](docs/RolesApi.md#remove_policy_collection_from_role) | **DELETE** /api/roles/{scope}/{code}/policycollections/{policycollectionscope}/{policycollectioncode} | RemovePolicyCollectionFromRole: Remove policy collection from role
+*RolesApi* | [**update_role**](docs/RolesApi.md#update_role) | **PUT** /api/roles/{code} | UpdateRole: Update Role
+*UserRolesApi* | [**add_policy_collection_to_user_role**](docs/UserRolesApi.md#add_policy_collection_to_user_role) | **POST** /api/userroles/{userid}/policycollections | AddPolicyCollectionToUserRole: Add a policy collection to a user-role
+*UserRolesApi* | [**add_policy_to_user_role**](docs/UserRolesApi.md#add_policy_to_user_role) | **POST** /api/userroles/{userid}/policies | AddPolicyToUserRole: Add a policy to a user-role
+*UserRolesApi* | [**create_user_role**](docs/UserRolesApi.md#create_user_role) | **POST** /api/userroles | CreateUserRole: Create a user-role
+*UserRolesApi* | [**delete_user_role**](docs/UserRolesApi.md#delete_user_role) | **DELETE** /api/userroles/{userid} | DeleteUserRole: Delete a user-role
+*UserRolesApi* | [**get_user_role**](docs/UserRolesApi.md#get_user_role) | **GET** /api/userroles/{userid} | GetUserRole: Get a user-role
+*UserRolesApi* | [**list_user_roles**](docs/UserRolesApi.md#list_user_roles) | **GET** /api/userroles | ListUserRoles: List user-roles
+*UserRolesApi* | [**remove_policy_collection_from_user_role**](docs/UserRolesApi.md#remove_policy_collection_from_user_role) | **DELETE** /api/userroles/{userid}/policycollections/{policyCollectionScope}/{policyCollectionCode} | RemovePolicyCollectionFromUserRole: Remove a policy collection from a user-role
+*UserRolesApi* | [**remove_policy_from_user_role**](docs/UserRolesApi.md#remove_policy_from_user_role) | **DELETE** /api/userroles/{userid}/policies/{policyScope}/{policyCode} | RemovePolicyFromUserRole: Remove a policy from a user-role
+*UserRolesApi* | [**update_user_role**](docs/UserRolesApi.md#update_user_role) | **POST** /api/userroles/{userid}/update | UpdateUserRole: Update a user-role
 
 
 ## Documentation For Models
 
  - [AccessControlledAction](docs/AccessControlledAction.md)
  - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionId](docs/ActionId.md)
```

