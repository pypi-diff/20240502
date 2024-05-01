# Comparing `tmp/spaceone-inventory-2.0.dev98.tar.gz` & `tmp/spaceone-inventory-2.0.dev99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceone-inventory-2.0.dev98.tar", last modified: Mon Mar 25 08:57:02 2024, max compression
+gzip compressed data, was "spaceone-inventory-2.0.dev99.tar", last modified: Fri Apr 12 00:57:41 2024, max compression
```

## Comparing `spaceone-inventory-2.0.dev98.tar` & `spaceone-inventory-2.0.dev99.tar`

### file list

```diff
@@ -1,185 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.620000 spaceone-inventory-2.0.dev98/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-25 08:57:02.620000 spaceone-inventory-2.0.dev98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 08:57:02.620000 spaceone-inventory-2.0.dev98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.592000 spaceone-inventory-2.0.dev98/spaceone/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.592000 spaceone-inventory-2.0.dev98/spaceone/inventory/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.592000 spaceone-inventory-2.0.dev98/spaceone/inventory/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/conf/collector_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/conf/global_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.596000 spaceone-inventory-2.0.dev98/spaceone/inventory/connector/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/connector/file_upload_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/connector/smtp_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.596000 spaceone-inventory-2.0.dev98/spaceone/inventory/error/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/error/cloud_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/error/cloud_service_query_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/error/cloud_service_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/error/cloud_service_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/error/collect_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/error/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/error/collector_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/error/export.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/error/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/error/region.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/error/smtp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.600000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/change_history_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/cloud_service_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/cloud_service_query_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/cloud_service_report_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/cloud_service_stats_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/cloud_service_type_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/collector_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/collector_rule_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/common_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/job_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/job_task_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/note_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/info/region_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.600000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.600000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/change_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/cloud_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/cloud_service_query_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/cloud_service_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/cloud_service_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/cloud_service_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/collector_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/job_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/note.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/region.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.600000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.600000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/task/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/task/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/task/v1/cleanup_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/task/v1/cloud_service_stats_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/interface/task/v1/inventory_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.604000 spaceone-inventory-2.0.dev98/spaceone/inventory/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/lib/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/lib/job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/lib/job_task_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/lib/resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/lib/rule_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/lib/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.608000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/change_history_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/cleanup_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    21731 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/cloud_service_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    21069 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/cloud_service_query_set_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/cloud_service_report_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/cloud_service_stats_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/cloud_service_type_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18364 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/collecting_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/collection_state_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/collector_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/collector_plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/collector_rule_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.608000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/export_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/export_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/export_manager/email_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/identity_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/job_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/job_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/note_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/record_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/reference_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/region_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/repository_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/manager/secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.608000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/cloud_service_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/cloud_service_query_set_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/cloud_service_report_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/cloud_service_stats_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/cloud_service_type_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/collection_state_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/collector_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/collector_rule_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/job_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/job_task_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/note_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/record_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/reference_resource_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/model/region_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.608000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.608000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.612000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/conf/global_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.612000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/error/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/error/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.612000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.612000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/interface/grpc/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/interface/grpc/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.612000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/lib/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    17519 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/lib/metadata_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/lib/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.612000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/cloud_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/cloud_service_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/collector_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/collector_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/dynamic_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/field.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/job_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/job_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/region.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.616000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/service/collector_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/service/job_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.616000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/skeleton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/skeleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/skeleton/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.616000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/change_history_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/cleanup_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13884 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/cloud_service_query_set_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/cloud_service_report_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    21994 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/cloud_service_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/cloud_service_stats_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/cloud_service_type_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/collector_rule_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    30794 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/collector_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/job_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/job_task_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/note_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/service/region_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.616000 spaceone-inventory-2.0.dev98/spaceone/inventory/template/
--rw-r--r--   0 runner    (1001) docker     (127)    15018 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/template/report_download_en.html
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/template/report_download_jp.html
--rw-r--r--   0 runner    (1001) docker     (127)    15079 2024-03-25 08:56:53.000000 spaceone-inventory-2.0.dev98/spaceone/inventory/template/report_download_ko.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 08:57:02.620000 spaceone-inventory-2.0.dev98/spaceone_inventory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-03-25 08:57:02.000000 spaceone-inventory-2.0.dev98/spaceone_inventory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-03-25 08:57:02.000000 spaceone-inventory-2.0.dev98/spaceone_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 08:57:02.000000 spaceone-inventory-2.0.dev98/spaceone_inventory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 08:57:02.000000 spaceone-inventory-2.0.dev98/spaceone_inventory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-25 08:57:02.000000 spaceone-inventory-2.0.dev98/spaceone_inventory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-25 08:57:02.000000 spaceone-inventory-2.0.dev98/spaceone_inventory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.373657 spaceone-inventory-2.0.dev99/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-12 00:57:41.373657 spaceone-inventory-2.0.dev99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 00:57:41.373657 spaceone-inventory-2.0.dev99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.345657 spaceone-inventory-2.0.dev99/spaceone/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.345657 spaceone-inventory-2.0.dev99/spaceone/inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.345657 spaceone-inventory-2.0.dev99/spaceone/inventory/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/conf/collector_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/conf/global_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.345657 spaceone-inventory-2.0.dev99/spaceone/inventory/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/connector/file_upload_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/connector/smtp_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.349657 spaceone-inventory-2.0.dev99/spaceone/inventory/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/error/cloud_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/error/cloud_service_query_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/error/cloud_service_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/error/cloud_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/error/collect_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/error/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/error/collector_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/error/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/error/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/error/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/error/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/error/smtp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.349657 spaceone-inventory-2.0.dev99/spaceone/inventory/info/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/info/change_history_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/info/cloud_service_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/info/cloud_service_query_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/info/cloud_service_report_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/info/cloud_service_stats_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/info/cloud_service_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/info/collector_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/info/collector_rule_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/info/common_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/info/job_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/info/job_task_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/info/note_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/info/region_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.349657 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.353657 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/change_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/cloud_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/cloud_service_query_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/cloud_service_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/cloud_service_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/cloud_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/collector_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/job_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/metric_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/region.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.353657 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.353657 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/task/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/task/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/task/v1/cleanup_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/task/v1/cloud_service_stats_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/interface/task/v1/inventory_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.353657 spaceone-inventory-2.0.dev99/spaceone/inventory/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/lib/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/lib/job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/lib/job_task_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/lib/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/lib/rule_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/lib/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.341657 spaceone-inventory-2.0.dev99/spaceone/inventory/managed_resource/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.357657 spaceone-inventory-2.0.dev99/spaceone/inventory/managed_resource/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/managed_resource/metric/created_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/managed_resource/metric/database_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/managed_resource/metric/deleted_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/managed_resource/metric/server_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/managed_resource/metric/storage_size.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.357657 spaceone-inventory-2.0.dev99/spaceone/inventory/managed_resource/namespace/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/managed_resource/namespace/asset_summary.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/managed_resource/namespace/job_history.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.361657 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/change_history_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/cleanup_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21731 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/cloud_service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21069 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/cloud_service_query_set_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/cloud_service_report_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/cloud_service_stats_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/cloud_service_type_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18364 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/collecting_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/collection_state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/collector_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/collector_plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/collector_rule_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.361657 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/export_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/export_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/export_manager/email_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/identity_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/job_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/managed_resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10418 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/metric_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/metric_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/namespace_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/note_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/record_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/reference_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/region_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/repository_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/manager/secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.361657 spaceone-inventory-2.0.dev99/spaceone/inventory/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/cloud_service_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/cloud_service_query_set_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/cloud_service_report_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/cloud_service_stats_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/cloud_service_type_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/collection_state_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/collector_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/collector_rule_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/job_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/job_task_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/note_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/record_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/reference_resource_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/model/region_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.361657 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.361657 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.361657 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/conf/global_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.365657 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/error/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/error/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.365657 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.365657 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/interface/grpc/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/interface/grpc/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.365657 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/lib/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17519 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/lib/metadata_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/lib/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.365657 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/cloud_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/cloud_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/collector_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/collector_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/dynamic_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/job_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/job_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/region.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.365657 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/service/collector_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/service/job_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.369657 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/skeleton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/skeleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/skeleton/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.369657 spaceone-inventory-2.0.dev99/spaceone/inventory/service/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/change_history_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/cleanup_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13884 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/cloud_service_query_set_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/cloud_service_report_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21994 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/cloud_service_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/cloud_service_stats_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/cloud_service_type_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/collector_rule_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30794 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/collector_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/job_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/job_task_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/metric_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/metric_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/namespace_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/note_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/service/region_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.369657 spaceone-inventory-2.0.dev99/spaceone/inventory/template/
+-rw-r--r--   0 runner    (1001) docker     (127)    15018 2024-04-12 00:57:31.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/template/report_download_en.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-12 00:57:32.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/template/report_download_jp.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15079 2024-04-12 00:57:32.000000 spaceone-inventory-2.0.dev99/spaceone/inventory/template/report_download_ko.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:57:41.373657 spaceone-inventory-2.0.dev99/spaceone_inventory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-12 00:57:41.000000 spaceone-inventory-2.0.dev99/spaceone_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-12 00:57:41.000000 spaceone-inventory-2.0.dev99/spaceone_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 00:57:41.000000 spaceone-inventory-2.0.dev99/spaceone_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 00:57:41.000000 spaceone-inventory-2.0.dev99/spaceone_inventory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 00:57:41.000000 spaceone-inventory-2.0.dev99/spaceone_inventory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 00:57:41.000000 spaceone-inventory-2.0.dev99/spaceone_inventory.egg-info/top_level.txt
```

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/conf/collector_conf.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/conf/collector_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/conf/global_conf.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/connector/file_upload_connector.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/connector/file_upload_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/connector/smtp_connector.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/connector/smtp_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/error/__init__.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/error/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/error/collector.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/error/collector.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/info/__init__.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/info/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/info/change_history_info.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/info/change_history_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/info/cloud_service_info.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/info/cloud_service_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/info/cloud_service_query_set_info.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/info/cloud_service_query_set_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/info/cloud_service_report_info.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/info/cloud_service_report_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/info/cloud_service_stats_info.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/info/cloud_service_stats_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/info/cloud_service_type_info.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/info/cloud_service_type_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/info/collector_info.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/info/collector_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/info/collector_rule_info.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/info/collector_rule_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/info/job_info.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/info/job_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/info/job_task_info.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/info/job_task_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/info/note_info.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/info/note_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/info/region_info.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/info/region_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/__init__.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from .job import Job
 from .job_task import JobTask
 from .change_history import ChangeHistory
 from .note import Note
 from .cloud_service_report import CloudServiceReport
 from .cloud_service_query_set import CloudServiceQuerySet
 from .cloud_service_stats import CloudServiceStats
+from .namespace import Namespace
+from .metric import Metric
+from .metric_data import MetricData
 
 _all_ = ["app"]
 
 app = GRPCServer()
 app.add_service(Region)
 app.add_service(CloudServiceType)
 app.add_service(CloudService)
@@ -23,7 +26,10 @@
 app.add_service(Job)
 app.add_service(JobTask)
 app.add_service(ChangeHistory)
 app.add_service(Note)
 app.add_service(CloudServiceReport)
 app.add_service(CloudServiceQuerySet)
 app.add_service(CloudServiceStats)
+app.add_service(Namespace)
+app.add_service(Metric)
+app.add_service(MetricData)
```

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/change_history.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/change_history.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/cloud_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/cloud_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/cloud_service_query_set.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/cloud_service_query_set.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/cloud_service_report.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/cloud_service_report.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/cloud_service_stats.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/cloud_service_stats.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/cloud_service_type.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/cloud_service_type.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/collector.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/collector.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/collector_rule.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/collector_rule.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/job.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/job.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/job_task.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/job_task.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/note.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/note.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/grpc/region.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/grpc/region.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/task/v1/cleanup_scheduler.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/task/v1/cleanup_scheduler.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/task/v1/cloud_service_stats_scheduler.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/task/v1/cloud_service_stats_scheduler.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/interface/task/v1/inventory_scheduler.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/interface/task/v1/inventory_scheduler.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/lib/ip_address.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/lib/ip_address.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/lib/job_state.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/lib/job_state.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/lib/job_task_state.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/lib/job_task_state.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/lib/resource_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/lib/resource_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/lib/rule_matcher.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/lib/rule_matcher.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/lib/scheduler.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/lib/scheduler.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/__init__.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/change_history_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/change_history_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/cleanup_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/cleanup_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/cloud_service_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/cloud_service_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/cloud_service_query_set_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/cloud_service_query_set_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/cloud_service_report_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/cloud_service_report_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/cloud_service_stats_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/cloud_service_stats_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/cloud_service_type_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/cloud_service_type_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/collecting_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/collecting_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/collection_state_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/collection_state_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/collector_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/collector_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/collector_plugin_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/collector_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/collector_rule_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/collector_rule_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/export_manager/__init__.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/export_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/export_manager/email_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/export_manager/email_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/file_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/identity_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/identity_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/job_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/job_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/job_task_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/job_task_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/note_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/note_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/plugin_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/record_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/record_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/reference_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/reference_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/region_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/region_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/repository_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/repository_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/manager/secret_manager.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/manager/secret_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/model/__init__.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/model/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,7 +12,14 @@
     CloudServiceStatsQueryHistory,
 )
 from spaceone.inventory.model.collection_state_model import CollectionState
 from spaceone.inventory.model.reference_resource_model import ReferenceResource
 from spaceone.inventory.model.record_model import Record
 from spaceone.inventory.model.note_model import Note
 from spaceone.inventory.model.collector_rule_model import CollectorRule
+from spaceone.inventory.model.namespace.database import Namespace
+from spaceone.inventory.model.metric.database import Metric
+from spaceone.inventory.model.metric_data.database import (
+    MetricData,
+    MonthlyMetricData,
+    MetricDataQueryHistory,
+)
```

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/model/cloud_service_model.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/model/cloud_service_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/model/cloud_service_query_set_model.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/model/cloud_service_query_set_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/model/cloud_service_report_model.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/model/cloud_service_report_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/model/cloud_service_stats_model.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/model/cloud_service_stats_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/model/cloud_service_type_model.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/model/cloud_service_type_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/model/collection_state_model.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/model/collection_state_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/model/collector_model.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/model/collector_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/model/collector_rule_model.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/model/collector_rule_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/model/job_model.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/model/job_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/model/job_task_model.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/model/job_task_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/model/note_model.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/model/note_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/model/record_model.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/model/record_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/model/region_model.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/model/region_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/error/response.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/error/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/interface/grpc/collector.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/interface/grpc/collector.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/interface/grpc/job.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/interface/grpc/job.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/lib/metadata.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/lib/metadata.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/lib/metadata_generator.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/lib/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/lib/server.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/lib/server.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/lib/utils.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/lib/utils.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/__init__.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/cloud_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/cloud_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/collector_request.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/collector_request.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/collector_response.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/collector_response.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/model/field.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/model/field.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/service/collector_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/service/collector_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/service/job_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/service/job_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/plugin/collector/skeleton/main.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/plugin/collector/skeleton/main.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/service/__init__.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/service/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/service/change_history_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/service/change_history_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/service/cleanup_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/service/cleanup_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/service/cloud_service_query_set_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/service/cloud_service_query_set_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/service/cloud_service_report_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/service/cloud_service_report_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/service/cloud_service_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/service/cloud_service_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/service/cloud_service_stats_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/service/cloud_service_stats_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/service/cloud_service_type_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/service/cloud_service_type_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/service/collector_rule_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/service/collector_rule_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/service/collector_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/service/collector_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/service/job_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/service/job_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/service/job_task_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/service/job_task_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/service/note_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/service/note_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/service/region_service.py` & `spaceone-inventory-2.0.dev99/spaceone/inventory/service/region_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/template/report_download_en.html` & `spaceone-inventory-2.0.dev99/spaceone/inventory/template/report_download_en.html`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/template/report_download_jp.html` & `spaceone-inventory-2.0.dev99/spaceone/inventory/template/report_download_jp.html`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone/inventory/template/report_download_ko.html` & `spaceone-inventory-2.0.dev99/spaceone/inventory/template/report_download_ko.html`

 * *Files identical despite different names*

### Comparing `spaceone-inventory-2.0.dev98/spaceone_inventory.egg-info/SOURCES.txt` & `spaceone-inventory-2.0.dev99/spaceone_inventory.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 spaceone/inventory/error/cloud_service_stats.py
 spaceone/inventory/error/cloud_service_type.py
 spaceone/inventory/error/collect_data.py
 spaceone/inventory/error/collector.py
 spaceone/inventory/error/collector_rule.py
 spaceone/inventory/error/export.py
 spaceone/inventory/error/file_upload.py
+spaceone/inventory/error/metric.py
 spaceone/inventory/error/region.py
 spaceone/inventory/error/smtp.py
 spaceone/inventory/info/__init__.py
 spaceone/inventory/info/change_history_info.py
 spaceone/inventory/info/cloud_service_info.py
 spaceone/inventory/info/cloud_service_query_set_info.py
 spaceone/inventory/info/cloud_service_report_info.py
@@ -41,28 +42,38 @@
 spaceone/inventory/interface/grpc/cloud_service_report.py
 spaceone/inventory/interface/grpc/cloud_service_stats.py
 spaceone/inventory/interface/grpc/cloud_service_type.py
 spaceone/inventory/interface/grpc/collector.py
 spaceone/inventory/interface/grpc/collector_rule.py
 spaceone/inventory/interface/grpc/job.py
 spaceone/inventory/interface/grpc/job_task.py
+spaceone/inventory/interface/grpc/metric.py
+spaceone/inventory/interface/grpc/metric_data.py
+spaceone/inventory/interface/grpc/namespace.py
 spaceone/inventory/interface/grpc/note.py
 spaceone/inventory/interface/grpc/region.py
 spaceone/inventory/interface/task/__init__.py
 spaceone/inventory/interface/task/v1/__init__.py
 spaceone/inventory/interface/task/v1/cleanup_scheduler.py
 spaceone/inventory/interface/task/v1/cloud_service_stats_scheduler.py
 spaceone/inventory/interface/task/v1/inventory_scheduler.py
 spaceone/inventory/lib/__init__.py
 spaceone/inventory/lib/ip_address.py
 spaceone/inventory/lib/job_state.py
 spaceone/inventory/lib/job_task_state.py
 spaceone/inventory/lib/resource_manager.py
 spaceone/inventory/lib/rule_matcher.py
 spaceone/inventory/lib/scheduler.py
+spaceone/inventory/managed_resource/metric/created_count.yaml
+spaceone/inventory/managed_resource/metric/database_count.yaml
+spaceone/inventory/managed_resource/metric/deleted_count.yaml
+spaceone/inventory/managed_resource/metric/server_count.yaml
+spaceone/inventory/managed_resource/metric/storage_size.yaml
+spaceone/inventory/managed_resource/namespace/asset_summary.yaml
+spaceone/inventory/managed_resource/namespace/job_history.yaml
 spaceone/inventory/manager/__init__.py
 spaceone/inventory/manager/change_history_manager.py
 spaceone/inventory/manager/cleanup_manager.py
 spaceone/inventory/manager/cloud_service_manager.py
 spaceone/inventory/manager/cloud_service_query_set_manager.py
 spaceone/inventory/manager/cloud_service_report_manager.py
 spaceone/inventory/manager/cloud_service_stats_manager.py
@@ -72,14 +83,18 @@
 spaceone/inventory/manager/collector_manager.py
 spaceone/inventory/manager/collector_plugin_manager.py
 spaceone/inventory/manager/collector_rule_manager.py
 spaceone/inventory/manager/file_manager.py
 spaceone/inventory/manager/identity_manager.py
 spaceone/inventory/manager/job_manager.py
 spaceone/inventory/manager/job_task_manager.py
+spaceone/inventory/manager/managed_resource_manager.py
+spaceone/inventory/manager/metric_data_manager.py
+spaceone/inventory/manager/metric_manager.py
+spaceone/inventory/manager/namespace_manager.py
 spaceone/inventory/manager/note_manager.py
 spaceone/inventory/manager/plugin_manager.py
 spaceone/inventory/manager/record_manager.py
 spaceone/inventory/manager/reference_manager.py
 spaceone/inventory/manager/region_manager.py
 spaceone/inventory/manager/repository_manager.py
 spaceone/inventory/manager/secret_manager.py
@@ -138,14 +153,17 @@
 spaceone/inventory/service/cloud_service_service.py
 spaceone/inventory/service/cloud_service_stats_service.py
 spaceone/inventory/service/cloud_service_type_service.py
 spaceone/inventory/service/collector_rule_service.py
 spaceone/inventory/service/collector_service.py
 spaceone/inventory/service/job_service.py
 spaceone/inventory/service/job_task_service.py
+spaceone/inventory/service/metric_data_service.py
+spaceone/inventory/service/metric_service.py
+spaceone/inventory/service/namespace_service.py
 spaceone/inventory/service/note_service.py
 spaceone/inventory/service/region_service.py
 spaceone/inventory/template/report_download_en.html
 spaceone/inventory/template/report_download_jp.html
 spaceone/inventory/template/report_download_ko.html
 spaceone_inventory.egg-info/PKG-INFO
 spaceone_inventory.egg-info/SOURCES.txt
```

