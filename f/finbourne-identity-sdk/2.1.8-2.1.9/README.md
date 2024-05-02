# Comparing `tmp/finbourne_identity_sdk-2.1.8.tar.gz` & `tmp/finbourne_identity_sdk-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finbourne_identity_sdk-2.1.8.tar", max compression
+gzip compressed data, was "finbourne_identity_sdk-2.1.9.tar", max compression
```

## Comparing `finbourne_identity_sdk-2.1.8.tar` & `finbourne_identity_sdk-2.1.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    15621 2024-04-16 17:50:38.272621 finbourne_identity_sdk-2.1.8/README.md
--rw-r--r--   0        0        0     7317 2024-04-16 17:50:38.267621 finbourne_identity_sdk-2.1.8/finbourne_identity/__init__.py
--rw-r--r--   0        0        0      882 2024-04-16 17:50:38.267621 finbourne_identity_sdk-2.1.8/finbourne_identity/api/__init__.py
--rw-r--r--   0        0        0     7528 2024-04-16 17:50:38.266621 finbourne_identity_sdk-2.1.8/finbourne_identity/api/application_metadata_api.py
--rw-r--r--   0        0        0    36614 2024-04-16 17:50:38.266621 finbourne_identity_sdk-2.1.8/finbourne_identity/api/applications_api.py
--rw-r--r--   0        0        0    53621 2024-04-16 17:50:38.266621 finbourne_identity_sdk-2.1.8/finbourne_identity/api/authentication_api.py
--rw-r--r--   0        0        0    15596 2024-04-16 17:50:38.266621 finbourne_identity_sdk-2.1.8/finbourne_identity/api/identity_provider_api.py
--rw-r--r--   0        0        0    14825 2024-04-16 17:50:38.266621 finbourne_identity_sdk-2.1.8/finbourne_identity/api/me_api.py
--rw-r--r--   0        0        0    21760 2024-04-16 17:50:38.267621 finbourne_identity_sdk-2.1.8/finbourne_identity/api/personal_authentication_tokens_api.py
--rw-r--r--   0        0        0    57442 2024-04-16 17:50:38.267621 finbourne_identity_sdk-2.1.8/finbourne_identity/api/roles_api.py
--rw-r--r--   0        0        0     6867 2024-04-16 17:50:38.267621 finbourne_identity_sdk-2.1.8/finbourne_identity/api/tokens_api.py
--rw-r--r--   0        0        0    95281 2024-04-16 17:50:38.267621 finbourne_identity_sdk-2.1.8/finbourne_identity/api/users_api.py
--rw-r--r--   0        0        0    30821 2024-04-16 17:50:38.267621 finbourne_identity_sdk-2.1.8/finbourne_identity/api_client.py
--rw-r--r--   0        0        0      852 2024-04-16 17:50:38.262621 finbourne_identity_sdk-2.1.8/finbourne_identity/api_response.py
--rw-r--r--   0        0        0    14468 2024-04-16 17:50:38.267621 finbourne_identity_sdk-2.1.8/finbourne_identity/configuration.py
--rw-r--r--   0        0        0     5347 2024-04-16 17:50:38.267621 finbourne_identity_sdk-2.1.8/finbourne_identity/exceptions.py
--rw-r--r--   0        0        0      599 2024-04-16 17:50:38.268621 finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/__init__.py
--rw-r--r--   0        0        0    30692 2024-04-16 17:50:38.268621 finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/api_client.py
--rw-r--r--   0        0        0     9902 2024-04-16 17:50:38.267621 finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8117 2024-04-16 17:50:38.268621 finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/api_configuration.py
--rw-r--r--   0        0        0     6812 2024-04-16 17:50:38.268621 finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-04-16 17:50:38.268621 finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-04-16 17:50:38.268621 finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12711 2024-04-16 17:50:38.268621 finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/rest.py
--rw-r--r--   0        0        0    11577 2024-04-16 17:50:38.268621 finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-04-16 17:50:38.268621 finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3890 2024-04-16 17:50:38.268621 finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     5374 2024-04-16 17:50:38.266621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/__init__.py
--rw-r--r--   0        0        0     3923 2024-04-16 17:50:38.262621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/access_controlled_action.py
--rw-r--r--   0        0        0     4866 2024-04-16 17:50:38.262621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2078 2024-04-16 17:50:38.262621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/action_id.py
--rw-r--r--   0        0        0     2436 2024-04-16 17:50:38.262621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/add_scim_response.py
--rw-r--r--   0        0        0     3349 2024-04-16 17:50:38.262621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/api_key.py
--rw-r--r--   0        0        0     5239 2024-04-16 17:50:38.263621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/authentication_information.py
--rw-r--r--   0        0        0     2784 2024-04-16 17:50:38.263621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/create_api_key.py
--rw-r--r--   0        0        0     4489 2024-04-16 17:50:38.263621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/create_application_request.py
--rw-r--r--   0        0        0     3118 2024-04-16 17:50:38.263621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/create_role_request.py
--rw-r--r--   0        0        0     5261 2024-04-16 17:50:38.263621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/create_user_request.py
--rw-r--r--   0        0        0     3526 2024-04-16 17:50:38.263621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/created_api_key.py
--rw-r--r--   0        0        0     3521 2024-04-16 17:50:38.263621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/current_user_response.py
--rw-r--r--   0        0        0     2776 2024-04-16 17:50:38.263621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/error_detail.py
--rw-r--r--   0        0        0     3192 2024-04-16 17:50:38.263621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/id_selector_definition.py
--rw-r--r--   0        0        0     3117 2024-04-16 17:50:38.263621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2270 2024-04-16 17:50:38.263621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/link.py
--rw-r--r--   0        0        0     4744 2024-04-16 17:50:38.263621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/list_users_response.py
--rw-r--r--   0        0        0     3865 2024-04-16 17:50:38.263621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4701 2024-04-16 17:50:38.264621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     2990 2024-04-16 17:50:38.264621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/o_auth_application.py
--rw-r--r--   0        0        0     2302 2024-04-16 17:50:38.264621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/password_policy_response.py
--rw-r--r--   0        0        0     2311 2024-04-16 17:50:38.264621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/password_policy_response_age.py
--rw-r--r--   0        0        0     2577 2024-04-16 17:50:38.264621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/password_policy_response_complexity.py
--rw-r--r--   0        0        0     3282 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/password_policy_response_conditions.py
--rw-r--r--   0        0        0     2104 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/password_policy_response_lockout.py
--rw-r--r--   0        0        0     4271 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     1922 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/role_id.py
--rw-r--r--   0        0        0     3430 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/role_response.py
--rw-r--r--   0        0        0     1912 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/set_password.py
--rw-r--r--   0        0        0     2770 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/set_password_response.py
--rw-r--r--   0        0        0     1993 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/support_access_expiry.py
--rw-r--r--   0        0        0     2388 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/support_access_expiry_with_role.py
--rw-r--r--   0        0        0     3923 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/support_access_request.py
--rw-r--r--   0        0        0     5257 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/support_access_response.py
--rw-r--r--   0        0        0     3186 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/support_role.py
--rw-r--r--   0        0        0     2681 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/support_roles_response.py
--rw-r--r--   0        0        0     1933 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/temporary_password.py
--rw-r--r--   0        0        0     2363 2024-04-16 17:50:38.265621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/update_password_policy_request.py
--rw-r--r--   0        0        0     2437 2024-04-16 17:50:38.266621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/update_password_policy_request_age.py
--rw-r--r--   0        0        0     2638 2024-04-16 17:50:38.266621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/update_password_policy_request_complexity.py
--rw-r--r--   0        0        0     3380 2024-04-16 17:50:38.266621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/update_password_policy_request_conditions.py
--rw-r--r--   0        0        0     2188 2024-04-16 17:50:38.266621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/update_password_policy_request_lockout.py
--rw-r--r--   0        0        0     2557 2024-04-16 17:50:38.266621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/update_role_request.py
--rw-r--r--   0        0        0     4752 2024-04-16 17:50:38.266621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/update_user_request.py
--rw-r--r--   0        0        0     5148 2024-04-16 17:50:38.266621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/user_response.py
--rw-r--r--   0        0        0     4920 2024-04-16 17:50:38.266621 finbourne_identity_sdk-2.1.8/finbourne_identity/models/user_summary.py
--rw-r--r--   0        0        0        0 2024-04-16 17:50:38.267621 finbourne_identity_sdk-2.1.8/finbourne_identity/py.typed
--rw-r--r--   0        0        0    10172 2024-04-16 17:50:38.262621 finbourne_identity_sdk-2.1.8/finbourne_identity/rest.py
--rw-r--r--   0        0        0      897 2024-04-16 17:50:38.272621 finbourne_identity_sdk-2.1.8/pyproject.toml
--rw-r--r--   0        0        0    16710 1970-01-01 00:00:00.000000 finbourne_identity_sdk-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0    15621 2024-04-16 18:37:15.455812 finbourne_identity_sdk-2.1.9/README.md
+-rw-r--r--   0        0        0     7317 2024-04-16 18:37:15.451812 finbourne_identity_sdk-2.1.9/finbourne_identity/__init__.py
+-rw-r--r--   0        0        0      882 2024-04-16 18:37:15.451812 finbourne_identity_sdk-2.1.9/finbourne_identity/api/__init__.py
+-rw-r--r--   0        0        0     7528 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/api/application_metadata_api.py
+-rw-r--r--   0        0        0    36614 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/api/applications_api.py
+-rw-r--r--   0        0        0    53621 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/api/authentication_api.py
+-rw-r--r--   0        0        0    15596 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/api/identity_provider_api.py
+-rw-r--r--   0        0        0    14825 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/api/me_api.py
+-rw-r--r--   0        0        0    21760 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/api/personal_authentication_tokens_api.py
+-rw-r--r--   0        0        0    57442 2024-04-16 18:37:15.451812 finbourne_identity_sdk-2.1.9/finbourne_identity/api/roles_api.py
+-rw-r--r--   0        0        0     6867 2024-04-16 18:37:15.451812 finbourne_identity_sdk-2.1.9/finbourne_identity/api/tokens_api.py
+-rw-r--r--   0        0        0    95281 2024-04-16 18:37:15.451812 finbourne_identity_sdk-2.1.9/finbourne_identity/api/users_api.py
+-rw-r--r--   0        0        0    30821 2024-04-16 18:37:15.451812 finbourne_identity_sdk-2.1.9/finbourne_identity/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-16 18:37:15.451812 finbourne_identity_sdk-2.1.9/finbourne_identity/api_response.py
+-rw-r--r--   0        0        0    14468 2024-04-16 18:37:15.451812 finbourne_identity_sdk-2.1.9/finbourne_identity/configuration.py
+-rw-r--r--   0        0        0     5347 2024-04-16 18:37:15.451812 finbourne_identity_sdk-2.1.9/finbourne_identity/exceptions.py
+-rw-r--r--   0        0        0      599 2024-04-16 18:37:15.452812 finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/__init__.py
+-rw-r--r--   0        0        0    30692 2024-04-16 18:37:15.452812 finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/api_client.py
+-rw-r--r--   0        0        0     9902 2024-04-16 18:37:15.451812 finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8117 2024-04-16 18:37:15.451812 finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6812 2024-04-16 18:37:15.451812 finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-16 18:37:15.452812 finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-16 18:37:15.452812 finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12711 2024-04-16 18:37:15.452812 finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/rest.py
+-rw-r--r--   0        0        0    11577 2024-04-16 18:37:15.452812 finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-16 18:37:15.452812 finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3890 2024-04-16 18:37:15.452812 finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     5374 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/__init__.py
+-rw-r--r--   0        0        0     3923 2024-04-16 18:37:15.447812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4866 2024-04-16 18:37:15.447812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2078 2024-04-16 18:37:15.447812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/action_id.py
+-rw-r--r--   0        0        0     2436 2024-04-16 18:37:15.447812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/add_scim_response.py
+-rw-r--r--   0        0        0     3349 2024-04-16 18:37:15.447812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/api_key.py
+-rw-r--r--   0        0        0     5239 2024-04-16 18:37:15.447812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/authentication_information.py
+-rw-r--r--   0        0        0     2784 2024-04-16 18:37:15.447812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/create_api_key.py
+-rw-r--r--   0        0        0     4489 2024-04-16 18:37:15.447812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/create_application_request.py
+-rw-r--r--   0        0        0     3118 2024-04-16 18:37:15.447812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/create_role_request.py
+-rw-r--r--   0        0        0     5261 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/create_user_request.py
+-rw-r--r--   0        0        0     3526 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/created_api_key.py
+-rw-r--r--   0        0        0     3521 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/current_user_response.py
+-rw-r--r--   0        0        0     2776 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/error_detail.py
+-rw-r--r--   0        0        0     3192 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3117 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2270 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/link.py
+-rw-r--r--   0        0        0     4744 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/list_users_response.py
+-rw-r--r--   0        0        0     3865 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4701 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     2990 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/o_auth_application.py
+-rw-r--r--   0        0        0     2302 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/password_policy_response.py
+-rw-r--r--   0        0        0     2311 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/password_policy_response_age.py
+-rw-r--r--   0        0        0     2577 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/password_policy_response_complexity.py
+-rw-r--r--   0        0        0     3282 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/password_policy_response_conditions.py
+-rw-r--r--   0        0        0     2104 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/password_policy_response_lockout.py
+-rw-r--r--   0        0        0     4271 2024-04-16 18:37:15.448812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     1922 2024-04-16 18:37:15.449812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/role_id.py
+-rw-r--r--   0        0        0     3430 2024-04-16 18:37:15.449812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/role_response.py
+-rw-r--r--   0        0        0     1912 2024-04-16 18:37:15.449812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/set_password.py
+-rw-r--r--   0        0        0     2770 2024-04-16 18:37:15.449812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/set_password_response.py
+-rw-r--r--   0        0        0     1993 2024-04-16 18:37:15.449812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/support_access_expiry.py
+-rw-r--r--   0        0        0     2388 2024-04-16 18:37:15.449812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/support_access_expiry_with_role.py
+-rw-r--r--   0        0        0     3923 2024-04-16 18:37:15.449812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/support_access_request.py
+-rw-r--r--   0        0        0     5257 2024-04-16 18:37:15.449812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/support_access_response.py
+-rw-r--r--   0        0        0     3186 2024-04-16 18:37:15.449812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/support_role.py
+-rw-r--r--   0        0        0     2681 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/support_roles_response.py
+-rw-r--r--   0        0        0     1933 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/temporary_password.py
+-rw-r--r--   0        0        0     2363 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/update_password_policy_request.py
+-rw-r--r--   0        0        0     2437 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/update_password_policy_request_age.py
+-rw-r--r--   0        0        0     2638 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/update_password_policy_request_complexity.py
+-rw-r--r--   0        0        0     3380 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/update_password_policy_request_conditions.py
+-rw-r--r--   0        0        0     2188 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/update_password_policy_request_lockout.py
+-rw-r--r--   0        0        0     2557 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/update_role_request.py
+-rw-r--r--   0        0        0     4752 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/update_user_request.py
+-rw-r--r--   0        0        0     5148 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/user_response.py
+-rw-r--r--   0        0        0     4920 2024-04-16 18:37:15.450812 finbourne_identity_sdk-2.1.9/finbourne_identity/models/user_summary.py
+-rw-r--r--   0        0        0        0 2024-04-16 18:37:15.451812 finbourne_identity_sdk-2.1.9/finbourne_identity/py.typed
+-rw-r--r--   0        0        0    10172 2024-04-16 18:37:15.451812 finbourne_identity_sdk-2.1.9/finbourne_identity/rest.py
+-rw-r--r--   0        0        0      897 2024-04-16 18:37:15.455812 finbourne_identity_sdk-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0    16710 1970-01-01 00:00:00.000000 finbourne_identity_sdk-2.1.9/PKG-INFO
```

### Comparing `finbourne_identity_sdk-2.1.8/README.md` & `finbourne_identity_sdk-2.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # finbourne-identity-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.2874
-- Package version: 2.1.8
+- API version: 0.0.2876
+- Package version: 2.1.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/__init__.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/api/__init__.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/api/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/api/application_metadata_api.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/api/applications_api.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/api/applications_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/api/authentication_api.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/api/identity_provider_api.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/api/identity_provider_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/api/me_api.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/api/me_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/api/personal_authentication_tokens_api.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/api/personal_authentication_tokens_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/api/roles_api.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/api/roles_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/api/tokens_api.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/api/tokens_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/api/users_api.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/api/users_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/api_client.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/api_response.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/api_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/configuration.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("finbourne_identity-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.2874\n"\
+               "Version of the API: 0.0.2876\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/exceptions.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/exceptions.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/__init__.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/api_client.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/api_client_factory.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/api_configuration.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/configuration_loaders.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/proxy_config.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/refreshing_token.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/rest.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/retry.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/socket_keep_alive.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/extensions/tcp_keep_alive_connector.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/__init__.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/access_controlled_action.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/access_controlled_resource.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/action_id.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/action_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/add_scim_response.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/add_scim_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/api_key.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/api_key.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/authentication_information.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/authentication_information.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/create_api_key.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/create_api_key.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/create_application_request.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/create_application_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/create_role_request.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/create_role_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/create_user_request.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/create_user_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/created_api_key.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/created_api_key.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/current_user_response.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/current_user_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/error_detail.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/error_detail.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/id_selector_definition.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/identifier_part_schema.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/link.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/link.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/list_users_response.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/list_users_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/lusid_problem_details.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/lusid_validation_problem_details.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/o_auth_application.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/o_auth_application.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/password_policy_response.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/password_policy_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/password_policy_response_age.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/password_policy_response_age.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/password_policy_response_complexity.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/password_policy_response_complexity.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/password_policy_response_conditions.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/password_policy_response_conditions.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/password_policy_response_lockout.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/password_policy_response_lockout.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/resource_list_of_access_controlled_resource.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/role_id.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/role_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/role_response.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/role_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/set_password.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/set_password.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/set_password_response.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/set_password_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/support_access_expiry.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/support_access_expiry.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/support_access_expiry_with_role.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/support_access_expiry_with_role.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/support_access_request.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/support_access_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/support_access_response.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/support_access_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/support_role.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/support_role.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/support_roles_response.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/support_roles_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/temporary_password.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/temporary_password.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/update_password_policy_request.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/update_password_policy_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/update_password_policy_request_age.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/update_password_policy_request_age.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/update_password_policy_request_complexity.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/update_password_policy_request_complexity.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/update_password_policy_request_conditions.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/update_password_policy_request_conditions.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/update_password_policy_request_lockout.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/update_password_policy_request_lockout.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/update_role_request.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/update_role_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/update_user_request.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/update_user_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/user_response.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/user_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/models/user_summary.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/models/user_summary.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/finbourne_identity/rest.py` & `finbourne_identity_sdk-2.1.9/finbourne_identity/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.1.8/pyproject.toml` & `finbourne_identity_sdk-2.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finbourne-identity-sdk"
-version = "2.1.8"
+version = "2.1.9"
 description = "FINBOURNE Identity Service API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/finbourne-identity-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Identity Service API", "finbourne-identity-sdk"]
 packages = [
```

### Comparing `finbourne_identity_sdk-2.1.8/PKG-INFO` & `finbourne_identity_sdk-2.1.9/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finbourne-identity-sdk
-Version: 2.1.8
+Version: 2.1.9
 Summary: FINBOURNE Identity Service API
 Home-page: https://github.com/finbourne/finbourne-identity-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Identity Service API,finbourne-identity-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # finbourne-identity-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.2874
-- Package version: 2.1.8
+- API version: 0.0.2876
+- Package version: 2.1.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

