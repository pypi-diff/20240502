# Comparing `tmp/Files.com-1.4.8.tar.gz` & `tmp/Files.com-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Files.com-1.4.8.tar", last modified: Fri Jan 12 15:22:30 2024, max compression
+gzip compressed data, was "Files.com-1.4.9.tar", last modified: Fri Jan 12 16:43:33 2024, max compression
```

## Comparing `Files.com-1.4.8.tar` & `Files.com-1.4.9.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-01-12 15:22:30.099447 Files.com-1.4.8/
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-01-12 15:22:30.091447 Files.com-1.4.8/Files.com.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)      232 2024-01-12 15:22:30.000000 Files.com-1.4.8/Files.com.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3129 2024-01-12 15:22:30.000000 Files.com-1.4.8/Files.com.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)        1 2024-01-12 15:22:30.000000 Files.com-1.4.8/Files.com.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)       43 2024-01-12 15:22:30.000000 Files.com-1.4.8/Files.com.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)       10 2024-01-12 15:22:30.000000 Files.com-1.4.8/Files.com.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)      232 2024-01-12 15:22:30.099447 Files.com-1.4.8/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5764 2024-01-12 15:22:20.000000 Files.com-1.4.8/README.md
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-01-12 15:22:30.091447 Files.com-1.4.8/files_sdk/
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9986 2024-01-12 15:22:28.000000 Files.com-1.4.8/files_sdk/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1606 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/api.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10789 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/api_client.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    57103 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/error.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1157 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/list_obj.py
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-01-12 15:22:30.099447 Files.com-1.4.8/files_sdk/models/
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4565 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1977 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/account_line_item.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1915 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/action.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6432 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/action_notification_export.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4071 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/action_notification_export_result.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2357 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/action_webhook_failure.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    16013 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/api_key.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4655 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/app.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7265 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/as2_incoming_message.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6808 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/as2_outgoing_message.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    11107 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/as2_partner.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10676 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/as2_station.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)      995 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/auto.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    29066 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/automation.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4467 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/automation_run.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4755 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/bandwidth_snapshot.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    17233 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/behavior.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    30540 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/bundle.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4865 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/bundle_download.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8563 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/bundle_notification.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5647 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/bundle_recipient.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3384 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/bundle_registration.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    11290 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/clickwrap.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2370 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/dns_record.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5313 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/email_incoming_message.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1101 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/errors.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7403 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/external_event.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    29891 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/file.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1230 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/file_action.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7152 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/file_comment.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4350 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/file_comment_reaction.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2552 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/file_migration.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2583 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/file_upload_part.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7285 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/folder.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1501 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/form_field.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9304 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/form_field_set.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10440 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/gpg_key.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    13089 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/group.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9760 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/group_user.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    14183 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/history.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    14156 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/history_export.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6188 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/history_export_result.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1052 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/image.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5603 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/inbox_recipient.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3341 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/inbox_registration.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4714 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/inbox_upload.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3801 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/invoice.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1657 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/invoice_line_item.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4660 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/ip_address.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6673 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/lock.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10184 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/message.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8265 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/message_comment.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6517 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/message_comment_reaction.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6288 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/message_reaction.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    18626 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/notification.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3801 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/payment.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1284 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/payment_line_item.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7575 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/permission.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1347 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/preview.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2679 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/priority.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7510 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/project.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1259 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/public_ip_address.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8414 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/public_key.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4509 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/remote_bandwidth_snapshot.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    74969 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/remote_server.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1721 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/remote_server_configuration_file.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8681 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/request.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3790 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/session.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3317 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/settings_change.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7918 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/sftp_host_key.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9058 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/share_group.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1248 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/share_group_member.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    43258 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/site.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8577 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/snapshot.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8580 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/sso_strategy.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1355 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/status.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5200 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/style.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5518 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/usage_daily_snapshot.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3999 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/usage_snapshot.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)    47558 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/user.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2954 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/user_cipher_use.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5929 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/user_request.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4601 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/models/webhook_test.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1694 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/path_util.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)      962 2024-01-12 15:22:20.000000 Files.com-1.4.8/files_sdk/util.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)      313 2024-01-12 15:22:20.000000 Files.com-1.4.8/pyproject.toml
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)       38 2024-01-12 15:22:30.099447 Files.com-1.4.8/setup.cfg
--rw-r--r--   0 jenkins   (1002) jenkins   (1003)      585 2024-01-12 15:22:20.000000 Files.com-1.4.8/setup.py
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-01-12 16:43:33.662317 Files.com-1.4.9/
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-01-12 16:43:33.654317 Files.com-1.4.9/Files.com.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)      232 2024-01-12 16:43:33.000000 Files.com-1.4.9/Files.com.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3129 2024-01-12 16:43:33.000000 Files.com-1.4.9/Files.com.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)        1 2024-01-12 16:43:33.000000 Files.com-1.4.9/Files.com.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)       43 2024-01-12 16:43:33.000000 Files.com-1.4.9/Files.com.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)       10 2024-01-12 16:43:33.000000 Files.com-1.4.9/Files.com.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)      232 2024-01-12 16:43:33.662317 Files.com-1.4.9/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5764 2024-01-12 16:43:22.000000 Files.com-1.4.9/README.md
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-01-12 16:43:33.654317 Files.com-1.4.9/files_sdk/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9986 2024-01-12 16:43:32.000000 Files.com-1.4.9/files_sdk/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1606 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/api.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10789 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/api_client.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    57103 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/error.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1157 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/list_obj.py
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1003)        0 2024-01-12 16:43:33.662317 Files.com-1.4.9/files_sdk/models/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4565 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1977 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/account_line_item.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1915 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/action.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6432 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/action_notification_export.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4071 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/action_notification_export_result.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2357 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/action_webhook_failure.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    16013 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/api_key.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4655 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/app.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7265 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/as2_incoming_message.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6808 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/as2_outgoing_message.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    11107 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/as2_partner.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10676 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/as2_station.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)      995 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/auto.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    29066 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/automation.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4467 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/automation_run.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4755 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/bandwidth_snapshot.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    17233 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/behavior.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    30540 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/bundle.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4865 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/bundle_download.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8563 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/bundle_notification.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5647 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/bundle_recipient.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3384 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/bundle_registration.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    11290 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/clickwrap.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2370 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/dns_record.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5313 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/email_incoming_message.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1101 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/errors.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7403 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/external_event.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    29891 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/file.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1230 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/file_action.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7152 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/file_comment.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4350 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/file_comment_reaction.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2552 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/file_migration.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2583 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/file_upload_part.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7285 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/folder.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1501 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/form_field.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9304 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/form_field_set.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10440 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/gpg_key.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    13089 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/group.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9760 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/group_user.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    14183 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/history.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    14156 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/history_export.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6188 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/history_export_result.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1052 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/image.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5603 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/inbox_recipient.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3341 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/inbox_registration.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4714 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/inbox_upload.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3801 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/invoice.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1657 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/invoice_line_item.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4660 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/ip_address.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6673 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/lock.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    10184 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/message.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8265 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/message_comment.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6517 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/message_comment_reaction.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     6288 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/message_reaction.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    18626 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/notification.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3801 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/payment.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1284 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/payment_line_item.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7575 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/permission.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1347 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/preview.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2679 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/priority.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7510 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/project.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1259 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/public_ip_address.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8414 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/public_key.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4509 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/remote_bandwidth_snapshot.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    74969 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/remote_server.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1721 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/remote_server_configuration_file.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8681 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/request.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3790 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/session.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3317 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/settings_change.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     7918 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/sftp_host_key.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     9058 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/share_group.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1248 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/share_group_member.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    43258 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/site.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8577 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/snapshot.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     8580 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/sso_strategy.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1355 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/status.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5200 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/style.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5518 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/usage_daily_snapshot.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     3999 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/usage_snapshot.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)    47558 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/user.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     2954 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/user_cipher_use.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     5929 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/user_request.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     4601 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/models/webhook_test.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)     1694 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/path_util.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)      962 2024-01-12 16:43:22.000000 Files.com-1.4.9/files_sdk/util.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)      313 2024-01-12 16:43:22.000000 Files.com-1.4.9/pyproject.toml
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)       38 2024-01-12 16:43:33.662317 Files.com-1.4.9/setup.cfg
+-rw-r--r--   0 jenkins   (1002) jenkins   (1003)      585 2024-01-12 16:43:22.000000 Files.com-1.4.9/setup.py
```

### Comparing `Files.com-1.4.8/Files.com.egg-info/SOURCES.txt` & `Files.com-1.4.9/Files.com.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/README.md` & `Files.com-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/__init__.py` & `Files.com-1.4.9/files_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
 import files_sdk.path_util
 
 the_api_key = ""
 session_id = None
 base_url = "https://app.files.com"
 base_path = "api/rest/v1"
-version = "1.4.8"
+version = "1.4.9"
 
 __version__ = version
 
 initial_network_retry_delay = 0.5
 max_network_retry_delay = 2
 open_timeout = 30
 read_timeout = 80
```

### Comparing `Files.com-1.4.8/files_sdk/api.py` & `Files.com-1.4.9/files_sdk/api.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/api_client.py` & `Files.com-1.4.9/files_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/error.py` & `Files.com-1.4.9/files_sdk/error.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/list_obj.py` & `Files.com-1.4.9/files_sdk/list_obj.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/__init__.py` & `Files.com-1.4.9/files_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/account_line_item.py` & `Files.com-1.4.9/files_sdk/models/account_line_item.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/action.py` & `Files.com-1.4.9/files_sdk/models/action.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/action_notification_export.py` & `Files.com-1.4.9/files_sdk/models/action_notification_export.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/action_notification_export_result.py` & `Files.com-1.4.9/files_sdk/models/action_notification_export_result.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/action_webhook_failure.py` & `Files.com-1.4.9/files_sdk/models/action_webhook_failure.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/api_key.py` & `Files.com-1.4.9/files_sdk/models/api_key.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/app.py` & `Files.com-1.4.9/files_sdk/models/app.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/as2_incoming_message.py` & `Files.com-1.4.9/files_sdk/models/as2_incoming_message.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/as2_outgoing_message.py` & `Files.com-1.4.9/files_sdk/models/as2_outgoing_message.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/as2_partner.py` & `Files.com-1.4.9/files_sdk/models/as2_partner.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/as2_station.py` & `Files.com-1.4.9/files_sdk/models/as2_station.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/auto.py` & `Files.com-1.4.9/files_sdk/models/auto.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/automation.py` & `Files.com-1.4.9/files_sdk/models/automation.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/automation_run.py` & `Files.com-1.4.9/files_sdk/models/automation_run.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/bandwidth_snapshot.py` & `Files.com-1.4.9/files_sdk/models/bandwidth_snapshot.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/behavior.py` & `Files.com-1.4.9/files_sdk/models/behavior.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/bundle.py` & `Files.com-1.4.9/files_sdk/models/bundle.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/bundle_download.py` & `Files.com-1.4.9/files_sdk/models/bundle_download.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/bundle_notification.py` & `Files.com-1.4.9/files_sdk/models/bundle_notification.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/bundle_recipient.py` & `Files.com-1.4.9/files_sdk/models/bundle_recipient.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/bundle_registration.py` & `Files.com-1.4.9/files_sdk/models/bundle_registration.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/clickwrap.py` & `Files.com-1.4.9/files_sdk/models/clickwrap.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/dns_record.py` & `Files.com-1.4.9/files_sdk/models/dns_record.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/email_incoming_message.py` & `Files.com-1.4.9/files_sdk/models/email_incoming_message.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/errors.py` & `Files.com-1.4.9/files_sdk/models/errors.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/external_event.py` & `Files.com-1.4.9/files_sdk/models/external_event.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/file.py` & `Files.com-1.4.9/files_sdk/models/file.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/file_action.py` & `Files.com-1.4.9/files_sdk/models/file_action.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/file_comment.py` & `Files.com-1.4.9/files_sdk/models/file_comment.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/file_comment_reaction.py` & `Files.com-1.4.9/files_sdk/models/file_comment_reaction.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/file_migration.py` & `Files.com-1.4.9/files_sdk/models/file_migration.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/file_upload_part.py` & `Files.com-1.4.9/files_sdk/models/file_upload_part.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/folder.py` & `Files.com-1.4.9/files_sdk/models/folder.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/form_field.py` & `Files.com-1.4.9/files_sdk/models/form_field.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/form_field_set.py` & `Files.com-1.4.9/files_sdk/models/form_field_set.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/gpg_key.py` & `Files.com-1.4.9/files_sdk/models/gpg_key.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/group.py` & `Files.com-1.4.9/files_sdk/models/group.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/group_user.py` & `Files.com-1.4.9/files_sdk/models/group_user.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/history.py` & `Files.com-1.4.9/files_sdk/models/history.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/history_export.py` & `Files.com-1.4.9/files_sdk/models/history_export.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/history_export_result.py` & `Files.com-1.4.9/files_sdk/models/history_export_result.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/image.py` & `Files.com-1.4.9/files_sdk/models/image.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/inbox_recipient.py` & `Files.com-1.4.9/files_sdk/models/inbox_recipient.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/inbox_registration.py` & `Files.com-1.4.9/files_sdk/models/inbox_registration.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/inbox_upload.py` & `Files.com-1.4.9/files_sdk/models/inbox_upload.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/invoice.py` & `Files.com-1.4.9/files_sdk/models/invoice.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/invoice_line_item.py` & `Files.com-1.4.9/files_sdk/models/invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/ip_address.py` & `Files.com-1.4.9/files_sdk/models/ip_address.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/lock.py` & `Files.com-1.4.9/files_sdk/models/lock.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/message.py` & `Files.com-1.4.9/files_sdk/models/message.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/message_comment.py` & `Files.com-1.4.9/files_sdk/models/message_comment.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/message_comment_reaction.py` & `Files.com-1.4.9/files_sdk/models/message_comment_reaction.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/message_reaction.py` & `Files.com-1.4.9/files_sdk/models/message_reaction.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/notification.py` & `Files.com-1.4.9/files_sdk/models/notification.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/payment.py` & `Files.com-1.4.9/files_sdk/models/payment.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/payment_line_item.py` & `Files.com-1.4.9/files_sdk/models/payment_line_item.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/permission.py` & `Files.com-1.4.9/files_sdk/models/permission.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/preview.py` & `Files.com-1.4.9/files_sdk/models/preview.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/priority.py` & `Files.com-1.4.9/files_sdk/models/priority.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/project.py` & `Files.com-1.4.9/files_sdk/models/project.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/public_ip_address.py` & `Files.com-1.4.9/files_sdk/models/public_ip_address.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/public_key.py` & `Files.com-1.4.9/files_sdk/models/public_key.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/remote_bandwidth_snapshot.py` & `Files.com-1.4.9/files_sdk/models/remote_bandwidth_snapshot.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/remote_server.py` & `Files.com-1.4.9/files_sdk/models/remote_server.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/remote_server_configuration_file.py` & `Files.com-1.4.9/files_sdk/models/remote_server_configuration_file.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/request.py` & `Files.com-1.4.9/files_sdk/models/request.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/session.py` & `Files.com-1.4.9/files_sdk/models/session.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/settings_change.py` & `Files.com-1.4.9/files_sdk/models/settings_change.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/sftp_host_key.py` & `Files.com-1.4.9/files_sdk/models/sftp_host_key.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/share_group.py` & `Files.com-1.4.9/files_sdk/models/share_group.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/share_group_member.py` & `Files.com-1.4.9/files_sdk/models/share_group_member.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/site.py` & `Files.com-1.4.9/files_sdk/models/site.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/snapshot.py` & `Files.com-1.4.9/files_sdk/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/sso_strategy.py` & `Files.com-1.4.9/files_sdk/models/sso_strategy.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/status.py` & `Files.com-1.4.9/files_sdk/models/status.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/style.py` & `Files.com-1.4.9/files_sdk/models/style.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/usage_daily_snapshot.py` & `Files.com-1.4.9/files_sdk/models/usage_daily_snapshot.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/usage_snapshot.py` & `Files.com-1.4.9/files_sdk/models/usage_snapshot.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/user.py` & `Files.com-1.4.9/files_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/user_cipher_use.py` & `Files.com-1.4.9/files_sdk/models/user_cipher_use.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/user_request.py` & `Files.com-1.4.9/files_sdk/models/user_request.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/models/webhook_test.py` & `Files.com-1.4.9/files_sdk/models/webhook_test.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/path_util.py` & `Files.com-1.4.9/files_sdk/path_util.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/files_sdk/util.py` & `Files.com-1.4.9/files_sdk/util.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.4.8/setup.py` & `Files.com-1.4.9/setup.py`

 * *Files identical despite different names*

