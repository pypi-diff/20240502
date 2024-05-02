# Comparing `tmp/moneykit-0.1.7.tar.gz` & `tmp/moneykit-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneykit-0.1.7.tar", max compression
+gzip compressed data, was "moneykit-0.1.8.tar", max compression
```

## Comparing `moneykit-0.1.7.tar` & `moneykit-0.1.8.tar`

### file list

```diff
@@ -1,148 +1,148 @@
--rw-r--r--   0        0        0     2640 2024-01-09 15:08:14.318040 moneykit-0.1.7/README.md
--rw-r--r--   0        0        0    11735 2024-01-09 15:08:14.318040 moneykit-0.1.7/moneykit/__init__.py
--rw-r--r--   0        0        0      684 2024-01-09 15:08:14.318040 moneykit-0.1.7/moneykit/api/__init__.py
--rw-r--r--   0        0        0    36162 2024-01-09 15:08:14.318040 moneykit-0.1.7/moneykit/api/access_token_api.py
--rw-r--r--   0        0        0    14982 2024-01-09 15:08:14.318040 moneykit-0.1.7/moneykit/api/account_numbers_api.py
--rw-r--r--   0        0        0    52772 2024-01-09 15:08:14.318040 moneykit-0.1.7/moneykit/api/accounts_api.py
--rw-r--r--   0        0        0    16125 2024-01-09 15:08:14.318040 moneykit-0.1.7/moneykit/api/identity_api.py
--rw-r--r--   0        0        0    26098 2024-01-09 15:08:14.318040 moneykit-0.1.7/moneykit/api/institutions_api.py
--rw-r--r--   0        0        0    36018 2024-01-09 15:08:14.318040 moneykit-0.1.7/moneykit/api/investments_api.py
--rw-r--r--   0        0        0    23893 2024-01-09 15:08:14.318040 moneykit-0.1.7/moneykit/api/link_session_api.py
--rw-r--r--   0        0        0    54809 2024-01-09 15:08:14.318040 moneykit-0.1.7/moneykit/api/links_api.py
--rw-r--r--   0        0        0    13400 2024-01-09 15:08:14.318040 moneykit-0.1.7/moneykit/api/products_api.py
--rw-r--r--   0        0        0    63001 2024-01-09 15:08:14.318040 moneykit-0.1.7/moneykit/api/transactions_api.py
--rw-r--r--   0        0        0    48800 2024-01-09 15:08:14.318040 moneykit-0.1.7/moneykit/api/users_api.py
--rw-r--r--   0        0        0    13480 2024-01-09 15:08:14.318040 moneykit-0.1.7/moneykit/api/webhooks_api.py
--rw-r--r--   0        0        0    24258 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/api_client.py
--rw-r--r--   0        0        0      670 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/api_response.py
--rw-r--r--   0        0        0    15031 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/configuration.py
--rw-r--r--   0        0        0     5401 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/exceptions.py
--rw-r--r--   0        0        0    10608 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/__init__.py
--rw-r--r--   0        0        0     5070 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/account.py
--rw-r--r--   0        0        0     4447 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/account_balances.py
--rw-r--r--   0        0        0     3764 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/account_group.py
--rw-r--r--   0        0        0     5643 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/account_identity.py
--rw-r--r--   0        0        0     5185 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/account_numbers.py
--rw-r--r--   0        0        0     4522 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/account_numbers_link_product.py
--rw-r--r--   0        0        0     3715 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/account_numbers_product_settings.py
--rw-r--r--   0        0        0     5562 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/account_with_account_numbers.py
--rw-r--r--   0        0        0     3998 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/accounts_link_product.py
--rw-r--r--   0        0        0     3470 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/ach_number.py
--rw-r--r--   0        0        0     4134 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/address.py
--rw-r--r--   0        0        0     4158 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/api_error_auth_expired_access_token_response.py
--rw-r--r--   0        0        0     3946 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/api_error_auth_unauthorized_response.py
--rw-r--r--   0        0        0     4112 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/api_error_rate_limit_exceeded_response.py
--rw-r--r--   0        0        0     3193 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/bacs_number.py
--rw-r--r--   0        0        0     3858 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/basic_account_details.py
--rw-r--r--   0        0        0     6364 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/body.py
--rw-r--r--   0        0        0      831 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/country.py
--rw-r--r--   0        0        0     6248 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/create_link_session_request.py
--rw-r--r--   0        0        0     3129 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/create_link_session_response.py
--rw-r--r--   0        0        0     3875 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/currency.py
--rw-r--r--   0        0        0     3073 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/cursor_pagination.py
--rw-r--r--   0        0        0     3131 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/customer_app.py
--rw-r--r--   0        0        0     3412 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/eft_number.py
--rw-r--r--   0        0        0     3360 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/email.py
--rw-r--r--   0        0        0     3133 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/exchange_token_request.py
--rw-r--r--   0        0        0     3472 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/exchange_token_response.py
--rw-r--r--   0        0        0     3455 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/generate_access_token_response.py
--rw-r--r--   0        0        0     3997 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/get_account_numbers_response.py
--rw-r--r--   0        0        0     3660 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/get_account_response.py
--rw-r--r--   0        0        0     3840 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/get_accounts_response.py
--rw-r--r--   0        0        0     5122 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/get_holdings_response.py
--rw-r--r--   0        0        0     3997 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/get_institutions_response.py
--rw-r--r--   0        0        0     5931 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/get_investment_transactions_response.py
--rw-r--r--   0        0        0     5029 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/get_transactions_response.py
--rw-r--r--   0        0        0     3303 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/get_user_accounts_response.py
--rw-r--r--   0        0        0     3278 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/get_user_links_response.py
--rw-r--r--   0        0        0     4374 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/get_user_transactions_response.py
--rw-r--r--   0        0        0     4560 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/holding_response.py
--rw-r--r--   0        0        0     4829 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/http_validation_error.py
--rw-r--r--   0        0        0     4464 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/identity_link_product.py
--rw-r--r--   0        0        0     3691 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/identity_product_settings.py
--rw-r--r--   0        0        0     3899 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/identity_response.py
--rw-r--r--   0        0        0     4411 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/institution.py
--rw-r--r--   0        0        0     4019 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/institution_error_not_found_response.py
--rw-r--r--   0        0        0     3080 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/international_number.py
--rw-r--r--   0        0        0     4099 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/introspect_client_response.py
--rw-r--r--   0        0        0     6641 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/investment_transaction_response.py
--rw-r--r--   0        0        0     4488 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/investments_link_product.py
--rw-r--r--   0        0        0     3703 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/investments_product_settings.py
--rw-r--r--   0        0        0     2895 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/jwk_set.py
--rw-r--r--   0        0        0     4821 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_common.py
--rw-r--r--   0        0        0     1003 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_error.py
--rw-r--r--   0        0        0     3801 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_error_bad_config_response.py
--rw-r--r--   0        0        0     3903 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_error_bad_state_response.py
--rw-r--r--   0        0        0     3903 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_error_deleted_response.py
--rw-r--r--   0        0        0     3946 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_error_forbidden_action_response.py
--rw-r--r--   0        0        0     3921 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_error_not_found_response.py
--rw-r--r--   0        0        0     4051 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_error_unauthorized_access_response.py
--rw-r--r--   0        0        0     1024 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_permission_scope.py
--rw-r--r--   0        0        0     3587 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_permissions.py
--rw-r--r--   0        0        0     1021 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_product_failure_reasons.py
--rw-r--r--   0        0        0     5697 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_product_refresh_webhook.py
--rw-r--r--   0        0        0      857 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_product_state.py
--rw-r--r--   0        0        0     5491 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_products.py
--rw-r--r--   0        0        0     5156 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_response.py
--rw-r--r--   0        0        0     4534 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_session_customer_user.py
--rw-r--r--   0        0        0     4099 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_session_customer_user_email.py
--rw-r--r--   0        0        0     4294 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_session_customer_user_phone.py
--rw-r--r--   0        0        0     4006 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_session_error_forbidden_config_response.py
--rw-r--r--   0        0        0     4018 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_session_error_invalid_token_exchange.py
--rw-r--r--   0        0        0     4302 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_session_setting_overrides.py
--rw-r--r--   0        0        0      951 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_state.py
--rw-r--r--   0        0        0     5549 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/link_state_changed_webhook.py
--rw-r--r--   0        0        0     3671 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/money_kit_connect_features.py
--rw-r--r--   0        0        0     4783 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/owner.py
--rw-r--r--   0        0        0     3514 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/phone_number.py
--rw-r--r--   0        0        0      883 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/phone_number_type.py
--rw-r--r--   0        0        0      962 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/product.py
--rw-r--r--   0        0        0     5151 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/products_settings.py
--rw-r--r--   0        0        0      945 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/provider.py
--rw-r--r--   0        0        0     1010 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/public_link_error.py
--rw-r--r--   0        0        0     3004 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/refresh_products_request.py
--rw-r--r--   0        0        0     3930 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/requested_link_permission.py
--rw-r--r--   0        0        0     6970 2024-01-09 15:08:14.322040 moneykit-0.1.7/moneykit/models/response401_disconnect_links_id_delete.py
--rw-r--r--   0        0        0     6024 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_exchange_token_link_session_exchange_token_post.py
--rw-r--r--   0        0        0     7068 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_account_links_id_accounts_account_id_get.py
--rw-r--r--   0        0        0     7127 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_account_numbers_links_id_accounts_numbers_get.py
--rw-r--r--   0        0        0     7012 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_accounts_links_id_accounts_get.py
--rw-r--r--   0        0        0     7089 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_holdings_links_id_investments_holdings_get.py
--rw-r--r--   0        0        0     7026 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_identities_links_id_identity_get.py
--rw-r--r--   0        0        0     6031 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_institution_institutions_institution_id_get.py
--rw-r--r--   0        0        0     5923 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_institutions_institutions_get.py
--rw-r--r--   0        0        0     7215 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_investment_transactions_links_id_investments_transactions_get.py
--rw-r--r--   0        0        0     6914 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_link_links_id_get.py
--rw-r--r--   0        0        0     6900 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_transactions.py
--rw-r--r--   0        0        0     7148 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_transactions_diff_links_id_transactions_sync_get.py
--rw-r--r--   0        0        0     7063 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_transactions_links_id_transactions_get.py
--rw-r--r--   0        0        0     5944 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_user_accounts_users_id_accounts_get.py
--rw-r--r--   0        0        0     5902 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_user_links_users_id_links_get.py
--rw-r--r--   0        0        0     5832 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_user_transactions.py
--rw-r--r--   0        0        0     6019 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_user_transactions_users_id_transactions_get.py
--rw-r--r--   0        0        0     5965 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_get_well_known_jwks_well_known_jwks_json_get.py
--rw-r--r--   0        0        0     5951 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_instrospect_client_auth_introspect_get.py
--rw-r--r--   0        0        0     7047 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_refresh_products_links_id_products_post.py
--rw-r--r--   0        0        0     6991 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_reset_login_links_id_reset_post.py
--rw-r--r--   0        0        0     7152 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_trigger_test_link_webhook_event_webhooks_test_link_id_post.py
--rw-r--r--   0        0        0     6963 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response401_update_link_links_id_patch.py
--rw-r--r--   0        0        0     6738 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/response_handle_link_webhook_event_request_body_webhook_post.py
--rw-r--r--   0        0        0     5198 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/security_response.py
--rw-r--r--   0        0        0     6205 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/transaction.py
--rw-r--r--   0        0        0     4150 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/transaction_diff.py
--rw-r--r--   0        0        0     4552 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/transaction_sync_response.py
--rw-r--r--   0        0        0      847 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/transaction_type.py
--rw-r--r--   0        0        0      859 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/transaction_type_filter.py
--rw-r--r--   0        0        0     5304 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/transaction_updates_available_webhook.py
--rw-r--r--   0        0        0     4496 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/transactions_link_product.py
--rw-r--r--   0        0        0     4198 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/transactions_product_settings.py
--rw-r--r--   0        0        0     3353 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/update_link_request.py
--rw-r--r--   0        0        0     3761 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/validation_error.py
--rw-r--r--   0        0        0     5101 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/validation_error_location_inner.py
--rw-r--r--   0        0        0      981 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/webhook_link_test_event.py
--rw-r--r--   0        0        0     3446 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/webhook_test_link_request.py
--rw-r--r--   0        0        0     2995 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/models/webhook_test_link_response.py
--rw-r--r--   0        0        0        0 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/py.typed
--rw-r--r--   0        0        0     8032 2024-01-09 15:08:14.326040 moneykit-0.1.7/moneykit/rest.py
--rw-r--r--   0        0        0      731 2024-01-09 15:08:14.326040 moneykit-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3544 1970-01-01 00:00:00.000000 moneykit-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2640 2024-01-31 19:58:09.007693 moneykit-0.1.8/README.md
+-rw-r--r--   0        0        0    11735 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/__init__.py
+-rw-r--r--   0        0        0      684 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api/__init__.py
+-rw-r--r--   0        0        0    36162 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api/access_token_api.py
+-rw-r--r--   0        0        0    14982 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api/account_numbers_api.py
+-rw-r--r--   0        0        0    52772 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api/accounts_api.py
+-rw-r--r--   0        0        0    16125 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api/identity_api.py
+-rw-r--r--   0        0        0    26098 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api/institutions_api.py
+-rw-r--r--   0        0        0    36018 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api/investments_api.py
+-rw-r--r--   0        0        0    23893 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api/link_session_api.py
+-rw-r--r--   0        0        0    54809 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api/links_api.py
+-rw-r--r--   0        0        0    14555 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api/products_api.py
+-rw-r--r--   0        0        0    63001 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api/transactions_api.py
+-rw-r--r--   0        0        0    48800 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api/users_api.py
+-rw-r--r--   0        0        0    13480 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api/webhooks_api.py
+-rw-r--r--   0        0        0    24258 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api_client.py
+-rw-r--r--   0        0        0      670 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/api_response.py
+-rw-r--r--   0        0        0    15031 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/configuration.py
+-rw-r--r--   0        0        0     5401 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/exceptions.py
+-rw-r--r--   0        0        0    10608 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/__init__.py
+-rw-r--r--   0        0        0     5070 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/account.py
+-rw-r--r--   0        0        0     4447 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/account_balances.py
+-rw-r--r--   0        0        0     3764 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/account_group.py
+-rw-r--r--   0        0        0     5643 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/account_identity.py
+-rw-r--r--   0        0        0     5185 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/account_numbers.py
+-rw-r--r--   0        0        0     4522 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/account_numbers_link_product.py
+-rw-r--r--   0        0        0     3715 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/account_numbers_product_settings.py
+-rw-r--r--   0        0        0     5562 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/account_with_account_numbers.py
+-rw-r--r--   0        0        0     3998 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/accounts_link_product.py
+-rw-r--r--   0        0        0     3470 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/ach_number.py
+-rw-r--r--   0        0        0     4134 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/address.py
+-rw-r--r--   0        0        0     4158 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/api_error_auth_expired_access_token_response.py
+-rw-r--r--   0        0        0     3946 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/api_error_auth_unauthorized_response.py
+-rw-r--r--   0        0        0     4112 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/api_error_rate_limit_exceeded_response.py
+-rw-r--r--   0        0        0     3193 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/bacs_number.py
+-rw-r--r--   0        0        0     3858 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/basic_account_details.py
+-rw-r--r--   0        0        0     6364 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/body.py
+-rw-r--r--   0        0        0      831 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/country.py
+-rw-r--r--   0        0        0     7616 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/create_link_session_request.py
+-rw-r--r--   0        0        0     3129 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/create_link_session_response.py
+-rw-r--r--   0        0        0     3875 2024-01-31 19:58:09.007693 moneykit-0.1.8/moneykit/models/currency.py
+-rw-r--r--   0        0        0     3073 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/cursor_pagination.py
+-rw-r--r--   0        0        0     3131 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/customer_app.py
+-rw-r--r--   0        0        0     3412 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/eft_number.py
+-rw-r--r--   0        0        0     3360 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/email.py
+-rw-r--r--   0        0        0     3133 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/exchange_token_request.py
+-rw-r--r--   0        0        0     3472 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/exchange_token_response.py
+-rw-r--r--   0        0        0     3455 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/generate_access_token_response.py
+-rw-r--r--   0        0        0     3997 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/get_account_numbers_response.py
+-rw-r--r--   0        0        0     3660 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/get_account_response.py
+-rw-r--r--   0        0        0     3840 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/get_accounts_response.py
+-rw-r--r--   0        0        0     5122 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/get_holdings_response.py
+-rw-r--r--   0        0        0     3997 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/get_institutions_response.py
+-rw-r--r--   0        0        0     5931 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/get_investment_transactions_response.py
+-rw-r--r--   0        0        0     5029 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/get_transactions_response.py
+-rw-r--r--   0        0        0     3303 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/get_user_accounts_response.py
+-rw-r--r--   0        0        0     3278 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/get_user_links_response.py
+-rw-r--r--   0        0        0     4374 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/get_user_transactions_response.py
+-rw-r--r--   0        0        0     4560 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/holding_response.py
+-rw-r--r--   0        0        0     4829 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/http_validation_error.py
+-rw-r--r--   0        0        0     4464 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/identity_link_product.py
+-rw-r--r--   0        0        0     3691 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/identity_product_settings.py
+-rw-r--r--   0        0        0     3899 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/identity_response.py
+-rw-r--r--   0        0        0     4411 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/institution.py
+-rw-r--r--   0        0        0     4019 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/institution_error_not_found_response.py
+-rw-r--r--   0        0        0     3080 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/international_number.py
+-rw-r--r--   0        0        0     4099 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/introspect_client_response.py
+-rw-r--r--   0        0        0     6641 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/investment_transaction_response.py
+-rw-r--r--   0        0        0     4488 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/investments_link_product.py
+-rw-r--r--   0        0        0     3703 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/investments_product_settings.py
+-rw-r--r--   0        0        0     2895 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/jwk_set.py
+-rw-r--r--   0        0        0     4821 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_common.py
+-rw-r--r--   0        0        0     1003 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_error.py
+-rw-r--r--   0        0        0     3801 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_error_bad_config_response.py
+-rw-r--r--   0        0        0     3903 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_error_bad_state_response.py
+-rw-r--r--   0        0        0     3903 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_error_deleted_response.py
+-rw-r--r--   0        0        0     3946 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_error_forbidden_action_response.py
+-rw-r--r--   0        0        0     3921 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_error_not_found_response.py
+-rw-r--r--   0        0        0     4051 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_error_unauthorized_access_response.py
+-rw-r--r--   0        0        0     1024 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_permission_scope.py
+-rw-r--r--   0        0        0     3587 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_permissions.py
+-rw-r--r--   0        0        0     1053 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_product_failure_reasons.py
+-rw-r--r--   0        0        0     5697 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_product_refresh_webhook.py
+-rw-r--r--   0        0        0      857 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_product_state.py
+-rw-r--r--   0        0        0     5491 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_products.py
+-rw-r--r--   0        0        0     5156 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_response.py
+-rw-r--r--   0        0        0     4534 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_session_customer_user.py
+-rw-r--r--   0        0        0     4099 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_session_customer_user_email.py
+-rw-r--r--   0        0        0     4294 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_session_customer_user_phone.py
+-rw-r--r--   0        0        0     4006 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_session_error_forbidden_config_response.py
+-rw-r--r--   0        0        0     4018 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_session_error_invalid_token_exchange.py
+-rw-r--r--   0        0        0     4302 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_session_setting_overrides.py
+-rw-r--r--   0        0        0      951 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_state.py
+-rw-r--r--   0        0        0     5549 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/link_state_changed_webhook.py
+-rw-r--r--   0        0        0     3671 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/money_kit_connect_features.py
+-rw-r--r--   0        0        0     4783 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/owner.py
+-rw-r--r--   0        0        0     3514 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/phone_number.py
+-rw-r--r--   0        0        0      883 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/phone_number_type.py
+-rw-r--r--   0        0        0      962 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/product.py
+-rw-r--r--   0        0        0     5151 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/products_settings.py
+-rw-r--r--   0        0        0      945 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/provider.py
+-rw-r--r--   0        0        0     1010 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/public_link_error.py
+-rw-r--r--   0        0        0     3004 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/refresh_products_request.py
+-rw-r--r--   0        0        0     3930 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/requested_link_permission.py
+-rw-r--r--   0        0        0     6970 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_disconnect_links_id_delete.py
+-rw-r--r--   0        0        0     6024 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_exchange_token_link_session_exchange_token_post.py
+-rw-r--r--   0        0        0     7068 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_account_links_id_accounts_account_id_get.py
+-rw-r--r--   0        0        0     7127 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_account_numbers_links_id_accounts_numbers_get.py
+-rw-r--r--   0        0        0     7012 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_accounts_links_id_accounts_get.py
+-rw-r--r--   0        0        0     7089 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_holdings_links_id_investments_holdings_get.py
+-rw-r--r--   0        0        0     7026 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_identities_links_id_identity_get.py
+-rw-r--r--   0        0        0     6031 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_institution_institutions_institution_id_get.py
+-rw-r--r--   0        0        0     5923 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_institutions_institutions_get.py
+-rw-r--r--   0        0        0     7215 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_investment_transactions_links_id_investments_transactions_get.py
+-rw-r--r--   0        0        0     6914 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_link_links_id_get.py
+-rw-r--r--   0        0        0     6900 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_transactions.py
+-rw-r--r--   0        0        0     7148 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_transactions_diff_links_id_transactions_sync_get.py
+-rw-r--r--   0        0        0     7063 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_transactions_links_id_transactions_get.py
+-rw-r--r--   0        0        0     5944 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_user_accounts_users_id_accounts_get.py
+-rw-r--r--   0        0        0     5902 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_user_links_users_id_links_get.py
+-rw-r--r--   0        0        0     5832 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_user_transactions.py
+-rw-r--r--   0        0        0     6019 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_user_transactions_users_id_transactions_get.py
+-rw-r--r--   0        0        0     5965 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_get_well_known_jwks_well_known_jwks_json_get.py
+-rw-r--r--   0        0        0     5951 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_instrospect_client_auth_introspect_get.py
+-rw-r--r--   0        0        0     7047 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_refresh_products_links_id_products_post.py
+-rw-r--r--   0        0        0     6991 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_reset_login_links_id_reset_post.py
+-rw-r--r--   0        0        0     7152 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_trigger_test_link_webhook_event_webhooks_test_link_id_post.py
+-rw-r--r--   0        0        0     6963 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response401_update_link_links_id_patch.py
+-rw-r--r--   0        0        0     6738 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/response_handle_link_webhook_event_request_body_webhook_post.py
+-rw-r--r--   0        0        0     5198 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/security_response.py
+-rw-r--r--   0        0        0     6205 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/transaction.py
+-rw-r--r--   0        0        0     4150 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/transaction_diff.py
+-rw-r--r--   0        0        0     4552 2024-01-31 19:58:09.011693 moneykit-0.1.8/moneykit/models/transaction_sync_response.py
+-rw-r--r--   0        0        0      847 2024-01-31 19:58:09.015693 moneykit-0.1.8/moneykit/models/transaction_type.py
+-rw-r--r--   0        0        0      859 2024-01-31 19:58:09.015693 moneykit-0.1.8/moneykit/models/transaction_type_filter.py
+-rw-r--r--   0        0        0     5304 2024-01-31 19:58:09.015693 moneykit-0.1.8/moneykit/models/transaction_updates_available_webhook.py
+-rw-r--r--   0        0        0     4614 2024-01-31 19:58:09.015693 moneykit-0.1.8/moneykit/models/transactions_link_product.py
+-rw-r--r--   0        0        0     4198 2024-01-31 19:58:09.015693 moneykit-0.1.8/moneykit/models/transactions_product_settings.py
+-rw-r--r--   0        0        0     3353 2024-01-31 19:58:09.015693 moneykit-0.1.8/moneykit/models/update_link_request.py
+-rw-r--r--   0        0        0     3761 2024-01-31 19:58:09.015693 moneykit-0.1.8/moneykit/models/validation_error.py
+-rw-r--r--   0        0        0     5101 2024-01-31 19:58:09.015693 moneykit-0.1.8/moneykit/models/validation_error_location_inner.py
+-rw-r--r--   0        0        0      981 2024-01-31 19:58:09.015693 moneykit-0.1.8/moneykit/models/webhook_link_test_event.py
+-rw-r--r--   0        0        0     3446 2024-01-31 19:58:09.015693 moneykit-0.1.8/moneykit/models/webhook_test_link_request.py
+-rw-r--r--   0        0        0     2995 2024-01-31 19:58:09.015693 moneykit-0.1.8/moneykit/models/webhook_test_link_response.py
+-rw-r--r--   0        0        0        0 2024-01-31 19:58:09.015693 moneykit-0.1.8/moneykit/py.typed
+-rw-r--r--   0        0        0     8032 2024-01-31 19:58:09.015693 moneykit-0.1.8/moneykit/rest.py
+-rw-r--r--   0        0        0      731 2024-01-31 19:58:09.015693 moneykit-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3544 1970-01-01 00:00:00.000000 moneykit-0.1.8/PKG-INFO
```

### Comparing `moneykit-0.1.7/README.md` & `moneykit-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/__init__.py` & `moneykit-0.1.8/moneykit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 2023-02-18
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 
 # import apis into sdk package
 from moneykit.api.access_token_api import AccessTokenApi
 from moneykit.api.account_numbers_api import AccountNumbersApi
 from moneykit.api.accounts_api import AccountsApi
 from moneykit.api.identity_api import IdentityApi
 from moneykit.api.institutions_api import InstitutionsApi
```

### Comparing `moneykit-0.1.7/moneykit/api/__init__.py` & `moneykit-0.1.8/moneykit/api/__init__.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/api/access_token_api.py` & `moneykit-0.1.8/moneykit/api/access_token_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/api/account_numbers_api.py` & `moneykit-0.1.8/moneykit/api/account_numbers_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/api/accounts_api.py` & `moneykit-0.1.8/moneykit/api/accounts_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/api/identity_api.py` & `moneykit-0.1.8/moneykit/api/identity_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/api/institutions_api.py` & `moneykit-0.1.8/moneykit/api/institutions_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/api/investments_api.py` & `moneykit-0.1.8/moneykit/api/investments_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/api/link_session_api.py` & `moneykit-0.1.8/moneykit/api/link_session_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/api/links_api.py` & `moneykit-0.1.8/moneykit/api/links_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/api/products_api.py` & `moneykit-0.1.8/moneykit/api/products_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 except ImportError:
     from typing_extensions import Annotated
 
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictStr
 
+from moneykit.models.link_common import LinkCommon
 from moneykit.models.refresh_products_request import RefreshProductsRequest
 
 from moneykit.api_client import ApiClient
 from moneykit.api_response import ApiResponse
 from moneykit.rest import RESTResponseType
 
 
@@ -56,15 +57,15 @@
                 Annotated[StrictFloat, Field(gt=0)], Annotated[StrictFloat, Field(gt=0)]
             ],
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> None:
+    ) -> LinkCommon:
         """/links/{id}/products
 
         Requests an update of the provided products for the link.     This is an asynchronous operation. The response will be a 202 Accepted if the request was successful.     Refreshes are subject to rate limiting.     <br><br>     <b>Rate Limiting</b><br>     <ul>         <li>1 refresh per link per hour for account data</li>         <li>1 refresh per link per hour for transaction data</li>         <li>1 refresh per link per day for account numbers</li>         <li>1 refresh per link per day for identity data</li>     </ul>
 
         :param id: The unique ID for this link. (required)
         :type id: str
         :param refresh_products_request: (required)
@@ -96,15 +97,23 @@
             refresh_products_request=refresh_products_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index,
         )
 
-        _response_types_map: Dict[str, Optional[str]] = {}
+        _response_types_map: Dict[str, Optional[str]] = {
+            "202": "LinkCommon",
+            "401": "Response401RefreshProductsLinksIdProductsPost",
+            "429": "APIErrorRateLimitExceededResponse",
+            "404": "LinkErrorNotFoundResponse",
+            "403": "LinkErrorForbiddenActionResponse",
+            "410": "LinkErrorDeletedResponse",
+            "422": "LinkErrorBadStateResponse",
+        }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
@@ -122,15 +131,15 @@
                 Annotated[StrictFloat, Field(gt=0)], Annotated[StrictFloat, Field(gt=0)]
             ],
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[None]:
+    ) -> ApiResponse[LinkCommon]:
         """/links/{id}/products
 
         Requests an update of the provided products for the link.     This is an asynchronous operation. The response will be a 202 Accepted if the request was successful.     Refreshes are subject to rate limiting.     <br><br>     <b>Rate Limiting</b><br>     <ul>         <li>1 refresh per link per hour for account data</li>         <li>1 refresh per link per hour for transaction data</li>         <li>1 refresh per link per day for account numbers</li>         <li>1 refresh per link per day for identity data</li>     </ul>
 
         :param id: The unique ID for this link. (required)
         :type id: str
         :param refresh_products_request: (required)
@@ -162,15 +171,23 @@
             refresh_products_request=refresh_products_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index,
         )
 
-        _response_types_map: Dict[str, Optional[str]] = {}
+        _response_types_map: Dict[str, Optional[str]] = {
+            "202": "LinkCommon",
+            "401": "Response401RefreshProductsLinksIdProductsPost",
+            "429": "APIErrorRateLimitExceededResponse",
+            "404": "LinkErrorNotFoundResponse",
+            "403": "LinkErrorForbiddenActionResponse",
+            "410": "LinkErrorDeletedResponse",
+            "422": "LinkErrorBadStateResponse",
+        }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
@@ -228,15 +245,23 @@
             refresh_products_request=refresh_products_request,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index,
         )
 
-        _response_types_map: Dict[str, Optional[str]] = {}
+        _response_types_map: Dict[str, Optional[str]] = {
+            "202": "LinkCommon",
+            "401": "Response401RefreshProductsLinksIdProductsPost",
+            "429": "APIErrorRateLimitExceededResponse",
+            "404": "LinkErrorNotFoundResponse",
+            "403": "LinkErrorForbiddenActionResponse",
+            "410": "LinkErrorDeletedResponse",
+            "422": "LinkErrorBadStateResponse",
+        }
         response_data = self.api_client.call_api(
             *_param, _request_timeout=_request_timeout
         )
         return response_data.response
 
     def _refresh_products_serialize(
         self,
```

### Comparing `moneykit-0.1.7/moneykit/api/transactions_api.py` & `moneykit-0.1.8/moneykit/api/transactions_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/api/users_api.py` & `moneykit-0.1.8/moneykit/api/users_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/api/webhooks_api.py` & `moneykit-0.1.8/moneykit/api/webhooks_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/api_client.py` & `moneykit-0.1.8/moneykit/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {"MoneyKit-Version": "2023-02-18"}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "OpenAPI-Generator/0.1.7/python"
+        self.user_agent = "OpenAPI-Generator/0.1.8/python"
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `moneykit-0.1.7/moneykit/api_response.py` & `moneykit-0.1.8/moneykit/api_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/configuration.py` & `moneykit-0.1.8/moneykit/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,15 @@
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: 2023-02-18\n"
-            "SDK Package Version: 0.1.7".format(env=sys.platform, pyversion=sys.version)
+            "SDK Package Version: 0.1.8".format(env=sys.platform, pyversion=sys.version)
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `moneykit-0.1.7/moneykit/exceptions.py` & `moneykit-0.1.8/moneykit/exceptions.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/__init__.py` & `moneykit-0.1.8/moneykit/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/account.py` & `moneykit-0.1.8/moneykit/models/account.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/account_balances.py` & `moneykit-0.1.8/moneykit/models/account_balances.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/account_group.py` & `moneykit-0.1.8/moneykit/models/account_group.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/account_identity.py` & `moneykit-0.1.8/moneykit/models/account_identity.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/account_numbers.py` & `moneykit-0.1.8/moneykit/models/account_numbers.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/account_numbers_link_product.py` & `moneykit-0.1.8/moneykit/models/account_numbers_link_product.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/account_numbers_product_settings.py` & `moneykit-0.1.8/moneykit/models/account_numbers_product_settings.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/account_with_account_numbers.py` & `moneykit-0.1.8/moneykit/models/account_with_account_numbers.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/accounts_link_product.py` & `moneykit-0.1.8/moneykit/models/accounts_link_product.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/ach_number.py` & `moneykit-0.1.8/moneykit/models/ach_number.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/address.py` & `moneykit-0.1.8/moneykit/models/address.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/api_error_auth_expired_access_token_response.py` & `moneykit-0.1.8/moneykit/models/api_error_auth_expired_access_token_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/api_error_auth_unauthorized_response.py` & `moneykit-0.1.8/moneykit/models/api_error_auth_unauthorized_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/api_error_rate_limit_exceeded_response.py` & `moneykit-0.1.8/moneykit/models/api_error_rate_limit_exceeded_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/bacs_number.py` & `moneykit-0.1.8/moneykit/models/bacs_number.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/basic_account_details.py` & `moneykit-0.1.8/moneykit/models/basic_account_details.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/body.py` & `moneykit-0.1.8/moneykit/models/body.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/country.py` & `moneykit-0.1.8/moneykit/models/country.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/create_link_session_request.py` & `moneykit-0.1.8/moneykit/models/transaction.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,67 +13,79 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-
+from datetime import date, datetime
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, StrictBool, StrictStr
 from pydantic import Field
-from typing_extensions import Annotated
-from moneykit.models.link_session_customer_user import LinkSessionCustomerUser
-from moneykit.models.link_session_setting_overrides import LinkSessionSettingOverrides
-from moneykit.models.money_kit_connect_features import MoneyKitConnectFeatures
+from moneykit.models.transaction_type import TransactionType
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class CreateLinkSessionRequest(BaseModel):
+class Transaction(BaseModel):
     """
-    CreateLinkSessionRequest
+    Transaction
     """  # noqa: E501
 
-    settings: Optional[LinkSessionSettingOverrides] = None
-    customer_user: LinkSessionCustomerUser
-    existing_link_id: Optional[StrictStr] = Field(
+    transaction_id: StrictStr = Field(description="The unique ID for this transaction.")
+    account_id: StrictStr = Field(
+        description="The ID of the account in which this transaction occurred."
+    )
+    amount: StrictStr = Field(
+        description="The amount of this transaction, denominated in account currency.  This amount is always         non-negative.  The `type` field indicates whether it is entering or leaving the account."
+    )
+    type: TransactionType
+    currency: StrictStr = Field(
+        description="The ISO-4217 currency code of the transaction."
+    )
+    date_: date = Field(
+        description="The effective (posted) date of the transaction, in ISO-8601 format.  For pending transactions,             this date is when the transaction was initiated.",
+        alias="date",
+    )
+    datetime_: Optional[datetime] = Field(
+        alias="datetime",
+        default=None,
+        description="If the institution has provided the actual time of the transaction, this field             contains the full date and time of the transaction, in ISO-8601 format.  If the time is             not available, this field will be null.             <p>Note that the time is generally reported in the timezone of the institution or the account holder.",
+    )
+    description: Optional[StrictStr] = Field(
         default=None,
-        description="Supply the existing `link_id` if you are asking the user to reconnect this link.",
+        description="A normalized, cleaned transaction description suitable for presentation to the end user.             Commonly this will be the merchant or counterparty name.",
     )
-    institution_id: Optional[StrictStr] = Field(
+    raw_description: Optional[StrictStr] = Field(
         default=None,
-        description="The ID of the institution you want to link to. Providing this will skip the institution         selection step. `existing_link_id` will take precedence over this field if both are provided.",
+        description="The raw transaction description as provided by the institution, where available.",
+    )
+    pending: StrictBool = Field(
+        description="If true, this transaction is pending or unsettled and has not yet affected the account.         Commonly these are credit card transactions, particularly approvals (holds) such as for hotel or restaurant         reservations placed in advance where the final amount is still to be determined."
     )
-    redirect_uri: Annotated[
-        str, Field(min_length=1, strict=True, max_length=65536)
-    ] = Field(
-        description="For Oauth linking, a URI indicating the destination, in your application, where the user should         be sent after authenticating with the institution.  The `redirect_uri` should not contain any query parameters,         and it must be pre-approved by MoneyKit during the customer setup process."
-    )
-    webhook: Optional[
-        Annotated[str, Field(min_length=1, strict=True, max_length=65536)]
-    ] = Field(
+    category: Optional[StrictStr] = Field(
         default=None,
-        description="The destination URL to which any webhooks should be sent.",
+        description="The category for this transaction, given as a dotted string indicating a hierarchical         categorization.  See <a href=/pages/categories>Transaction Categories</a> for the list of possible transaction types.",
     )
-    link_tags: Optional[List[StrictStr]] = None
-    connect_features: Optional[MoneyKitConnectFeatures] = None
     additional_properties: Dict[str, Any] = {}
     __properties: ClassVar[List[str]] = [
-        "settings",
-        "customer_user",
-        "existing_link_id",
-        "institution_id",
-        "redirect_uri",
-        "webhook",
-        "link_tags",
-        "connect_features",
+        "transaction_id",
+        "account_id",
+        "amount",
+        "type",
+        "currency",
+        "date",
+        "datetime",
+        "description",
+        "raw_description",
+        "pending",
+        "category",
     ]
 
     model_config = {"populate_by_name": True, "validate_assignment": True}
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
@@ -81,15 +93,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of CreateLinkSessionRequest from a JSON string"""
+        """Create an instance of Transaction from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -102,59 +114,43 @@
         _dict = self.model_dump(
             by_alias=True,
             exclude={
                 "additional_properties",
             },
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of settings
-        if self.settings:
-            _dict["settings"] = self.settings.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of customer_user
-        if self.customer_user:
-            _dict["customer_user"] = self.customer_user.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of connect_features
-        if self.connect_features:
-            _dict["connect_features"] = self.connect_features.to_dict()
         # puts key-value pairs in additional_properties in the top level
         if self.additional_properties is not None:
             for _key, _value in self.additional_properties.items():
                 _dict[_key] = _value
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of CreateLinkSessionRequest from a dict"""
+        """Create an instance of Transaction from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate(
             {
-                "settings": LinkSessionSettingOverrides.from_dict(obj.get("settings"))
-                if obj.get("settings") is not None
-                else None,
-                "customer_user": LinkSessionCustomerUser.from_dict(
-                    obj.get("customer_user")
-                )
-                if obj.get("customer_user") is not None
-                else None,
-                "existing_link_id": obj.get("existing_link_id"),
-                "institution_id": obj.get("institution_id"),
-                "redirect_uri": obj.get("redirect_uri"),
-                "webhook": obj.get("webhook"),
-                "link_tags": obj.get("link_tags"),
-                "connect_features": MoneyKitConnectFeatures.from_dict(
-                    obj.get("connect_features")
-                )
-                if obj.get("connect_features") is not None
-                else None,
+                "transaction_id": obj.get("transaction_id"),
+                "account_id": obj.get("account_id"),
+                "amount": obj.get("amount"),
+                "type": obj.get("type"),
+                "currency": obj.get("currency"),
+                "date": obj.get("date"),
+                "datetime": obj.get("datetime"),
+                "description": obj.get("description"),
+                "raw_description": obj.get("raw_description"),
+                "pending": obj.get("pending"),
+                "category": obj.get("category"),
             }
         )
         # store additional fields in additional_properties
         for _key in obj.keys():
             if _key not in cls.__properties:
                 _obj.additional_properties[_key] = obj.get(_key)
```

### Comparing `moneykit-0.1.7/moneykit/models/create_link_session_response.py` & `moneykit-0.1.8/moneykit/models/create_link_session_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/currency.py` & `moneykit-0.1.8/moneykit/models/currency.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/cursor_pagination.py` & `moneykit-0.1.8/moneykit/models/cursor_pagination.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/customer_app.py` & `moneykit-0.1.8/moneykit/models/customer_app.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/eft_number.py` & `moneykit-0.1.8/moneykit/models/eft_number.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/email.py` & `moneykit-0.1.8/moneykit/models/email.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/exchange_token_request.py` & `moneykit-0.1.8/moneykit/models/exchange_token_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/exchange_token_response.py` & `moneykit-0.1.8/moneykit/models/exchange_token_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/generate_access_token_response.py` & `moneykit-0.1.8/moneykit/models/generate_access_token_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/get_account_numbers_response.py` & `moneykit-0.1.8/moneykit/models/get_account_numbers_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/get_account_response.py` & `moneykit-0.1.8/moneykit/models/get_account_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/get_accounts_response.py` & `moneykit-0.1.8/moneykit/models/get_accounts_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/get_holdings_response.py` & `moneykit-0.1.8/moneykit/models/get_holdings_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/get_institutions_response.py` & `moneykit-0.1.8/moneykit/models/get_institutions_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/get_investment_transactions_response.py` & `moneykit-0.1.8/moneykit/models/get_investment_transactions_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/get_transactions_response.py` & `moneykit-0.1.8/moneykit/models/get_transactions_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/get_user_accounts_response.py` & `moneykit-0.1.8/moneykit/models/get_user_accounts_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/get_user_links_response.py` & `moneykit-0.1.8/moneykit/models/get_user_links_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/get_user_transactions_response.py` & `moneykit-0.1.8/moneykit/models/get_user_transactions_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/holding_response.py` & `moneykit-0.1.8/moneykit/models/holding_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/http_validation_error.py` & `moneykit-0.1.8/moneykit/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/identity_link_product.py` & `moneykit-0.1.8/moneykit/models/identity_link_product.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/identity_product_settings.py` & `moneykit-0.1.8/moneykit/models/identity_product_settings.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/identity_response.py` & `moneykit-0.1.8/moneykit/models/identity_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/institution.py` & `moneykit-0.1.8/moneykit/models/institution.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/institution_error_not_found_response.py` & `moneykit-0.1.8/moneykit/models/institution_error_not_found_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/international_number.py` & `moneykit-0.1.8/moneykit/models/international_number.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/introspect_client_response.py` & `moneykit-0.1.8/moneykit/models/introspect_client_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/investment_transaction_response.py` & `moneykit-0.1.8/moneykit/models/investment_transaction_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/investments_link_product.py` & `moneykit-0.1.8/moneykit/models/investments_link_product.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/investments_product_settings.py` & `moneykit-0.1.8/moneykit/models/investments_product_settings.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/jwk_set.py` & `moneykit-0.1.8/moneykit/models/jwk_set.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_common.py` & `moneykit-0.1.8/moneykit/models/link_common.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_error.py` & `moneykit-0.1.8/moneykit/models/link_error.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_error_bad_config_response.py` & `moneykit-0.1.8/moneykit/models/link_error_bad_config_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_error_bad_state_response.py` & `moneykit-0.1.8/moneykit/models/link_error_bad_state_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_error_deleted_response.py` & `moneykit-0.1.8/moneykit/models/link_error_deleted_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_error_forbidden_action_response.py` & `moneykit-0.1.8/moneykit/models/link_error_forbidden_action_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_error_not_found_response.py` & `moneykit-0.1.8/moneykit/models/link_error_not_found_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_error_unauthorized_access_response.py` & `moneykit-0.1.8/moneykit/models/link_error_unauthorized_access_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_permission_scope.py` & `moneykit-0.1.8/moneykit/models/link_permission_scope.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_permissions.py` & `moneykit-0.1.8/moneykit/models/link_permissions.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_product_failure_reasons.py` & `moneykit-0.1.8/moneykit/models/link_product_failure_reasons.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,12 +34,13 @@
     """
     RATE_LIMIT = "rate_limit"
     AUTH_EXPIRED = "auth_expired"
     INVALID_CREDENTIALS = "invalid_credentials"
     NOT_SUPPORTED = "not_supported"
     TIMEOUT = "timeout"
     UNKNOWN = "unknown"
+    NO_ACCOUNTS = "no_accounts"
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Create an instance of LinkProductFailureReasons from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `moneykit-0.1.7/moneykit/models/link_product_refresh_webhook.py` & `moneykit-0.1.8/moneykit/models/link_product_refresh_webhook.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_product_state.py` & `moneykit-0.1.8/moneykit/models/link_product_state.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_products.py` & `moneykit-0.1.8/moneykit/models/link_products.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_response.py` & `moneykit-0.1.8/moneykit/models/link_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_session_customer_user.py` & `moneykit-0.1.8/moneykit/models/link_session_customer_user.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_session_customer_user_email.py` & `moneykit-0.1.8/moneykit/models/link_session_customer_user_email.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_session_customer_user_phone.py` & `moneykit-0.1.8/moneykit/models/link_session_customer_user_phone.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_session_error_forbidden_config_response.py` & `moneykit-0.1.8/moneykit/models/link_session_error_forbidden_config_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_session_error_invalid_token_exchange.py` & `moneykit-0.1.8/moneykit/models/link_session_error_invalid_token_exchange.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_session_setting_overrides.py` & `moneykit-0.1.8/moneykit/models/link_session_setting_overrides.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_state.py` & `moneykit-0.1.8/moneykit/models/link_state.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/link_state_changed_webhook.py` & `moneykit-0.1.8/moneykit/models/link_state_changed_webhook.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/money_kit_connect_features.py` & `moneykit-0.1.8/moneykit/models/money_kit_connect_features.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/owner.py` & `moneykit-0.1.8/moneykit/models/owner.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/phone_number.py` & `moneykit-0.1.8/moneykit/models/phone_number.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/phone_number_type.py` & `moneykit-0.1.8/moneykit/models/phone_number_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/product.py` & `moneykit-0.1.8/moneykit/models/product.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/products_settings.py` & `moneykit-0.1.8/moneykit/models/products_settings.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/provider.py` & `moneykit-0.1.8/moneykit/models/provider.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/public_link_error.py` & `moneykit-0.1.8/moneykit/models/public_link_error.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/refresh_products_request.py` & `moneykit-0.1.8/moneykit/models/refresh_products_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/requested_link_permission.py` & `moneykit-0.1.8/moneykit/models/requested_link_permission.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_disconnect_links_id_delete.py` & `moneykit-0.1.8/moneykit/models/response401_disconnect_links_id_delete.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_exchange_token_link_session_exchange_token_post.py` & `moneykit-0.1.8/moneykit/models/response401_exchange_token_link_session_exchange_token_post.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_account_links_id_accounts_account_id_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_account_links_id_accounts_account_id_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_account_numbers_links_id_accounts_numbers_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_account_numbers_links_id_accounts_numbers_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_accounts_links_id_accounts_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_accounts_links_id_accounts_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_holdings_links_id_investments_holdings_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_holdings_links_id_investments_holdings_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_identities_links_id_identity_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_identities_links_id_identity_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_institution_institutions_institution_id_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_institution_institutions_institution_id_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_institutions_institutions_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_institutions_institutions_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_investment_transactions_links_id_investments_transactions_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_investment_transactions_links_id_investments_transactions_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_link_links_id_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_link_links_id_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_transactions.py` & `moneykit-0.1.8/moneykit/models/response401_get_transactions.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_transactions_diff_links_id_transactions_sync_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_transactions_diff_links_id_transactions_sync_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_transactions_links_id_transactions_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_transactions_links_id_transactions_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_user_accounts_users_id_accounts_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_user_accounts_users_id_accounts_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_user_links_users_id_links_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_user_links_users_id_links_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_user_transactions.py` & `moneykit-0.1.8/moneykit/models/response401_get_user_transactions.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_user_transactions_users_id_transactions_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_user_transactions_users_id_transactions_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_get_well_known_jwks_well_known_jwks_json_get.py` & `moneykit-0.1.8/moneykit/models/response401_get_well_known_jwks_well_known_jwks_json_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_instrospect_client_auth_introspect_get.py` & `moneykit-0.1.8/moneykit/models/response401_instrospect_client_auth_introspect_get.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_refresh_products_links_id_products_post.py` & `moneykit-0.1.8/moneykit/models/response401_refresh_products_links_id_products_post.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_reset_login_links_id_reset_post.py` & `moneykit-0.1.8/moneykit/models/response401_reset_login_links_id_reset_post.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_trigger_test_link_webhook_event_webhooks_test_link_id_post.py` & `moneykit-0.1.8/moneykit/models/response401_trigger_test_link_webhook_event_webhooks_test_link_id_post.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response401_update_link_links_id_patch.py` & `moneykit-0.1.8/moneykit/models/response401_update_link_links_id_patch.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/response_handle_link_webhook_event_request_body_webhook_post.py` & `moneykit-0.1.8/moneykit/models/response_handle_link_webhook_event_request_body_webhook_post.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/security_response.py` & `moneykit-0.1.8/moneykit/models/security_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/transaction_diff.py` & `moneykit-0.1.8/moneykit/models/transaction_diff.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/transaction_sync_response.py` & `moneykit-0.1.8/moneykit/models/transaction_sync_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/transaction_type.py` & `moneykit-0.1.8/moneykit/models/transaction_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/transaction_type_filter.py` & `moneykit-0.1.8/moneykit/models/transaction_type_filter.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/transaction_updates_available_webhook.py` & `moneykit-0.1.8/moneykit/models/transaction_updates_available_webhook.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/transactions_link_product.py` & `moneykit-0.1.8/moneykit/models/transactions_link_product.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, StrictBool, StrictStr
 from pydantic import Field
 from moneykit.models.link_product_failure_reasons import LinkProductFailureReasons
 from moneykit.models.transactions_product_settings import TransactionsProductSettings
 
 try:
     from typing import Self
 except ImportError:
@@ -44,21 +44,23 @@
         description="An ISO-8601 timestamp indicating the last time that the product was attempted.",
     )
     error_code: Optional[LinkProductFailureReasons] = None
     error_message: Optional[StrictStr] = Field(
         default=None,
         description="The error message, if the last attempt to refresh the product failed.",
     )
+    has_history: StrictBool
     settings: TransactionsProductSettings
     additional_properties: Dict[str, Any] = {}
     __properties: ClassVar[List[str]] = [
         "refreshed_at",
         "last_attempted_at",
         "error_code",
         "error_message",
+        "has_history",
         "settings",
     ]
 
     model_config = {"populate_by_name": True, "validate_assignment": True}
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -113,14 +115,15 @@
 
         _obj = cls.model_validate(
             {
                 "refreshed_at": obj.get("refreshed_at"),
                 "last_attempted_at": obj.get("last_attempted_at"),
                 "error_code": obj.get("error_code"),
                 "error_message": obj.get("error_message"),
+                "has_history": obj.get("has_history"),
                 "settings": TransactionsProductSettings.from_dict(obj.get("settings"))
                 if obj.get("settings") is not None
                 else None,
             }
         )
         # store additional fields in additional_properties
         for _key in obj.keys():
```

### Comparing `moneykit-0.1.7/moneykit/models/transactions_product_settings.py` & `moneykit-0.1.8/moneykit/models/transactions_product_settings.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/update_link_request.py` & `moneykit-0.1.8/moneykit/models/update_link_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/validation_error.py` & `moneykit-0.1.8/moneykit/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/validation_error_location_inner.py` & `moneykit-0.1.8/moneykit/models/validation_error_location_inner.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/webhook_link_test_event.py` & `moneykit-0.1.8/moneykit/models/webhook_link_test_event.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/webhook_test_link_request.py` & `moneykit-0.1.8/moneykit/models/webhook_test_link_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/models/webhook_test_link_response.py` & `moneykit-0.1.8/moneykit/models/webhook_test_link_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/moneykit/rest.py` & `moneykit-0.1.8/moneykit/rest.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.1.7/pyproject.toml` & `moneykit-0.1.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "moneykit"
-version = "0.1.7"
+version = "0.1.8"
 description = "MoneyKit API"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "MoneyKit API"]
 include = ["moneykit/py.typed"]
```

### Comparing `moneykit-0.1.7/PKG-INFO` & `moneykit-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneykit
-Version: 0.1.7
+Version: 0.1.8
 Summary: MoneyKit API
 Home-page: https://github.com/GIT_USER_ID/GIT_REPO_ID
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,MoneyKit API
 Author: OpenAPI Generator Community
 Author-email: team@openapitools.org
 Requires-Python: >=3.8,<4.0
```

