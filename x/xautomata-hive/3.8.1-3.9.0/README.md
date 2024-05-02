# Comparing `tmp/xautomata-hive-3.8.1.tar.gz` & `tmp/xautomata-hive-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xautomata-hive-3.8.1.tar", last modified: Tue Oct  3 16:26:34 2023, max compression
+gzip compressed data, was "xautomata-hive-3.9.0.tar", last modified: Fri Oct  6 12:07:49 2023, max compression
```

## Comparing `xautomata-hive-3.8.1.tar` & `xautomata-hive-3.9.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 16:26:34.588160 xautomata-hive-3.8.1/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10746 2023-10-03 16:26:34.588160 xautomata-hive-3.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10385 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 16:26:34.572160 xautomata-hive-3.8.1/hive/
--rw-r--r--   0 root         (0) root         (0)       68 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39342 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 16:26:34.588160 xautomata-hive-3.8.1/hive/cookbook/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/__init__.py
--rw-r--r--   0 root         (0) root         (0)      786 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/acl_docs.py
--rw-r--r--   0 root         (0) root         (0)     9506 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/acl_overrides.py
--rw-r--r--   0 root         (0) root         (0)     3485 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/analytics.py
--rw-r--r--   0 root         (0) root         (0)    11902 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/anomalies.py
--rw-r--r--   0 root         (0) root         (0)    23357 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/calendars.py
--rw-r--r--   0 root         (0) root         (0)    40792 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/contacts.py
--rw-r--r--   0 root         (0) root         (0)    70793 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/customers.py
--rw-r--r--   0 root         (0) root         (0)    28877 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/dashboards.py
--rw-r--r--   0 root         (0) root         (0)    43423 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/dispatchers.py
--rw-r--r--   0 root         (0) root         (0)    47118 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/downtimes.py
--rw-r--r--   0 root         (0) root         (0)    29622 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/external_tickets.py
--rw-r--r--   0 root         (0) root         (0)     5904 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/firmware_updates.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/google.py
--rw-r--r--   0 root         (0) root         (0)    40064 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/groups.py
--rw-r--r--   0 root         (0) root         (0)    13327 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/last_status.py
--rw-r--r--   0 root         (0) root         (0)    16458 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/login.py
--rw-r--r--   0 root         (0) root         (0)    14925 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/messages.py
--rw-r--r--   0 root         (0) root         (0)     2764 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/metric_ingest.py
--rw-r--r--   0 root         (0) root         (0)    29241 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/metric_types.py
--rw-r--r--   0 root         (0) root         (0)    36089 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/metrics.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/microsoft.py
--rw-r--r--   0 root         (0) root         (0)    14086 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/notification_provider_types.py
--rw-r--r--   0 root         (0) root         (0)    11771 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/notification_providers.py
--rw-r--r--   0 root         (0) root         (0)    43906 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/objects.py
--rw-r--r--   0 root         (0) root         (0)    12621 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/opening_reasons.py
--rw-r--r--   0 root         (0) root         (0)    13640 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/probe_types.py
--rw-r--r--   0 root         (0) root         (0)    23957 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/probes.py
--rw-r--r--   0 root         (0) root         (0)     1769 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/probes_log_ingest.py
--rw-r--r--   0 root         (0) root         (0)    10946 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/profile_topics.py
--rw-r--r--   0 root         (0) root         (0)    11705 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/reason_for_closure.py
--rw-r--r--   0 root         (0) root         (0)     7820 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/retention_rules.py
--rw-r--r--   0 root         (0) root         (0)     6732 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/schedules.py
--rw-r--r--   0 root         (0) root         (0)    47038 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/services.py
--rw-r--r--   0 root         (0) root         (0)    34579 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/sites.py
--rw-r--r--   0 root         (0) root         (0)    23289 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/tree_hierarchy.py
--rw-r--r--   0 root         (0) root         (0)    34235 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/ts_cost_azure_raw.py
--rw-r--r--   0 root         (0) root         (0)    36373 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/ts_cost_management.py
--rw-r--r--   0 root         (0) root         (0)     6412 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/ts_metric_status.py
--rw-r--r--   0 root         (0) root         (0)     6157 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/ts_metric_value.py
--rw-r--r--   0 root         (0) root         (0)    16342 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/ts_ntop_flows.py
--rw-r--r--   0 root         (0) root         (0)    15791 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/ts_service_status.py
--rw-r--r--   0 root         (0) root         (0)    15077 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/ts_service_value.py
--rw-r--r--   0 root         (0) root         (0)    45185 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/users.py
--rw-r--r--   0 root         (0) root         (0)     6367 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/users_notifications.py
--rw-r--r--   0 root         (0) root         (0)    24158 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/virtual_domains.py
--rw-r--r--   0 root         (0) root         (0)     6567 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/webhooks.py
--rw-r--r--   0 root         (0) root         (0)    15981 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/widget_groups.py
--rw-r--r--   0 root         (0) root         (0)    24348 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/cookbook/widgets.py
--rw-r--r--   0 root         (0) root         (0)     9478 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/decorators.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3570 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/infrastrucure_keys.py
--rw-r--r--   0 root         (0) root         (0)       17 2023-10-03 16:26:33.000000 xautomata-hive-3.8.1/hive/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-03 16:26:34.588160 xautomata-hive-3.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      884 2023-10-03 16:26:34.000000 xautomata-hive-3.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-03 16:26:34.588160 xautomata-hive-3.8.1/xautomata_hive.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10746 2023-10-03 16:26:34.000000 xautomata-hive-3.8.1/xautomata_hive.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1786 2023-10-03 16:26:34.000000 xautomata-hive-3.8.1/xautomata_hive.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-03 16:26:34.000000 xautomata-hive-3.8.1/xautomata_hive.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-10-03 16:26:34.000000 xautomata-hive-3.8.1/xautomata_hive.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-10-03 16:26:34.000000 xautomata-hive-3.8.1/xautomata_hive.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-06 12:07:49.643594 xautomata-hive-3.9.0/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10748 2023-10-06 12:07:49.643594 xautomata-hive-3.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10385 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-06 12:07:49.627594 xautomata-hive-3.9.0/hive/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39342 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-06 12:07:49.639594 xautomata-hive-3.9.0/hive/cookbook/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      786 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/acl_docs.py
+-rw-r--r--   0 root         (0) root         (0)     9506 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/acl_overrides.py
+-rw-r--r--   0 root         (0) root         (0)     3485 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/analytics.py
+-rw-r--r--   0 root         (0) root         (0)    11902 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/anomalies.py
+-rw-r--r--   0 root         (0) root         (0)    23357 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/calendars.py
+-rw-r--r--   0 root         (0) root         (0)    40792 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/contacts.py
+-rw-r--r--   0 root         (0) root         (0)    70793 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/customers.py
+-rw-r--r--   0 root         (0) root         (0)    28877 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/dashboards.py
+-rw-r--r--   0 root         (0) root         (0)    43423 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/dispatchers.py
+-rw-r--r--   0 root         (0) root         (0)    47118 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/downtimes.py
+-rw-r--r--   0 root         (0) root         (0)    29622 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/external_tickets.py
+-rw-r--r--   0 root         (0) root         (0)     5904 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/firmware_updates.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/google.py
+-rw-r--r--   0 root         (0) root         (0)    40064 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/groups.py
+-rw-r--r--   0 root         (0) root         (0)    13327 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/last_status.py
+-rw-r--r--   0 root         (0) root         (0)    16458 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/login.py
+-rw-r--r--   0 root         (0) root         (0)    14925 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/messages.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/metric_ingest.py
+-rw-r--r--   0 root         (0) root         (0)    29241 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/metric_types.py
+-rw-r--r--   0 root         (0) root         (0)    36089 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/microsoft.py
+-rw-r--r--   0 root         (0) root         (0)    14086 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/notification_provider_types.py
+-rw-r--r--   0 root         (0) root         (0)    11771 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/notification_providers.py
+-rw-r--r--   0 root         (0) root         (0)    43906 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/objects.py
+-rw-r--r--   0 root         (0) root         (0)    12621 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/opening_reasons.py
+-rw-r--r--   0 root         (0) root         (0)    13640 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/probe_types.py
+-rw-r--r--   0 root         (0) root         (0)    23957 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/probes.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/probes_log_ingest.py
+-rw-r--r--   0 root         (0) root         (0)    10946 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/profile_topics.py
+-rw-r--r--   0 root         (0) root         (0)    11705 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/reason_for_closure.py
+-rw-r--r--   0 root         (0) root         (0)     7820 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/retention_rules.py
+-rw-r--r--   0 root         (0) root         (0)     6732 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/schedules.py
+-rw-r--r--   0 root         (0) root         (0)    47038 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/services.py
+-rw-r--r--   0 root         (0) root         (0)    34579 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/sites.py
+-rw-r--r--   0 root         (0) root         (0)    23289 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/tree_hierarchy.py
+-rw-r--r--   0 root         (0) root         (0)    34235 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/ts_cost_azure_raw.py
+-rw-r--r--   0 root         (0) root         (0)    36373 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/ts_cost_management.py
+-rw-r--r--   0 root         (0) root         (0)     6412 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/ts_metric_status.py
+-rw-r--r--   0 root         (0) root         (0)     6157 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/ts_metric_value.py
+-rw-r--r--   0 root         (0) root         (0)    16342 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/ts_ntop_flows.py
+-rw-r--r--   0 root         (0) root         (0)    15791 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/ts_service_status.py
+-rw-r--r--   0 root         (0) root         (0)    15077 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/ts_service_value.py
+-rw-r--r--   0 root         (0) root         (0)    45185 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/users.py
+-rw-r--r--   0 root         (0) root         (0)     6367 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/users_notifications.py
+-rw-r--r--   0 root         (0) root         (0)    24158 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/virtual_domains.py
+-rw-r--r--   0 root         (0) root         (0)     6567 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/webhooks.py
+-rw-r--r--   0 root         (0) root         (0)    15981 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/widget_groups.py
+-rw-r--r--   0 root         (0) root         (0)    24348 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/cookbook/widgets.py
+-rw-r--r--   0 root         (0) root         (0)     9478 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3570 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/infrastrucure_keys.py
+-rw-r--r--   0 root         (0) root         (0)       17 2023-10-06 12:07:48.000000 xautomata-hive-3.9.0/hive/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-10-06 12:07:49.643594 xautomata-hive-3.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      886 2023-10-06 12:07:49.000000 xautomata-hive-3.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-06 12:07:49.639594 xautomata-hive-3.9.0/xautomata_hive.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10748 2023-10-06 12:07:49.000000 xautomata-hive-3.9.0/xautomata_hive.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-10-06 12:07:49.000000 xautomata-hive-3.9.0/xautomata_hive.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-06 12:07:49.000000 xautomata-hive-3.9.0/xautomata_hive.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-10-06 12:07:49.000000 xautomata-hive-3.9.0/xautomata_hive.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-10-06 12:07:49.000000 xautomata-hive-3.9.0/xautomata_hive.egg-info/top_level.txt
```

### Comparing `xautomata-hive-3.8.1/LICENSE` & `xautomata-hive-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/PKG-INFO` & `xautomata-hive-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: xautomata-hive
-Version: 3.8.1
+Version: 3.9.0
 Home-page: https://github.com/sherlogic/xautomata-hive.git
 Author: Enrico Ferro - Andrea Jacassi
 Author-email: 
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: urllib3==2.0.4
+Requires-Dist: urllib3==1.26.17
 Requires-Dist: tqdm==4.64.1
 Requires-Dist: requests==2.31.0
 
 # Xautomata API
 Pacchetto che fornisca una interfaccia semplice per usare le API di Xautomata in python
 
 The full documentation can be fount at https://sherlogic.github.io/xautomata-hive/
```

### Comparing `xautomata-hive-3.8.1/README.md` & `xautomata-hive-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/api.py` & `xautomata-hive-3.9.0/hive/api.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/acl_docs.py` & `xautomata-hive-3.9.0/hive/cookbook/acl_docs.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/acl_overrides.py` & `xautomata-hive-3.9.0/hive/cookbook/acl_overrides.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/analytics.py` & `xautomata-hive-3.9.0/hive/cookbook/analytics.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/anomalies.py` & `xautomata-hive-3.9.0/hive/cookbook/anomalies.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/calendars.py` & `xautomata-hive-3.9.0/hive/cookbook/calendars.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/contacts.py` & `xautomata-hive-3.9.0/hive/cookbook/contacts.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/customers.py` & `xautomata-hive-3.9.0/hive/cookbook/customers.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/dashboards.py` & `xautomata-hive-3.9.0/hive/cookbook/dashboards.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/dispatchers.py` & `xautomata-hive-3.9.0/hive/cookbook/dispatchers.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/downtimes.py` & `xautomata-hive-3.9.0/hive/cookbook/downtimes.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/external_tickets.py` & `xautomata-hive-3.9.0/hive/cookbook/external_tickets.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/firmware_updates.py` & `xautomata-hive-3.9.0/hive/cookbook/firmware_updates.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/google.py` & `xautomata-hive-3.9.0/hive/cookbook/google.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/groups.py` & `xautomata-hive-3.9.0/hive/cookbook/groups.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/last_status.py` & `xautomata-hive-3.9.0/hive/cookbook/last_status.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/login.py` & `xautomata-hive-3.9.0/hive/cookbook/login.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/messages.py` & `xautomata-hive-3.9.0/hive/cookbook/messages.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/metric_ingest.py` & `xautomata-hive-3.9.0/hive/cookbook/metric_ingest.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/metric_types.py` & `xautomata-hive-3.9.0/hive/cookbook/metric_types.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/metrics.py` & `xautomata-hive-3.9.0/hive/cookbook/metrics.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/microsoft.py` & `xautomata-hive-3.9.0/hive/cookbook/microsoft.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/notification_provider_types.py` & `xautomata-hive-3.9.0/hive/cookbook/notification_provider_types.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/notification_providers.py` & `xautomata-hive-3.9.0/hive/cookbook/notification_providers.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/objects.py` & `xautomata-hive-3.9.0/hive/cookbook/objects.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/opening_reasons.py` & `xautomata-hive-3.9.0/hive/cookbook/opening_reasons.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/probe_types.py` & `xautomata-hive-3.9.0/hive/cookbook/probe_types.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/probes.py` & `xautomata-hive-3.9.0/hive/cookbook/probes.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/probes_log_ingest.py` & `xautomata-hive-3.9.0/hive/cookbook/probes_log_ingest.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/profile_topics.py` & `xautomata-hive-3.9.0/hive/cookbook/profile_topics.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/reason_for_closure.py` & `xautomata-hive-3.9.0/hive/cookbook/reason_for_closure.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/retention_rules.py` & `xautomata-hive-3.9.0/hive/cookbook/retention_rules.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/schedules.py` & `xautomata-hive-3.9.0/hive/cookbook/schedules.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/services.py` & `xautomata-hive-3.9.0/hive/cookbook/services.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/sites.py` & `xautomata-hive-3.9.0/hive/cookbook/sites.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/tree_hierarchy.py` & `xautomata-hive-3.9.0/hive/cookbook/tree_hierarchy.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/ts_cost_azure_raw.py` & `xautomata-hive-3.9.0/hive/cookbook/ts_cost_azure_raw.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/ts_cost_management.py` & `xautomata-hive-3.9.0/hive/cookbook/ts_cost_management.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/ts_metric_status.py` & `xautomata-hive-3.9.0/hive/cookbook/ts_metric_status.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/ts_metric_value.py` & `xautomata-hive-3.9.0/hive/cookbook/ts_metric_value.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/ts_ntop_flows.py` & `xautomata-hive-3.9.0/hive/cookbook/ts_ntop_flows.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/ts_service_status.py` & `xautomata-hive-3.9.0/hive/cookbook/ts_service_status.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/ts_service_value.py` & `xautomata-hive-3.9.0/hive/cookbook/ts_service_value.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/users.py` & `xautomata-hive-3.9.0/hive/cookbook/users.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/users_notifications.py` & `xautomata-hive-3.9.0/hive/cookbook/users_notifications.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/virtual_domains.py` & `xautomata-hive-3.9.0/hive/cookbook/virtual_domains.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/webhooks.py` & `xautomata-hive-3.9.0/hive/cookbook/webhooks.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/widget_groups.py` & `xautomata-hive-3.9.0/hive/cookbook/widget_groups.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/cookbook/widgets.py` & `xautomata-hive-3.9.0/hive/cookbook/widgets.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/decorators.py` & `xautomata-hive-3.9.0/hive/decorators.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/hive/infrastrucure_keys.py` & `xautomata-hive-3.9.0/hive/infrastrucure_keys.py`

 * *Files identical despite different names*

### Comparing `xautomata-hive-3.8.1/setup.py` & `xautomata-hive-3.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         version.append(str(line.strip()))
 
 version = version[0].split("'")[1]
 
 # version go
 tqdm = 'tqdm==4.64.1'
 requests = 'requests==2.31.0'
-urllib3 = 'urllib3==2.0.4'
+urllib3 = 'urllib3==1.26.17'
 # version end
 
 setup(
     name='xautomata-hive',
     python_requires='>=3.8.0',
     version=version,
     packages=find_packages(include=['hive*']),
```

### Comparing `xautomata-hive-3.8.1/xautomata_hive.egg-info/PKG-INFO` & `xautomata-hive-3.9.0/xautomata_hive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: xautomata-hive
-Version: 3.8.1
+Version: 3.9.0
 Home-page: https://github.com/sherlogic/xautomata-hive.git
 Author: Enrico Ferro - Andrea Jacassi
 Author-email: 
 License: MIT
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: urllib3==2.0.4
+Requires-Dist: urllib3==1.26.17
 Requires-Dist: tqdm==4.64.1
 Requires-Dist: requests==2.31.0
 
 # Xautomata API
 Pacchetto che fornisca una interfaccia semplice per usare le API di Xautomata in python
 
 The full documentation can be fount at https://sherlogic.github.io/xautomata-hive/
```

### Comparing `xautomata-hive-3.8.1/xautomata_hive.egg-info/SOURCES.txt` & `xautomata-hive-3.9.0/xautomata_hive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

