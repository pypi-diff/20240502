# Comparing `tmp/lusid_notifications_sdk-2.1.1.tar.gz` & `tmp/lusid_notifications_sdk-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_notifications_sdk-2.1.1.tar", max compression
+gzip compressed data, was "lusid_notifications_sdk-2.1.2.tar", max compression
```

## Comparing `lusid_notifications_sdk-2.1.1.tar` & `lusid_notifications_sdk-2.1.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    11699 2024-04-10 10:43:04.950297 lusid_notifications_sdk-2.1.1/README.md
--rw-r--r--   0        0        0     6885 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/__init__.py
--rw-r--r--   0        0        0      629 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/api/__init__.py
--rw-r--r--   0        0        0     7559 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/api/application_metadata_api.py
--rw-r--r--   0        0        0    13222 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/api/deliveries_api.py
--rw-r--r--   0        0        0    14134 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/api/event_types_api.py
--rw-r--r--   0        0        0     8484 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/api/manual_event_api.py
--rw-r--r--   0        0        0    45089 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/api/notifications_api.py
--rw-r--r--   0        0        0    44727 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/api/subscriptions_api.py
--rw-r--r--   0        0        0    30825 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/api_client.py
--rw-r--r--   0        0        0      852 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/api_response.py
--rw-r--r--   0        0        0    14474 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/configuration.py
--rw-r--r--   0        0        0     5344 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/exceptions.py
--rw-r--r--   0        0        0      602 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/__init__.py
--rw-r--r--   0        0        0    30697 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/api_client.py
--rw-r--r--   0        0        0     9912 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8122 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/api_configuration.py
--rw-r--r--   0        0        0     6816 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12712 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/rest.py
--rw-r--r--   0        0        0    11578 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3891 2024-04-10 10:43:04.947297 lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     5187 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/__init__.py
--rw-r--r--   0        0        0     3923 2024-04-10 10:43:04.942297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/access_controlled_action.py
--rw-r--r--   0        0        0     4866 2024-04-10 10:43:04.942297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2075 2024-04-10 10:43:04.942297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/action_id.py
--rw-r--r--   0        0        0     3498 2024-04-10 10:43:04.942297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/amazon_sqs_notification_type.py
--rw-r--r--   0        0        0     3925 2024-04-10 10:43:04.942297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/amazon_sqs_notification_type_response.py
--rw-r--r--   0        0        0     3109 2024-04-10 10:43:04.942297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/amazon_sqs_principal_auth_notification_type.py
--rw-r--r--   0        0        0     3188 2024-04-10 10:43:04.942297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/amazon_sqs_principal_auth_notification_type_response.py
--rw-r--r--   0        0        0     2522 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/attempt.py
--rw-r--r--   0        0        0     2415 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/attempt_status.py
--rw-r--r--   0        0        0     4251 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/create_notification_request.py
--rw-r--r--   0        0        0     5204 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/create_subscription.py
--rw-r--r--   0        0        0     3816 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/delivery.py
--rw-r--r--   0        0        0     5208 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/email_notification_type.py
--rw-r--r--   0        0        0     4820 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/email_notification_type_response.py
--rw-r--r--   0        0        0     2462 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/event_field_definition.py
--rw-r--r--   0        0        0     5527 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/event_type_schema.py
--rw-r--r--   0        0        0     3190 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/id_selector_definition.py
--rw-r--r--   0        0        0     3115 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2267 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/link.py
--rw-r--r--   0        0        0     3862 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4698 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     2533 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event.py
--rw-r--r--   0        0        0     3132 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event_body.py
--rw-r--r--   0        0        0     3199 2024-04-10 10:43:04.943297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event_header.py
--rw-r--r--   0        0        0     2191 2024-04-10 10:43:04.944297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event_request.py
--rw-r--r--   0        0        0     3244 2024-04-10 10:43:04.944297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/matching_pattern.py
--rw-r--r--   0        0        0     5026 2024-04-10 10:43:04.944297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification.py
--rw-r--r--   0        0        0     2407 2024-04-10 10:43:04.944297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification_status.py
--rw-r--r--   0        0        0     8333 2024-04-10 10:43:04.944297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification_type.py
--rw-r--r--   0        0        0     9013 2024-04-10 10:43:04.944297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification_type_response.py
--rw-r--r--   0        0        0     2082 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_id.py
--rw-r--r--   0        0        0     4270 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4076 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_delivery.py
--rw-r--r--   0        0        0     4162 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_event_type_schema.py
--rw-r--r--   0        0        0     4124 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_notification.py
--rw-r--r--   0        0        0     4124 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_subscription.py
--rw-r--r--   0        0        0     2914 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/sms_notification_type.py
--rw-r--r--   0        0        0     3007 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/sms_notification_type_response.py
--rw-r--r--   0        0        0     4773 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/subscription.py
--rw-r--r--   0        0        0     3704 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/update_notification_request.py
--rw-r--r--   0        0        0     4865 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/update_subscription.py
--rw-r--r--   0        0        0     5545 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/webhook_notification_type.py
--rw-r--r--   0        0        0     5675 2024-04-10 10:43:04.945297 lusid_notifications_sdk-2.1.1/lusid_notifications/models/webhook_notification_type_response.py
--rw-r--r--   0        0        0        0 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/py.typed
--rw-r--r--   0        0        0    10170 2024-04-10 10:43:04.946297 lusid_notifications_sdk-2.1.1/lusid_notifications/rest.py
--rw-r--r--   0        0        0      890 2024-04-10 10:43:04.951297 lusid_notifications_sdk-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    12774 1970-01-01 00:00:00.000000 lusid_notifications_sdk-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11699 2024-05-01 18:06:04.960438 lusid_notifications_sdk-2.1.2/README.md
+-rw-r--r--   0        0        0     6885 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/__init__.py
+-rw-r--r--   0        0        0      629 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/api/__init__.py
+-rw-r--r--   0        0        0     7559 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/api/application_metadata_api.py
+-rw-r--r--   0        0        0    13222 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/api/deliveries_api.py
+-rw-r--r--   0        0        0    14134 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/api/event_types_api.py
+-rw-r--r--   0        0        0     8484 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/api/manual_event_api.py
+-rw-r--r--   0        0        0    45089 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/api/notifications_api.py
+-rw-r--r--   0        0        0    44727 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/api/subscriptions_api.py
+-rw-r--r--   0        0        0    30825 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/api_response.py
+-rw-r--r--   0        0        0    14474 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/configuration.py
+-rw-r--r--   0        0        0     5344 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/exceptions.py
+-rw-r--r--   0        0        0      602 2024-05-01 18:06:04.958438 lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/__init__.py
+-rw-r--r--   0        0        0    30697 2024-05-01 18:06:04.958438 lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/api_client.py
+-rw-r--r--   0        0        0     9912 2024-05-01 18:06:04.958438 lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8122 2024-05-01 18:06:04.958438 lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6816 2024-05-01 18:06:04.958438 lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-05-01 18:06:04.958438 lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-05-01 18:06:04.958438 lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12712 2024-05-01 18:06:04.958438 lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/rest.py
+-rw-r--r--   0        0        0    11578 2024-05-01 18:06:04.958438 lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-05-01 18:06:04.958438 lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3891 2024-05-01 18:06:04.958438 lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     5187 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/__init__.py
+-rw-r--r--   0        0        0     3923 2024-05-01 18:06:04.954438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4866 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2075 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/action_id.py
+-rw-r--r--   0        0        0     3498 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/amazon_sqs_notification_type.py
+-rw-r--r--   0        0        0     3925 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/amazon_sqs_notification_type_response.py
+-rw-r--r--   0        0        0     3109 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/amazon_sqs_principal_auth_notification_type.py
+-rw-r--r--   0        0        0     3188 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/amazon_sqs_principal_auth_notification_type_response.py
+-rw-r--r--   0        0        0     2522 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/attempt.py
+-rw-r--r--   0        0        0     2415 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/attempt_status.py
+-rw-r--r--   0        0        0     4251 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/create_notification_request.py
+-rw-r--r--   0        0        0     5204 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/create_subscription.py
+-rw-r--r--   0        0        0     3816 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/delivery.py
+-rw-r--r--   0        0        0     5208 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/email_notification_type.py
+-rw-r--r--   0        0        0     4820 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/email_notification_type_response.py
+-rw-r--r--   0        0        0     2462 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/event_field_definition.py
+-rw-r--r--   0        0        0     5527 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/event_type_schema.py
+-rw-r--r--   0        0        0     3190 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3115 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2267 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/link.py
+-rw-r--r--   0        0        0     3862 2024-05-01 18:06:04.955438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4698 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     2533 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/manual_event.py
+-rw-r--r--   0        0        0     3132 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/manual_event_body.py
+-rw-r--r--   0        0        0     3199 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/manual_event_header.py
+-rw-r--r--   0        0        0     2191 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/manual_event_request.py
+-rw-r--r--   0        0        0     3244 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/matching_pattern.py
+-rw-r--r--   0        0        0     5026 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/notification.py
+-rw-r--r--   0        0        0     2407 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/notification_status.py
+-rw-r--r--   0        0        0     8333 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/notification_type.py
+-rw-r--r--   0        0        0     9013 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/notification_type_response.py
+-rw-r--r--   0        0        0     2082 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/resource_id.py
+-rw-r--r--   0        0        0     4270 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4076 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/resource_list_of_delivery.py
+-rw-r--r--   0        0        0     4162 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0        0        0     4124 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/resource_list_of_notification.py
+-rw-r--r--   0        0        0     4124 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/resource_list_of_subscription.py
+-rw-r--r--   0        0        0     2914 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/sms_notification_type.py
+-rw-r--r--   0        0        0     3007 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/sms_notification_type_response.py
+-rw-r--r--   0        0        0     4773 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/subscription.py
+-rw-r--r--   0        0        0     3704 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/update_notification_request.py
+-rw-r--r--   0        0        0     4865 2024-05-01 18:06:04.956438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/update_subscription.py
+-rw-r--r--   0        0        0     5545 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/webhook_notification_type.py
+-rw-r--r--   0        0        0     5675 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/models/webhook_notification_type_response.py
+-rw-r--r--   0        0        0        0 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/py.typed
+-rw-r--r--   0        0        0    10170 2024-05-01 18:06:04.957438 lusid_notifications_sdk-2.1.2/lusid_notifications/rest.py
+-rw-r--r--   0        0        0      890 2024-05-01 18:06:04.961438 lusid_notifications_sdk-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0    12774 1970-01-01 00:00:00.000000 lusid_notifications_sdk-2.1.2/PKG-INFO
```

### Comparing `lusid_notifications_sdk-2.1.1/README.md` & `lusid_notifications_sdk-2.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notifications-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.929
-- Package version: 2.1.1
+- API version: 0.1.930
+- Package version: 2.1.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/__init__.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/api/__init__.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/api/application_metadata_api.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/api/deliveries_api.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/api/deliveries_api.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/api/event_types_api.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/api/event_types_api.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/api/manual_event_api.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/api/manual_event_api.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/api/notifications_api.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/api/notifications_api.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/api/subscriptions_api.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/api/subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/api_client.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/api_response.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/configuration.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid_notifications-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.929\n"\
+               "Version of the API: 0.1.930\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/exceptions.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/__init__.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/api_client.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/api_client_factory.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/api_configuration.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/configuration_loaders.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/proxy_config.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/refreshing_token.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/rest.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/retry.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/socket_keep_alive.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/extensions/tcp_keep_alive_connector.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/__init__.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/access_controlled_action.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/access_controlled_resource.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/action_id.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/action_id.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/amazon_sqs_notification_type.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/amazon_sqs_notification_type.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/amazon_sqs_notification_type_response.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/amazon_sqs_notification_type_response.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/amazon_sqs_principal_auth_notification_type.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/amazon_sqs_principal_auth_notification_type.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/amazon_sqs_principal_auth_notification_type_response.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/amazon_sqs_principal_auth_notification_type_response.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/attempt.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/attempt.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/attempt_status.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/attempt_status.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/create_notification_request.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/create_notification_request.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/create_subscription.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/create_subscription.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/delivery.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/delivery.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/email_notification_type.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/email_notification_type.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/email_notification_type_response.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/email_notification_type_response.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/event_field_definition.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/event_field_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/event_type_schema.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/event_type_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/id_selector_definition.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/identifier_part_schema.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/link.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/link.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/lusid_problem_details.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/lusid_validation_problem_details.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/manual_event.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event_body.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/manual_event_body.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event_header.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/manual_event_header.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/manual_event_request.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/manual_event_request.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/matching_pattern.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/matching_pattern.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/notification.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification_status.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/notification_status.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification_type.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/notification_type.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/notification_type_response.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/notification_type_response.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_id.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_access_controlled_resource.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_delivery.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/resource_list_of_delivery.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_event_type_schema.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/resource_list_of_event_type_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_notification.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/resource_list_of_notification.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/resource_list_of_subscription.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/resource_list_of_subscription.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/sms_notification_type.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/sms_notification_type.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/sms_notification_type_response.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/sms_notification_type_response.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/subscription.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/subscription.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/update_notification_request.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/update_notification_request.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/update_subscription.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/update_subscription.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/webhook_notification_type.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/webhook_notification_type.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/models/webhook_notification_type_response.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/models/webhook_notification_type_response.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/lusid_notifications/rest.py` & `lusid_notifications_sdk-2.1.2/lusid_notifications/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_notifications_sdk-2.1.1/pyproject.toml` & `lusid_notifications_sdk-2.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-notifications-sdk"
-version = "2.1.1"
+version = "2.1.2"
 description = "FINBOURNE Notifications API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/notifications-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Notifications API", "lusid-notifications-sdk"]
 packages = [
```

### Comparing `lusid_notifications_sdk-2.1.1/PKG-INFO` & `lusid_notifications_sdk-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-notifications-sdk
-Version: 2.1.1
+Version: 2.1.2
 Summary: FINBOURNE Notifications API
 Home-page: https://github.com/finbourne/notifications-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Notifications API,lusid-notifications-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # lusid-notifications-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.929
-- Package version: 2.1.1
+- API version: 0.1.930
+- Package version: 2.1.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

