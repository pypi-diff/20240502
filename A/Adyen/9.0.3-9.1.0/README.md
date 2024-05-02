# Comparing `tmp/Adyen-9.0.3.tar.gz` & `tmp/Adyen-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Adyen-9.0.3.tar", last modified: Mon Sep 18 13:04:32 2023, max compression
+gzip compressed data, was "Adyen-9.1.0.tar", last modified: Fri Oct 20 09:52:11 2023, max compression
```

## Comparing `Adyen-9.0.3.tar` & `Adyen-9.1.0.tar`

### file list

```diff
@@ -1,117 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 13:04:32.916165 Adyen-9.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 13:04:32.904165 Adyen-9.0.3/Adyen/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21186 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13185 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/httpclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 13:04:32.904165 Adyen-9.0.3/Adyen/services/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 13:04:32.908165 Adyen-9.0.3/Adyen/services/balancePlatform/
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/balancePlatform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/balancePlatform/account_holders_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/balancePlatform/balance_accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/balancePlatform/bank_account_validation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/balancePlatform/grant_accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/balancePlatform/grant_offers_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/balancePlatform/payment_instrument_groups_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/balancePlatform/payment_instruments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/balancePlatform/platform_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/balancePlatform/transaction_rules_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/binlookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 13:04:32.908165 Adyen-9.0.3/Adyen/services/checkout/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/checkout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/checkout/classic_checkout_sdk_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/checkout/modifications_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/checkout/orders_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/checkout/payment_links_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/checkout/payments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/checkout/recurring_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/checkout/utility_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/dataProtection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 13:04:32.908165 Adyen-9.0.3/Adyen/services/legalEntityManagement/
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/legalEntityManagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/legalEntityManagement/business_lines_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/legalEntityManagement/documents_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/legalEntityManagement/hosted_onboarding_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/legalEntityManagement/legal_entities_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/legalEntityManagement/pci_questionnaires_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/legalEntityManagement/terms_of_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/legalEntityManagement/transfer_instruments_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 13:04:32.912165 Adyen-9.0.3/Adyen/services/management/
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/account_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/account_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/account_store_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/allowed_origins_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/allowed_origins_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/api_credentials_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/api_credentials_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/api_key_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/api_key_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/client_key_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/client_key_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/my_api_credential_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/payment_methods_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/payout_settings_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/terminal_actions_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/terminal_actions_terminal_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/terminal_orders_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/terminal_orders_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/terminal_settings_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/terminal_settings_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/terminal_settings_store_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/terminal_settings_terminal_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/terminals_terminal_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/users_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/users_merchant_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/webhooks_company_level_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/management/webhooks_merchant_level_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 13:04:32.912165 Adyen-9.0.3/Adyen/services/payments/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/payments/general_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/payments/modifications_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 13:04:32.912165 Adyen-9.0.3/Adyen/services/payouts/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/payouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/payouts/initialization_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/payouts/instant_payouts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/payouts/reviewing_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/recurring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/storedValue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 13:04:32.916165 Adyen-9.0.3/Adyen/services/transfers/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/transfers/transactions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/services/transfers/transfers_api.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2023-09-18 13:04:23.000000 Adyen-9.0.3/Adyen/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 13:04:32.904165 Adyen-9.0.3/Adyen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-09-18 13:04:32.000000 Adyen-9.0.3/Adyen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2023-09-18 13:04:32.000000 Adyen-9.0.3/Adyen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-18 13:04:32.000000 Adyen-9.0.3/Adyen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-18 13:04:32.000000 Adyen-9.0.3/Adyen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-09-18 13:04:23.000000 Adyen-9.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-09-18 13:04:32.916165 Adyen-9.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2023-09-18 13:04:23.000000 Adyen-9.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-09-18 13:04:32.916165 Adyen-9.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2023-09-18 13:04:23.000000 Adyen-9.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 13:04:32.916165 Adyen-9.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/BaseTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/BinLookupTest.py
--rw-r--r--   0 runner    (1001) docker     (127)    32428 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/CheckoutTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/CheckoutUtilityTest.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/ClientTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/ConfigurationTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/DataProtectionTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/DetermineEndpointTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/LegalEntityManagementTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/ManagementTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/ModificationTest.py
--rw-r--r--   0 runner    (1001) docker     (127)    18978 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/PaymentTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/RecurringTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/StoredValueTest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10005 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/TerminalTest.py
--rw-r--r--   0 runner    (1001) docker     (127)    14146 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/ThirdPartyPayoutTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/TransfersTest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/UtilTest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-18 13:04:23.000000 Adyen-9.0.3/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 09:52:11.068571 Adyen-9.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 09:52:11.052571 Adyen-9.1.0/Adyen/
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21414 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13185 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/httpclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 09:52:11.056571 Adyen-9.1.0/Adyen/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 09:52:11.056571 Adyen-9.1.0/Adyen/services/balancePlatform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/balancePlatform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/balancePlatform/account_holders_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/balancePlatform/balance_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/balancePlatform/bank_account_validation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/balancePlatform/grant_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/balancePlatform/grant_offers_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/balancePlatform/payment_instrument_groups_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/balancePlatform/payment_instruments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/balancePlatform/platform_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/balancePlatform/transaction_rules_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/binlookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 09:52:11.056571 Adyen-9.1.0/Adyen/services/checkout/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/checkout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/checkout/classic_checkout_sdk_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/checkout/modifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/checkout/orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/checkout/payment_links_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/checkout/payments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/checkout/recurring_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/checkout/utility_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/dataProtection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/disputes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 09:52:11.056571 Adyen-9.1.0/Adyen/services/legalEntityManagement/
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/legalEntityManagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/legalEntityManagement/business_lines_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/legalEntityManagement/documents_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/legalEntityManagement/hosted_onboarding_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/legalEntityManagement/legal_entities_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/legalEntityManagement/pci_questionnaires_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/legalEntityManagement/terms_of_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/legalEntityManagement/transfer_instruments_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 09:52:11.064571 Adyen-9.1.0/Adyen/services/management/
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/account_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/account_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/account_store_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/allowed_origins_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/allowed_origins_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/api_credentials_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/api_credentials_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/api_key_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/api_key_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/client_key_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/client_key_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/my_api_credential_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/payment_methods_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/payout_settings_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/terminal_actions_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/terminal_actions_terminal_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/terminal_orders_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/terminal_orders_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/terminal_settings_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/terminal_settings_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/terminal_settings_store_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/terminal_settings_terminal_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/terminals_terminal_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/users_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/users_merchant_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/webhooks_company_level_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/management/webhooks_merchant_level_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 09:52:11.064571 Adyen-9.1.0/Adyen/services/payments/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/payments/general_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/payments/modifications_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 09:52:11.064571 Adyen-9.1.0/Adyen/services/payouts/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/payouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/payouts/initialization_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/payouts/instant_payouts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/payouts/reviewing_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/recurring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/storedValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 09:52:11.064571 Adyen-9.1.0/Adyen/services/transfers/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/transfers/transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/services/transfers/transfers_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2023-10-20 09:52:01.000000 Adyen-9.1.0/Adyen/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 09:52:11.052571 Adyen-9.1.0/Adyen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2023-10-20 09:52:11.000000 Adyen-9.1.0/Adyen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2023-10-20 09:52:11.000000 Adyen-9.1.0/Adyen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 09:52:11.000000 Adyen-9.1.0/Adyen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-20 09:52:11.000000 Adyen-9.1.0/Adyen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-10-20 09:52:01.000000 Adyen-9.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2023-10-20 09:52:11.068571 Adyen-9.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12929 2023-10-20 09:52:01.000000 Adyen-9.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2023-10-20 09:52:11.068571 Adyen-9.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2023-10-20 09:52:01.000000 Adyen-9.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 09:52:11.068571 Adyen-9.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/BaseTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/BinLookupTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32428 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/CheckoutTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/CheckoutUtilityTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/ClientTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/ConfigurationTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/DataProtectionTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/DetermineEndpointTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/DisputesTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/LegalEntityManagementTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/ManagementTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/ModificationTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18978 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/PaymentTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/RecurringTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/StoredValueTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/TerminalTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14146 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/ThirdPartyPayoutTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/TransfersTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/UtilTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-20 09:52:01.000000 Adyen-9.1.0/test/__init__.py
```

### Comparing `Adyen-9.0.3/Adyen/__init__.py` & `Adyen-9.1.0/Adyen/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     AdyenCheckoutApi,
     AdyenTerminalApi,
     AdyenLegalEntityManagementApi,
     AdyenDataProtectionApi,
     AdyenTransfersApi,
     AdyenStoredValueApi,
     AdyenBalancePlatformApi,
+    AdyenDisputesApi,
 )
 
 from .httpclient import HTTPClient
 
 
 class Adyen(AdyenBase):
     def __init__(self, **kwargs):
@@ -43,14 +44,15 @@
         self.terminal = AdyenTerminalApi(client=self.client)
         self.management = AdyenManagementApi(client=self.client)
         self.legalEntityManagement = AdyenLegalEntityManagementApi(client=self.client)
         self.dataProtection = AdyenDataProtectionApi(client=self.client)
         self.transfers = AdyenTransfersApi(client=self.client)
         self.storedValue = AdyenStoredValueApi(client=self.client)
         self.balancePlatform = AdyenBalancePlatformApi(client=self.client)
+        self.disputes = AdyenDisputesApi(client=self.client)
 
 
 _base_adyen_obj = Adyen()
 recurring = _base_adyen_obj.recurring
 payment = _base_adyen_obj.payment
 payout = _base_adyen_obj.payout
 checkout = _base_adyen_obj.checkout
@@ -58,7 +60,8 @@
 terminal = _base_adyen_obj.terminal
 management = _base_adyen_obj.management
 legalEntityManagement = _base_adyen_obj.legalEntityManagement
 dataProtection = _base_adyen_obj.dataProtection
 transfers = _base_adyen_obj.transfers
 storedValue = _base_adyen_obj.storedValue
 balancePlatform = _base_adyen_obj.balancePlatform
+disputes = _base_adyen_obj.disputes
```

### Comparing `Adyen-9.0.3/Adyen/client.py` & `Adyen-9.1.0/Adyen/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
             api_recurring_version=None,
             api_terminal_version=None,
             api_legal_entity_management_version=None,
             api_data_protection_version=None,
             api_transfers_version=None,
             api_stored_value_version=None,
             api_balance_platform_version=None,
+            api_disputes_version=None,
 
     ):
         self.username = username
         self.password = password
         self.xapikey = xapikey
         self.review_payout_username = review_payout_username
         self.review_payout_password = review_payout_password
@@ -123,14 +124,15 @@
         self.api_recurring_version = api_recurring_version
         self.api_terminal_version = api_terminal_version
         self.api_legal_entity_management_version = api_legal_entity_management_version
         self.api_data_protection_version = api_data_protection_version
         self.api_transfers_version = api_transfers_version
         self.api_stored_value_version = api_stored_value_version
         self.api_balance_platform_version = api_balance_platform_version
+        self.api_disputes_version = api_disputes_version
 
     def _determine_api_url(self, platform, endpoint):
         if platform == "test":
             return endpoint
 
         if "pal-" in endpoint:
             if self.live_endpoint_prefix is None:
@@ -270,15 +272,17 @@
                    "payouts": self.api_payout_version,
                    "recurring": self.api_recurring_version,
                    "terminal": self.api_terminal_version,
                    "legalEntityManagement": self.api_legal_entity_management_version,
                    "dataProtection": self.api_data_protection_version,
                    "transfers": self.api_transfers_version,
                    "storedValue": self.api_stored_value_version,
-                   "balancePlatform": self.api_balance_platform_version}
+                   "balancePlatform": self.api_balance_platform_version,
+                   "disputes": self.api_disputes_version
+                          }
 
         new_version = f"v{version_lookup[service]}"
         endpoint = re.sub(r'\.com/v\d{1,2}', f".com/{new_version}", endpoint)
         return endpoint
 
     def call_adyen_api(
             self,
@@ -324,15 +328,16 @@
                     self.api_payout_version,
                     self.api_recurring_version,
                     self.api_terminal_version,
                     self.api_legal_entity_management_version,
                     self.api_data_protection_version,
                     self.api_transfers_version,
                     self.api_stored_value_version,
-                    self.api_balance_platform_version]
+                    self.api_balance_platform_version,
+                    self.api_disputes_version]
         if any(versions):
             endpoint = self._set_url_version(service, endpoint)
 
         headers = {
             self.APPLICATION_INFO_HEADER_NAME: settings.LIB_NAME,
             self.APPLICATION_VERSION_HEADER_NAME: settings.LIB_VERSION
         }
```

### Comparing `Adyen-9.0.3/Adyen/exceptions.py` & `Adyen-9.1.0/Adyen/exceptions.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/httpclient.py` & `Adyen-9.1.0/Adyen/httpclient.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/__init__.py` & `Adyen-9.1.0/Adyen/services/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 from .terminal import AdyenTerminalApi
 from .management import AdyenManagementApi
 from .legalEntityManagement import AdyenLegalEntityManagementApi
 from .dataProtection import AdyenDataProtectionApi
 from .transfers import AdyenTransfersApi
 from .storedValue import AdyenStoredValueApi
 from .balancePlatform import AdyenBalancePlatformApi
+from .disputes import AdyenDisputesApi
```

### Comparing `Adyen-9.0.3/Adyen/services/balancePlatform/__init__.py` & `Adyen-9.1.0/Adyen/services/balancePlatform/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/balancePlatform/account_holders_api.py` & `Adyen-9.1.0/Adyen/services/balancePlatform/account_holders_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/balancePlatform/balance_accounts_api.py` & `Adyen-9.1.0/Adyen/services/balancePlatform/balance_accounts_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/balancePlatform/bank_account_validation_api.py` & `Adyen-9.1.0/Adyen/services/balancePlatform/bank_account_validation_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/balancePlatform/grant_accounts_api.py` & `Adyen-9.1.0/Adyen/services/balancePlatform/grant_accounts_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/balancePlatform/grant_offers_api.py` & `Adyen-9.1.0/Adyen/services/balancePlatform/grant_offers_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/balancePlatform/payment_instrument_groups_api.py` & `Adyen-9.1.0/Adyen/services/balancePlatform/payment_instrument_groups_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/balancePlatform/payment_instruments_api.py` & `Adyen-9.1.0/Adyen/services/balancePlatform/payment_instruments_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/balancePlatform/platform_api.py` & `Adyen-9.1.0/Adyen/services/balancePlatform/platform_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/balancePlatform/transaction_rules_api.py` & `Adyen-9.1.0/Adyen/services/balancePlatform/transaction_rules_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/base.py` & `Adyen-9.1.0/Adyen/services/base.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/binlookup.py` & `Adyen-9.1.0/Adyen/services/binlookup.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/checkout/__init__.py` & `Adyen-9.1.0/Adyen/services/checkout/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/checkout/classic_checkout_sdk_api.py` & `Adyen-9.1.0/Adyen/services/checkout/classic_checkout_sdk_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/checkout/modifications_api.py` & `Adyen-9.1.0/Adyen/services/checkout/modifications_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/checkout/orders_api.py` & `Adyen-9.1.0/Adyen/services/checkout/orders_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/checkout/payment_links_api.py` & `Adyen-9.1.0/Adyen/services/checkout/payment_links_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/checkout/payments_api.py` & `Adyen-9.1.0/Adyen/services/checkout/payments_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/checkout/recurring_api.py` & `Adyen-9.1.0/Adyen/services/checkout/recurring_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/checkout/utility_api.py` & `Adyen-9.1.0/Adyen/services/checkout/utility_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/dataProtection.py` & `Adyen-9.1.0/Adyen/services/dataProtection.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/legalEntityManagement/__init__.py` & `Adyen-9.1.0/Adyen/services/legalEntityManagement/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/legalEntityManagement/business_lines_api.py` & `Adyen-9.1.0/Adyen/services/legalEntityManagement/business_lines_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/legalEntityManagement/documents_api.py` & `Adyen-9.1.0/Adyen/services/legalEntityManagement/documents_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/legalEntityManagement/hosted_onboarding_api.py` & `Adyen-9.1.0/Adyen/services/legalEntityManagement/hosted_onboarding_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/legalEntityManagement/legal_entities_api.py` & `Adyen-9.1.0/Adyen/services/legalEntityManagement/legal_entities_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/legalEntityManagement/pci_questionnaires_api.py` & `Adyen-9.1.0/Adyen/services/legalEntityManagement/pci_questionnaires_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/legalEntityManagement/terms_of_service_api.py` & `Adyen-9.1.0/Adyen/services/legalEntityManagement/terms_of_service_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/legalEntityManagement/transfer_instruments_api.py` & `Adyen-9.1.0/Adyen/services/legalEntityManagement/transfer_instruments_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/__init__.py` & `Adyen-9.1.0/Adyen/services/management/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/account_company_level_api.py` & `Adyen-9.1.0/Adyen/services/management/account_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/account_merchant_level_api.py` & `Adyen-9.1.0/Adyen/services/management/account_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/account_store_level_api.py` & `Adyen-9.1.0/Adyen/services/management/account_store_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/allowed_origins_company_level_api.py` & `Adyen-9.1.0/Adyen/services/management/allowed_origins_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/allowed_origins_merchant_level_api.py` & `Adyen-9.1.0/Adyen/services/management/allowed_origins_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/api_credentials_company_level_api.py` & `Adyen-9.1.0/Adyen/services/management/api_credentials_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/api_credentials_merchant_level_api.py` & `Adyen-9.1.0/Adyen/services/management/api_credentials_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/api_key_company_level_api.py` & `Adyen-9.1.0/Adyen/services/management/api_key_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/api_key_merchant_level_api.py` & `Adyen-9.1.0/Adyen/services/management/api_key_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/client_key_company_level_api.py` & `Adyen-9.1.0/Adyen/services/management/client_key_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/client_key_merchant_level_api.py` & `Adyen-9.1.0/Adyen/services/management/client_key_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/my_api_credential_api.py` & `Adyen-9.1.0/Adyen/services/management/my_api_credential_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/payment_methods_merchant_level_api.py` & `Adyen-9.1.0/Adyen/services/management/payment_methods_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/payout_settings_merchant_level_api.py` & `Adyen-9.1.0/Adyen/services/management/payout_settings_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/terminal_actions_company_level_api.py` & `Adyen-9.1.0/Adyen/services/management/terminal_actions_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/terminal_actions_terminal_level_api.py` & `Adyen-9.1.0/Adyen/services/management/terminal_actions_terminal_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/terminal_orders_company_level_api.py` & `Adyen-9.1.0/Adyen/services/management/terminal_orders_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/terminal_orders_merchant_level_api.py` & `Adyen-9.1.0/Adyen/services/management/terminal_orders_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/terminal_settings_company_level_api.py` & `Adyen-9.1.0/Adyen/services/management/terminal_settings_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/terminal_settings_merchant_level_api.py` & `Adyen-9.1.0/Adyen/services/management/terminal_settings_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/terminal_settings_store_level_api.py` & `Adyen-9.1.0/Adyen/services/management/terminal_settings_store_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/terminal_settings_terminal_level_api.py` & `Adyen-9.1.0/Adyen/services/management/terminal_settings_terminal_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/terminals_terminal_level_api.py` & `Adyen-9.1.0/Adyen/services/management/terminals_terminal_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/users_company_level_api.py` & `Adyen-9.1.0/Adyen/services/management/users_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/users_merchant_level_api.py` & `Adyen-9.1.0/Adyen/services/management/users_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/webhooks_company_level_api.py` & `Adyen-9.1.0/Adyen/services/management/webhooks_company_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/management/webhooks_merchant_level_api.py` & `Adyen-9.1.0/Adyen/services/management/webhooks_merchant_level_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/payments/__init__.py` & `Adyen-9.1.0/Adyen/services/payments/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/payments/general_api.py` & `Adyen-9.1.0/Adyen/services/payments/general_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/payments/modifications_api.py` & `Adyen-9.1.0/Adyen/services/payments/modifications_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/payouts/__init__.py` & `Adyen-9.1.0/Adyen/services/payouts/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/payouts/initialization_api.py` & `Adyen-9.1.0/Adyen/services/payouts/initialization_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/payouts/instant_payouts_api.py` & `Adyen-9.1.0/Adyen/services/payouts/instant_payouts_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/payouts/reviewing_api.py` & `Adyen-9.1.0/Adyen/services/payouts/reviewing_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/recurring.py` & `Adyen-9.1.0/Adyen/services/recurring.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/storedValue.py` & `Adyen-9.1.0/Adyen/services/storedValue.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/terminal.py` & `Adyen-9.1.0/Adyen/services/terminal.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/transfers/__init__.py` & `Adyen-9.1.0/Adyen/services/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/transfers/transactions_api.py` & `Adyen-9.1.0/Adyen/services/transfers/transactions_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/services/transfers/transfers_api.py` & `Adyen-9.1.0/Adyen/services/transfers/transfers_api.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen/util.py` & `Adyen-9.1.0/Adyen/util.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/Adyen.egg-info/PKG-INFO` & `Adyen-9.1.0/Adyen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Adyen
-Version: 9.0.3
+Version: 9.1.0
 Summary: Adyen Python Api
 Home-page: https://github.com/Adyen/adyen-python-api-library
 Author: Adyen
 Author-email: support@adyen.com
 Maintainer: Adyen
 Maintainer-email: support@adyen.com
 Keywords: payments,adyen,fintech
```

### Comparing `Adyen-9.0.3/Adyen.egg-info/SOURCES.txt` & `Adyen-9.1.0/Adyen.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 Adyen.egg-info/SOURCES.txt
 Adyen.egg-info/dependency_links.txt
 Adyen.egg-info/top_level.txt
 Adyen/services/__init__.py
 Adyen/services/base.py
 Adyen/services/binlookup.py
 Adyen/services/dataProtection.py
+Adyen/services/disputes.py
 Adyen/services/recurring.py
 Adyen/services/storedValue.py
 Adyen/services/terminal.py
 Adyen/services/balancePlatform/__init__.py
 Adyen/services/balancePlatform/account_holders_api.py
 Adyen/services/balancePlatform/balance_accounts_api.py
 Adyen/services/balancePlatform/bank_account_validation_api.py
@@ -87,14 +88,15 @@
 test/BinLookupTest.py
 test/CheckoutTest.py
 test/CheckoutUtilityTest.py
 test/ClientTest.py
 test/ConfigurationTest.py
 test/DataProtectionTest.py
 test/DetermineEndpointTest.py
+test/DisputesTest.py
 test/LegalEntityManagementTest.py
 test/ManagementTest.py
 test/ModificationTest.py
 test/PaymentTest.py
 test/RecurringTest.py
 test/StoredValueTest.py
 test/TerminalTest.py
```

### Comparing `Adyen-9.0.3/LICENSE.md` & `Adyen-9.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/PKG-INFO` & `Adyen-9.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Adyen
-Version: 9.0.3
+Version: 9.1.0
 Summary: Adyen Python Api
 Home-page: https://github.com/Adyen/adyen-python-api-library
 Author: Adyen
 Author-email: support@adyen.com
 Maintainer: Adyen
 Maintainer-email: support@adyen.com
 Keywords: payments,adyen,fintech
```

### Comparing `Adyen-9.0.3/setup.py` & `Adyen-9.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Adyen',
     packages=find_packages(include="Adyen*"),
-    version='9.0.3',
+    version='9.1.0',
     maintainer='Adyen',
     maintainer_email='support@adyen.com',
     description='Adyen Python Api',
     long_description="A Python client library for accessing Adyen APIs",
     author='Adyen',
     author_email='support@adyen.com',
     url='https://github.com/Adyen/adyen-python-api-library',
```

### Comparing `Adyen-9.0.3/test/BaseTest.py` & `Adyen-9.1.0/test/BaseTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/BinLookupTest.py` & `Adyen-9.1.0/test/BinLookupTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/CheckoutTest.py` & `Adyen-9.1.0/test/CheckoutTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/CheckoutUtilityTest.py` & `Adyen-9.1.0/test/CheckoutUtilityTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/ConfigurationTest.py` & `Adyen-9.1.0/test/ConfigurationTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/DataProtectionTest.py` & `Adyen-9.1.0/test/DataProtectionTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/DetermineEndpointTest.py` & `Adyen-9.1.0/test/DetermineEndpointTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/LegalEntityManagementTest.py` & `Adyen-9.1.0/test/LegalEntityManagementTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/ManagementTest.py` & `Adyen-9.1.0/test/ManagementTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/ModificationTest.py` & `Adyen-9.1.0/test/ModificationTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/PaymentTest.py` & `Adyen-9.1.0/test/PaymentTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/RecurringTest.py` & `Adyen-9.1.0/test/RecurringTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/StoredValueTest.py` & `Adyen-9.1.0/test/StoredValueTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/TerminalTest.py` & `Adyen-9.1.0/test/TerminalTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/ThirdPartyPayoutTest.py` & `Adyen-9.1.0/test/ThirdPartyPayoutTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/TransfersTest.py` & `Adyen-9.1.0/test/TransfersTest.py`

 * *Files identical despite different names*

### Comparing `Adyen-9.0.3/test/UtilTest.py` & `Adyen-9.1.0/test/UtilTest.py`

 * *Files identical despite different names*

