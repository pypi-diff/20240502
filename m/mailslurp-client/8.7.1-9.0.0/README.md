# Comparing `tmp/mailslurp-client-8.7.1.tar.gz` & `tmp/mailslurp-client-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mailslurp-client-8.7.1.tar", last modified: Mon Dec 21 22:39:32 2020, max compression
+gzip compressed data, was "dist/mailslurp-client-9.0.0.tar", last modified: Fri Jan  8 20:01:57 2021, max compression
```

## Comparing `mailslurp-client-8.7.1.tar` & `mailslurp-client-9.0.0.tar`

### file list

```diff
@@ -1,210 +1,218 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-12-21 22:39:32.966416 mailslurp-client-8.7.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9659 2020-12-21 22:39:32.966416 mailslurp-client-8.7.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7611 2020-12-21 22:38:59.000000 mailslurp-client-8.7.1/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-12-21 22:39:32.930416 mailslurp-client-8.7.1/mailslurp_client/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8075 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-12-21 22:39:32.934416 mailslurp-client-8.7.1/mailslurp_client/api/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1263 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    53327 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/alias_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22751 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/attachment_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16095 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/bulk_actions_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19916 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/common_actions_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25446 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/contact_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20979 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/domain_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    93035 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/email_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12296 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/form_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    48740 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/group_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    92603 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/inbox_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22149 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/mail_server_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11677 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/sent_emails_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25601 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/template_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    40087 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/wait_for_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    33350 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api/webhook_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26619 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/api_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13688 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/configuration.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4154 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/exceptions.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-12-21 22:39:32.950416 mailslurp-client-8.7.1/mailslurp_client/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6449 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/models/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8899 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/alias.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11050 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/alias_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9411 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/alias_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6154 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/attachment_meta_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4728 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/basic_auth_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4840 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/bulk_send_email_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10239 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/contact_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8908 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/contact_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4731 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/content_match_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7768 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/create_alias_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9412 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/create_contact_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3871 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/create_domain_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4570 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/create_group_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9342 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/create_inbox_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4683 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/create_template_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5611 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/create_webhook_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3895 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/describe_domain_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5661 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/describe_mail_server_domain_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7156 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/dns_lookup_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7233 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/dns_lookup_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3930 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/dns_lookup_results.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9856 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/domain_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5399 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/domain_preview.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5951 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/download_attachment_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16893 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/email.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7496 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/email_analysis.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4788 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/email_content_match_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9883 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/email_preview.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10708 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/email_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7255 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/email_verification_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5906 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/forward_email_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4719 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/group_contacts_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5978 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/group_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6118 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/group_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5619 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/html_validation_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11099 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/inbox.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7461 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/inbox_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4695 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/ip_address_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6412 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/match_option.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3985 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/match_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6284 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/name_server_record.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10170 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/page_alias.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10752 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/page_contact_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10497 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/page_email_preview.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10650 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/page_email_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10650 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/page_group_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10650 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/page_inbox_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10854 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/page_sent_email_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10803 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/page_template_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10701 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/page_thread_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10752 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/page_webhook_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6767 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/pageable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3844 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/raw_email_json.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9744 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/reply_to_alias_email_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11170 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/reply_to_email_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18962 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/send_email_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13170 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/sent_email_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11579 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/sent_email_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3862 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/set_inbox_favourited_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6087 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/simple_send_email_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4802 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/sort.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7004 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/template_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7210 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/template_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5108 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/template_variable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11145 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/thread_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3794 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/unread_count.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3767 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/update_alias_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4001 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/update_group_contacts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7804 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/update_inbox_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6165 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/upload_attachment_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4442 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/validation_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4624 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/validation_message.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6556 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/verify_email_address_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11111 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/wait_for_conditions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10940 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/webhook_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7722 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/webhook_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6515 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/webhook_test_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4487 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/webhook_test_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5469 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/mailslurp_client/models/webhook_test_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12688 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/mailslurp_client/rest.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-12-21 22:39:32.934416 mailslurp-client-8.7.1/mailslurp_client.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9659 2020-12-21 22:39:32.000000 mailslurp-client-8.7.1/mailslurp_client.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7895 2020-12-21 22:39:32.000000 mailslurp-client-8.7.1/mailslurp_client.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-12-21 22:39:32.000000 mailslurp-client-8.7.1/mailslurp_client.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2020-12-21 22:39:32.000000 mailslurp-client-8.7.1/mailslurp_client.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       17 2020-12-21 22:39:32.000000 mailslurp-client-8.7.1/mailslurp_client.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       69 2020-12-21 22:39:32.970416 mailslurp-client-8.7.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8240 2020-12-21 22:39:28.000000 mailslurp-client-8.7.1/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-12-21 22:39:32.966416 mailslurp-client-8.7.1/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2378 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_alias.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2630 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_alias_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2238 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_alias_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2516 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_alias_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2015 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_attachment_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1930 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_attachment_meta_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1907 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_basic_auth_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1657 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_bulk_actions_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2883 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_bulk_send_email_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1828 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_common_actions_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1852 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_contact_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2531 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_contact_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2305 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_contact_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1842 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_content_match_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1936 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_create_alias_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2220 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_create_contact_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1841 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_create_domain_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1892 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_create_group_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2074 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_create_inbox_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1952 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_create_template_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2045 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_create_webhook_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_describe_domain_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2619 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_describe_mail_server_domain_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1935 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_dns_lookup_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2006 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_dns_lookup_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2348 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_dns_lookup_results.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1687 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_domain_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2435 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_domain_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2071 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_domain_preview.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1948 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_download_attachment_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2885 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_email.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1928 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_email_analysis.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2070 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_email_content_match_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3824 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_email_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2252 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_email_preview.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2591 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_email_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2152 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_email_verification_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1352 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_form_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2056 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_forward_email_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3885 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_group_contacts_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2569 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_group_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2048 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_group_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2125 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_group_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2291 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_html_validation_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2065 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_inbox.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3614 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_inbox_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2241 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_inbox_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1894 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_ip_address_result.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1880 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_mail_server_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1823 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_match_option.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1981 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_match_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2027 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_name_server_record.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3181 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_page_alias.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3309 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_page_contact_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3434 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_page_email_preview.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3560 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_page_email_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3049 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_page_group_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3191 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_page_inbox_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3617 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_page_sent_email_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3262 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_page_template_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3582 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_page_thread_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3224 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_page_webhook_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2017 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_pageable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1796 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_raw_email_json.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2171 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_reply_to_alias_email_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2177 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_reply_to_email_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2559 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_send_email_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2555 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_sent_email_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2890 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_sent_email_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1491 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_sent_emails_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1909 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_set_inbox_favourited_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1967 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_simple_send_email_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1738 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_sort.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_template_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2553 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_template_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2492 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_template_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1917 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_template_variable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2796 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_thread_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1777 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_unread_count.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1828 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_update_alias_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1969 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_update_group_contacts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_update_inbox_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1964 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_upload_attachment_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2384 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_validation_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1887 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_validation_message.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2069 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_verify_email_address_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2250 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_wait_for_conditions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2327 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_wait_for_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2077 2020-12-21 22:39:02.000000 mailslurp-client-8.7.1/test/test_webhook_controller_api.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2262 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_webhook_dto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2418 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_webhook_projection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2118 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_webhook_test_request.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1877 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_webhook_test_response.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2752 2020-12-21 22:39:01.000000 mailslurp-client-8.7.1/test/test_webhook_test_result.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 20:01:57.539490 mailslurp-client-9.0.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9659 2021-01-08 20:01:57.539490 mailslurp-client-9.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7611 2021-01-08 20:01:19.000000 mailslurp-client-9.0.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 20:01:57.515489 mailslurp-client-9.0.0/mailslurp_client/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8420 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 20:01:57.519489 mailslurp-client-9.0.0/mailslurp_client/api/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1263 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    53329 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/alias_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22751 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/attachment_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16095 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/bulk_actions_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21697 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/common_actions_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25446 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/contact_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20979 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/domain_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    93035 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/email_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12296 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/form_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    48740 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/group_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   114601 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/inbox_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22149 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/mail_server_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11677 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/sent_emails_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25601 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/template_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    40087 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/wait_for_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    33350 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api/webhook_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26619 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/api_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13688 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/configuration.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4154 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/exceptions.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 20:01:57.531489 mailslurp-client-9.0.0/mailslurp_client/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6794 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/models/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8899 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/alias.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11050 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/alias_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9411 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/alias_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6154 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/attachment_meta_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4728 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/basic_auth_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4840 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/bulk_send_email_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10239 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/contact_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8908 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/contact_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4731 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/content_match_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7768 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/create_alias_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9412 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/create_contact_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3871 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/create_domain_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4570 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/create_group_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13214 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/create_inbox_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4683 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/create_template_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5611 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/create_webhook_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3895 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/describe_domain_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5661 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/describe_mail_server_domain_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7156 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/dns_lookup_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7233 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/dns_lookup_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3930 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/dns_lookup_results.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10898 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/domain_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7459 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/domain_name_record.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5399 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/domain_preview.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5951 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/download_attachment_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16893 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/email.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7496 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/email_analysis.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4788 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/email_content_match_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9883 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/email_preview.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10708 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/email_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7255 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/email_verification_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5520 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/expired_inbox_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6642 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/expired_inbox_record_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5906 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/forward_email_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4719 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/group_contacts_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5978 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/group_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6118 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/group_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5619 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/html_validation_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12511 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/inbox.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7461 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/inbox_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4695 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/ip_address_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6412 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/match_option.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3985 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/match_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6284 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/name_server_record.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10170 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/page_alias.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10752 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/page_contact_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10497 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/page_email_preview.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10650 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/page_email_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11313 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/page_expired_inbox_record_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10650 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/page_group_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10650 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/page_inbox_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10854 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/page_sent_email_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10803 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/page_template_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10701 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/page_thread_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10752 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/page_webhook_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6767 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/pageable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3844 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/raw_email_json.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9744 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/reply_to_alias_email_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11170 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/reply_to_email_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18962 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/send_email_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13170 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/sent_email_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11579 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/sent_email_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4016 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/set_inbox_favourited_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6179 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/simple_send_email_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4802 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/sort.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7004 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/template_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7210 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/template_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5108 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/template_variable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11145 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/thread_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3794 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/unread_count.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3767 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/update_alias_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4001 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/update_group_contacts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8370 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/update_inbox_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6165 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/upload_attachment_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4442 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/validation_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4624 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/validation_message.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6556 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/verify_email_address_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11111 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/mailslurp_client/models/wait_for_conditions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10940 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/models/webhook_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7722 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/models/webhook_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6515 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/models/webhook_test_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4487 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/models/webhook_test_response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5469 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/models/webhook_test_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12688 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/mailslurp_client/rest.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 20:01:57.519489 mailslurp-client-9.0.0/mailslurp_client.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9659 2021-01-08 20:01:57.000000 mailslurp-client-9.0.0/mailslurp_client.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8267 2021-01-08 20:01:57.000000 mailslurp-client-9.0.0/mailslurp_client.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-01-08 20:01:57.000000 mailslurp-client-9.0.0/mailslurp_client.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2021-01-08 20:01:57.000000 mailslurp-client-9.0.0/mailslurp_client.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       17 2021-01-08 20:01:57.000000 mailslurp-client-9.0.0/mailslurp_client.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       69 2021-01-08 20:01:57.543490 mailslurp-client-9.0.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8240 2021-01-08 20:01:54.000000 mailslurp-client-9.0.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-01-08 20:01:57.539490 mailslurp-client-9.0.0/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2378 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_alias.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2630 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_alias_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2238 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_alias_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2516 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_alias_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2015 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_attachment_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1930 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_attachment_meta_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1907 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_basic_auth_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1657 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_bulk_actions_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2883 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_bulk_send_email_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1828 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_common_actions_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1852 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_contact_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2531 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_contact_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2305 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_contact_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1842 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_content_match_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1936 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_create_alias_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2220 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_create_contact_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1841 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_create_domain_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1892 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_create_group_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2115 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_create_inbox_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1952 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_create_template_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2045 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_create_webhook_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_describe_domain_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2619 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_describe_mail_server_domain_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1935 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_dns_lookup_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2006 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_dns_lookup_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2348 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_dns_lookup_results.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1687 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_domain_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2804 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_domain_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2123 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_domain_name_record.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2071 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_domain_preview.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1948 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_download_attachment_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2885 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_email.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1928 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_email_analysis.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2070 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_email_content_match_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3824 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_email_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2252 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_email_preview.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2591 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_email_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2152 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_email_verification_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1959 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_expired_inbox_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2317 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_expired_inbox_record_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1352 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_form_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2056 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_forward_email_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3885 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_group_contacts_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2569 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_group_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2048 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_group_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2125 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_group_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2291 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_html_validation_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2065 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_inbox.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4201 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_inbox_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2241 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_inbox_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1894 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_ip_address_result.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1880 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_mail_server_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1823 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_match_option.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1981 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_match_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2027 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_name_server_record.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3181 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_page_alias.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3309 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_page_contact_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3434 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_page_email_preview.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3560 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_page_email_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3229 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_page_expired_inbox_record_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3049 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_page_group_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3191 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_page_inbox_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3617 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_page_sent_email_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3262 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_page_template_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3582 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_page_thread_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3224 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_page_webhook_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2017 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_pageable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1796 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_raw_email_json.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2171 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_reply_to_alias_email_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2177 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_reply_to_email_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2559 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_send_email_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2555 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_sent_email_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2890 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_sent_email_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1491 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_sent_emails_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1909 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_set_inbox_favourited_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1967 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_simple_send_email_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1738 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_sort.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_template_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2553 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_template_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2492 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_template_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1917 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_template_variable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2796 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_thread_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1777 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_unread_count.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1828 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_update_alias_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1969 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_update_group_contacts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2080 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_update_inbox_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1964 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_upload_attachment_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2384 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_validation_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1887 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_validation_message.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2069 2021-01-08 20:01:21.000000 mailslurp-client-9.0.0/test/test_verify_email_address_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2250 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_wait_for_conditions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2327 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_wait_for_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2077 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_webhook_controller_api.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2262 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_webhook_dto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2418 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_webhook_projection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2118 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_webhook_test_request.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1877 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_webhook_test_response.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2752 2021-01-08 20:01:22.000000 mailslurp-client-9.0.0/test/test_webhook_test_result.py
```

### Comparing `mailslurp-client-8.7.1/PKG-INFO` & `mailslurp-client-9.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailslurp-client
-Version: 8.7.1
+Version: 9.0.0
 Summary: Official MailSlurp Python SDK Email API
 Home-page: https://www.mailslurp.com/docs/python
 Author: MailSlurp
 Author-email: support@mailslurp.zendesk.com
 License: UNKNOWN
 Description: 
         # MailSlurp Python Client
```

### Comparing `mailslurp-client-8.7.1/README.md` & `mailslurp-client-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/__init__.py` & `mailslurp-client-9.0.0/mailslurp_client/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 6.5.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "8.7.1"
+__version__ = "9.0.0"
 
 # import apis into sdk package
 from mailslurp_client.api.alias_controller_api import AliasControllerApi
 from mailslurp_client.api.attachment_controller_api import AttachmentControllerApi
 from mailslurp_client.api.bulk_actions_controller_api import BulkActionsControllerApi
 from mailslurp_client.api.common_actions_controller_api import CommonActionsControllerApi
 from mailslurp_client.api.contact_controller_api import ContactControllerApi
@@ -60,22 +60,25 @@
 from mailslurp_client.models.create_webhook_options import CreateWebhookOptions
 from mailslurp_client.models.dns_lookup_options import DNSLookupOptions
 from mailslurp_client.models.dns_lookup_result import DNSLookupResult
 from mailslurp_client.models.dns_lookup_results import DNSLookupResults
 from mailslurp_client.models.describe_domain_options import DescribeDomainOptions
 from mailslurp_client.models.describe_mail_server_domain_result import DescribeMailServerDomainResult
 from mailslurp_client.models.domain_dto import DomainDto
+from mailslurp_client.models.domain_name_record import DomainNameRecord
 from mailslurp_client.models.domain_preview import DomainPreview
 from mailslurp_client.models.download_attachment_dto import DownloadAttachmentDto
 from mailslurp_client.models.email import Email
 from mailslurp_client.models.email_analysis import EmailAnalysis
 from mailslurp_client.models.email_content_match_result import EmailContentMatchResult
 from mailslurp_client.models.email_preview import EmailPreview
 from mailslurp_client.models.email_projection import EmailProjection
 from mailslurp_client.models.email_verification_result import EmailVerificationResult
+from mailslurp_client.models.expired_inbox_dto import ExpiredInboxDto
+from mailslurp_client.models.expired_inbox_record_projection import ExpiredInboxRecordProjection
 from mailslurp_client.models.forward_email_options import ForwardEmailOptions
 from mailslurp_client.models.group_contacts_dto import GroupContactsDto
 from mailslurp_client.models.group_dto import GroupDto
 from mailslurp_client.models.group_projection import GroupProjection
 from mailslurp_client.models.html_validation_result import HTMLValidationResult
 from mailslurp_client.models.ip_address_result import IPAddressResult
 from mailslurp_client.models.inbox import Inbox
@@ -83,14 +86,15 @@
 from mailslurp_client.models.match_option import MatchOption
 from mailslurp_client.models.match_options import MatchOptions
 from mailslurp_client.models.name_server_record import NameServerRecord
 from mailslurp_client.models.page_alias import PageAlias
 from mailslurp_client.models.page_contact_projection import PageContactProjection
 from mailslurp_client.models.page_email_preview import PageEmailPreview
 from mailslurp_client.models.page_email_projection import PageEmailProjection
+from mailslurp_client.models.page_expired_inbox_record_projection import PageExpiredInboxRecordProjection
 from mailslurp_client.models.page_group_projection import PageGroupProjection
 from mailslurp_client.models.page_inbox_projection import PageInboxProjection
 from mailslurp_client.models.page_sent_email_projection import PageSentEmailProjection
 from mailslurp_client.models.page_template_projection import PageTemplateProjection
 from mailslurp_client.models.page_thread_projection import PageThreadProjection
 from mailslurp_client.models.page_webhook_projection import PageWebhookProjection
 from mailslurp_client.models.pageable import Pageable
```

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/__init__.py` & `mailslurp-client-9.0.0/mailslurp_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/alias_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/alias_controller_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -889,15 +889,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def send_alias_email(self, alias_id, **kwargs):  # noqa: E501
         """Send an email from an alias inbox  # noqa: E501
 
-        Send an email from an alias. Replies to the email will be forwared to the alias masked email address  # noqa: E501
+        Send an email from an alias. Replies to the email will be forwarded to the alias masked email address  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.send_alias_email(alias_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str alias_id: aliasId (required)
@@ -915,15 +915,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.send_alias_email_with_http_info(alias_id, **kwargs)  # noqa: E501
 
     def send_alias_email_with_http_info(self, alias_id, **kwargs):  # noqa: E501
         """Send an email from an alias inbox  # noqa: E501
 
-        Send an email from an alias. Replies to the email will be forwared to the alias masked email address  # noqa: E501
+        Send an email from an alias. Replies to the email will be forwarded to the alias masked email address  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.send_alias_email_with_http_info(alias_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str alias_id: aliasId (required)
```

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/attachment_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/attachment_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/bulk_actions_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/bulk_actions_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/common_actions_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/common_actions_controller_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,48 +32,50 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def create_new_email_address(self, **kwargs):  # noqa: E501
+    def create_new_email_address(self, use_domain_pool, **kwargs):  # noqa: E501
         """Create new random inbox  # noqa: E501
 
         Returns an Inbox with an `id` and an `emailAddress`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_new_email_address(async_req=True)
+        >>> thread = api.create_new_email_address(use_domain_pool, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param bool use_domain_pool: useDomainPool (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Inbox
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_new_email_address_with_http_info(**kwargs)  # noqa: E501
+        return self.create_new_email_address_with_http_info(use_domain_pool, **kwargs)  # noqa: E501
 
-    def create_new_email_address_with_http_info(self, **kwargs):  # noqa: E501
+    def create_new_email_address_with_http_info(self, use_domain_pool, **kwargs):  # noqa: E501
         """Create new random inbox  # noqa: E501
 
         Returns an Inbox with an `id` and an `emailAddress`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_new_email_address_with_http_info(async_req=True)
+        >>> thread = api.create_new_email_address_with_http_info(use_domain_pool, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param bool use_domain_pool: useDomainPool (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -83,14 +85,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
+            'use_domain_pool'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -101,20 +104,26 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method create_new_email_address" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'use_domain_pool' is set
+        if self.api_client.client_side_validation and ('use_domain_pool' not in local_var_params or  # noqa: E501
+                                                        local_var_params['use_domain_pool'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `use_domain_pool` when calling `create_new_email_address`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'use_domain_pool' in local_var_params and local_var_params['use_domain_pool'] is not None:  # noqa: E501
+            query_params.append(('useDomainPool', local_var_params['use_domain_pool']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -137,48 +146,50 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def create_new_email_address1(self, **kwargs):  # noqa: E501
+    def create_new_email_address1(self, use_domain_pool, **kwargs):  # noqa: E501
         """Create new random inbox  # noqa: E501
 
         Returns an Inbox with an `id` and an `emailAddress`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_new_email_address1(async_req=True)
+        >>> thread = api.create_new_email_address1(use_domain_pool, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param bool use_domain_pool: useDomainPool (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Inbox
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_new_email_address1_with_http_info(**kwargs)  # noqa: E501
+        return self.create_new_email_address1_with_http_info(use_domain_pool, **kwargs)  # noqa: E501
 
-    def create_new_email_address1_with_http_info(self, **kwargs):  # noqa: E501
+    def create_new_email_address1_with_http_info(self, use_domain_pool, **kwargs):  # noqa: E501
         """Create new random inbox  # noqa: E501
 
         Returns an Inbox with an `id` and an `emailAddress`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.create_new_email_address1_with_http_info(async_req=True)
+        >>> thread = api.create_new_email_address1_with_http_info(use_domain_pool, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param bool use_domain_pool: useDomainPool (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -188,14 +199,15 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
+            'use_domain_pool'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -206,20 +218,26 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method create_new_email_address1" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'use_domain_pool' is set
+        if self.api_client.client_side_validation and ('use_domain_pool' not in local_var_params or  # noqa: E501
+                                                        local_var_params['use_domain_pool'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `use_domain_pool` when calling `create_new_email_address1`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'use_domain_pool' in local_var_params and local_var_params['use_domain_pool'] is not None:  # noqa: E501
+            query_params.append(('useDomainPool', local_var_params['use_domain_pool']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
```

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/contact_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/contact_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/domain_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/domain_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/email_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/email_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/form_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/form_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/group_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/group_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/inbox_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/inbox_controller_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,20 +42,21 @@
         Create a new inbox and with a randomized email address to send and receive from. Pass emailAddress parameter if you wish to use a specific email address. Creating an inbox is required before sending or receiving emails. If writing tests it is recommended that you create a new inbox during each test method so that it is unique and empty.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_inbox(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str description: Optional description for an inbox.
-        :param str email_address: Optional email address including domain you wish inbox to use (eg: test123@mydomain.com). Only supports domains that you have registered and verified with MailSlurp using dashboard or `createDomain` method.
-        :param datetime expires_at: Optional expires at timestamp. If your plan supports this feature you can specify when an inbox should expire. If left empty inbox will exist permanently or expire when your plan dictates
-        :param bool favourite: Is inbox favourited.
-        :param str name: Optional name for an inbox.
-        :param list[str] tags: Optional tags for an inbox. Can be used for searching and filtering inboxes.
+        :param str description: Optional description of the inbox for labelling purposes. Is shown in the dashboard and can be used with
+        :param str email_address: A custom email address to use with the inbox. Defaults to null. When null MailSlurp will assign a random email address to the inbox such as `123@mailslurp.com`. If you use the `useDomainPool` option when the email address is null it will generate an email address with a more varied domain ending such as `123@mailslurp.info` or `123@mailslurp.biz`. When a custom email address is provided the address is split into a domain and the domain is queried against your user. If you have created the domain in the MailSlurp dashboard and verified it you can use any email address that ends with the domain. Send an email to this address and the inbox will receive and store it for you. To retrieve the email use the Inbox and Email Controller endpoints with the inbox ID.
+        :param datetime expires_at: Optional inbox expiration date. If null then this inbox is permanent and the emails in it won't be deleted. If an expiration date is provided or is required by your plan the inbox will be closed when the expiration time is reached. Expired inboxes still contain their emails but can no longer send or receive emails. An ExpiredInboxRecord is created when an inbox and the email address and inbox ID are recorded. The expiresAt property is a timestamp string in ISO DateTime Format yyyy-MM-dd'T'HH:mm:ss.SSSXXX.
+        :param bool favourite: Is the inbox favorited. Favouriting inboxes is typically done in the dashboard for quick access or filtering
+        :param str name: Optional name of the inbox. Displayed in the dashboard for easier search
+        :param list[str] tags: Tags that inbox has been tagged with. Tags can be added to inboxes to group different inboxes within an account. You can also search for inboxes by tag in the dashboard UI.
+        :param bool use_domain_pool: Use the MailSlurp domain name pool with this inbox when creating the email address. Defaults to null. If enabled the inbox will be an email address with a domain randomly chosen from a list of the MailSlurp domains. This is useful when the default `@mailslurp.com` email addresses used with inboxes are blocked or considered spam by a provider or receiving service. When domain pool is enabled an email address will be generated ending in `@mailslurp.{world,info,xyz,...}` . This means a TLD is randomly selecting from a list of `.biz`, `.info`, `.xyz` etc to add variance to the generated email addresses. When null or false MailSlurp uses the default behavior of `@mailslurp.com` or custom email address provided by the emailAddress field.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -72,20 +73,21 @@
         Create a new inbox and with a randomized email address to send and receive from. Pass emailAddress parameter if you wish to use a specific email address. Creating an inbox is required before sending or receiving emails. If writing tests it is recommended that you create a new inbox during each test method so that it is unique and empty.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_inbox_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str description: Optional description for an inbox.
-        :param str email_address: Optional email address including domain you wish inbox to use (eg: test123@mydomain.com). Only supports domains that you have registered and verified with MailSlurp using dashboard or `createDomain` method.
-        :param datetime expires_at: Optional expires at timestamp. If your plan supports this feature you can specify when an inbox should expire. If left empty inbox will exist permanently or expire when your plan dictates
-        :param bool favourite: Is inbox favourited.
-        :param str name: Optional name for an inbox.
-        :param list[str] tags: Optional tags for an inbox. Can be used for searching and filtering inboxes.
+        :param str description: Optional description of the inbox for labelling purposes. Is shown in the dashboard and can be used with
+        :param str email_address: A custom email address to use with the inbox. Defaults to null. When null MailSlurp will assign a random email address to the inbox such as `123@mailslurp.com`. If you use the `useDomainPool` option when the email address is null it will generate an email address with a more varied domain ending such as `123@mailslurp.info` or `123@mailslurp.biz`. When a custom email address is provided the address is split into a domain and the domain is queried against your user. If you have created the domain in the MailSlurp dashboard and verified it you can use any email address that ends with the domain. Send an email to this address and the inbox will receive and store it for you. To retrieve the email use the Inbox and Email Controller endpoints with the inbox ID.
+        :param datetime expires_at: Optional inbox expiration date. If null then this inbox is permanent and the emails in it won't be deleted. If an expiration date is provided or is required by your plan the inbox will be closed when the expiration time is reached. Expired inboxes still contain their emails but can no longer send or receive emails. An ExpiredInboxRecord is created when an inbox and the email address and inbox ID are recorded. The expiresAt property is a timestamp string in ISO DateTime Format yyyy-MM-dd'T'HH:mm:ss.SSSXXX.
+        :param bool favourite: Is the inbox favorited. Favouriting inboxes is typically done in the dashboard for quick access or filtering
+        :param str name: Optional name of the inbox. Displayed in the dashboard for easier search
+        :param list[str] tags: Tags that inbox has been tagged with. Tags can be added to inboxes to group different inboxes within an account. You can also search for inboxes by tag in the dashboard UI.
+        :param bool use_domain_pool: Use the MailSlurp domain name pool with this inbox when creating the email address. Defaults to null. If enabled the inbox will be an email address with a domain randomly chosen from a list of the MailSlurp domains. This is useful when the default `@mailslurp.com` email addresses used with inboxes are blocked or considered spam by a provider or receiving service. When domain pool is enabled an email address will be generated ending in `@mailslurp.{world,info,xyz,...}` . This means a TLD is randomly selecting from a list of `.biz`, `.info`, `.xyz` etc to add variance to the generated email addresses. When null or false MailSlurp uses the default behavior of `@mailslurp.com` or custom email address provided by the emailAddress field.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -100,15 +102,16 @@
 
         all_params = [
             'description',
             'email_address',
             'expires_at',
             'favourite',
             'name',
-            'tags'
+            'tags',
+            'use_domain_pool'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -138,14 +141,16 @@
         if 'favourite' in local_var_params and local_var_params['favourite'] is not None:  # noqa: E501
             query_params.append(('favourite', local_var_params['favourite']))  # noqa: E501
         if 'name' in local_var_params and local_var_params['name'] is not None:  # noqa: E501
             query_params.append(('name', local_var_params['name']))  # noqa: E501
         if 'tags' in local_var_params and local_var_params['tags'] is not None:  # noqa: E501
             query_params.append(('tags', local_var_params['tags']))  # noqa: E501
             collection_formats['tags'] = 'multi'  # noqa: E501
+        if 'use_domain_pool' in local_var_params and local_var_params['use_domain_pool'] is not None:  # noqa: E501
+            query_params.append(('useDomainPool', local_var_params['use_domain_pool']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -390,15 +395,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_inbox(self, inbox_id, **kwargs):  # noqa: E501
         """Delete inbox  # noqa: E501
 
-        Permanently delete an inbox and associated email address aswell as all emails within the given inbox. This action cannot be undone. Note: deleting an inbox will not affect your account usage. Monthly inbox usage is based on how many inboxes you create within 30 days, not how many exist at time of request.  # noqa: E501
+        Permanently delete an inbox and associated email address as well as all emails within the given inbox. This action cannot be undone. Note: deleting an inbox will not affect your account usage. Monthly inbox usage is based on how many inboxes you create within 30 days, not how many exist at time of request.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_inbox(inbox_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str inbox_id: inboxId (required)
@@ -415,15 +420,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.delete_inbox_with_http_info(inbox_id, **kwargs)  # noqa: E501
 
     def delete_inbox_with_http_info(self, inbox_id, **kwargs):  # noqa: E501
         """Delete inbox  # noqa: E501
 
-        Permanently delete an inbox and associated email address aswell as all emails within the given inbox. This action cannot be undone. Note: deleting an inbox will not affect your account usage. Monthly inbox usage is based on how many inboxes you create within 30 days, not how many exist at time of request.  # noqa: E501
+        Permanently delete an inbox and associated email address as well as all emails within the given inbox. This action cannot be undone. Note: deleting an inbox will not affect your account usage. Monthly inbox usage is based on how many inboxes you create within 30 days, not how many exist at time of request.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_inbox_with_http_info(inbox_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str inbox_id: inboxId (required)
@@ -776,14 +781,362 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def get_expired_inbox_record_by_id(self, expired_id, **kwargs):  # noqa: E501
+        """Get an expired inbox record  # noqa: E501
+
+        Inboxes created with an expiration date will expire after the given date and be moved to an ExpiredInbox entity. You can still read emails in the inbox but it can no longer send or receive emails. Fetch the expired inboxes to view the old inboxes properties  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_expired_inbox_record_by_id(expired_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str expired_id: ID of the ExpiredInboxRecord you want to retrieve. This is different from the ID of the inbox you are interested in. See other methods for getting ExpiredInboxRecord for an inbox inboxId) (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: ExpiredInboxDto
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_expired_inbox_record_by_id_with_http_info(expired_id, **kwargs)  # noqa: E501
+
+    def get_expired_inbox_record_by_id_with_http_info(self, expired_id, **kwargs):  # noqa: E501
+        """Get an expired inbox record  # noqa: E501
+
+        Inboxes created with an expiration date will expire after the given date and be moved to an ExpiredInbox entity. You can still read emails in the inbox but it can no longer send or receive emails. Fetch the expired inboxes to view the old inboxes properties  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_expired_inbox_record_by_id_with_http_info(expired_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str expired_id: ID of the ExpiredInboxRecord you want to retrieve. This is different from the ID of the inbox you are interested in. See other methods for getting ExpiredInboxRecord for an inbox inboxId) (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(ExpiredInboxDto, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'expired_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_expired_inbox_record_by_id" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'expired_id' is set
+        if self.api_client.client_side_validation and ('expired_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['expired_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `expired_id` when calling `get_expired_inbox_record_by_id`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'expired_id' in local_var_params:
+            path_params['expiredId'] = local_var_params['expired_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['API_KEY']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/inboxes/expired-records/{expiredId}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='ExpiredInboxDto',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_expired_inbox_record_by_inbox_id(self, inbox_id, **kwargs):  # noqa: E501
+        """Get expired inbox record for a previously existing inbox  # noqa: E501
+
+        Use the inboxId to return an ExpiredInboxRecord if an inbox has expired. Inboxes expire and are disabled if an expiration date is set or plan requires. Returns 404 if no expired inbox is found for the inboxId  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_expired_inbox_record_by_inbox_id(inbox_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str inbox_id: ID of inbox you want to retrieve (not the inbox ID) (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: ExpiredInboxDto
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_expired_inbox_record_by_inbox_id_with_http_info(inbox_id, **kwargs)  # noqa: E501
+
+    def get_expired_inbox_record_by_inbox_id_with_http_info(self, inbox_id, **kwargs):  # noqa: E501
+        """Get expired inbox record for a previously existing inbox  # noqa: E501
+
+        Use the inboxId to return an ExpiredInboxRecord if an inbox has expired. Inboxes expire and are disabled if an expiration date is set or plan requires. Returns 404 if no expired inbox is found for the inboxId  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_expired_inbox_record_by_inbox_id_with_http_info(inbox_id, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param str inbox_id: ID of inbox you want to retrieve (not the inbox ID) (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(ExpiredInboxDto, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'inbox_id'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_expired_inbox_record_by_inbox_id" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'inbox_id' is set
+        if self.api_client.client_side_validation and ('inbox_id' not in local_var_params or  # noqa: E501
+                                                        local_var_params['inbox_id'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `inbox_id` when calling `get_expired_inbox_record_by_inbox_id`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'inbox_id' in local_var_params:
+            path_params['inboxId'] = local_var_params['inbox_id']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['API_KEY']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/inboxes/{inboxId}/expired-record', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='ExpiredInboxDto',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_expired_inbox_records(self, **kwargs):  # noqa: E501
+        """List records of expired inboxes  # noqa: E501
+
+        Inboxes created with an expiration date will expire after the given date. An ExpiredInboxRecord is created that records the inboxes old ID and email address. You can still read emails in the inbox (using the inboxes old ID) but the email address associated with the inbox can no longer send or receive emails. Fetch expired inbox records to view the old inboxes properties  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_expired_inbox_records(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int page: Optional page index in inbox sent email list pagination
+        :param int size: Optional page size in inbox sent email list pagination
+        :param str sort: Optional createdAt sort direction ASC or DESC
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: PageExpiredInboxRecordProjection
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_expired_inbox_records_with_http_info(**kwargs)  # noqa: E501
+
+    def get_expired_inbox_records_with_http_info(self, **kwargs):  # noqa: E501
+        """List records of expired inboxes  # noqa: E501
+
+        Inboxes created with an expiration date will expire after the given date. An ExpiredInboxRecord is created that records the inboxes old ID and email address. You can still read emails in the inbox (using the inboxes old ID) but the email address associated with the inbox can no longer send or receive emails. Fetch expired inbox records to view the old inboxes properties  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_expired_inbox_records_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param int page: Optional page index in inbox sent email list pagination
+        :param int size: Optional page size in inbox sent email list pagination
+        :param str sort: Optional createdAt sort direction ASC or DESC
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(PageExpiredInboxRecordProjection, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'page',
+            'size',
+            'sort'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_expired_inbox_records" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'page' in local_var_params and local_var_params['page'] is not None:  # noqa: E501
+            query_params.append(('page', local_var_params['page']))  # noqa: E501
+        if 'size' in local_var_params and local_var_params['size'] is not None:  # noqa: E501
+            query_params.append(('size', local_var_params['size']))  # noqa: E501
+        if 'sort' in local_var_params and local_var_params['sort'] is not None:  # noqa: E501
+            query_params.append(('sort', local_var_params['sort']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['API_KEY']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/inboxes/expired-records', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='PageExpiredInboxRecordProjection',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def get_inbox(self, inbox_id, **kwargs):  # noqa: E501
         """Get Inbox  # noqa: E501
 
         Returns an inbox's properties, including its email address and ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_inbox(inbox_id, async_req=True)
```

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/mail_server_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/mail_server_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/sent_emails_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/sent_emails_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/template_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/template_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/wait_for_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/wait_for_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api/webhook_controller_api.py` & `mailslurp-client-9.0.0/mailslurp_client/api/webhook_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/api_client.py` & `mailslurp-client-9.0.0/mailslurp_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/8.7.1/python'
+        self.user_agent = 'OpenAPI-Generator/9.0.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `mailslurp-client-8.7.1/mailslurp_client/configuration.py` & `mailslurp-client-9.0.0/mailslurp_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 6.5.2\n"\
-               "SDK Package Version: 8.7.1".\
+               "SDK Package Version: 9.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `mailslurp-client-8.7.1/mailslurp_client/exceptions.py` & `mailslurp-client-9.0.0/mailslurp_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/__init__.py` & `mailslurp-client-9.0.0/mailslurp_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,25 @@
 from mailslurp_client.models.create_webhook_options import CreateWebhookOptions
 from mailslurp_client.models.dns_lookup_options import DNSLookupOptions
 from mailslurp_client.models.dns_lookup_result import DNSLookupResult
 from mailslurp_client.models.dns_lookup_results import DNSLookupResults
 from mailslurp_client.models.describe_domain_options import DescribeDomainOptions
 from mailslurp_client.models.describe_mail_server_domain_result import DescribeMailServerDomainResult
 from mailslurp_client.models.domain_dto import DomainDto
+from mailslurp_client.models.domain_name_record import DomainNameRecord
 from mailslurp_client.models.domain_preview import DomainPreview
 from mailslurp_client.models.download_attachment_dto import DownloadAttachmentDto
 from mailslurp_client.models.email import Email
 from mailslurp_client.models.email_analysis import EmailAnalysis
 from mailslurp_client.models.email_content_match_result import EmailContentMatchResult
 from mailslurp_client.models.email_preview import EmailPreview
 from mailslurp_client.models.email_projection import EmailProjection
 from mailslurp_client.models.email_verification_result import EmailVerificationResult
+from mailslurp_client.models.expired_inbox_dto import ExpiredInboxDto
+from mailslurp_client.models.expired_inbox_record_projection import ExpiredInboxRecordProjection
 from mailslurp_client.models.forward_email_options import ForwardEmailOptions
 from mailslurp_client.models.group_contacts_dto import GroupContactsDto
 from mailslurp_client.models.group_dto import GroupDto
 from mailslurp_client.models.group_projection import GroupProjection
 from mailslurp_client.models.html_validation_result import HTMLValidationResult
 from mailslurp_client.models.ip_address_result import IPAddressResult
 from mailslurp_client.models.inbox import Inbox
@@ -55,14 +58,15 @@
 from mailslurp_client.models.match_option import MatchOption
 from mailslurp_client.models.match_options import MatchOptions
 from mailslurp_client.models.name_server_record import NameServerRecord
 from mailslurp_client.models.page_alias import PageAlias
 from mailslurp_client.models.page_contact_projection import PageContactProjection
 from mailslurp_client.models.page_email_preview import PageEmailPreview
 from mailslurp_client.models.page_email_projection import PageEmailProjection
+from mailslurp_client.models.page_expired_inbox_record_projection import PageExpiredInboxRecordProjection
 from mailslurp_client.models.page_group_projection import PageGroupProjection
 from mailslurp_client.models.page_inbox_projection import PageInboxProjection
 from mailslurp_client.models.page_sent_email_projection import PageSentEmailProjection
 from mailslurp_client.models.page_template_projection import PageTemplateProjection
 from mailslurp_client.models.page_thread_projection import PageThreadProjection
 from mailslurp_client.models.page_webhook_projection import PageWebhookProjection
 from mailslurp_client.models.pageable import Pageable
```

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/alias.py` & `mailslurp-client-9.0.0/mailslurp_client/models/alias.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/alias_dto.py` & `mailslurp-client-9.0.0/mailslurp_client/models/alias_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/alias_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/alias_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/attachment_meta_data.py` & `mailslurp-client-9.0.0/mailslurp_client/models/attachment_meta_data.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/basic_auth_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/basic_auth_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/bulk_send_email_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/bulk_send_email_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/contact_dto.py` & `mailslurp-client-9.0.0/mailslurp_client/models/contact_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/contact_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/contact_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/content_match_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/content_match_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/create_alias_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/create_alias_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/create_contact_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/create_contact_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/create_domain_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/create_domain_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/create_group_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/create_group_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/create_inbox_dto.py` & `mailslurp-client-9.0.0/mailslurp_client/models/inbox.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,211 +14,295 @@
 import re  # noqa: F401
 
 import six
 
 from mailslurp_client.configuration import Configuration
 
 
-class CreateInboxDto(object):
+class Inbox(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
+        'created_at': 'datetime',
         'description': 'str',
         'email_address': 'str',
-        'expires_at': 'datetime',
+        'expires_at': 'str',
         'favourite': 'bool',
+        'id': 'str',
         'name': 'str',
-        'tags': 'list[str]'
+        'tags': 'list[str]',
+        'user_id': 'str'
     }
 
     attribute_map = {
+        'created_at': 'createdAt',
         'description': 'description',
         'email_address': 'emailAddress',
         'expires_at': 'expiresAt',
         'favourite': 'favourite',
+        'id': 'id',
         'name': 'name',
-        'tags': 'tags'
+        'tags': 'tags',
+        'user_id': 'userId'
     }
 
-    def __init__(self, description=None, email_address=None, expires_at=None, favourite=None, name=None, tags=None, local_vars_configuration=None):  # noqa: E501
-        """CreateInboxDto - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, created_at=None, description=None, email_address=None, expires_at=None, favourite=None, id=None, name=None, tags=None, user_id=None, local_vars_configuration=None):  # noqa: E501
+        """Inbox - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
+        self._created_at = None
         self._description = None
         self._email_address = None
         self._expires_at = None
         self._favourite = None
+        self._id = None
         self._name = None
         self._tags = None
+        self._user_id = None
         self.discriminator = None
 
+        if created_at is not None:
+            self.created_at = created_at
         if description is not None:
             self.description = description
         if email_address is not None:
             self.email_address = email_address
         if expires_at is not None:
             self.expires_at = expires_at
         if favourite is not None:
             self.favourite = favourite
+        if id is not None:
+            self.id = id
         if name is not None:
             self.name = name
         if tags is not None:
             self.tags = tags
+        if user_id is not None:
+            self.user_id = user_id
+
+    @property
+    def created_at(self):
+        """Gets the created_at of this Inbox.  # noqa: E501
+
+        When the inbox was created. Time stamps are in ISO DateTime Format `yyyy-MM-dd'T'HH:mm:ss.SSSXXX` e.g. `2000-10-31T01:30:00.000-05:00`.  # noqa: E501
+
+        :return: The created_at of this Inbox.  # noqa: E501
+        :rtype: datetime
+        """
+        return self._created_at
+
+    @created_at.setter
+    def created_at(self, created_at):
+        """Sets the created_at of this Inbox.
+
+        When the inbox was created. Time stamps are in ISO DateTime Format `yyyy-MM-dd'T'HH:mm:ss.SSSXXX` e.g. `2000-10-31T01:30:00.000-05:00`.  # noqa: E501
+
+        :param created_at: The created_at of this Inbox.  # noqa: E501
+        :type: datetime
+        """
+
+        self._created_at = created_at
 
     @property
     def description(self):
-        """Gets the description of this CreateInboxDto.  # noqa: E501
+        """Gets the description of this Inbox.  # noqa: E501
 
-        Optional description of an inbox for labelling purposes  # noqa: E501
+        Description of an inbox for labelling and searching purposes  # noqa: E501
 
-        :return: The description of this CreateInboxDto.  # noqa: E501
+        :return: The description of this Inbox.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this CreateInboxDto.
+        """Sets the description of this Inbox.
 
-        Optional description of an inbox for labelling purposes  # noqa: E501
+        Description of an inbox for labelling and searching purposes  # noqa: E501
 
-        :param description: The description of this CreateInboxDto.  # noqa: E501
+        :param description: The description of this Inbox.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
     def email_address(self):
-        """Gets the email_address of this CreateInboxDto.  # noqa: E501
+        """Gets the email_address of this Inbox.  # noqa: E501
 
-        Optionally specify an email address you want the inbox to have. When left blank an email address will be randomly assigned to the inbox usually ending in `@mailslurp.com`. Custom email addresses must include your own custom domain that you have configured in MailSlurp. So if your domain is `mysite.com` you can created any email address ending in `@mysite.com`. All email addresses are transformed to lowercase!  # noqa: E501
+        The inbox's email address. Send an email to this address and the inbox will receive and store it for you. Note the email address in MailSlurp match characters exactly and are case sensitive so `+123` additions are considered different addresses. To retrieve the email use the Inbox and Email Controller endpoints with the inbox ID.  # noqa: E501
 
-        :return: The email_address of this CreateInboxDto.  # noqa: E501
+        :return: The email_address of this Inbox.  # noqa: E501
         :rtype: str
         """
         return self._email_address
 
     @email_address.setter
     def email_address(self, email_address):
-        """Sets the email_address of this CreateInboxDto.
+        """Sets the email_address of this Inbox.
 
-        Optionally specify an email address you want the inbox to have. When left blank an email address will be randomly assigned to the inbox usually ending in `@mailslurp.com`. Custom email addresses must include your own custom domain that you have configured in MailSlurp. So if your domain is `mysite.com` you can created any email address ending in `@mysite.com`. All email addresses are transformed to lowercase!  # noqa: E501
+        The inbox's email address. Send an email to this address and the inbox will receive and store it for you. Note the email address in MailSlurp match characters exactly and are case sensitive so `+123` additions are considered different addresses. To retrieve the email use the Inbox and Email Controller endpoints with the inbox ID.  # noqa: E501
 
-        :param email_address: The email_address of this CreateInboxDto.  # noqa: E501
+        :param email_address: The email_address of this Inbox.  # noqa: E501
         :type: str
         """
 
         self._email_address = email_address
 
     @property
     def expires_at(self):
-        """Gets the expires_at of this CreateInboxDto.  # noqa: E501
+        """Gets the expires_at of this Inbox.  # noqa: E501
 
-        When, if ever, will the inbox expire and be deleted. If null then this inbox is permanent and the emails in it won't be deleted. Timestamp passed as string.  # noqa: E501
+        Inbox expiration time. When, if ever, the inbox should expire and be deleted. If null then this inbox is permanent and the emails in it won't be deleted. This is the default behavior unless expiration date is set. If an expiration date is set and the time is reached MailSlurp will expire the inbox and move it to an expired inbox entity. You can still access the emails belonging to it but it can no longer send or receive email.  # noqa: E501
 
-        :return: The expires_at of this CreateInboxDto.  # noqa: E501
-        :rtype: datetime
+        :return: The expires_at of this Inbox.  # noqa: E501
+        :rtype: str
         """
         return self._expires_at
 
     @expires_at.setter
     def expires_at(self, expires_at):
-        """Sets the expires_at of this CreateInboxDto.
+        """Sets the expires_at of this Inbox.
 
-        When, if ever, will the inbox expire and be deleted. If null then this inbox is permanent and the emails in it won't be deleted. Timestamp passed as string.  # noqa: E501
+        Inbox expiration time. When, if ever, the inbox should expire and be deleted. If null then this inbox is permanent and the emails in it won't be deleted. This is the default behavior unless expiration date is set. If an expiration date is set and the time is reached MailSlurp will expire the inbox and move it to an expired inbox entity. You can still access the emails belonging to it but it can no longer send or receive email.  # noqa: E501
 
-        :param expires_at: The expires_at of this CreateInboxDto.  # noqa: E501
-        :type: datetime
+        :param expires_at: The expires_at of this Inbox.  # noqa: E501
+        :type: str
         """
 
         self._expires_at = expires_at
 
     @property
     def favourite(self):
-        """Gets the favourite of this CreateInboxDto.  # noqa: E501
+        """Gets the favourite of this Inbox.  # noqa: E501
 
-        Is the inbox favorited. Favouriting inboxes is typically done in the dashboard for quick access  # noqa: E501
+        Is the inbox favorited. Favouriting inboxes is typically done in the dashboard for quick access or filtering  # noqa: E501
 
-        :return: The favourite of this CreateInboxDto.  # noqa: E501
+        :return: The favourite of this Inbox.  # noqa: E501
         :rtype: bool
         """
         return self._favourite
 
     @favourite.setter
     def favourite(self, favourite):
-        """Sets the favourite of this CreateInboxDto.
+        """Sets the favourite of this Inbox.
 
-        Is the inbox favorited. Favouriting inboxes is typically done in the dashboard for quick access  # noqa: E501
+        Is the inbox favorited. Favouriting inboxes is typically done in the dashboard for quick access or filtering  # noqa: E501
 
-        :param favourite: The favourite of this CreateInboxDto.  # noqa: E501
+        :param favourite: The favourite of this Inbox.  # noqa: E501
         :type: bool
         """
 
         self._favourite = favourite
 
     @property
+    def id(self):
+        """Gets the id of this Inbox.  # noqa: E501
+
+        ID of the inbox. The ID is a UUID-V4 format string. Use the inboxId for calls to Inbox and Email Controller endpoints. See the emailAddress property for the email address or the inbox. To get emails in an inbox use the WaitFor and Inbox Controller methods `waitForLatestEmail` and `getEmails` methods respectively. Inboxes can be used with aliases to forward emails automatically.  # noqa: E501
+
+        :return: The id of this Inbox.  # noqa: E501
+        :rtype: str
+        """
+        return self._id
+
+    @id.setter
+    def id(self, id):
+        """Sets the id of this Inbox.
+
+        ID of the inbox. The ID is a UUID-V4 format string. Use the inboxId for calls to Inbox and Email Controller endpoints. See the emailAddress property for the email address or the inbox. To get emails in an inbox use the WaitFor and Inbox Controller methods `waitForLatestEmail` and `getEmails` methods respectively. Inboxes can be used with aliases to forward emails automatically.  # noqa: E501
+
+        :param id: The id of this Inbox.  # noqa: E501
+        :type: str
+        """
+
+        self._id = id
+
+    @property
     def name(self):
-        """Gets the name of this CreateInboxDto.  # noqa: E501
+        """Gets the name of this Inbox.  # noqa: E501
 
-        Optional name of the inbox. Displayed in the dashboard for easier search  # noqa: E501
+        Name of the inbox. Displayed in the dashboard for easier search  # noqa: E501
 
-        :return: The name of this CreateInboxDto.  # noqa: E501
+        :return: The name of this Inbox.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this CreateInboxDto.
+        """Sets the name of this Inbox.
 
-        Optional name of the inbox. Displayed in the dashboard for easier search  # noqa: E501
+        Name of the inbox. Displayed in the dashboard for easier search  # noqa: E501
 
-        :param name: The name of this CreateInboxDto.  # noqa: E501
+        :param name: The name of this Inbox.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
     def tags(self):
-        """Gets the tags of this CreateInboxDto.  # noqa: E501
+        """Gets the tags of this Inbox.  # noqa: E501
 
         Tags that inbox has been tagged with. Tags can be added to inboxes to group different inboxes within an account. You can also search for inboxes by tag in the dashboard UI.  # noqa: E501
 
-        :return: The tags of this CreateInboxDto.  # noqa: E501
+        :return: The tags of this Inbox.  # noqa: E501
         :rtype: list[str]
         """
         return self._tags
 
     @tags.setter
     def tags(self, tags):
-        """Sets the tags of this CreateInboxDto.
+        """Sets the tags of this Inbox.
 
         Tags that inbox has been tagged with. Tags can be added to inboxes to group different inboxes within an account. You can also search for inboxes by tag in the dashboard UI.  # noqa: E501
 
-        :param tags: The tags of this CreateInboxDto.  # noqa: E501
+        :param tags: The tags of this Inbox.  # noqa: E501
         :type: list[str]
         """
 
         self._tags = tags
 
+    @property
+    def user_id(self):
+        """Gets the user_id of this Inbox.  # noqa: E501
+
+        ID of user that inbox belongs to  # noqa: E501
+
+        :return: The user_id of this Inbox.  # noqa: E501
+        :rtype: str
+        """
+        return self._user_id
+
+    @user_id.setter
+    def user_id(self, user_id):
+        """Sets the user_id of this Inbox.
+
+        ID of user that inbox belongs to  # noqa: E501
+
+        :param user_id: The user_id of this Inbox.  # noqa: E501
+        :type: str
+        """
+
+        self._user_id = user_id
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -245,18 +329,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreateInboxDto):
+        if not isinstance(other, Inbox):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, CreateInboxDto):
+        if not isinstance(other, Inbox):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/create_template_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/create_template_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/create_webhook_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/create_webhook_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/describe_domain_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/describe_domain_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/describe_mail_server_domain_result.py` & `mailslurp-client-9.0.0/mailslurp_client/models/describe_mail_server_domain_result.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/dns_lookup_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/dns_lookup_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/dns_lookup_result.py` & `mailslurp-client-9.0.0/mailslurp_client/models/dns_lookup_result.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/dns_lookup_results.py` & `mailslurp-client-9.0.0/mailslurp_client/models/dns_lookup_results.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/domain_dto.py` & `mailslurp-client-9.0.0/mailslurp_client/models/domain_dto.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,53 +32,58 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'created_at': 'datetime',
         'dkim_tokens': 'list[str]',
         'domain': 'str',
+        'domain_name_records': 'list[DomainNameRecord]',
         'id': 'str',
         'is_verified': 'bool',
         'updated_at': 'datetime',
         'user_id': 'str',
         'verification_token': 'str'
     }
 
     attribute_map = {
         'created_at': 'createdAt',
         'dkim_tokens': 'dkimTokens',
         'domain': 'domain',
+        'domain_name_records': 'domainNameRecords',
         'id': 'id',
         'is_verified': 'isVerified',
         'updated_at': 'updatedAt',
         'user_id': 'userId',
         'verification_token': 'verificationToken'
     }
 
-    def __init__(self, created_at=None, dkim_tokens=None, domain=None, id=None, is_verified=None, updated_at=None, user_id=None, verification_token=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, created_at=None, dkim_tokens=None, domain=None, domain_name_records=None, id=None, is_verified=None, updated_at=None, user_id=None, verification_token=None, local_vars_configuration=None):  # noqa: E501
         """DomainDto - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._created_at = None
         self._dkim_tokens = None
         self._domain = None
+        self._domain_name_records = None
         self._id = None
         self._is_verified = None
         self._updated_at = None
         self._user_id = None
         self._verification_token = None
         self.discriminator = None
 
         self.created_at = created_at
         if dkim_tokens is not None:
             self.dkim_tokens = dkim_tokens
         if domain is not None:
             self.domain = domain
+        if domain_name_records is not None:
+            self.domain_name_records = domain_name_records
         self.id = id
         if is_verified is not None:
             self.is_verified = is_verified
         self.updated_at = updated_at
         self.user_id = user_id
         if verification_token is not None:
             self.verification_token = verification_token
@@ -106,26 +111,26 @@
 
         self._created_at = created_at
 
     @property
     def dkim_tokens(self):
         """Gets the dkim_tokens of this DomainDto.  # noqa: E501
 
-        DNS records for DKIM approval  # noqa: E501
+        Unique token DKIM tokens  # noqa: E501
 
         :return: The dkim_tokens of this DomainDto.  # noqa: E501
         :rtype: list[str]
         """
         return self._dkim_tokens
 
     @dkim_tokens.setter
     def dkim_tokens(self, dkim_tokens):
         """Sets the dkim_tokens of this DomainDto.
 
-        DNS records for DKIM approval  # noqa: E501
+        Unique token DKIM tokens  # noqa: E501
 
         :param dkim_tokens: The dkim_tokens of this DomainDto.  # noqa: E501
         :type: list[str]
         """
 
         self._dkim_tokens = dkim_tokens
 
@@ -149,14 +154,37 @@
         :param domain: The domain of this DomainDto.  # noqa: E501
         :type: str
         """
 
         self._domain = domain
 
     @property
+    def domain_name_records(self):
+        """Gets the domain_name_records of this DomainDto.  # noqa: E501
+
+        List of DNS domain name records (C, MX, TXT) etc that you must add to the DNS server associated with your domain provider.  # noqa: E501
+
+        :return: The domain_name_records of this DomainDto.  # noqa: E501
+        :rtype: list[DomainNameRecord]
+        """
+        return self._domain_name_records
+
+    @domain_name_records.setter
+    def domain_name_records(self, domain_name_records):
+        """Sets the domain_name_records of this DomainDto.
+
+        List of DNS domain name records (C, MX, TXT) etc that you must add to the DNS server associated with your domain provider.  # noqa: E501
+
+        :param domain_name_records: The domain_name_records of this DomainDto.  # noqa: E501
+        :type: list[DomainNameRecord]
+        """
+
+        self._domain_name_records = domain_name_records
+
+    @property
     def id(self):
         """Gets the id of this DomainDto.  # noqa: E501
 
 
         :return: The id of this DomainDto.  # noqa: E501
         :rtype: str
         """
@@ -244,26 +272,26 @@
 
         self._user_id = user_id
 
     @property
     def verification_token(self):
         """Gets the verification_token of this DomainDto.  # noqa: E501
 
-        A TXT record that you must place in the DNS settings of the domain to complete domain verification  # noqa: E501
+        Verification tokens  # noqa: E501
 
         :return: The verification_token of this DomainDto.  # noqa: E501
         :rtype: str
         """
         return self._verification_token
 
     @verification_token.setter
     def verification_token(self, verification_token):
         """Sets the verification_token of this DomainDto.
 
-        A TXT record that you must place in the DNS settings of the domain to complete domain verification  # noqa: E501
+        Verification tokens  # noqa: E501
 
         :param verification_token: The verification_token of this DomainDto.  # noqa: E501
         :type: str
         """
 
         self._verification_token = verification_token
```

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/domain_preview.py` & `mailslurp-client-9.0.0/mailslurp_client/models/domain_preview.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/download_attachment_dto.py` & `mailslurp-client-9.0.0/mailslurp_client/models/download_attachment_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/email.py` & `mailslurp-client-9.0.0/mailslurp_client/models/email.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/email_analysis.py` & `mailslurp-client-9.0.0/mailslurp_client/models/email_analysis.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/email_content_match_result.py` & `mailslurp-client-9.0.0/mailslurp_client/models/email_content_match_result.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/email_preview.py` & `mailslurp-client-9.0.0/mailslurp_client/models/email_preview.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/email_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/email_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/email_verification_result.py` & `mailslurp-client-9.0.0/mailslurp_client/models/email_verification_result.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/forward_email_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/forward_email_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/group_contacts_dto.py` & `mailslurp-client-9.0.0/mailslurp_client/models/group_contacts_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/group_dto.py` & `mailslurp-client-9.0.0/mailslurp_client/models/group_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/group_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/group_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/html_validation_result.py` & `mailslurp-client-9.0.0/mailslurp_client/models/html_validation_result.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/inbox.py` & `mailslurp-client-9.0.0/mailslurp_client/models/sent_email_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,290 +14,441 @@
 import re  # noqa: F401
 
 import six
 
 from mailslurp_client.configuration import Configuration
 
 
-class Inbox(object):
+class SentEmailDto(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'created_at': 'datetime',
-        'description': 'str',
-        'email_address': 'str',
-        'expires_at': 'str',
-        'favourite': 'bool',
+        'attachments': 'list[str]',
+        'bcc': 'list[str]',
+        'body': 'str',
+        'body_md5_hash': 'str',
+        'cc': 'list[str]',
+        'charset': 'str',
+        '_from': 'str',
         'id': 'str',
-        'name': 'str',
-        'tags': 'list[str]',
+        'inbox_id': 'str',
+        'is_html': 'bool',
+        'reply_to': 'str',
+        'sent_at': 'datetime',
+        'subject': 'str',
+        'to': 'list[str]',
         'user_id': 'str'
     }
 
     attribute_map = {
-        'created_at': 'createdAt',
-        'description': 'description',
-        'email_address': 'emailAddress',
-        'expires_at': 'expiresAt',
-        'favourite': 'favourite',
+        'attachments': 'attachments',
+        'bcc': 'bcc',
+        'body': 'body',
+        'body_md5_hash': 'bodyMD5Hash',
+        'cc': 'cc',
+        'charset': 'charset',
+        '_from': 'from',
         'id': 'id',
-        'name': 'name',
-        'tags': 'tags',
+        'inbox_id': 'inboxId',
+        'is_html': 'isHTML',
+        'reply_to': 'replyTo',
+        'sent_at': 'sentAt',
+        'subject': 'subject',
+        'to': 'to',
         'user_id': 'userId'
     }
 
-    def __init__(self, created_at=None, description=None, email_address=None, expires_at=None, favourite=None, id=None, name=None, tags=None, user_id=None, local_vars_configuration=None):  # noqa: E501
-        """Inbox - a model defined in OpenAPI"""  # noqa: E501
+    def __init__(self, attachments=None, bcc=None, body=None, body_md5_hash=None, cc=None, charset=None, _from=None, id=None, inbox_id=None, is_html=None, reply_to=None, sent_at=None, subject=None, to=None, user_id=None, local_vars_configuration=None):  # noqa: E501
+        """SentEmailDto - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._created_at = None
-        self._description = None
-        self._email_address = None
-        self._expires_at = None
-        self._favourite = None
+        self._attachments = None
+        self._bcc = None
+        self._body = None
+        self._body_md5_hash = None
+        self._cc = None
+        self._charset = None
+        self.__from = None
         self._id = None
-        self._name = None
-        self._tags = None
+        self._inbox_id = None
+        self._is_html = None
+        self._reply_to = None
+        self._sent_at = None
+        self._subject = None
+        self._to = None
         self._user_id = None
         self.discriminator = None
 
-        if created_at is not None:
-            self.created_at = created_at
-        if description is not None:
-            self.description = description
-        if email_address is not None:
-            self.email_address = email_address
-        if expires_at is not None:
-            self.expires_at = expires_at
-        if favourite is not None:
-            self.favourite = favourite
+        if attachments is not None:
+            self.attachments = attachments
+        if bcc is not None:
+            self.bcc = bcc
+        if body is not None:
+            self.body = body
+        if body_md5_hash is not None:
+            self.body_md5_hash = body_md5_hash
+        if cc is not None:
+            self.cc = cc
+        if charset is not None:
+            self.charset = charset
+        if _from is not None:
+            self._from = _from
         if id is not None:
             self.id = id
-        if name is not None:
-            self.name = name
-        if tags is not None:
-            self.tags = tags
+        if inbox_id is not None:
+            self.inbox_id = inbox_id
+        if is_html is not None:
+            self.is_html = is_html
+        if reply_to is not None:
+            self.reply_to = reply_to
+        self.sent_at = sent_at
+        if subject is not None:
+            self.subject = subject
+        if to is not None:
+            self.to = to
         if user_id is not None:
             self.user_id = user_id
 
     @property
-    def created_at(self):
-        """Gets the created_at of this Inbox.  # noqa: E501
+    def attachments(self):
+        """Gets the attachments of this SentEmailDto.  # noqa: E501
 
-        When was the inbox created. Time stamps are in ISO DateTime Format `yyyy-MM-dd'T'HH:mm:ss.SSSXXX` e.g. `2000-10-31T01:30:00.000-05:00`.  # noqa: E501
+        Array of IDs of attachments that were sent with this email  # noqa: E501
 
-        :return: The created_at of this Inbox.  # noqa: E501
-        :rtype: datetime
+        :return: The attachments of this SentEmailDto.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._created_at
+        return self._attachments
 
-    @created_at.setter
-    def created_at(self, created_at):
-        """Sets the created_at of this Inbox.
+    @attachments.setter
+    def attachments(self, attachments):
+        """Sets the attachments of this SentEmailDto.
 
-        When was the inbox created. Time stamps are in ISO DateTime Format `yyyy-MM-dd'T'HH:mm:ss.SSSXXX` e.g. `2000-10-31T01:30:00.000-05:00`.  # noqa: E501
+        Array of IDs of attachments that were sent with this email  # noqa: E501
 
-        :param created_at: The created_at of this Inbox.  # noqa: E501
-        :type: datetime
+        :param attachments: The attachments of this SentEmailDto.  # noqa: E501
+        :type: list[str]
+        """
+
+        self._attachments = attachments
+
+    @property
+    def bcc(self):
+        """Gets the bcc of this SentEmailDto.  # noqa: E501
+
+
+        :return: The bcc of this SentEmailDto.  # noqa: E501
+        :rtype: list[str]
+        """
+        return self._bcc
+
+    @bcc.setter
+    def bcc(self, bcc):
+        """Sets the bcc of this SentEmailDto.
+
+
+        :param bcc: The bcc of this SentEmailDto.  # noqa: E501
+        :type: list[str]
         """
 
-        self._created_at = created_at
+        self._bcc = bcc
 
     @property
-    def description(self):
-        """Gets the description of this Inbox.  # noqa: E501
+    def body(self):
+        """Gets the body of this SentEmailDto.  # noqa: E501
 
-        Optional description of an inbox for labelling purposes  # noqa: E501
 
-        :return: The description of this Inbox.  # noqa: E501
+        :return: The body of this SentEmailDto.  # noqa: E501
         :rtype: str
         """
-        return self._description
+        return self._body
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this Inbox.
+    @body.setter
+    def body(self, body):
+        """Sets the body of this SentEmailDto.
 
-        Optional description of an inbox for labelling purposes  # noqa: E501
 
-        :param description: The description of this Inbox.  # noqa: E501
+        :param body: The body of this SentEmailDto.  # noqa: E501
         :type: str
         """
 
-        self._description = description
+        self._body = body
 
     @property
-    def email_address(self):
-        """Gets the email_address of this Inbox.  # noqa: E501
+    def body_md5_hash(self):
+        """Gets the body_md5_hash of this SentEmailDto.  # noqa: E501
 
-        The inbox's email address. Send an email to this address and the inbox will receive and store it for you. To retrieve the email use the Inbox and Email Controller endpoints with the inbox ID.  # noqa: E501
+        MD5 Hash  # noqa: E501
 
-        :return: The email_address of this Inbox.  # noqa: E501
+        :return: The body_md5_hash of this SentEmailDto.  # noqa: E501
         :rtype: str
         """
-        return self._email_address
+        return self._body_md5_hash
 
-    @email_address.setter
-    def email_address(self, email_address):
-        """Sets the email_address of this Inbox.
+    @body_md5_hash.setter
+    def body_md5_hash(self, body_md5_hash):
+        """Sets the body_md5_hash of this SentEmailDto.
 
-        The inbox's email address. Send an email to this address and the inbox will receive and store it for you. To retrieve the email use the Inbox and Email Controller endpoints with the inbox ID.  # noqa: E501
+        MD5 Hash  # noqa: E501
 
-        :param email_address: The email_address of this Inbox.  # noqa: E501
+        :param body_md5_hash: The body_md5_hash of this SentEmailDto.  # noqa: E501
         :type: str
         """
 
-        self._email_address = email_address
+        self._body_md5_hash = body_md5_hash
+
+    @property
+    def cc(self):
+        """Gets the cc of this SentEmailDto.  # noqa: E501
+
+
+        :return: The cc of this SentEmailDto.  # noqa: E501
+        :rtype: list[str]
+        """
+        return self._cc
+
+    @cc.setter
+    def cc(self, cc):
+        """Sets the cc of this SentEmailDto.
+
+
+        :param cc: The cc of this SentEmailDto.  # noqa: E501
+        :type: list[str]
+        """
+
+        self._cc = cc
 
     @property
-    def expires_at(self):
-        """Gets the expires_at of this Inbox.  # noqa: E501
+    def charset(self):
+        """Gets the charset of this SentEmailDto.  # noqa: E501
 
-        When, if ever, will the inbox expire and be deleted. If null then this inbox is permanent and the emails in it won't be deleted. Timestamp passed as string.  # noqa: E501
 
-        :return: The expires_at of this Inbox.  # noqa: E501
+        :return: The charset of this SentEmailDto.  # noqa: E501
         :rtype: str
         """
-        return self._expires_at
+        return self._charset
 
-    @expires_at.setter
-    def expires_at(self, expires_at):
-        """Sets the expires_at of this Inbox.
+    @charset.setter
+    def charset(self, charset):
+        """Sets the charset of this SentEmailDto.
 
-        When, if ever, will the inbox expire and be deleted. If null then this inbox is permanent and the emails in it won't be deleted. Timestamp passed as string.  # noqa: E501
 
-        :param expires_at: The expires_at of this Inbox.  # noqa: E501
+        :param charset: The charset of this SentEmailDto.  # noqa: E501
         :type: str
         """
 
-        self._expires_at = expires_at
+        self._charset = charset
 
     @property
-    def favourite(self):
-        """Gets the favourite of this Inbox.  # noqa: E501
+    def _from(self):
+        """Gets the _from of this SentEmailDto.  # noqa: E501
 
-        Is the inbox favorited. Favouriting inboxes is typically done in the dashboard for quick access  # noqa: E501
 
-        :return: The favourite of this Inbox.  # noqa: E501
-        :rtype: bool
+        :return: The _from of this SentEmailDto.  # noqa: E501
+        :rtype: str
         """
-        return self._favourite
+        return self.__from
 
-    @favourite.setter
-    def favourite(self, favourite):
-        """Sets the favourite of this Inbox.
+    @_from.setter
+    def _from(self, _from):
+        """Sets the _from of this SentEmailDto.
 
-        Is the inbox favorited. Favouriting inboxes is typically done in the dashboard for quick access  # noqa: E501
 
-        :param favourite: The favourite of this Inbox.  # noqa: E501
-        :type: bool
+        :param _from: The _from of this SentEmailDto.  # noqa: E501
+        :type: str
         """
 
-        self._favourite = favourite
+        self.__from = _from
 
     @property
     def id(self):
-        """Gets the id of this Inbox.  # noqa: E501
+        """Gets the id of this SentEmailDto.  # noqa: E501
 
-        ID of the inbox. The ID is a UUID-V4 string. See the emailAddress property for the email address.  # noqa: E501
+        ID of sent email  # noqa: E501
 
-        :return: The id of this Inbox.  # noqa: E501
+        :return: The id of this SentEmailDto.  # noqa: E501
         :rtype: str
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this Inbox.
+        """Sets the id of this SentEmailDto.
 
-        ID of the inbox. The ID is a UUID-V4 string. See the emailAddress property for the email address.  # noqa: E501
+        ID of sent email  # noqa: E501
 
-        :param id: The id of this Inbox.  # noqa: E501
+        :param id: The id of this SentEmailDto.  # noqa: E501
         :type: str
         """
 
         self._id = id
 
     @property
-    def name(self):
-        """Gets the name of this Inbox.  # noqa: E501
+    def inbox_id(self):
+        """Gets the inbox_id of this SentEmailDto.  # noqa: E501
+
+        Inbox ID email was sent from  # noqa: E501
+
+        :return: The inbox_id of this SentEmailDto.  # noqa: E501
+        :rtype: str
+        """
+        return self._inbox_id
+
+    @inbox_id.setter
+    def inbox_id(self, inbox_id):
+        """Sets the inbox_id of this SentEmailDto.
+
+        Inbox ID email was sent from  # noqa: E501
+
+        :param inbox_id: The inbox_id of this SentEmailDto.  # noqa: E501
+        :type: str
+        """
+
+        self._inbox_id = inbox_id
+
+    @property
+    def is_html(self):
+        """Gets the is_html of this SentEmailDto.  # noqa: E501
+
+
+        :return: The is_html of this SentEmailDto.  # noqa: E501
+        :rtype: bool
+        """
+        return self._is_html
+
+    @is_html.setter
+    def is_html(self, is_html):
+        """Sets the is_html of this SentEmailDto.
+
+
+        :param is_html: The is_html of this SentEmailDto.  # noqa: E501
+        :type: bool
+        """
+
+        self._is_html = is_html
+
+    @property
+    def reply_to(self):
+        """Gets the reply_to of this SentEmailDto.  # noqa: E501
+
+
+        :return: The reply_to of this SentEmailDto.  # noqa: E501
+        :rtype: str
+        """
+        return self._reply_to
+
+    @reply_to.setter
+    def reply_to(self, reply_to):
+        """Sets the reply_to of this SentEmailDto.
+
+
+        :param reply_to: The reply_to of this SentEmailDto.  # noqa: E501
+        :type: str
+        """
+
+        self._reply_to = reply_to
+
+    @property
+    def sent_at(self):
+        """Gets the sent_at of this SentEmailDto.  # noqa: E501
+
+
+        :return: The sent_at of this SentEmailDto.  # noqa: E501
+        :rtype: datetime
+        """
+        return self._sent_at
+
+    @sent_at.setter
+    def sent_at(self, sent_at):
+        """Sets the sent_at of this SentEmailDto.
+
+
+        :param sent_at: The sent_at of this SentEmailDto.  # noqa: E501
+        :type: datetime
+        """
+        if self.local_vars_configuration.client_side_validation and sent_at is None:  # noqa: E501
+            raise ValueError("Invalid value for `sent_at`, must not be `None`")  # noqa: E501
+
+        self._sent_at = sent_at
+
+    @property
+    def subject(self):
+        """Gets the subject of this SentEmailDto.  # noqa: E501
 
-        Optional name of the inbox. Displayed in the dashboard for easier search  # noqa: E501
 
-        :return: The name of this Inbox.  # noqa: E501
+        :return: The subject of this SentEmailDto.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._subject
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this Inbox.
+    @subject.setter
+    def subject(self, subject):
+        """Sets the subject of this SentEmailDto.
 
-        Optional name of the inbox. Displayed in the dashboard for easier search  # noqa: E501
 
-        :param name: The name of this Inbox.  # noqa: E501
+        :param subject: The subject of this SentEmailDto.  # noqa: E501
         :type: str
         """
 
-        self._name = name
+        self._subject = subject
 
     @property
-    def tags(self):
-        """Gets the tags of this Inbox.  # noqa: E501
+    def to(self):
+        """Gets the to of this SentEmailDto.  # noqa: E501
 
-        Tags that inbox has been tagged with. Tags can be added to inboxes to group different inboxes within an account. You can also search for inboxes by tag in the dashboard UI.  # noqa: E501
+        Recipients email was sent to  # noqa: E501
 
-        :return: The tags of this Inbox.  # noqa: E501
+        :return: The to of this SentEmailDto.  # noqa: E501
         :rtype: list[str]
         """
-        return self._tags
+        return self._to
 
-    @tags.setter
-    def tags(self, tags):
-        """Sets the tags of this Inbox.
+    @to.setter
+    def to(self, to):
+        """Sets the to of this SentEmailDto.
 
-        Tags that inbox has been tagged with. Tags can be added to inboxes to group different inboxes within an account. You can also search for inboxes by tag in the dashboard UI.  # noqa: E501
+        Recipients email was sent to  # noqa: E501
 
-        :param tags: The tags of this Inbox.  # noqa: E501
+        :param to: The to of this SentEmailDto.  # noqa: E501
         :type: list[str]
         """
 
-        self._tags = tags
+        self._to = to
 
     @property
     def user_id(self):
-        """Gets the user_id of this Inbox.  # noqa: E501
+        """Gets the user_id of this SentEmailDto.  # noqa: E501
 
-        ID of user that inbox belongs to  # noqa: E501
+        User ID  # noqa: E501
 
-        :return: The user_id of this Inbox.  # noqa: E501
+        :return: The user_id of this SentEmailDto.  # noqa: E501
         :rtype: str
         """
         return self._user_id
 
     @user_id.setter
     def user_id(self, user_id):
-        """Sets the user_id of this Inbox.
+        """Sets the user_id of this SentEmailDto.
 
-        ID of user that inbox belongs to  # noqa: E501
+        User ID  # noqa: E501
 
-        :param user_id: The user_id of this Inbox.  # noqa: E501
+        :param user_id: The user_id of this SentEmailDto.  # noqa: E501
         :type: str
         """
 
         self._user_id = user_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -329,18 +480,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Inbox):
+        if not isinstance(other, SentEmailDto):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Inbox):
+        if not isinstance(other, SentEmailDto):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/inbox_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/inbox_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/ip_address_result.py` & `mailslurp-client-9.0.0/mailslurp_client/models/ip_address_result.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/match_option.py` & `mailslurp-client-9.0.0/mailslurp_client/models/match_option.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/match_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/match_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/name_server_record.py` & `mailslurp-client-9.0.0/mailslurp_client/models/name_server_record.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/page_alias.py` & `mailslurp-client-9.0.0/mailslurp_client/models/page_alias.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/page_contact_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/page_contact_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/page_email_preview.py` & `mailslurp-client-9.0.0/mailslurp_client/models/page_email_preview.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/page_email_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/page_email_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/page_group_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/page_group_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/page_inbox_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/page_inbox_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/page_sent_email_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/page_sent_email_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/page_template_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/page_template_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/page_thread_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/page_thread_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/page_webhook_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/page_webhook_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/pageable.py` & `mailslurp-client-9.0.0/mailslurp_client/models/pageable.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/raw_email_json.py` & `mailslurp-client-9.0.0/mailslurp_client/models/raw_email_json.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/reply_to_alias_email_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/reply_to_alias_email_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/reply_to_email_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/reply_to_email_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/send_email_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/send_email_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/sent_email_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/sent_email_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/set_inbox_favourited_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/set_inbox_favourited_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,26 +52,26 @@
         if state is not None:
             self.state = state
 
     @property
     def state(self):
         """Gets the state of this SetInboxFavouritedOptions.  # noqa: E501
 
-        Should the inbox be favourited?  # noqa: E501
+        Is the inbox favorited. Favouriting inboxes is typically done in the dashboard for quick access or filtering  # noqa: E501
 
         :return: The state of this SetInboxFavouritedOptions.  # noqa: E501
         :rtype: bool
         """
         return self._state
 
     @state.setter
     def state(self, state):
         """Sets the state of this SetInboxFavouritedOptions.
 
-        Should the inbox be favourited?  # noqa: E501
+        Is the inbox favorited. Favouriting inboxes is typically done in the dashboard for quick access or filtering  # noqa: E501
 
         :param state: The state of this SetInboxFavouritedOptions.  # noqa: E501
         :type: bool
         """
 
         self._state = state
```

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/simple_send_email_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/simple_send_email_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,26 +90,26 @@
 
         self._body = body
 
     @property
     def sender_id(self):
         """Gets the sender_id of this SimpleSendEmailOptions.  # noqa: E501
 
-        ID of inbox to send from  # noqa: E501
+        ID of inbox to send from. If null an inbox will be created for sending  # noqa: E501
 
         :return: The sender_id of this SimpleSendEmailOptions.  # noqa: E501
         :rtype: str
         """
         return self._sender_id
 
     @sender_id.setter
     def sender_id(self, sender_id):
         """Sets the sender_id of this SimpleSendEmailOptions.
 
-        ID of inbox to send from  # noqa: E501
+        ID of inbox to send from. If null an inbox will be created for sending  # noqa: E501
 
         :param sender_id: The sender_id of this SimpleSendEmailOptions.  # noqa: E501
         :type: str
         """
 
         self._sender_id = sender_id
```

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/sort.py` & `mailslurp-client-9.0.0/mailslurp_client/models/sort.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/template_dto.py` & `mailslurp-client-9.0.0/mailslurp_client/models/template_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/template_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/template_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/template_variable.py` & `mailslurp-client-9.0.0/mailslurp_client/models/template_variable.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/thread_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/thread_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/unread_count.py` & `mailslurp-client-9.0.0/mailslurp_client/models/unread_count.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/update_alias_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/update_alias_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/update_group_contacts.py` & `mailslurp-client-9.0.0/mailslurp_client/models/update_group_contacts.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/update_inbox_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/update_inbox_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,95 +72,95 @@
         if tags is not None:
             self.tags = tags
 
     @property
     def description(self):
         """Gets the description of this UpdateInboxOptions.  # noqa: E501
 
-        Optional description of an inbox for labelling purposes  # noqa: E501
+        Description of an inbox for labelling and searching purposes  # noqa: E501
 
         :return: The description of this UpdateInboxOptions.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
         """Sets the description of this UpdateInboxOptions.
 
-        Optional description of an inbox for labelling purposes  # noqa: E501
+        Description of an inbox for labelling and searching purposes  # noqa: E501
 
         :param description: The description of this UpdateInboxOptions.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
     def expires_at(self):
         """Gets the expires_at of this UpdateInboxOptions.  # noqa: E501
 
-        When, if ever, will the inbox expire and be deleted. If null then this inbox is permanent and the emails in it won't be deleted. Timestamp passed as string.  # noqa: E501
+        Inbox expiration time. When, if ever, the inbox should expire and be deleted. If null then this inbox is permanent and the emails in it won't be deleted. This is the default behavior unless expiration date is set. If an expiration date is set and the time is reached MailSlurp will expire the inbox and move it to an expired inbox entity. You can still access the emails belonging to it but it can no longer send or receive email.  # noqa: E501
 
         :return: The expires_at of this UpdateInboxOptions.  # noqa: E501
         :rtype: datetime
         """
         return self._expires_at
 
     @expires_at.setter
     def expires_at(self, expires_at):
         """Sets the expires_at of this UpdateInboxOptions.
 
-        When, if ever, will the inbox expire and be deleted. If null then this inbox is permanent and the emails in it won't be deleted. Timestamp passed as string.  # noqa: E501
+        Inbox expiration time. When, if ever, the inbox should expire and be deleted. If null then this inbox is permanent and the emails in it won't be deleted. This is the default behavior unless expiration date is set. If an expiration date is set and the time is reached MailSlurp will expire the inbox and move it to an expired inbox entity. You can still access the emails belonging to it but it can no longer send or receive email.  # noqa: E501
 
         :param expires_at: The expires_at of this UpdateInboxOptions.  # noqa: E501
         :type: datetime
         """
 
         self._expires_at = expires_at
 
     @property
     def favourite(self):
         """Gets the favourite of this UpdateInboxOptions.  # noqa: E501
 
-        Is the inbox favorited. Favouriting inboxes is typically done in the dashboard for quick access  # noqa: E501
+        Is the inbox favorited. Favouriting inboxes is typically done in the dashboard for quick access or filtering  # noqa: E501
 
         :return: The favourite of this UpdateInboxOptions.  # noqa: E501
         :rtype: bool
         """
         return self._favourite
 
     @favourite.setter
     def favourite(self, favourite):
         """Sets the favourite of this UpdateInboxOptions.
 
-        Is the inbox favorited. Favouriting inboxes is typically done in the dashboard for quick access  # noqa: E501
+        Is the inbox favorited. Favouriting inboxes is typically done in the dashboard for quick access or filtering  # noqa: E501
 
         :param favourite: The favourite of this UpdateInboxOptions.  # noqa: E501
         :type: bool
         """
 
         self._favourite = favourite
 
     @property
     def name(self):
         """Gets the name of this UpdateInboxOptions.  # noqa: E501
 
-        Optional name of the inbox. Displayed in the dashboard for easier search  # noqa: E501
+        Name of the inbox. Displayed in the dashboard for easier search  # noqa: E501
 
         :return: The name of this UpdateInboxOptions.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
         """Sets the name of this UpdateInboxOptions.
 
-        Optional name of the inbox. Displayed in the dashboard for easier search  # noqa: E501
+        Name of the inbox. Displayed in the dashboard for easier search  # noqa: E501
 
         :param name: The name of this UpdateInboxOptions.  # noqa: E501
         :type: str
         """
 
         self._name = name
```

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/upload_attachment_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/upload_attachment_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/validation_dto.py` & `mailslurp-client-9.0.0/mailslurp_client/models/validation_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/validation_message.py` & `mailslurp-client-9.0.0/mailslurp_client/models/validation_message.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/verify_email_address_options.py` & `mailslurp-client-9.0.0/mailslurp_client/models/verify_email_address_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/wait_for_conditions.py` & `mailslurp-client-9.0.0/mailslurp_client/models/wait_for_conditions.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/webhook_dto.py` & `mailslurp-client-9.0.0/mailslurp_client/models/webhook_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/webhook_projection.py` & `mailslurp-client-9.0.0/mailslurp_client/models/webhook_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/webhook_test_request.py` & `mailslurp-client-9.0.0/mailslurp_client/models/webhook_test_request.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/webhook_test_response.py` & `mailslurp-client-9.0.0/mailslurp_client/models/webhook_test_response.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/models/webhook_test_result.py` & `mailslurp-client-9.0.0/mailslurp_client/models/webhook_test_result.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client/rest.py` & `mailslurp-client-9.0.0/mailslurp_client/rest.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/mailslurp_client.egg-info/PKG-INFO` & `mailslurp-client-9.0.0/mailslurp_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailslurp-client
-Version: 8.7.1
+Version: 9.0.0
 Summary: Official MailSlurp Python SDK Email API
 Home-page: https://www.mailslurp.com/docs/python
 Author: MailSlurp
 Author-email: support@mailslurp.zendesk.com
 License: UNKNOWN
 Description: 
         # MailSlurp Python Client
```

### Comparing `mailslurp-client-8.7.1/mailslurp_client.egg-info/SOURCES.txt` & `mailslurp-client-9.0.0/mailslurp_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,22 +46,25 @@
 mailslurp_client/models/create_webhook_options.py
 mailslurp_client/models/describe_domain_options.py
 mailslurp_client/models/describe_mail_server_domain_result.py
 mailslurp_client/models/dns_lookup_options.py
 mailslurp_client/models/dns_lookup_result.py
 mailslurp_client/models/dns_lookup_results.py
 mailslurp_client/models/domain_dto.py
+mailslurp_client/models/domain_name_record.py
 mailslurp_client/models/domain_preview.py
 mailslurp_client/models/download_attachment_dto.py
 mailslurp_client/models/email.py
 mailslurp_client/models/email_analysis.py
 mailslurp_client/models/email_content_match_result.py
 mailslurp_client/models/email_preview.py
 mailslurp_client/models/email_projection.py
 mailslurp_client/models/email_verification_result.py
+mailslurp_client/models/expired_inbox_dto.py
+mailslurp_client/models/expired_inbox_record_projection.py
 mailslurp_client/models/forward_email_options.py
 mailslurp_client/models/group_contacts_dto.py
 mailslurp_client/models/group_dto.py
 mailslurp_client/models/group_projection.py
 mailslurp_client/models/html_validation_result.py
 mailslurp_client/models/inbox.py
 mailslurp_client/models/inbox_projection.py
@@ -69,14 +72,15 @@
 mailslurp_client/models/match_option.py
 mailslurp_client/models/match_options.py
 mailslurp_client/models/name_server_record.py
 mailslurp_client/models/page_alias.py
 mailslurp_client/models/page_contact_projection.py
 mailslurp_client/models/page_email_preview.py
 mailslurp_client/models/page_email_projection.py
+mailslurp_client/models/page_expired_inbox_record_projection.py
 mailslurp_client/models/page_group_projection.py
 mailslurp_client/models/page_inbox_projection.py
 mailslurp_client/models/page_sent_email_projection.py
 mailslurp_client/models/page_template_projection.py
 mailslurp_client/models/page_thread_projection.py
 mailslurp_client/models/page_webhook_projection.py
 mailslurp_client/models/pageable.py
@@ -131,23 +135,26 @@
 test/test_describe_domain_options.py
 test/test_describe_mail_server_domain_result.py
 test/test_dns_lookup_options.py
 test/test_dns_lookup_result.py
 test/test_dns_lookup_results.py
 test/test_domain_controller_api.py
 test/test_domain_dto.py
+test/test_domain_name_record.py
 test/test_domain_preview.py
 test/test_download_attachment_dto.py
 test/test_email.py
 test/test_email_analysis.py
 test/test_email_content_match_result.py
 test/test_email_controller_api.py
 test/test_email_preview.py
 test/test_email_projection.py
 test/test_email_verification_result.py
+test/test_expired_inbox_dto.py
+test/test_expired_inbox_record_projection.py
 test/test_form_controller_api.py
 test/test_forward_email_options.py
 test/test_group_contacts_dto.py
 test/test_group_controller_api.py
 test/test_group_dto.py
 test/test_group_projection.py
 test/test_html_validation_result.py
@@ -159,14 +166,15 @@
 test/test_match_option.py
 test/test_match_options.py
 test/test_name_server_record.py
 test/test_page_alias.py
 test/test_page_contact_projection.py
 test/test_page_email_preview.py
 test/test_page_email_projection.py
+test/test_page_expired_inbox_record_projection.py
 test/test_page_group_projection.py
 test/test_page_inbox_projection.py
 test/test_page_sent_email_projection.py
 test/test_page_template_projection.py
 test/test_page_thread_projection.py
 test/test_page_webhook_projection.py
 test/test_pageable.py
```

### Comparing `mailslurp-client-8.7.1/setup.py` & `mailslurp-client-9.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages 
 
 setup(
     name="mailslurp-client",
-    version="8.7.1",
+    version="9.0.0",
     description="Official MailSlurp Python SDK Email API",
     author="MailSlurp",
     author_email="support@mailslurp.zendesk.com",
     url="https://www.mailslurp.com/docs/python",
     keywords=["MailSlurp", "Email", "SMTP", "Mailer", "MailSlurp API", "Test"],
     install_requires=["urllib3 >= 1.15", "six >= 1.10", "certifi", "python-dateutil"],
     packages=find_packages(exclude=["test", "tests"]),
```

### Comparing `mailslurp-client-8.7.1/test/test_alias.py` & `mailslurp-client-9.0.0/test/test_alias.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_alias_controller_api.py` & `mailslurp-client-9.0.0/test/test_alias_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_alias_dto.py` & `mailslurp-client-9.0.0/test/test_alias_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_alias_projection.py` & `mailslurp-client-9.0.0/test/test_alias_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_attachment_controller_api.py` & `mailslurp-client-9.0.0/test/test_attachment_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_attachment_meta_data.py` & `mailslurp-client-9.0.0/test/test_attachment_meta_data.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_basic_auth_options.py` & `mailslurp-client-9.0.0/test/test_basic_auth_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_bulk_actions_controller_api.py` & `mailslurp-client-9.0.0/test/test_bulk_actions_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_bulk_send_email_options.py` & `mailslurp-client-9.0.0/test/test_bulk_send_email_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_common_actions_controller_api.py` & `mailslurp-client-9.0.0/test/test_common_actions_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_contact_controller_api.py` & `mailslurp-client-9.0.0/test/test_contact_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_contact_dto.py` & `mailslurp-client-9.0.0/test/test_contact_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_contact_projection.py` & `mailslurp-client-9.0.0/test/test_contact_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_content_match_options.py` & `mailslurp-client-9.0.0/test/test_content_match_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_create_alias_options.py` & `mailslurp-client-9.0.0/test/test_create_alias_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_create_contact_options.py` & `mailslurp-client-9.0.0/test/test_create_contact_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_create_domain_options.py` & `mailslurp-client-9.0.0/test/test_create_domain_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_create_group_options.py` & `mailslurp-client-9.0.0/test/test_create_group_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_create_inbox_dto.py` & `mailslurp-client-9.0.0/test/test_create_inbox_dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,16 @@
                 description = '0', 
                 email_address = '0', 
                 expires_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 favourite = True, 
                 name = '0', 
                 tags = [
                     '0'
-                    ]
+                    ], 
+                use_domain_pool = True
             )
         else :
             return CreateInboxDto(
         )
 
     def testCreateInboxDto(self):
         """Test CreateInboxDto"""
```

### Comparing `mailslurp-client-8.7.1/test/test_create_template_options.py` & `mailslurp-client-9.0.0/test/test_create_template_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_create_webhook_options.py` & `mailslurp-client-9.0.0/test/test_create_webhook_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_describe_domain_options.py` & `mailslurp-client-9.0.0/test/test_describe_domain_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_describe_mail_server_domain_result.py` & `mailslurp-client-9.0.0/test/test_describe_mail_server_domain_result.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_dns_lookup_options.py` & `mailslurp-client-9.0.0/test/test_dns_lookup_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_dns_lookup_result.py` & `mailslurp-client-9.0.0/test/test_dns_lookup_result.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_dns_lookup_results.py` & `mailslurp-client-9.0.0/test/test_dns_lookup_results.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_domain_controller_api.py` & `mailslurp-client-9.0.0/test/test_domain_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_domain_dto.py` & `mailslurp-client-9.0.0/test/test_domain_preview.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,54 +12,46 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mailslurp_client
-from mailslurp_client.models.domain_dto import DomainDto  # noqa: E501
+from mailslurp_client.models.domain_preview import DomainPreview  # noqa: E501
 from mailslurp_client.rest import ApiException
 
-class TestDomainDto(unittest.TestCase):
-    """DomainDto unit test stubs"""
+class TestDomainPreview(unittest.TestCase):
+    """DomainPreview unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test DomainDto
+        """Test DomainPreview
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mailslurp_client.models.domain_dto.DomainDto()  # noqa: E501
+        # model = mailslurp_client.models.domain_preview.DomainPreview()  # noqa: E501
         if include_optional :
-            return DomainDto(
+            return DomainPreview(
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                dkim_tokens = [
-                    '0'
-                    ], 
                 domain = '0', 
-                id = '0', 
-                is_verified = True, 
-                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                user_id = '0', 
-                verification_token = '0'
+                id = '0'
             )
         else :
-            return DomainDto(
+            return DomainPreview(
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                domain = '0',
                 id = '0',
-                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                user_id = '0',
         )
 
-    def testDomainDto(self):
-        """Test DomainDto"""
+    def testDomainPreview(self):
+        """Test DomainPreview"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mailslurp-client-8.7.1/test/test_domain_preview.py` & `mailslurp-client-9.0.0/test/test_update_group_contacts.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,46 +12,46 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mailslurp_client
-from mailslurp_client.models.domain_preview import DomainPreview  # noqa: E501
+from mailslurp_client.models.update_group_contacts import UpdateGroupContacts  # noqa: E501
 from mailslurp_client.rest import ApiException
 
-class TestDomainPreview(unittest.TestCase):
-    """DomainPreview unit test stubs"""
+class TestUpdateGroupContacts(unittest.TestCase):
+    """UpdateGroupContacts unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test DomainPreview
+        """Test UpdateGroupContacts
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mailslurp_client.models.domain_preview.DomainPreview()  # noqa: E501
+        # model = mailslurp_client.models.update_group_contacts.UpdateGroupContacts()  # noqa: E501
         if include_optional :
-            return DomainPreview(
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                domain = '0', 
-                id = '0'
+            return UpdateGroupContacts(
+                contact_ids = [
+                    '0'
+                    ]
             )
         else :
-            return DomainPreview(
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                domain = '0',
-                id = '0',
+            return UpdateGroupContacts(
+                contact_ids = [
+                    '0'
+                    ],
         )
 
-    def testDomainPreview(self):
-        """Test DomainPreview"""
+    def testUpdateGroupContacts(self):
+        """Test UpdateGroupContacts"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mailslurp-client-8.7.1/test/test_download_attachment_dto.py` & `mailslurp-client-9.0.0/test/test_download_attachment_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_email.py` & `mailslurp-client-9.0.0/test/test_email.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_email_analysis.py` & `mailslurp-client-9.0.0/test/test_email_analysis.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_email_content_match_result.py` & `mailslurp-client-9.0.0/test/test_email_content_match_result.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_email_controller_api.py` & `mailslurp-client-9.0.0/test/test_email_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_email_preview.py` & `mailslurp-client-9.0.0/test/test_email_preview.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_email_projection.py` & `mailslurp-client-9.0.0/test/test_email_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_email_verification_result.py` & `mailslurp-client-9.0.0/test/test_email_verification_result.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_form_controller_api.py` & `mailslurp-client-9.0.0/test/test_form_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_forward_email_options.py` & `mailslurp-client-9.0.0/test/test_forward_email_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_group_contacts_dto.py` & `mailslurp-client-9.0.0/test/test_group_contacts_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_group_controller_api.py` & `mailslurp-client-9.0.0/test/test_group_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_group_dto.py` & `mailslurp-client-9.0.0/test/test_group_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_group_projection.py` & `mailslurp-client-9.0.0/test/test_group_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_html_validation_result.py` & `mailslurp-client-9.0.0/test/test_html_validation_result.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_inbox.py` & `mailslurp-client-9.0.0/test/test_inbox.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_inbox_controller_api.py` & `mailslurp-client-9.0.0/test/test_inbox_controller_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,35 @@
     def test_get_emails(self):
         """Test case for get_emails
 
         Get emails in an Inbox. This method is not idempotent as it allows retries and waits if you want certain conditions to be met before returning. For simple listing and sorting of known emails use the email controller instead.  # noqa: E501
         """
         pass
 
+    def test_get_expired_inbox_record_by_id(self):
+        """Test case for get_expired_inbox_record_by_id
+
+        Get an expired inbox record  # noqa: E501
+        """
+        pass
+
+    def test_get_expired_inbox_record_by_inbox_id(self):
+        """Test case for get_expired_inbox_record_by_inbox_id
+
+        Get expired inbox record for a previously existing inbox  # noqa: E501
+        """
+        pass
+
+    def test_get_expired_inbox_records(self):
+        """Test case for get_expired_inbox_records
+
+        List records of expired inboxes  # noqa: E501
+        """
+        pass
+
     def test_get_inbox(self):
         """Test case for get_inbox
 
         Get Inbox  # noqa: E501
         """
         pass
```

### Comparing `mailslurp-client-8.7.1/test/test_inbox_projection.py` & `mailslurp-client-9.0.0/test/test_inbox_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_ip_address_result.py` & `mailslurp-client-9.0.0/test/test_ip_address_result.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_mail_server_controller_api.py` & `mailslurp-client-9.0.0/test/test_mail_server_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_match_option.py` & `mailslurp-client-9.0.0/test/test_match_option.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_match_options.py` & `mailslurp-client-9.0.0/test/test_match_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_name_server_record.py` & `mailslurp-client-9.0.0/test/test_name_server_record.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_page_alias.py` & `mailslurp-client-9.0.0/test/test_page_alias.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_page_contact_projection.py` & `mailslurp-client-9.0.0/test/test_page_contact_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_page_email_preview.py` & `mailslurp-client-9.0.0/test/test_page_email_preview.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_page_email_projection.py` & `mailslurp-client-9.0.0/test/test_page_email_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_page_group_projection.py` & `mailslurp-client-9.0.0/test/test_page_group_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_page_inbox_projection.py` & `mailslurp-client-9.0.0/test/test_page_inbox_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_page_sent_email_projection.py` & `mailslurp-client-9.0.0/test/test_page_sent_email_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_page_template_projection.py` & `mailslurp-client-9.0.0/test/test_page_template_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_page_thread_projection.py` & `mailslurp-client-9.0.0/test/test_page_thread_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_page_webhook_projection.py` & `mailslurp-client-9.0.0/test/test_page_webhook_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_pageable.py` & `mailslurp-client-9.0.0/test/test_pageable.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_raw_email_json.py` & `mailslurp-client-9.0.0/test/test_raw_email_json.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_reply_to_alias_email_options.py` & `mailslurp-client-9.0.0/test/test_reply_to_alias_email_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_reply_to_email_options.py` & `mailslurp-client-9.0.0/test/test_reply_to_email_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_send_email_options.py` & `mailslurp-client-9.0.0/test/test_send_email_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_sent_email_dto.py` & `mailslurp-client-9.0.0/test/test_sent_email_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_sent_email_projection.py` & `mailslurp-client-9.0.0/test/test_sent_email_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_sent_emails_controller_api.py` & `mailslurp-client-9.0.0/test/test_sent_emails_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_set_inbox_favourited_options.py` & `mailslurp-client-9.0.0/test/test_set_inbox_favourited_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_simple_send_email_options.py` & `mailslurp-client-9.0.0/test/test_simple_send_email_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_sort.py` & `mailslurp-client-9.0.0/test/test_sort.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_template_controller_api.py` & `mailslurp-client-9.0.0/test/test_template_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_template_dto.py` & `mailslurp-client-9.0.0/test/test_template_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_template_projection.py` & `mailslurp-client-9.0.0/test/test_template_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_template_variable.py` & `mailslurp-client-9.0.0/test/test_template_variable.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_thread_projection.py` & `mailslurp-client-9.0.0/test/test_thread_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_unread_count.py` & `mailslurp-client-9.0.0/test/test_unread_count.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_update_alias_options.py` & `mailslurp-client-9.0.0/test/test_update_alias_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_update_group_contacts.py` & `mailslurp-client-9.0.0/test/test_expired_inbox_dto.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,46 +12,46 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import mailslurp_client
-from mailslurp_client.models.update_group_contacts import UpdateGroupContacts  # noqa: E501
+from mailslurp_client.models.expired_inbox_dto import ExpiredInboxDto  # noqa: E501
 from mailslurp_client.rest import ApiException
 
-class TestUpdateGroupContacts(unittest.TestCase):
-    """UpdateGroupContacts unit test stubs"""
+class TestExpiredInboxDto(unittest.TestCase):
+    """ExpiredInboxDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test UpdateGroupContacts
+        """Test ExpiredInboxDto
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = mailslurp_client.models.update_group_contacts.UpdateGroupContacts()  # noqa: E501
+        # model = mailslurp_client.models.expired_inbox_dto.ExpiredInboxDto()  # noqa: E501
         if include_optional :
-            return UpdateGroupContacts(
-                contact_ids = [
-                    '0'
-                    ]
+            return ExpiredInboxDto(
+                email_address = '0', 
+                id = '0', 
+                inbox_id = '0'
             )
         else :
-            return UpdateGroupContacts(
-                contact_ids = [
-                    '0'
-                    ],
+            return ExpiredInboxDto(
+                email_address = '0',
+                id = '0',
+                inbox_id = '0',
         )
 
-    def testUpdateGroupContacts(self):
-        """Test UpdateGroupContacts"""
+    def testExpiredInboxDto(self):
+        """Test ExpiredInboxDto"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `mailslurp-client-8.7.1/test/test_update_inbox_options.py` & `mailslurp-client-9.0.0/test/test_update_inbox_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_upload_attachment_options.py` & `mailslurp-client-9.0.0/test/test_upload_attachment_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_validation_dto.py` & `mailslurp-client-9.0.0/test/test_validation_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_validation_message.py` & `mailslurp-client-9.0.0/test/test_validation_message.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_verify_email_address_options.py` & `mailslurp-client-9.0.0/test/test_verify_email_address_options.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_wait_for_conditions.py` & `mailslurp-client-9.0.0/test/test_wait_for_conditions.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_wait_for_controller_api.py` & `mailslurp-client-9.0.0/test/test_wait_for_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_webhook_controller_api.py` & `mailslurp-client-9.0.0/test/test_webhook_controller_api.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_webhook_dto.py` & `mailslurp-client-9.0.0/test/test_webhook_dto.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_webhook_projection.py` & `mailslurp-client-9.0.0/test/test_webhook_projection.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_webhook_test_request.py` & `mailslurp-client-9.0.0/test/test_webhook_test_request.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_webhook_test_response.py` & `mailslurp-client-9.0.0/test/test_webhook_test_response.py`

 * *Files identical despite different names*

### Comparing `mailslurp-client-8.7.1/test/test_webhook_test_result.py` & `mailslurp-client-9.0.0/test/test_webhook_test_result.py`

 * *Files identical despite different names*

