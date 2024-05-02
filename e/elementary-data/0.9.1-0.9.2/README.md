# Comparing `tmp/elementary-data-0.9.1.tar.gz` & `tmp/elementary-data-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/elementary/elementary/dist/.tmp-v66we379/elementary-data-0.9.1.tar", last modified: Thu Jul 20 13:03:13 2023, max compression
+gzip compressed data, was "/home/runner/work/elementary/elementary/dist/.tmp-ml2ahzek/elementary-data-0.9.2.tar", last modified: Mon Jul 31 12:18:50 2023, max compression
```

## Comparing `elementary-data-0.9.1.tar` & `elementary-data-0.9.2.tar`

### file list

```diff
@@ -1,303 +1,303 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-07-20 13:02:53.000000 elementary-data-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-07-20 13:02:53.000000 elementary-data-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    15119 2023-07-20 13:03:13.000000 elementary-data-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14240 2023-07-20 13:02:53.000000 elementary-data-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/cli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/cli/upgrade.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/clients/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/clients/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      489 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/api/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/clients/dbt/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/dbt/base_dbt_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/dbt/dbt_log.py
--rw-r--r--   0 runner    (1001) docker     (122)     8424 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/dbt/dbt_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     7780 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/dbt/slim_dbt_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/clients/fetcher/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/fetcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/fetcher/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/clients/gcs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3765 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/gcs/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/clients/s3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5613 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/s3/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/clients/slack/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8288 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/slack/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/slack/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/clients/slack/slack_message_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/config/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8170 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/exceptions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5214 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7634 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/alerts/alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/alerts/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)    13504 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/alerts/group_of_alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     1653 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/alerts/malformed.py
--rw-r--r--   0 runner    (1001) docker     (122)     7559 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/alerts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/alerts/schema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/alerts/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/alerts/schema/alert.py
--rw-r--r--   0 runner    (1001) docker     (122)      418 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/alerts/schema/alert_group_component.py
--rw-r--r--   0 runner    (1001) docker     (122)      487 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/alerts/schema/test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6275 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/alerts/source_freshness.py
--rw-r--r--   0 runner    (1001) docker     (122)    15928 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/alerts/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/alerts/alert_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     8554 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/alerts/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/api/filters/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4252 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/filters/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/filters/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/api/groups/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3685 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/groups/groups.py
--rw-r--r--   0 runner    (1001) docker     (122)      447 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/groups/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/api/invocations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/invocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/invocations/invocations.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/invocations/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/api/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/lineage/lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/lineage/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/api/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10013 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/models/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2672 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/models/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/api/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7891 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/report/report.py
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/report/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/api/selector/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/selector/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/selector/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/api/test_management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/test_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/test_management/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/test_management/test_management.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)    20989 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/api/totals_schema.py
--rw-r--r--   0 runner    (1001) docker     (122)    20225 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/data_monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/data_monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7919 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/data_monitoring/data_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    10682 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/data_monitoring/data_monitoring_alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/data_monitoring/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/data_monitoring/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11902 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/data_monitoring/report/data_monitoring_report.py
--rw-r--r--   0 runner    (1001) docker     (122)  1791216 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/data_monitoring/report/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     7912 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/data_monitoring/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     4354 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/data_monitoring/selector_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      571 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql
--rw-r--r--   0 runner    (1001) docker     (122)     6956 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql
--rw-r--r--   0 runner    (1001) docker     (122)     6387 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)     7562 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      611 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/base_queries/
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/base_queries/owners.sql
--rw-r--r--   0 runner    (1001) docker     (122)     3606 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/base_queries/resources.sql
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/base_queries/tags.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/base_queries/tests.sql
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_adapter_type_and_unique_id.sql
--rw-r--r--   0 runner    (1001) docker     (122)      305 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_alerts_time_limit.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_elementary_database_and_schema.sql
--rw-r--r--   0 runner    (1001) docker     (122)      324 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_elementary_table_nodes.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_exposures.sql
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_invocations_by_ids.sql
--rw-r--r--   0 runner    (1001) docker     (122)      678 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_latest_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_models.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_models_runs.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_resources_latest_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_result_rows_agate.sql
--rw-r--r--   0 runner    (1001) docker     (122)      991 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_sources.sql
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql
--rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_test_results.sql
--rw-r--r--   0 runner    (1001) docker     (122)      683 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/internal_tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/internal_tests/validate_alert_statuses_are_updated.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (122)      494 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/materializations/nothing.sql
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/test_conn.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/tests/unique_if_exists.sql
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/macros/upload_source_freshness.sql
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/models/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/models/alerts/alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/models/alerts/alerts_models.sql
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/models/elementary.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/models/update_alerts/
--rw-r--r--   0 runner    (1001) docker     (122)      300 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/models/update_alerts/update_sent_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/models/update_alerts/update_skipped_alerts.sql
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/packages.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/dbt_project_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/fetchers/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6201 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/alerts/alerts.py
--rw-r--r--   0 runner    (1001) docker     (122)     5356 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/alerts/normalized_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/base_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/fetchers/invocations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/invocations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/invocations/invocations.py
--rw-r--r--   0 runner    (1001) docker     (122)      906 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/invocations/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/fetchers/lineage/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/lineage/lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/lineage/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/fetchers/models/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/models/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/models/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/fetchers/selector/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/selector/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/selector/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/fetchers/test_management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/test_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/test_management/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     8086 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/test_management/test_management.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/monitor/fetchers/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/tests/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/monitor/fetchers/tests/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/operations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/operations/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/operations/upload_source_freshness.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/tracking/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4598 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/tracking/anonymous_tracking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/tracking/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/tracking/tracking_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/utils/bucket_path.py
--rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/utils/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/utils/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (122)     2281 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (122)      201 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/utils/ordered_yaml.py
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/utils/package.py
--rw-r--r--   0 runner    (1001) docker     (122)      865 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-07-20 13:02:53.000000 elementary-data-0.9.1/elementary/utils/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15119 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10508 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-20 13:03:12.000000 elementary-data-0.9.1/elementary_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 13:03:13.000000 elementary-data-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-07-20 13:02:53.000000 elementary-data-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/tests/integration/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/integration/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/tests/integration/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/integration/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:12.000000 elementary-data-0.9.1/tests/integration/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/integration/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/integration/monitor/api/alerts/test_alerts_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/tests/integration/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/integration/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/integration/monitor/api/tests/test_tests_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/mocks/anonymous_tracking_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/tests/mocks/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/mocks/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/mocks/api/alerts_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/mocks/api/invocations_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/mocks/api/tests_api_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/mocks/dbt_runner_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/tests/mocks/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/mocks/fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19060 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/mocks/fetchers/alerts_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/mocks/fetchers/invocations_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/mocks/fetchers/selector_fetcher_mock.py
--rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/mocks/fetchers/tests_fetcher_mock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/tests/unit/monitor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/tests/unit/monitor/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/alerts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/tests/unit/monitor/alerts/group_alerts_by_table/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/alerts/group_alerts_by_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    12751 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/alerts/group_alerts_by_table/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/alerts/test_malformed_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     8238 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/alerts/test_normalized_alert.py
--rw-r--r--   0 runner    (1001) docker     (122)     7342 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/alerts/test_slack_alert_message_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/tests/unit/monitor/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/tests/unit/monitor/api/alerts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/api/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12260 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/api/alerts/test_alert_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/api/alerts/test_alerts_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/tests/unit/monitor/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/api/tests/test_tests_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/tests/unit/monitor/data_monitoring/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/data_monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/tests/unit/monitor/data_monitoring/report/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/data_monitoring/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7890 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py
--rw-r--r--   0 runner    (1001) docker     (122)     5152 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/data_monitoring/test_selector_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 13:03:13.000000 elementary-data-0.9.1/tests/unit/monitor/fetchers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2536 2023-07-20 13:02:53.000000 elementary-data-0.9.1/tests/unit/monitor/fetchers/test_alerts_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-07-31 12:18:30.000000 elementary-data-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-07-31 12:18:30.000000 elementary-data-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15201 2023-07-31 12:18:50.000000 elementary-data-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14322 2023-07-31 12:18:30.000000 elementary-data-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/cli/upgrade.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/clients/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/api/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/clients/dbt/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/dbt/base_dbt_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/dbt/dbt_log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8543 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/dbt/dbt_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7780 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/dbt/slim_dbt_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/clients/fetcher/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/fetcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/fetcher/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/clients/gcs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3765 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/gcs/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/clients/s3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5613 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/s3/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/clients/slack/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8288 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/slack/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/slack/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5731 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/clients/slack/slack_message_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/config/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8170 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5214 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7675 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/alerts/alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/alerts/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14113 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/alerts/group_of_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1653 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/alerts/malformed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7559 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/alerts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/alerts/schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/alerts/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/alerts/schema/alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      418 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/alerts/schema/alert_group_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/alerts/schema/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6275 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/alerts/source_freshness.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15928 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/alerts/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5596 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/alerts/alert_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8731 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/alerts/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/api/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4252 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/filters/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/filters/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/api/groups/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3685 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/groups/groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/groups/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/api/invocations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/invocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/invocations/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/invocations/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/api/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/lineage/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/lineage/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10013 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2672 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/models/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/api/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7891 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/report/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/api/selector/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/selector/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/selector/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/api/test_management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/test_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/test_management/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1463 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/test_management/test_management.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21047 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/api/totals_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20656 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/data_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/data_monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7733 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/data_monitoring/data_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10955 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/data_monitoring/data_monitoring_alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/data_monitoring/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/data_monitoring/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11902 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/data_monitoring/report/data_monitoring_report.py
+-rw-r--r--   0 runner    (1001) docker     (122)  1791216 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/data_monitoring/report/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     7912 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2813 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/data_monitoring/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5647 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/data_monitoring/selector_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6956 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     6387 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     7562 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/base_queries/
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/base_queries/owners.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     3606 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/base_queries/resources.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/base_queries/tags.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/base_queries/tests.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_adapter_type_and_unique_id.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      305 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_alerts_time_limit.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_elementary_database_and_schema.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      324 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_elementary_table_nodes.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1190 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_exposures.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      872 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_invocations_by_ids.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_latest_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1129 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_models.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_models_runs.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_resources_latest_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_result_rows_agate.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_sources.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql
+-rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_test_results.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      683 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/internal_tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/internal_tests/validate_alert_statuses_are_updated.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/materializations/nothing.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/test_conn.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/tests/unique_if_exists.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/macros/upload_source_freshness.sql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/models/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/models/alerts/alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/models/alerts/alerts_models.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/models/elementary.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/models/update_alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/models/update_alerts/update_sent_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/models/update_alerts/update_skipped_alerts.sql
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/packages.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/dbt_project_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/fetchers/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6201 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/alerts/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5356 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/alerts/normalized_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/base_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/fetchers/invocations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/invocations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/invocations/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      906 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/invocations/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/fetchers/lineage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/lineage/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1057 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/lineage/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/fetchers/models/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2646 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2553 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/models/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/fetchers/selector/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/selector/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/selector/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/fetchers/test_management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/test_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2251 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/test_management/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8086 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/test_management/test_management.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/monitor/fetchers/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/tests/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/monitor/fetchers/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/operations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/operations/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2589 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/operations/upload_source_freshness.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/tracking/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4598 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/tracking/anonymous_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/tracking/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/tracking/tracking_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/utils/bucket_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/utils/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/utils/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2281 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/utils/ordered_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/utils/package.py
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2748 2023-07-31 12:18:30.000000 elementary-data-0.9.2/elementary/utils/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15201 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10508 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-31 12:18:50.000000 elementary-data-0.9.2/elementary_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-31 12:18:50.000000 elementary-data-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-07-31 12:18:30.000000 elementary-data-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/integration/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/integration/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/integration/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/integration/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/integration/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/integration/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1764 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/integration/monitor/api/alerts/test_alerts_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/integration/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/integration/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/integration/monitor/api/tests/test_tests_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/mocks/anonymous_tracking_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/mocks/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/mocks/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/mocks/api/alerts_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/mocks/api/invocations_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/mocks/api/tests_api_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/mocks/dbt_runner_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/mocks/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/mocks/fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19060 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/mocks/fetchers/alerts_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/mocks/fetchers/invocations_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/mocks/fetchers/selector_fetcher_mock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8394 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/mocks/fetchers/tests_fetcher_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/unit/monitor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/unit/monitor/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/alerts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/unit/monitor/alerts/group_alerts_by_table/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/alerts/group_alerts_by_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3274 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14074 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/alerts/group_alerts_by_table/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      927 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/alerts/test_malformed_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8238 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/alerts/test_normalized_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7342 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/alerts/test_slack_alert_message_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/unit/monitor/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/unit/monitor/api/alerts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/api/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14673 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/api/alerts/test_alert_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2982 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/api/alerts/test_alerts_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/unit/monitor/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/api/tests/test_tests_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/unit/monitor/data_monitoring/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/data_monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/unit/monitor/data_monitoring/report/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/data_monitoring/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7890 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6057 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/data_monitoring/test_selector_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:50.000000 elementary-data-0.9.2/tests/unit/monitor/fetchers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2536 2023-07-31 12:18:30.000000 elementary-data-0.9.2/tests/unit/monitor/fetchers/test_alerts_fetcher.py
```

### Comparing `elementary-data-0.9.1/LICENSE` & `elementary-data-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/PKG-INFO` & `elementary-data-0.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementary-data
-Version: 0.9.1
+Version: 0.9.2
 Summary: Data monitoring and lineage
 Home-page: https://github.com/elementary-data/elementary
 Author: Elementary
 Author-email: or@elementary-data.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
@@ -21,19 +21,19 @@
 Provides-Extra: postgres
 Provides-Extra: databricks
 Provides-Extra: spark
 Provides-Extra: all
 License-File: LICENSE
 
 <p align="center">
-<img alt="Logo" src="static/header_git.png"/ width="1000">
+<img alt="Logo" src="static/github_banner.png"/ width="1000">
 </p>
 
 <h2 align="center">
- Data observability for analytics & data engineers
+ dbt native data observability for analytics & data engineers
 </h2>
 <h4 align="center">
 Monitor your data quality, operation and performance directly from your dbt project.
 </h4>
 
 <p align="center">
 <a href="https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg"><img src="https://img.shields.io/badge/join-Slack-ff69b4"/></a>
@@ -49,98 +49,89 @@
 
 </div>
 
 ## What is Elementary?
 
 Elementary is an open-source data observability solution, built for dbt users. Setup in minutes, gain immediate visibility, detect data issues, send actionable alerts, and understand impact and root cause.
 
-
 <kbd align="center">
         <a href="https://storage.googleapis.com/elementary_static/elementary_demo.html"><img align="center" style="max-width:300px;" src="static/report_ui.gif"> </a>
 </kbd>
 
 <br>
 
 ## Quick start
 
-Step 1 - [Install Elementary dbt package](https://docs.elementary-data.com/quickstart) 
+Step 1 - [Install Elementary dbt package](https://docs.elementary-data.com/quickstart)
 
 Step 2 - [Install Elementary CLI](https://docs.elementary-data.com/quickstart-cli)
 
-   
 ## Features
 
+<img src="static/happy_fire.ico" width="16"/> **Data observability report** - Generate a data observability report, host it or share with your team.
 
- <img src="static/elementary_icon.ico" width="16"/> **Data observability report** - Generate a data observability report, host it or share with your team.
-
- <img src="static/elementary_icon.ico" width="16"/> **Anomaly detection dbt tests** - Collect data quality metrics and detect anomalies, as native dbt tests.
-
- <img src="static/elementary_icon.ico" width="16"/> **Test results** - Enriched with details for fast triage of issues.
+<img src="static/happy_fire.ico" width="16"/> **Anomaly detection dbt tests** - Collect data quality metrics and detect anomalies, as native dbt tests.
 
- <img src="static/elementary_icon.ico" width="16"/> **Models performance** - Visibility of execution times, easy detection of degradation and bottlenecks.
+<img src="static/happy_fire.ico" width="16"/> **Test results** - Enriched with details for fast triage of issues.
 
- <img src="static/elementary_icon.ico" width="16"/> **Data lineage** - Enriched with test results, easy to navigate and filter.
+<img src="static/happy_fire.ico" width="16"/> **Models performance** - Visibility of execution times, easy detection of degradation and bottlenecks.
 
- <img src="static/elementary_icon.ico" width="16"/> **dbt artifacts uploader** - Save metadata and run results as part of your dbt runs. 
+<img src="static/happy_fire.ico" width="16"/> **Data lineage** - Enriched with test results, easy to navigate and filter.
 
- <img src="static/elementary_icon.ico" width="16"/> **Slack alerts** - Actionable alerts, including custom channels and tagging of owners and subscribers.
+<img src="static/happy_fire.ico" width="16"/> **dbt artifacts uploader** - Save metadata and run results as part of your dbt runs.
 
+<img src="static/happy_fire.ico" width="16"/> **Slack alerts** - Actionable alerts, including custom channels and tagging of owners and subscribers.
 
 ##
- 
+
 Join [Slack](https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) to learn more on Elementary.
 
 Our full documentation is [available here](https://docs.elementary-data.com/).
 
-
 ## How it works?
 
-Elementary [dbt package](https://github.com/elementary-data/dbt-data-reliability) creates tables of metadata and test results in your data warehouse, as part of your dbt runs. The CLI tool reads the data from these tables, and is used to generate the UI and alerts. 
+Elementary [dbt package](https://github.com/elementary-data/dbt-data-reliability) creates tables of metadata and test results in your data warehouse, as part of your dbt runs. The CLI tool reads the data from these tables, and is used to generate the UI and alerts.
 
 <img align="center" style="max-width:300px;" src="static/how_elementary_works.png">
 
 ## Community & Support
 
 For additional information and help, you can use one of these channels:
 
-* [Slack](https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) \(Live chat with the team, support, discussions, etc.\)
-* [GitHub issues](https://github.com/elementary-data/elementary/issues) \(Bug reports, feature requests)
-* [Twitter](https://twitter.com/ElementaryData) \(Updates on new releases and stuff)
-
+- [Slack](https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) \(Live chat with the team, support, discussions, etc.\)
+- [GitHub issues](https://github.com/elementary-data/elementary/issues) \(Bug reports, feature requests)
+- [Twitter](https://twitter.com/ElementaryData) \(Updates on new releases and stuff)
 
 ## **Integrations**
 
-* [x] **dbt core (>=1.0.0)** ![](static/dbt-16.png)
-* [x] **dbt cloud**  ![](static/dbt-16.png)
+- [x] **dbt core (>=1.0.0)** ![](static/dbt-16.png)
+- [x] **dbt cloud** ![](static/dbt-16.png)
 
 **Data warehouses:**
-* [x] **Snowflake** ![](static/snowflake-16.png) 
-* [x] **BigQuery**  ![](static/bigquery-16.svg) 
-* [x] **Redshift**  ![](static/redshift-16.png)
-* [x] **Databricks SQL**  ![](static/databricks-16.png)
-* [x] **Postgres**  ![](static/postgres-16.png)
 
-**Operations:**
-
-* [x] **Slack** ![](static/slack-16.png)
-* [x] **GitHub Actions**  ![](static/github-actions-16.png)
-* [x] **Amazon S3**  ![](static/s3-16.svg)
-* [x] **Google Cloud Storage**  ![](static/gcs-16.png)
+- [x] **Snowflake** ![](static/snowflake-16.png)
+- [x] **BigQuery** ![](static/bigquery-16.svg)
+- [x] **Redshift** ![](static/redshift-16.png)
+- [x] **Databricks SQL** ![](static/databricks-16.png)
+- [x] **Postgres** ![](static/postgres-16.png)
 
+**Operations:**
 
+- [x] **Slack** ![](static/slack-16.png)
+- [x] **GitHub Actions** ![](static/github-actions-16.png)
+- [x] **Amazon S3** ![](static/s3-16.svg)
+- [x] **Google Cloud Storage** ![](static/gcs-16.png)
 
 Ask us for integrations on [Slack](https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) or as a [GitHub issue](https://github.com/elementary-data/elementary-lineage/issues/new).
 
-
 ## **Contributions**
 
 Thank you :orange_heart: Whether it’s a bug fix, new feature, or additional documentation - we greatly appreciate contributions!
 
-Check out the [contributions guide](https://docs.elementary-data.com/general/contributions) and [open issues](https://github.com/elementary-data/elementary/issues). 
-
+Check out the [contributions guide](https://docs.elementary-data.com/general/contributions) and [open issues](https://github.com/elementary-data/elementary/issues).
 
 **Elementary contributors: ✨**
 
 [//]: contributor-faces
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
@@ -205,12 +196,13 @@
 <a href="https://github.com/will-warner"><img src="https://avatars.githubusercontent.com/u/110092386?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/winzee"><img src="https://avatars.githubusercontent.com/u/1001577?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vinooganesh"><img src="https://avatars.githubusercontent.com/u/2461070?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/dimoschi"><img src="https://avatars.githubusercontent.com/u/13113025?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/manulpatel"><img src="https://avatars.githubusercontent.com/u/77568048?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/arilmav"><img src="https://avatars.githubusercontent.com/u/60354578?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/kochalex"><img src="https://avatars.githubusercontent.com/u/3217653?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/mossyyy"><img src="https://avatars.githubusercontent.com/u/11269029?v=4" width="50" height="50" alt=""/></a>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: elementary-data Version: 0.9.1 Summary: Data
+Metadata-Version: 2.1 Name: elementary-data Version: 0.9.2 Summary: Data
 monitoring and lineage Home-page: https://github.com/elementary-data/elementary
 Author: Elementary Author-email: or@elementary-data.com Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Requires-Python: >=3.6.2 Description-Content-Type: text/markdown
 Provides-Extra: snowflake Provides-Extra: bigquery Provides-Extra: redshift
 Provides-Extra: postgres Provides-Extra: databricks Provides-Extra: spark
 Provides-Extra: all License-File: LICENSE
                                  width="1000">
-         ********** DDaattaa oobbsseerrvvaabbiilliittyy ffoorr aannaallyyttiiccss && ddaattaa eennggiinneeeerrss **********
+   ********** ddbbtt nnaattiivvee ddaattaa oobbsseerrvvaabbiilliittyy ffoorr aannaallyyttiiccss && ddaattaa eennggiinneeeerrss **********
 ****** MMoonniittoorr yyoouurr ddaattaa qquuaalliittyy,, ooppeerraattiioonn aanndd ppeerrffoorrmmaannccee ddiirreeccttllyy ffrroomm yyoouurr ddbbtt
                                  pprroojjeecctt.. ******
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_j_o_i_n_-_S_l_a_c_k_-_f_f_6_9_b_4_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
             _d_o_c_s_-_q_u_i_c_k_s_t_a_r_t_-_o_r_a_n_g_e_][License]left_text=Downloads"/>
   â­ï¸ Star the repo _[_s_t_a_t_i_c_/_s_t_a_r___g_i_t_h_u_b_._p_n_g_]â­ [Demo Â»](https://bit.ly/
  3IAp9wf) | [Docs Â»](https://docs.elementary-data.com/) | [Slack Â»](https://
        join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-
@@ -23,48 +23,47 @@
     ## What is Elementary? Elementary is an open-source data observability
   solution, built for dbt users. Setup in minutes, gain immediate visibility,
   detect data issues, send actionable alerts, and understand impact and root
                          cause. _[_s_t_a_t_i_c_/_r_e_p_o_r_t___u_i_._g_i_f_]
        ## Quick start Step 1 - [Install Elementary dbt package](https://
 docs.elementary-data.com/quickstart) Step 2 - [Install Elementary CLI](https://
          docs.elementary-data.com/quickstart-cli) ## Features [static/
-      elementary_icon.ico]**Data observability report** - Generate a data
-        observability report, host it or share with your team. [static/
-  elementary_icon.ico]**Anomaly detection dbt tests** - Collect data quality
-          metrics and detect anomalies, as native dbt tests. [static/
-elementary_icon.ico]**Test results** - Enriched with details for fast triage of
-  issues. [static/elementary_icon.ico]**Models performance** - Visibility of
-   execution times, easy detection of degradation and bottlenecks. [static/
-  elementary_icon.ico]**Data lineage** - Enriched with test results, easy to
- navigate and filter. [static/elementary_icon.ico]**dbt artifacts uploader** -
-       Save metadata and run results as part of your dbt runs. [static/
-  elementary_icon.ico]**Slack alerts** - Actionable alerts, including custom
-   channels and tagging of owners and subscribers. ## Join [Slack](https://
+ happy_fire.ico]**Data observability report** - Generate a data observability
+   report, host it or share with your team. [static/happy_fire.ico]**Anomaly
+ detection dbt tests** - Collect data quality metrics and detect anomalies, as
+   native dbt tests. [static/happy_fire.ico]**Test results** - Enriched with
+      details for fast triage of issues. [static/happy_fire.ico]**Models
+ performance** - Visibility of execution times, easy detection of degradation
+ and bottlenecks. [static/happy_fire.ico]**Data lineage** - Enriched with test
+ results, easy to navigate and filter. [static/happy_fire.ico]**dbt artifacts
+ uploader** - Save metadata and run results as part of your dbt runs. [static/
+happy_fire.ico]**Slack alerts** - Actionable alerts, including custom channels
+and tagging of owners and subscribers. ## Join [Slack](https://join.slack.com/
+  t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) to
+ learn more on Elementary. Our full documentation is [available here](https://
+docs.elementary-data.com/). ## How it works? Elementary [dbt package](https://
+github.com/elementary-data/dbt-data-reliability) creates tables of metadata and
+  test results in your data warehouse, as part of your dbt runs. The CLI tool
+ reads the data from these tables, and is used to generate the UI and alerts.
+    [static/how_elementary_works.png]## Community & Support For additional
+  information and help, you can use one of these channels: - [Slack](https://
        join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-
-zXeVTtXrjYRbdE_V6xq4Rg) to learn more on Elementary. Our full documentation is
-     [available here](https://docs.elementary-data.com/). ## How it works?
-     Elementary [dbt package](https://github.com/elementary-data/dbt-data-
-     reliability) creates tables of metadata and test results in your data
-  warehouse, as part of your dbt runs. The CLI tool reads the data from these
-          tables, and is used to generate the UI and alerts. [static/
-how_elementary_works.png]## Community & Support For additional information and
- help, you can use one of these channels: * [Slack](https://join.slack.com/t/
- elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) \(Live
-  chat with the team, support, discussions, etc.\) * [GitHub issues](https://
-github.com/elementary-data/elementary/issues) \(Bug reports, feature requests)
- * [Twitter](https://twitter.com/ElementaryData) \(Updates on new releases and
-stuff) ## **Integrations** * [x] **dbt core (>=1.0.0)** ![](static/dbt-16.png)
-     * [x] **dbt cloud** ![](static/dbt-16.png) **Data warehouses:** * [x]
-   **Snowflake** ![](static/snowflake-16.png) * [x] **BigQuery** ![](static/
-     bigquery-16.svg) * [x] **Redshift** ![](static/redshift-16.png) * [x]
-**Databricks SQL** ![](static/databricks-16.png) * [x] **Postgres** ![](static/
-postgres-16.png) **Operations:** * [x] **Slack** ![](static/slack-16.png) * [x]
- **GitHub Actions** ![](static/github-actions-16.png) * [x] **Amazon S3** ![]
-(static/s3-16.svg) * [x] **Google Cloud Storage** ![](static/gcs-16.png) Ask us
-  for integrations on [Slack](https://join.slack.com/t/elementary-community/
-shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) or as a [GitHub issue](https:
-        //github.com/elementary-data/elementary-lineage/issues/new). ##
-   **Contributions** Thank you :orange_heart: Whether itâs a bug fix, new
-  feature, or additional documentation - we greatly appreciate contributions!
- Check out the [contributions guide](https://docs.elementary-data.com/general/
-contributions) and [open issues](https://github.com/elementary-data/elementary/
-       issues). **Elementary contributors: â¨** [//]: contributor-faces
+zXeVTtXrjYRbdE_V6xq4Rg) \(Live chat with the team, support, discussions, etc.\)
+ - [GitHub issues](https://github.com/elementary-data/elementary/issues) \(Bug
+ reports, feature requests) - [Twitter](https://twitter.com/ElementaryData) \
+   (Updates on new releases and stuff) ## **Integrations** - [x] **dbt core
+ (>=1.0.0)** ![](static/dbt-16.png) - [x] **dbt cloud** ![](static/dbt-16.png)
+  **Data warehouses:** - [x] **Snowflake** ![](static/snowflake-16.png) - [x]
+    **BigQuery** ![](static/bigquery-16.svg) - [x] **Redshift** ![](static/
+ redshift-16.png) - [x] **Databricks SQL** ![](static/databricks-16.png) - [x]
+ **Postgres** ![](static/postgres-16.png) **Operations:** - [x] **Slack** ![]
+   (static/slack-16.png) - [x] **GitHub Actions** ![](static/github-actions-
+    16.png) - [x] **Amazon S3** ![](static/s3-16.svg) - [x] **Google Cloud
+ Storage** ![](static/gcs-16.png) Ask us for integrations on [Slack](https://
+       join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-
+ zXeVTtXrjYRbdE_V6xq4Rg) or as a [GitHub issue](https://github.com/elementary-
+     data/elementary-lineage/issues/new). ## **Contributions** Thank you :
+      orange_heart: Whether itâs a bug fix, new feature, or additional
+      documentation - we greatly appreciate contributions! Check out the
+ [contributions guide](https://docs.elementary-data.com/general/contributions)
+   and [open issues](https://github.com/elementary-data/elementary/issues).
+           **Elementary contributors: â¨** [//]: contributor-faces
```

### Comparing `elementary-data-0.9.1/README.md` & `elementary-data-0.9.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <p align="center">
-<img alt="Logo" src="static/header_git.png"/ width="1000">
+<img alt="Logo" src="static/github_banner.png"/ width="1000">
 </p>
 
 <h2 align="center">
- Data observability for analytics & data engineers
+ dbt native data observability for analytics & data engineers
 </h2>
 <h4 align="center">
 Monitor your data quality, operation and performance directly from your dbt project.
 </h4>
 
 <p align="center">
 <a href="https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg"><img src="https://img.shields.io/badge/join-Slack-ff69b4"/></a>
@@ -23,98 +23,89 @@
 
 </div>
 
 ## What is Elementary?
 
 Elementary is an open-source data observability solution, built for dbt users. Setup in minutes, gain immediate visibility, detect data issues, send actionable alerts, and understand impact and root cause.
 
-
 <kbd align="center">
         <a href="https://storage.googleapis.com/elementary_static/elementary_demo.html"><img align="center" style="max-width:300px;" src="static/report_ui.gif"> </a>
 </kbd>
 
 <br>
 
 ## Quick start
 
-Step 1 - [Install Elementary dbt package](https://docs.elementary-data.com/quickstart) 
+Step 1 - [Install Elementary dbt package](https://docs.elementary-data.com/quickstart)
 
 Step 2 - [Install Elementary CLI](https://docs.elementary-data.com/quickstart-cli)
 
-   
 ## Features
 
+<img src="static/happy_fire.ico" width="16"/> **Data observability report** - Generate a data observability report, host it or share with your team.
 
- <img src="static/elementary_icon.ico" width="16"/> **Data observability report** - Generate a data observability report, host it or share with your team.
-
- <img src="static/elementary_icon.ico" width="16"/> **Anomaly detection dbt tests** - Collect data quality metrics and detect anomalies, as native dbt tests.
-
- <img src="static/elementary_icon.ico" width="16"/> **Test results** - Enriched with details for fast triage of issues.
+<img src="static/happy_fire.ico" width="16"/> **Anomaly detection dbt tests** - Collect data quality metrics and detect anomalies, as native dbt tests.
 
- <img src="static/elementary_icon.ico" width="16"/> **Models performance** - Visibility of execution times, easy detection of degradation and bottlenecks.
+<img src="static/happy_fire.ico" width="16"/> **Test results** - Enriched with details for fast triage of issues.
 
- <img src="static/elementary_icon.ico" width="16"/> **Data lineage** - Enriched with test results, easy to navigate and filter.
+<img src="static/happy_fire.ico" width="16"/> **Models performance** - Visibility of execution times, easy detection of degradation and bottlenecks.
 
- <img src="static/elementary_icon.ico" width="16"/> **dbt artifacts uploader** - Save metadata and run results as part of your dbt runs. 
+<img src="static/happy_fire.ico" width="16"/> **Data lineage** - Enriched with test results, easy to navigate and filter.
 
- <img src="static/elementary_icon.ico" width="16"/> **Slack alerts** - Actionable alerts, including custom channels and tagging of owners and subscribers.
+<img src="static/happy_fire.ico" width="16"/> **dbt artifacts uploader** - Save metadata and run results as part of your dbt runs.
 
+<img src="static/happy_fire.ico" width="16"/> **Slack alerts** - Actionable alerts, including custom channels and tagging of owners and subscribers.
 
 ##
- 
+
 Join [Slack](https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) to learn more on Elementary.
 
 Our full documentation is [available here](https://docs.elementary-data.com/).
 
-
 ## How it works?
 
-Elementary [dbt package](https://github.com/elementary-data/dbt-data-reliability) creates tables of metadata and test results in your data warehouse, as part of your dbt runs. The CLI tool reads the data from these tables, and is used to generate the UI and alerts. 
+Elementary [dbt package](https://github.com/elementary-data/dbt-data-reliability) creates tables of metadata and test results in your data warehouse, as part of your dbt runs. The CLI tool reads the data from these tables, and is used to generate the UI and alerts.
 
 <img align="center" style="max-width:300px;" src="static/how_elementary_works.png">
 
 ## Community & Support
 
 For additional information and help, you can use one of these channels:
 
-* [Slack](https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) \(Live chat with the team, support, discussions, etc.\)
-* [GitHub issues](https://github.com/elementary-data/elementary/issues) \(Bug reports, feature requests)
-* [Twitter](https://twitter.com/ElementaryData) \(Updates on new releases and stuff)
-
+- [Slack](https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) \(Live chat with the team, support, discussions, etc.\)
+- [GitHub issues](https://github.com/elementary-data/elementary/issues) \(Bug reports, feature requests)
+- [Twitter](https://twitter.com/ElementaryData) \(Updates on new releases and stuff)
 
 ## **Integrations**
 
-* [x] **dbt core (>=1.0.0)** ![](static/dbt-16.png)
-* [x] **dbt cloud**  ![](static/dbt-16.png)
+- [x] **dbt core (>=1.0.0)** ![](static/dbt-16.png)
+- [x] **dbt cloud** ![](static/dbt-16.png)
 
 **Data warehouses:**
-* [x] **Snowflake** ![](static/snowflake-16.png) 
-* [x] **BigQuery**  ![](static/bigquery-16.svg) 
-* [x] **Redshift**  ![](static/redshift-16.png)
-* [x] **Databricks SQL**  ![](static/databricks-16.png)
-* [x] **Postgres**  ![](static/postgres-16.png)
 
-**Operations:**
-
-* [x] **Slack** ![](static/slack-16.png)
-* [x] **GitHub Actions**  ![](static/github-actions-16.png)
-* [x] **Amazon S3**  ![](static/s3-16.svg)
-* [x] **Google Cloud Storage**  ![](static/gcs-16.png)
+- [x] **Snowflake** ![](static/snowflake-16.png)
+- [x] **BigQuery** ![](static/bigquery-16.svg)
+- [x] **Redshift** ![](static/redshift-16.png)
+- [x] **Databricks SQL** ![](static/databricks-16.png)
+- [x] **Postgres** ![](static/postgres-16.png)
 
+**Operations:**
 
+- [x] **Slack** ![](static/slack-16.png)
+- [x] **GitHub Actions** ![](static/github-actions-16.png)
+- [x] **Amazon S3** ![](static/s3-16.svg)
+- [x] **Google Cloud Storage** ![](static/gcs-16.png)
 
 Ask us for integrations on [Slack](https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) or as a [GitHub issue](https://github.com/elementary-data/elementary-lineage/issues/new).
 
-
 ## **Contributions**
 
 Thank you :orange_heart: Whether it’s a bug fix, new feature, or additional documentation - we greatly appreciate contributions!
 
-Check out the [contributions guide](https://docs.elementary-data.com/general/contributions) and [open issues](https://github.com/elementary-data/elementary/issues). 
-
+Check out the [contributions guide](https://docs.elementary-data.com/general/contributions) and [open issues](https://github.com/elementary-data/elementary/issues).
 
 **Elementary contributors: ✨**
 
 [//]: contributor-faces
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
@@ -179,12 +170,13 @@
 <a href="https://github.com/will-warner"><img src="https://avatars.githubusercontent.com/u/110092386?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/winzee"><img src="https://avatars.githubusercontent.com/u/1001577?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vinooganesh"><img src="https://avatars.githubusercontent.com/u/2461070?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/dimoschi"><img src="https://avatars.githubusercontent.com/u/13113025?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/manulpatel"><img src="https://avatars.githubusercontent.com/u/77568048?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/arilmav"><img src="https://avatars.githubusercontent.com/u/60354578?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/kochalex"><img src="https://avatars.githubusercontent.com/u/3217653?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/mossyyy"><img src="https://avatars.githubusercontent.com/u/11269029?v=4" width="50" height="50" alt=""/></a>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
                                  width="1000">
-         ********** DDaattaa oobbsseerrvvaabbiilliittyy ffoorr aannaallyyttiiccss && ddaattaa eennggiinneeeerrss **********
+   ********** ddbbtt nnaattiivvee ddaattaa oobbsseerrvvaabbiilliittyy ffoorr aannaallyyttiiccss && ddaattaa eennggiinneeeerrss **********
 ****** MMoonniittoorr yyoouurr ddaattaa qquuaalliittyy,, ooppeerraattiioonn aanndd ppeerrffoorrmmaannccee ddiirreeccttllyy ffrroomm yyoouurr ddbbtt
                                  pprroojjeecctt.. ******
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_j_o_i_n_-_S_l_a_c_k_-_f_f_6_9_b_4_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
             _d_o_c_s_-_q_u_i_c_k_s_t_a_r_t_-_o_r_a_n_g_e_][License]left_text=Downloads"/>
   â­ï¸ Star the repo _[_s_t_a_t_i_c_/_s_t_a_r___g_i_t_h_u_b_._p_n_g_]â­ [Demo Â»](https://bit.ly/
  3IAp9wf) | [Docs Â»](https://docs.elementary-data.com/) | [Slack Â»](https://
        join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-
@@ -11,48 +11,47 @@
     ## What is Elementary? Elementary is an open-source data observability
   solution, built for dbt users. Setup in minutes, gain immediate visibility,
   detect data issues, send actionable alerts, and understand impact and root
                          cause. _[_s_t_a_t_i_c_/_r_e_p_o_r_t___u_i_._g_i_f_]
        ## Quick start Step 1 - [Install Elementary dbt package](https://
 docs.elementary-data.com/quickstart) Step 2 - [Install Elementary CLI](https://
          docs.elementary-data.com/quickstart-cli) ## Features [static/
-      elementary_icon.ico]**Data observability report** - Generate a data
-        observability report, host it or share with your team. [static/
-  elementary_icon.ico]**Anomaly detection dbt tests** - Collect data quality
-          metrics and detect anomalies, as native dbt tests. [static/
-elementary_icon.ico]**Test results** - Enriched with details for fast triage of
-  issues. [static/elementary_icon.ico]**Models performance** - Visibility of
-   execution times, easy detection of degradation and bottlenecks. [static/
-  elementary_icon.ico]**Data lineage** - Enriched with test results, easy to
- navigate and filter. [static/elementary_icon.ico]**dbt artifacts uploader** -
-       Save metadata and run results as part of your dbt runs. [static/
-  elementary_icon.ico]**Slack alerts** - Actionable alerts, including custom
-   channels and tagging of owners and subscribers. ## Join [Slack](https://
+ happy_fire.ico]**Data observability report** - Generate a data observability
+   report, host it or share with your team. [static/happy_fire.ico]**Anomaly
+ detection dbt tests** - Collect data quality metrics and detect anomalies, as
+   native dbt tests. [static/happy_fire.ico]**Test results** - Enriched with
+      details for fast triage of issues. [static/happy_fire.ico]**Models
+ performance** - Visibility of execution times, easy detection of degradation
+ and bottlenecks. [static/happy_fire.ico]**Data lineage** - Enriched with test
+ results, easy to navigate and filter. [static/happy_fire.ico]**dbt artifacts
+ uploader** - Save metadata and run results as part of your dbt runs. [static/
+happy_fire.ico]**Slack alerts** - Actionable alerts, including custom channels
+and tagging of owners and subscribers. ## Join [Slack](https://join.slack.com/
+  t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) to
+ learn more on Elementary. Our full documentation is [available here](https://
+docs.elementary-data.com/). ## How it works? Elementary [dbt package](https://
+github.com/elementary-data/dbt-data-reliability) creates tables of metadata and
+  test results in your data warehouse, as part of your dbt runs. The CLI tool
+ reads the data from these tables, and is used to generate the UI and alerts.
+    [static/how_elementary_works.png]## Community & Support For additional
+  information and help, you can use one of these channels: - [Slack](https://
        join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-
-zXeVTtXrjYRbdE_V6xq4Rg) to learn more on Elementary. Our full documentation is
-     [available here](https://docs.elementary-data.com/). ## How it works?
-     Elementary [dbt package](https://github.com/elementary-data/dbt-data-
-     reliability) creates tables of metadata and test results in your data
-  warehouse, as part of your dbt runs. The CLI tool reads the data from these
-          tables, and is used to generate the UI and alerts. [static/
-how_elementary_works.png]## Community & Support For additional information and
- help, you can use one of these channels: * [Slack](https://join.slack.com/t/
- elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) \(Live
-  chat with the team, support, discussions, etc.\) * [GitHub issues](https://
-github.com/elementary-data/elementary/issues) \(Bug reports, feature requests)
- * [Twitter](https://twitter.com/ElementaryData) \(Updates on new releases and
-stuff) ## **Integrations** * [x] **dbt core (>=1.0.0)** ![](static/dbt-16.png)
-     * [x] **dbt cloud** ![](static/dbt-16.png) **Data warehouses:** * [x]
-   **Snowflake** ![](static/snowflake-16.png) * [x] **BigQuery** ![](static/
-     bigquery-16.svg) * [x] **Redshift** ![](static/redshift-16.png) * [x]
-**Databricks SQL** ![](static/databricks-16.png) * [x] **Postgres** ![](static/
-postgres-16.png) **Operations:** * [x] **Slack** ![](static/slack-16.png) * [x]
- **GitHub Actions** ![](static/github-actions-16.png) * [x] **Amazon S3** ![]
-(static/s3-16.svg) * [x] **Google Cloud Storage** ![](static/gcs-16.png) Ask us
-  for integrations on [Slack](https://join.slack.com/t/elementary-community/
-shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) or as a [GitHub issue](https:
-        //github.com/elementary-data/elementary-lineage/issues/new). ##
-   **Contributions** Thank you :orange_heart: Whether itâs a bug fix, new
-  feature, or additional documentation - we greatly appreciate contributions!
- Check out the [contributions guide](https://docs.elementary-data.com/general/
-contributions) and [open issues](https://github.com/elementary-data/elementary/
-       issues). **Elementary contributors: â¨** [//]: contributor-faces
+zXeVTtXrjYRbdE_V6xq4Rg) \(Live chat with the team, support, discussions, etc.\)
+ - [GitHub issues](https://github.com/elementary-data/elementary/issues) \(Bug
+ reports, feature requests) - [Twitter](https://twitter.com/ElementaryData) \
+   (Updates on new releases and stuff) ## **Integrations** - [x] **dbt core
+ (>=1.0.0)** ![](static/dbt-16.png) - [x] **dbt cloud** ![](static/dbt-16.png)
+  **Data warehouses:** - [x] **Snowflake** ![](static/snowflake-16.png) - [x]
+    **BigQuery** ![](static/bigquery-16.svg) - [x] **Redshift** ![](static/
+ redshift-16.png) - [x] **Databricks SQL** ![](static/databricks-16.png) - [x]
+ **Postgres** ![](static/postgres-16.png) **Operations:** - [x] **Slack** ![]
+   (static/slack-16.png) - [x] **GitHub Actions** ![](static/github-actions-
+    16.png) - [x] **Amazon S3** ![](static/s3-16.svg) - [x] **Google Cloud
+ Storage** ![](static/gcs-16.png) Ask us for integrations on [Slack](https://
+       join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-
+ zXeVTtXrjYRbdE_V6xq4Rg) or as a [GitHub issue](https://github.com/elementary-
+     data/elementary-lineage/issues/new). ## **Contributions** Thank you :
+      orange_heart: Whether itâs a bug fix, new feature, or additional
+      documentation - we greatly appreciate contributions! Check out the
+ [contributions guide](https://docs.elementary-data.com/general/contributions)
+   and [open issues](https://github.com/elementary-data/elementary/issues).
+           **Elementary contributors: â¨** [//]: contributor-faces
```

### Comparing `elementary-data-0.9.1/elementary/cli/cli.py` & `elementary-data-0.9.2/elementary/cli/cli.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/cli/upgrade.py` & `elementary-data-0.9.2/elementary/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/clients/dbt/base_dbt_runner.py` & `elementary-data-0.9.2/elementary/clients/dbt/base_dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/clients/dbt/dbt_log.py` & `elementary-data-0.9.2/elementary/clients/dbt/dbt_log.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/clients/dbt/dbt_runner.py` & `elementary-data-0.9.2/elementary/clients/dbt/dbt_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,26 +156,29 @@
                     )
         return run_operation_results
 
     def run(
         self,
         models: Optional[str] = None,
         select: Optional[str] = None,
+        selector: Optional[str] = None,
         full_refresh: bool = False,
         vars: Optional[dict] = None,
         quiet: bool = False,
         capture_output: bool = False,
     ) -> bool:
         command_args = ["run"]
         if full_refresh:
             command_args.append("--full-refresh")
         if models:
             command_args.extend(["-m", models])
         if select:
             command_args.extend(["-s", select])
+        if selector:
+            command_args.extend(["--selector", selector])
         success, _ = self._run_command(
             command_args=command_args,
             vars=vars,
             quiet=quiet,
             capture_output=capture_output,
         )
         return success
```

### Comparing `elementary-data-0.9.1/elementary/clients/dbt/slim_dbt_runner.py` & `elementary-data-0.9.2/elementary/clients/dbt/slim_dbt_runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/clients/gcs/client.py` & `elementary-data-0.9.2/elementary/clients/gcs/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/clients/s3/client.py` & `elementary-data-0.9.2/elementary/clients/s3/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/clients/slack/client.py` & `elementary-data-0.9.2/elementary/clients/slack/client.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/clients/slack/schema.py` & `elementary-data-0.9.2/elementary/clients/slack/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/clients/slack/slack_message_builder.py` & `elementary-data-0.9.2/elementary/clients/slack/slack_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/config/config.py` & `elementary-data-0.9.2/elementary/config/config.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/exceptions/exceptions.py` & `elementary-data-0.9.2/elementary/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/alerts/alert.py` & `elementary-data-0.9.2/elementary/monitor/alerts/alert.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         self.alert_suppression_interval = alert_suppression_interval
         self.alert_fields = alert_fields
         self.slack_group_alerts_by = slack_group_alerts_by
 
         # Defined in the base class so type checks will not complain
         self.data: Dict[str, Any] = {}
         self.model_unique_id: Optional[str] = None
+        self.alerts_table = alerts_table
 
     _LONGEST_MARKDOWN_SUFFIX_LEN = 3
     _CONTINUATION_SYMBOL = "..."
 
     def to_slack(self, is_slack_workflow: bool = False) -> SlackMessageSchema:
         raise NotImplementedError
```

### Comparing `elementary-data-0.9.1/elementary/monitor/alerts/alerts.py` & `elementary-data-0.9.2/elementary/monitor/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/alerts/group_of_alerts.py` & `elementary-data-0.9.2/elementary/monitor/alerts/group_of_alerts.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,19 +60,26 @@
 SubsComponent = NotificationComponent(
     order=2, name_in_summary="Subscribers", empty_section_content="No subscribers"
 )
 
 
 class GroupOfAlerts:
     def __init__(
-        self, alerts: List[Alert], default_channel_destination: str, env: str = "dev"
+        self,
+        alerts: List[Alert],
+        default_channel_destination: str,
+        override_slack_channel: bool,
+        env: str = "dev",
     ):
         self.alerts = alerts
         self._title = self._get_title()
-        self._sort_channel_destination(default_channel=default_channel_destination)
+        self._sort_channel_destination(
+            default_channel=default_channel_destination,
+            override_channel=override_slack_channel,
+        )
         self._fill_components_to_alerts()
         hashtag = SlackMessageBuilder._HASHTAG
         self._components_to_attention_required: Dict[
             NotificationComponent, str
         ] = dict()
         self._components_to_attention_required[
             TagsComponent
@@ -97,15 +104,15 @@
 
     def set_owners(self, owners: List[str]):
         self._components_to_attention_required[OwnersComponent] = ", ".join(owners)
 
     def set_subscribers(self, subscribers: List[str]):
         self._components_to_attention_required[SubsComponent] = ", ".join(subscribers)
 
-    def _sort_channel_destination(self, default_channel):
+    def _sort_channel_destination(self, default_channel, override_channel):
         raise NotImplementedError
 
     def _fill_components_to_alerts(self):
         test_errors = []
         test_warnings = []
         test_failures = []
         model_errors: List[Alert] = []
@@ -257,44 +264,56 @@
 
     def _get_title(self):
         return None
 
 
 class GroupOfAlertsByTable(GroupOfAlerts):
     def __init__(
-        self, alerts: List[Alert], default_channel_destination: str, env: str = "dev"
+        self,
+        alerts: List[Alert],
+        default_channel_destination: str,
+        override_slack_channel: bool,
+        env: str = "dev",
     ):
         # sort out model unique id
         models = set([alert.model_unique_id for alert in alerts])
         if len(models) != 1:
             raise ValueError(
                 f"failed initializing a GroupOfAlertsByTable, for alerts with multiple models: {list(models)}"
             )
         self._model = get_shortened_model_name(list(models)[0])
         self._db = alerts[0].database_name
         self._schema = alerts[0].schema_name
-        super().__init__(alerts, default_channel_destination, env)
+        super().__init__(
+            alerts, default_channel_destination, override_slack_channel, env
+        )
 
     def _get_title(self) -> str:
         return f"Table issues detected - {self._model}"
 
-    def _sort_channel_destination(self, default_channel):
+    def _sort_channel_destination(self, default_channel, override_channel):
         """
         where do we send a group of alerts to?
         Definitions:
         1. "default_channel" is the project yaml level definition, over-rided by CLI if given
-        2. "per alert" is the definition for tests (if exists), or for the related model (if exists).
+        2. override_channel dictates whether the default channel should override the alert-specific channel
+        3. "per alert" is the definition for tests (if exists), or for the related model (if exists).
         Sorting out:
         if grouping is "by table",
          if model has specific channels configured:
           - Send to the Model's configured channel.
          else
           - send it to the default channel
         """
 
+        # if override_channel is set, we just use the default channel
+        if override_channel:
+            self.channel_destination = default_channel
+            return
+
         # Check for a model level configuration.
         model_specific_channel_config = None
         for alert in self.alerts:
             if isinstance(alert, ModelAlert):
                 if alert.slack_channel:
                     model_specific_channel_config = alert.slack_channel
                     break
@@ -316,25 +335,25 @@
         preview_blocks.extend(
             super(GroupOfAlertsByTable, self)._attention_required_blocks()
         )
         return preview_blocks
 
 
 class GroupOfAlertsBySingleAlert(GroupOfAlerts):
-    def _sort_channel_destination(self, default_channel):
+    def _sort_channel_destination(self, default_channel, override_channel):
         """
         where do we send a group of alerts to?
         Definitions:
         1. "default_channel" is the project yaml level definition, over-rided by CLI if given
         2. "per alert" is the definition for tests (if exists), or for the related model (if exists).
         Sorting out:
 
         if grouping is "by alert", test definition or model definition or CLI if given or project-yaml definition
         """
-        if self.alerts[0].slack_channel:
+        if self.alerts[0].slack_channel and not override_channel:
             self.channel_destination = self.alerts[0].slack_channel
         else:
             self.channel_destination = default_channel
 
     def to_slack(self):
         return self.alerts[0].to_slack()
```

### Comparing `elementary-data-0.9.1/elementary/monitor/alerts/malformed.py` & `elementary-data-0.9.2/elementary/monitor/alerts/malformed.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/alerts/model.py` & `elementary-data-0.9.2/elementary/monitor/alerts/model.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/alerts/source_freshness.py` & `elementary-data-0.9.2/elementary/monitor/alerts/source_freshness.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/alerts/test.py` & `elementary-data-0.9.2/elementary/monitor/alerts/test.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/api/alerts/alert_filters.py` & `elementary-data-0.9.2/elementary/monitor/api/alerts/alert_filters.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,126 @@
-from typing import List
+from typing import Callable, List
 
 from elementary.monitor.alerts.alert import AlertType
 from elementary.monitor.alerts.malformed import MalformedAlert
 from elementary.monitor.alerts.model import ModelAlert
 from elementary.monitor.alerts.source_freshness import SourceFreshnessAlert
 from elementary.monitor.alerts.test import TestAlert
-from elementary.monitor.data_monitoring.schema import SelectorFilterSchema
+from elementary.monitor.data_monitoring.schema import (
+    ResourceType,
+    SelectorFilterSchema,
+    Status,
+)
 from elementary.utils.json_utils import try_load_json
 from elementary.utils.log import get_logger
 
 logger = get_logger(__name__)
 
 
 def filter_alerts(
     alerts: List[AlertType],
-    filter: SelectorFilterSchema = SelectorFilterSchema(),
+    alerts_filter: SelectorFilterSchema = SelectorFilterSchema(),
 ) -> List[AlertType]:
-    filtered_alerts = []
+    # If the filter is on invocation stuff, it's not relevant to alerts and we return an empty list
+    if (
+        alerts_filter.invocation_id is not None
+        or alerts_filter.invocation_time is not None
+        or alerts_filter.last_invocation
+    ):
+        logger.warning("Invalid filter for alerts: %s", alerts_filter.selector)
+        return []
+
     # If the filter is empty, we want to return all of the alerts
-    if not filter.selector:
-        filtered_alerts = alerts
-    elif filter.tag:
-        filtered_alerts = _filter_alerts_by_tag(alerts, filter)
-    elif filter.model:
-        filtered_alerts = _filter_alerts_by_model(alerts, filter)
-    elif filter.owner:
-        filtered_alerts = _filter_alerts_by_owner(alerts, filter)
-    elif filter.node_names is not None:
-        filtered_alerts = _filter_alerts_by_node_names(alerts, filter)
-    # If the filter contains a filter that we don't support, we want to return an empty list of alerts
-    elif filter.selector:
-        logger.error(
-            f"An unsupported alerts selector has been provided - {filter.selector}!\nNo alert has been sent!"
+    filtered_alerts = alerts
+    if alerts_filter.tag is not None:
+        filtered_alerts = _filter_alerts_by_tag(filtered_alerts, alerts_filter)
+    if alerts_filter.model is not None:
+        filtered_alerts = _filter_alerts_by_model(filtered_alerts, alerts_filter)
+    if alerts_filter.owner is not None:
+        filtered_alerts = _filter_alerts_by_owner(filtered_alerts, alerts_filter)
+    if alerts_filter.statuses is not None:
+        filtered_alerts = _filter_alerts_by_status(filtered_alerts, alerts_filter)
+    if alerts_filter.resource_types is not None:
+        filtered_alerts = _filter_alerts_by_resource_type(
+            filtered_alerts, alerts_filter
         )
+    if alerts_filter.node_names is not None:
+        filtered_alerts = _filter_alerts_by_node_names(filtered_alerts, alerts_filter)
+
     return filtered_alerts
 
 
 def _filter_alerts_by_tag(
     alerts: List[AlertType],
-    filter: SelectorFilterSchema,
+    tag_filter: SelectorFilterSchema,
 ) -> List[AlertType]:
-    if filter.tag is None:
+
+    if tag_filter.tag is None:
         return alerts
 
     filtered_alerts = []
     for alert in alerts:
         raw_tags = (
             alert.tags
             if not isinstance(alert, MalformedAlert)
             else alert.data.get("tags")
         )
         alert_tags = try_load_json(raw_tags) if isinstance(raw_tags, str) else raw_tags
 
-        if alert_tags and filter.tag in alert_tags:
+        if alert_tags and tag_filter.tag in alert_tags:
             filtered_alerts.append(alert)
     return filtered_alerts
 
 
 def _filter_alerts_by_owner(
     alerts: List[AlertType],
-    filter: SelectorFilterSchema,
+    owner_filter: SelectorFilterSchema,
 ) -> List[AlertType]:
-    if filter.owner is None:
+
+    if owner_filter.owner is None:
         return alerts
 
     filtered_alerts = []
     for alert in alerts:
         raw_owners = (
             alert.owners
             if not isinstance(alert, MalformedAlert)
             else alert.data.get("owners")
         )
         alert_owners = (
             try_load_json(raw_owners) if isinstance(raw_owners, str) else raw_owners
         )
 
-        if alert_owners and filter.owner in alert_owners:
+        if alert_owners and owner_filter.owner in alert_owners:
             filtered_alerts.append(alert)
     return filtered_alerts
 
 
 def _filter_alerts_by_model(
     alerts: List[AlertType],
-    filter: SelectorFilterSchema,
+    model_filter: SelectorFilterSchema,
 ) -> List[AlertType]:
-    if filter.model is None:
+
+    if model_filter.model is None:
         return alerts
 
     filtered_alerts: List[AlertType] = []
     for alert in alerts:
         alert_model_unique_id = alert.model_unique_id
-        if alert_model_unique_id and alert_model_unique_id.endswith(filter.model):
+        if alert_model_unique_id and alert_model_unique_id.endswith(model_filter.model):
             filtered_alerts.append(alert)
     return filtered_alerts
 
 
 def _filter_alerts_by_node_names(
     alerts: List[AlertType],
-    filter: SelectorFilterSchema,
+    node_name_filter: SelectorFilterSchema,
 ) -> List[AlertType]:
-    if filter.node_names is None:
+
+    if node_name_filter.node_names is None:
         return alerts
 
     filtered_alerts = []
     for alert in alerts:
         alert_node_name = None
         if isinstance(alert, TestAlert):
             alert_node_name = alert.test_name
@@ -112,14 +129,44 @@
         elif isinstance(alert, MalformedAlert):
             alert_node_name = alert.test_name or alert.model_unique_id
         else:
             # Shouldn't happen
             raise Exception(f"Unexpected alert type: {type(alert)}")
 
         if alert_node_name:
-            for node_name in filter.node_names:
+            for node_name in node_name_filter.node_names:
                 if alert_node_name.endswith(node_name) or node_name.endswith(
                     alert_node_name
                 ):
                     filtered_alerts.append(alert)
                     break
     return filtered_alerts
+
+
+def _filter_alerts_by_status(
+    alerts: List[AlertType],
+    status_filter: SelectorFilterSchema,
+) -> List[AlertType]:
+
+    if status_filter.statuses is None:
+        return alerts
+
+    statuses: List[Status] = status_filter.statuses
+    filter_func: Callable[[AlertType], bool] = (
+        lambda alert: Status(alert.status) in statuses
+    )
+    return list(filter(filter_func, alerts))
+
+
+def _filter_alerts_by_resource_type(
+    alerts: List[AlertType],
+    resource_type_filter: SelectorFilterSchema,
+) -> List[AlertType]:
+
+    if resource_type_filter.resource_types is None:
+        return alerts
+
+    resource_types: List[ResourceType] = resource_type_filter.resource_types
+    filter_func: Callable[[AlertType], bool] = (
+        lambda alert: ResourceType.from_table_name(alert.alerts_table) in resource_types
+    )
+    return list(filter(filter_func, alerts))
```

### Comparing `elementary-data-0.9.1/elementary/monitor/api/alerts/alerts.py` & `elementary-data-0.9.2/elementary/monitor/api/alerts/alerts.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,24 +22,26 @@
 class AlertsAPI(APIClient):
     def __init__(
         self,
         dbt_runner: DbtRunner,
         config: Config,
         elementary_database_and_schema: str,
         global_suppression_interval: int,
+        override_meta_suppression_interval: bool = False,
     ):
         super().__init__(dbt_runner)
         self.config = config
         self.elementary_database_and_schema = elementary_database_and_schema
         self.alerts_fetcher = AlertsFetcher(
             dbt_runner=self.dbt_runner,
             config=self.config,
             elementary_database_and_schema=self.elementary_database_and_schema,
         )
         self.global_suppression_interval = global_suppression_interval
+        self.override_meta_suppression_interval = override_meta_suppression_interval
 
     def get_new_alerts(
         self,
         days_back: int,
         disable_samples: bool = False,
         filter: SelectorFilterSchema = SelectorFilterSchema(),
     ) -> Alerts:
@@ -114,15 +116,15 @@
     def _sort_alerts(
         self,
         pending_alerts: AlertsQueryResult[AlertType],
         last_alert_sent_times: Dict[str, str],
         filter: SelectorFilterSchema = SelectorFilterSchema(),
     ) -> AlertsQueryResult[AlertType]:
         suppressed_alerts = self._get_suppressed_alerts(
-            pending_alerts, last_alert_sent_times, self.global_suppression_interval
+            pending_alerts, last_alert_sent_times
         )
         latest_alert_ids = self._get_latest_alerts(pending_alerts)
         alerts_to_skip: List[Union[AlertType, MalformedAlert]] = []
         alerts_to_send: List[AlertType] = []
         malformed_alerts_to_send: List[MalformedAlert] = []
 
         for valid_alert in pending_alerts.alerts:
@@ -145,33 +147,33 @@
 
         return AlertsQueryResult(
             alerts=filter_alerts(alerts_to_send, filter),
             malformed_alerts=filter_alerts(malformed_alerts_to_send, filter),
             alerts_to_skip=filter_alerts(alerts_to_skip, filter),
         )
 
-    @classmethod
     def _get_suppressed_alerts(
-        cls,
+        self,
         alerts: AlertsQueryResult[AlertType],
         last_alert_sent_times: Dict[str, str],
-        global_suppression_interval: int,
     ) -> List[str]:
         suppressed_alerts = []
         current_time_utc = datetime.utcnow()
         all_alerts: List[Alert] = [*alerts.alerts, *alerts.malformed_alerts]
         for alert in all_alerts:
             alert_class_id = alert.alert_class_id
             if alert_class_id is None:
                 # Shouldn't happen, but logging in any case
                 logger.debug("Alert without an id detected!")
                 continue
 
-            suppression_interval = cls._get_suppression_interval(
-                alert.alert_suppression_interval, global_suppression_interval
+            suppression_interval = self._get_suppression_interval(
+                alert.alert_suppression_interval,
+                self.global_suppression_interval,
+                self.override_meta_suppression_interval,
             )
             last_sent_time = (
                 datetime.fromisoformat(last_alert_sent_times[alert_class_id])
                 if last_alert_sent_times.get(alert_class_id)
                 else None
             )
             is_alert_in_suppression = (
@@ -210,11 +212,13 @@
                 )
 
         for alert_last_time in alert_last_times.values():
             latest_alert_ids.append(alert_last_time["alert_id"])
         return latest_alert_ids
 
     @staticmethod
-    def _get_suppression_interval(interval_from_alert, interval_from_cli):
-        if interval_from_alert is not None:
-            return interval_from_alert
-        return interval_from_cli
+    def _get_suppression_interval(
+        interval_from_alert, interval_from_cli, override_by_cli
+    ):
+        if interval_from_alert is None or override_by_cli:
+            return interval_from_cli
+        return interval_from_alert
```

### Comparing `elementary-data-0.9.1/elementary/monitor/api/filters/filters.py` & `elementary-data-0.9.2/elementary/monitor/api/filters/filters.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/api/filters/schema.py` & `elementary-data-0.9.2/elementary/monitor/api/filters/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/api/groups/groups.py` & `elementary-data-0.9.2/elementary/monitor/api/groups/groups.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/api/invocations/invocations.py` & `elementary-data-0.9.2/elementary/monitor/api/invocations/invocations.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/api/lineage/lineage.py` & `elementary-data-0.9.2/elementary/monitor/api/lineage/lineage.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/api/lineage/schema.py` & `elementary-data-0.9.2/elementary/monitor/api/lineage/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/api/models/models.py` & `elementary-data-0.9.2/elementary/monitor/api/models/models.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/api/models/schema.py` & `elementary-data-0.9.2/elementary/monitor/api/models/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/api/report/report.py` & `elementary-data-0.9.2/elementary/monitor/api/report/report.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/api/report/schema.py` & `elementary-data-0.9.2/elementary/monitor/api/report/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/api/selector/selector.py` & `elementary-data-0.9.2/elementary/monitor/api/selector/selector.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/api/test_management/test_management.py` & `elementary-data-0.9.2/elementary/monitor/api/test_management/test_management.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/api/tests/schema.py` & `elementary-data-0.9.2/elementary/monitor/api/tests/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/api/tests/tests.py` & `elementary-data-0.9.2/elementary/monitor/api/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,16 @@
             time_bucket_configuration = test_params.get("time_bucket", {})
             time_bucket_count = time_bucket_configuration.get("count", 1)
             time_bucket_period = time_bucket_configuration.get("period", "day")
             configuration = dict(
                 test_name=test_result_db_row.test_name,
                 timestamp_column=test_params.get("timestamp_column"),
                 testing_timeframe=f"{time_bucket_count} {time_bucket_period}{'s' if time_bucket_count > 1 else ''}",
-                anomaly_threshold=test_params.get("sensitivity"),
+                anomaly_threshold=test_params.get("sensitivity")
+                or test_params.get("anomaly_sensitivity"),
             )
 
         return TestMetadataSchema(
             test_unique_id=test_result_db_row.test_unique_id,
             elementary_unique_id=test_result_db_row.elementary_unique_id,
             database_name=test_result_db_row.database_name,
             schema_name=test_result_db_row.schema_name,
```

### Comparing `elementary-data-0.9.1/elementary/monitor/api/totals_schema.py` & `elementary-data-0.9.2/elementary/monitor/api/totals_schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/cli.py` & `elementary-data-0.9.2/elementary/monitor/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,16 @@
         )(func)
         func = click.option(
             "--select",
             type=str,
             default=None,
             help="Filter the report by last_invocation / invocation_id:<INVOCATION_ID> / invocation_time:<INVOCATION_TIME>."
             if cmd in (Command.REPORT, Command.SEND_REPORT)
-            else "Filter the alerts by tag:<TAG> / owner:<OWNER> / model:<MODEL>.",
+            else "Filter the alerts by tag:<TAG> / owner:<OWNER> / model:<MODEL> / "
+            "statuses:<warn/fail/error/skipped> / resource_types:<model/test>.",
         )(func)
         return func
 
     return decorator
 
 
 def get_cli_properties() -> dict:
@@ -222,14 +223,21 @@
 )
 @click.option(
     "--group-by",
     type=click.Choice(["alert", "table"]),
     default=None,
     help="Whether to group alerts by 'alert' or by 'table'",
 )
+@click.option(
+    "--override-dbt-project-config",
+    "-oc",
+    is_flag=True,
+    help="Whether to override the settings (slack channel, suppression interval) "
+    "in the model or test meta in the dbt project with the parameters provided by the CLI.",
+)
 @click.pass_context
 def monitor(
     ctx,
     days_back,
     slack_webhook,
     deprecated_slack_webhook,
     slack_token,
@@ -247,14 +255,15 @@
     test,
     disable_samples,
     env,
     select,
     group_by,
     target_path,
     suppression_interval,
+    override_dbt_project_config,
 ):
     """
     Get alerts on failures in dbt jobs.
     """
     if ctx.invoked_subcommand is not None:
         return
     if deprecated_slack_webhook is not None:
@@ -288,14 +297,15 @@
             config=config,
             tracking=anonymous_tracking,
             force_update_dbt_package=update_dbt_package,
             send_test_message_on_success=test,
             disable_samples=disable_samples,
             filter=select,
             global_suppression_interval=suppression_interval,
+            override_config=override_dbt_project_config,
         )
         # The call to track_cli_start must be after the constructor of DataMonitoringAlerts as it enriches the tracking
         # properties. This is a tech-debt that should be fixed in the future.
         anonymous_tracking.track_cli_start(
             Command.MONITOR, get_cli_properties(), ctx.command.name
         )
         success = data_monitoring.run_alerts(
```

### Comparing `elementary-data-0.9.1/elementary/monitor/data_monitoring/data_monitoring.py` & `elementary-data-0.9.2/elementary/monitor/data_monitoring/data_monitoring.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,20 +26,20 @@
         self,
         config: Config,
         tracking: Optional[Tracking] = None,
         force_update_dbt_package: bool = False,
         disable_samples: bool = False,
         filter: Optional[str] = None,
     ):
+        self.execution_properties: Dict[str, Any] = {}
         self.config = config
         self.tracking = tracking
         self.internal_dbt_runner = self._init_internal_dbt_runner()
         self.user_dbt_runner = self._init_user_dbt_runner()
-
-        self.execution_properties: Dict[str, Any] = {}
+        self._download_dbt_package_if_needed(force_update_dbt_package)
         latest_invocation = self.get_latest_invocation()
         self.project_name = latest_invocation.get("project_name")
         dbt_pkg_version = latest_invocation.get("elementary_version")
         self.warehouse_info = self._get_warehouse_info(
             hash_id=isinstance(tracking, AnonymousTracking)
         )
         if tracking:
@@ -55,15 +55,14 @@
             tracking.set_env("dbt_pkg_version", dbt_pkg_version)
         if dbt_pkg_version:
             self._check_dbt_package_compatibility(dbt_pkg_version)
         # slack client is optional
         self.slack_client = SlackClient.create_client(
             self.config, tracking=self.tracking
         )
-        self._download_dbt_package_if_needed(force_update_dbt_package)
         self.elementary_database_and_schema = self.get_elementary_database_and_schema()
         self.success = True
         self.disable_samples = disable_samples
         self.raw_filter = filter
         self.filter = SelectorFilter(
             tracking=tracking,
             user_dbt_runner=self.user_dbt_runner,
@@ -171,25 +170,19 @@
             return
 
         logger.info(
             f"edr ({py_pkg_ver}) and Elementary's dbt package ({dbt_pkg_ver}) are compatible."
         )
 
     def _get_warehouse_info(self, hash_id: bool = False) -> Optional[WarehouseInfo]:
-        dbt_runner = DbtRunner(
-            dbt_project_utils.PATH,
-            self.config.profiles_dir,
-            self.config.profile_target,
-            env_vars=self.config.env_vars,
-        )
         try:
             warehouse_type, warehouse_unique_id = json.loads(
-                dbt_runner.run_operation("get_adapter_type_and_unique_id", quiet=True)[
-                    0
-                ]
+                self.internal_dbt_runner.run_operation(
+                    "get_adapter_type_and_unique_id", quiet=True
+                )[0]
             )
             return WarehouseInfo(
                 id=warehouse_unique_id if not hash_id else hash(warehouse_unique_id),
                 type=warehouse_type,
             )
         except Exception:
             logger.debug("Could not get warehouse info.", exc_info=True)
```

### Comparing `elementary-data-0.9.1/elementary/monitor/data_monitoring/data_monitoring_alerts.py` & `elementary-data-0.9.2/elementary/monitor/data_monitoring/data_monitoring_alerts.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,27 +37,30 @@
         config: Config,
         tracking: Optional[Tracking] = None,
         filter: Optional[str] = None,
         force_update_dbt_package: bool = False,
         disable_samples: bool = False,
         send_test_message_on_success: bool = False,
         global_suppression_interval: int = 0,
+        override_config: bool = False,
     ):
         super().__init__(
             config, tracking, force_update_dbt_package, disable_samples, filter
         )
 
         self.alerts_api = AlertsAPI(
             self.internal_dbt_runner,
             self.config,
             self.elementary_database_and_schema,
             global_suppression_interval,
+            override_config,
         )
         self.sent_alert_count = 0
         self.send_test_message_on_success = send_test_message_on_success
+        self.override_meta_slack_channel = override_config
 
         if self.slack_client is None:
             raise Exception("Could not initialize slack client!")
 
         # Type hint to mark that in this class the slack client cannot be None
         self.slack_client: SlackClient
 
@@ -133,23 +136,25 @@
                 continue
             table_to_alerts[alert.model_unique_id].append(alert)
 
         by_table_group: List[GroupOfAlerts] = [
             GroupOfAlertsByTable(
                 alerts=table_to_alerts[model_unique_id],
                 default_channel_destination=self.config.slack_channel_name,
+                override_slack_channel=self.override_meta_slack_channel,
                 env=self.config.env,
             )
             for model_unique_id in table_to_alerts.keys()
         ]
 
         by_alert_group: List[GroupOfAlerts] = [
             GroupOfAlertsBySingleAlert(
                 alerts=[al],
                 default_channel_destination=self.config.slack_channel_name,
+                override_slack_channel=self.override_meta_slack_channel,
                 env=self.config.env,
             )
             for al in alerts_by_grouping_mechanism[GroupingType.BY_ALERT]
         ]
 
         self.execution_properties["had_group_by_table"] = len(by_table_group) > 0
         self.execution_properties["had_group_by_alert"] = len(by_alert_group) > 0
```

### Comparing `elementary-data-0.9.1/elementary/monitor/data_monitoring/report/data_monitoring_report.py` & `elementary-data-0.9.2/elementary/monitor/data_monitoring/report/data_monitoring_report.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/data_monitoring/report/index.html` & `elementary-data-0.9.2/elementary/monitor/data_monitoring/report/index.html`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py` & `elementary-data-0.9.2/elementary/monitor/data_monitoring/report/slack_report_summary_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/data_monitoring/schema.py` & `elementary-data-0.9.2/elementary/monitor/fetchers/models/schema.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,93 @@
-from datetime import datetime
-from typing import Dict, List, Optional
+import os
+import posixpath
+from typing import Any, Dict, List, Optional, TypeVar
 
-from pydantic import BaseModel, validator
+from pydantic import Field, validator
 
-from elementary.monitor.api.tests.schema import (
-    InvocationSchema,
-    TestResultSchema,
-    TestRunSchema,
-)
-from elementary.monitor.api.totals_schema import TotalsSchema
-from elementary.utils.log import get_logger
-from elementary.utils.time import DATETIME_FORMAT, convert_local_time_to_timezone
-
-logger = get_logger(__name__)
-
-
-class SelectorFilterSchema(BaseModel):
-    selector: Optional[str] = None
-    invocation_id: Optional[str] = None
-    invocation_time: Optional[str] = None
-    last_invocation: Optional[bool] = False
-    tag: Optional[str] = None
-    owner: Optional[str] = None
-    model: Optional[str] = None
-    node_names: Optional[List[str]] = None
-
-    @validator("invocation_time", pre=True)
-    def format_invocation_time(cls, invocation_time):
-        if invocation_time:
-            try:
-                invocation_datetime = convert_local_time_to_timezone(
-                    datetime.fromisoformat(invocation_time)
-                )
-                return invocation_datetime.strftime(DATETIME_FORMAT)
-            except ValueError as err:
-                logger.error(
-                    f"Failed to parse invocaton time filter: {err}\nPlease use a valid ISO 8601 format"
-                )
-                raise
-        return None
-
-
-class DataMonitoringReportTestResultsSchema(BaseModel):
-    results: Dict[Optional[str], List[TestResultSchema]] = dict()
-    totals: Dict[Optional[str], TotalsSchema] = dict()
-    invocation: InvocationSchema
-
-
-class DataMonitoringReportTestRunsSchema(BaseModel):
-    runs: Dict[Optional[str], List[TestRunSchema]] = dict()
-    totals: Dict[Optional[str], TotalsSchema] = dict()
-
-
-class WarehouseInfo(BaseModel):
-    id: str
-    type: str
+from elementary.utils.schema import ExtendedBaseModel
+from elementary.utils.time import convert_partial_iso_format_to_full_iso_format
+
+
+class ModelRunSchema(ExtendedBaseModel):
+    unique_id: str
+    invocation_id: str
+    name: str
+    schema_name: Optional[str] = Field(alias="schema", default=None)
+    status: str
+    execution_time: float
+    full_refresh: Optional[bool] = None
+    materialization: Optional[str] = None
+    generated_at: str
+
+    @validator("generated_at", pre=True)
+    def format_generated_at(cls, generated_at):
+        return convert_partial_iso_format_to_full_iso_format(generated_at)
+
+
+class ArtifactSchema(ExtendedBaseModel):
+    name: Optional[str] = None
+    unique_id: Optional[str] = None
+    owners: Optional[List[str]] = None
+    tags: Optional[List[str]] = None
+    package_name: Optional[str] = None
+    description: Optional[str] = None
+    full_path: Optional[str] = None
+    meta: Optional[Dict[str, Any]] = None
+
+    @validator("tags", pre=True)
+    def load_tags(cls, tags):
+        return cls._load_var_to_list(tags)
+
+    @validator("owners", pre=True)
+    def load_owners(cls, owners):
+        return cls._load_var_to_list(owners)
+
+    @validator("full_path", pre=True)
+    def format_full_path_sep(cls, full_path: str) -> str:
+        return posixpath.sep.join(full_path.split(os.path.sep))
+
+    @validator("meta", pre=True)
+    def load_meta(cls, meta):
+        return cls._load_var_to_dict(meta)
+
+
+ArtifactSchemaType = TypeVar("ArtifactSchemaType", bound=ArtifactSchema)
+
+
+class ModelSchema(ArtifactSchema):
+    database_name: Optional[str] = None
+    schema_name: str
+    table_name: str
+
+    def ref(self):
+        return f"ref('{self.name}')"
+
+
+class SourceSchema(ArtifactSchema):
+    source_name: Optional[str] = None
+    database_name: Optional[str] = None
+    schema_name: str
+    table_name: str
+
+    def ref(self):
+        return f"source('{self.source_name}', '{self.table_name}')"
+
+
+class OwnerSchema(ExtendedBaseModel):
+    name: Optional[str] = None
+    email: Optional[str] = None
+
+
+class ExposureSchema(ArtifactSchema):
+    label: Optional[str] = None
+    url: Optional[str] = None
+    type: Optional[str] = None
+    maturity: Optional[str] = None
+    depends_on: Optional[List[str]] = None
+    owner: Optional[OwnerSchema] = None
+
+
+class ModelTestCoverage(ExtendedBaseModel):
+    model_unique_id: Optional[str] = None
+    column_tests: int = 0
+    table_tests: int = 0
```

### Comparing `elementary-data-0.9.1/elementary/monitor/data_monitoring/selector_filter.py` & `elementary-data-0.9.2/elementary/monitor/data_monitoring/selector_filter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import re
 from typing import Optional
 
 from elementary.clients.dbt.dbt_runner import DbtRunner
-from elementary.monitor.data_monitoring.schema import SelectorFilterSchema
+from elementary.monitor.data_monitoring.schema import (
+    ResourceType,
+    SelectorFilterSchema,
+    Status,
+)
 from elementary.monitor.fetchers.selector.selector import SelectorFetcher
 from elementary.tracking.tracking_interface import Tracking
 from elementary.utils.log import get_logger
 
 logger = get_logger(__name__)
 
 
@@ -31,62 +35,86 @@
                 if self.tracking:
                     self.tracking.set_env("select_method", "dbt selector")
                 node_names = self.selector_fetcher.get_selector_results(
                     selector=selector
                 )
                 return SelectorFilterSchema(node_names=node_names, selector=selector)
             else:
-                invocation_id_regex = re.compile(r"invocation_id:.*")
-                invocation_time_regex = re.compile(r"invocation_time:.*")
+                invocation_id_regex = re.compile(r"invocation_id:(.*)")
+                invocation_time_regex = re.compile(r"invocation_time:(.*)")
                 last_invocation_regex = re.compile(r"last_invocation")
-                tag_regex = re.compile(r"tag:.*")
-                owner_regex = re.compile(r"config.meta.owner:.*")
-                model_regex = re.compile(r"model:.*")
+                tag_regex = re.compile(r"tag:(.*)")
+                owner_regex = re.compile(r"config.meta.owner:(.*)")
+                model_regex = re.compile(r"model:(.*)")
+                statuses_regex = re.compile(r"statuses:(.*)")
+                resource_types_regex = re.compile(r"resource_types:(.*)")
 
                 invocation_id_match = invocation_id_regex.search(selector)
                 invocation_time_match = invocation_time_regex.search(selector)
                 last_invocation_match = last_invocation_regex.search(selector)
                 tag_match = tag_regex.search(selector)
                 owner_match = owner_regex.search(selector)
                 model_match = model_regex.search(selector)
+                statuses_match = statuses_regex.search(selector)
+                resource_types_match = resource_types_regex.search(selector)
 
                 if last_invocation_match:
                     data_monitoring_filter = SelectorFilterSchema(
                         last_invocation=True, selector=selector
                     )
                 elif invocation_id_match:
                     data_monitoring_filter = SelectorFilterSchema(
-                        invocation_id=invocation_id_match.group().split(":", 1)[1],
+                        invocation_id=invocation_id_match.group(1),
                         selector=selector,
                     )
                 elif invocation_time_match:
                     data_monitoring_filter = SelectorFilterSchema(
-                        invocation_time=invocation_time_match.group().split(":", 1)[1],
+                        invocation_time=invocation_time_match.group(1),
                         selector=selector,
                     )
                 elif tag_match:
                     if self.tracking:
                         self.tracking.set_env("select_method", "tag")
                     data_monitoring_filter = SelectorFilterSchema(
-                        tag=tag_match.group().split(":", 1)[1], selector=selector
+                        tag=tag_match.group(1), selector=selector
                     )
                 elif owner_match:
                     if self.tracking:
                         self.tracking.set_env("select_method", "owner")
                     data_monitoring_filter = SelectorFilterSchema(
-                        owner=owner_match.group().split(":", 1)[1], selector=selector
+                        owner=owner_match.group(1), selector=selector
                     )
                 elif model_match:
                     if self.tracking:
                         self.tracking.set_env("select_method", "model")
                     data_monitoring_filter = SelectorFilterSchema(
-                        model=model_match.group().split(":", 1)[1], selector=selector
+                        model=model_match.group(1), selector=selector
+                    )
+                elif statuses_match:
+                    if self.tracking:
+                        self.tracking.set_env("select_method", "statuses")
+                    statuses = [
+                        Status(status) for status in statuses_match.group(1).split(",")
+                    ]
+                    data_monitoring_filter = SelectorFilterSchema(
+                        statuses=statuses, selector=selector
+                    )
+                elif resource_types_match:
+                    if self.tracking:
+                        self.tracking.set_env("select_method", "resource_types")
+                    resource_types = [
+                        ResourceType(resource_type)
+                        for resource_type in resource_types_match.group(1).split(",")
+                    ]
+                    data_monitoring_filter = SelectorFilterSchema(
+                        resource_types=resource_types, selector=selector
                     )
                 else:
                     logger.error(f"Could not parse the given -s/--select: {selector}")
+                    return SelectorFilterSchema(selector=selector, statuses=[])
         return data_monitoring_filter
 
     def get_filter(self) -> SelectorFilterSchema:
         return self.filter
 
     def get_selector(self) -> Optional[str]:
         return self.selector
```

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/README.md` & `elementary-data-0.9.2/elementary/monitor/dbt_project/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Welcome to your new dbt project!
 
 ### Using the starter project
 
 Try running the following commands:
+
 - dbt run
 - dbt test
 
-
 ### Resources:
+
 - Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
 - Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
 - Join the [chat](https://community.getdbt.com/) on Slack for live discussions and support
 - Find [dbt events](https://events.getdbt.com) near you
 - Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices
```

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/dbt_project.yml` & `elementary-data-0.9.2/elementary/monitor/dbt_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/empty_alert_tables.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/get_model_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/get_new_alerts_where_clause.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/get_source_freshness_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/get_test_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/update_sent_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/alerts/update_skipped_alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/base_queries/current_tests_run_results_query.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/base_queries/owners.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/base_queries/owners.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/base_queries/resources.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/base_queries/resources.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/base_queries/tags.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/base_queries/tags.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/base_queries/tests.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/base_queries/tests.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_dbt_models_test_coverage.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_exposures.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_exposures.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_invocations_by_ids.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_invocations_by_ids.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_latest_invocation.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_latest_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_models.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_models.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_models_runs.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_models_runs.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_nodes_depends_on_nodes.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_resources_latest_invocation.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_resources_latest_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_sources.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_sources.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_test_last_invocation.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_test_results.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_test_results.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/get_test_rows_sample.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/internal_tests/validate_alert_statuses_are_updated.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/internal_tests/validate_alert_statuses_are_updated.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/materializations/incremental.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/macros/materializations/table.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/models/alerts/alerts.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/models/alerts/alerts.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/models/alerts/alerts_models.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/models/alerts/alerts_models.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql` & `elementary-data-0.9.2/elementary/monitor/dbt_project/models/alerts/alerts_source_freshness.sql`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project/models/elementary.yml` & `elementary-data-0.9.2/elementary/monitor/dbt_project/models/elementary.yml`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/dbt_project_utils.py` & `elementary-data-0.9.2/elementary/monitor/dbt_project_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/debug.py` & `elementary-data-0.9.2/elementary/monitor/debug.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/fetchers/alerts/alerts.py` & `elementary-data-0.9.2/elementary/monitor/fetchers/alerts/alerts.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/fetchers/alerts/normalized_alert.py` & `elementary-data-0.9.2/elementary/monitor/fetchers/alerts/normalized_alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/fetchers/invocations/invocations.py` & `elementary-data-0.9.2/elementary/monitor/fetchers/invocations/invocations.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/fetchers/invocations/schema.py` & `elementary-data-0.9.2/elementary/monitor/fetchers/invocations/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/fetchers/lineage/lineage.py` & `elementary-data-0.9.2/elementary/monitor/fetchers/lineage/lineage.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/fetchers/lineage/schema.py` & `elementary-data-0.9.2/elementary/monitor/fetchers/lineage/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/fetchers/models/models.py` & `elementary-data-0.9.2/elementary/monitor/fetchers/models/models.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/fetchers/models/schema.py` & `elementary-data-0.9.2/elementary/monitor/fetchers/test_management/schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,76 @@
-import os
-import posixpath
-from typing import Any, Dict, List, Optional, TypeVar
+from typing import List, Literal, Optional
 
-from pydantic import Field, validator
+from pydantic import BaseModel, Field, validator
 
-from elementary.utils.schema import ExtendedBaseModel
 from elementary.utils.time import convert_partial_iso_format_to_full_iso_format
 
 
-class ModelRunSchema(ExtendedBaseModel):
-    unique_id: str
-    invocation_id: str
+class ResourceColumnModel(BaseModel):
     name: str
-    schema_name: Optional[str] = Field(alias="schema", default=None)
-    status: str
-    execution_time: float
-    full_refresh: Optional[bool] = None
-    materialization: Optional[str] = None
-    generated_at: str
+    type: str
 
-    @validator("generated_at", pre=True)
-    def format_generated_at(cls, generated_at):
-        return convert_partial_iso_format_to_full_iso_format(generated_at)
-
-
-class ArtifactSchema(ExtendedBaseModel):
-    name: Optional[str] = None
-    unique_id: Optional[str] = None
-    owners: Optional[List[str]] = None
-    tags: Optional[List[str]] = None
-    package_name: Optional[str] = None
-    description: Optional[str] = None
-    full_path: Optional[str] = None
-    meta: Optional[Dict[str, Any]] = None
-
-    @validator("tags", pre=True)
-    def load_tags(cls, tags):
-        return cls._load_var_to_list(tags)
-
-    @validator("owners", pre=True)
-    def load_owners(cls, owners):
-        return cls._load_var_to_list(owners)
-
-    @validator("full_path", pre=True)
-    def format_full_path_sep(cls, full_path: str) -> str:
-        return posixpath.sep.join(full_path.split(os.path.sep))
-
-    @validator("meta", pre=True)
-    def load_meta(cls, meta):
-        return cls._load_var_to_dict(meta)
-
-
-ArtifactSchemaType = TypeVar("ArtifactSchemaType", bound=ArtifactSchema)
 
+class ResourceModel(BaseModel):
+    id: str
+    name: str
+    source_name: Optional[str] = None
+    db_schema: str = Field(alias="schema")
+    tags: List[str] = Field(default_factory=list)
+    owners: List[str] = Field(default_factory=list)
+    columns: List[ResourceColumnModel] = Field(default_factory=list)
 
-class ModelSchema(ArtifactSchema):
-    database_name: Optional[str] = None
-    schema_name: str
-    table_name: str
 
-    def ref(self):
-        return f"ref('{self.name}')"
+class ResourcesModel(BaseModel):
+    models: List[ResourceModel] = Field(default_factory=list)
+    sources: List[ResourceModel] = Field(default_factory=list)
 
 
-class SourceSchema(ArtifactSchema):
+class TestModel(BaseModel):
+    id: str
+    db_schema: str = Field(alias="schema")
+    table: Optional[str] = None
     source_name: Optional[str] = None
-    database_name: Optional[str] = None
-    schema_name: str
-    table_name: str
-
-    def ref(self):
-        return f"source('{self.source_name}', '{self.table_name}')"
+    column: Optional[str] = None
+    package: Optional[str] = None
+    name: str
+    type: Optional[str] = None
+    args: Optional[dict] = None
+    severity: str
+    owners: List[str] = Field(default_factory=list)
+    model_owners: List[str] = Field(default_factory=list)
+    tags: List[str] = Field(default_factory=list)
+    model_tags: List[str] = Field(default_factory=list)
+    meta: dict = Field(default_factory=dict)
+    description: Optional[str]
+    is_singular: bool
+    updated_at: str
+    updated_by: Optional[str] = None
+
+    @validator("severity", pre=True)
+    def validate_severity(cls, severity: str) -> str:
+        severity_lower_string = severity.lower()
+        if severity_lower_string not in ["error", "warn"]:
+            raise ValueError('Severity must be "warn" or "error"')
+        return severity_lower_string
+
+    @validator("updated_at", pre=True)
+    def validate_updated_at(cls, updated_at: str) -> str:
+        return convert_partial_iso_format_to_full_iso_format(updated_at)
+
+
+class TestsModel(BaseModel):
+    tests: List[TestModel] = Field(default_factory=list)
 
 
-class OwnerSchema(ExtendedBaseModel):
-    name: Optional[str] = None
-    email: Optional[str] = None
+class TagsModel(BaseModel):
+    tags: List[str] = Field(default_factory=list)
 
 
-class ExposureSchema(ArtifactSchema):
-    label: Optional[str] = None
-    url: Optional[str] = None
-    type: Optional[str] = None
-    maturity: Optional[str] = None
-    depends_on: Optional[List[str]] = None
-    owner: Optional[OwnerSchema] = None
+class UserModel(BaseModel):
+    name: str
+    email: Optional[str] = None
+    origin: Literal["account", "project"]
 
 
-class ModelTestCoverage(ExtendedBaseModel):
-    model_unique_id: Optional[str] = None
-    column_tests: int = 0
-    table_tests: int = 0
+class UsersModel(BaseModel):
+    users: List[UserModel] = Field(default_factory=list)
```

### Comparing `elementary-data-0.9.1/elementary/monitor/fetchers/test_management/test_management.py` & `elementary-data-0.9.2/elementary/monitor/fetchers/test_management/test_management.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/fetchers/tests/schema.py` & `elementary-data-0.9.2/elementary/monitor/fetchers/tests/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/monitor/fetchers/tests/tests.py` & `elementary-data-0.9.2/elementary/monitor/fetchers/tests/tests.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/operations/cli.py` & `elementary-data-0.9.2/elementary/operations/cli.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/operations/upload_source_freshness.py` & `elementary-data-0.9.2/elementary/operations/upload_source_freshness.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 
     def upload_results(self, results: dict):
         dbt_runner = DbtRunner(
             dbt_project_utils.PATH,
             self.config.profiles_dir,
             self.config.profile_target,
         )
+        if not dbt_project_utils.is_dbt_package_up_to_date():
+            dbt_runner.deps()
+
         chunk_size = 100
         chunk_list = list(range(0, len(results), chunk_size))
         upload_with_progress_bar = alive_it(
             chunk_list, title="Uploading source freshness results"
         )
         for chunk in upload_with_progress_bar:
             results_segment = results[chunk : chunk + chunk_size]
```

### Comparing `elementary-data-0.9.1/elementary/tracking/anonymous_tracking.py` & `elementary-data-0.9.2/elementary/tracking/anonymous_tracking.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/tracking/runner.py` & `elementary-data-0.9.2/elementary/tracking/runner.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/tracking/tracking_interface.py` & `elementary-data-0.9.2/elementary/tracking/tracking_interface.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/utils/cli_utils.py` & `elementary-data-0.9.2/elementary/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/utils/json_utils.py` & `elementary-data-0.9.2/elementary/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/utils/log.py` & `elementary-data-0.9.2/elementary/utils/log.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/utils/ordered_yaml.py` & `elementary-data-0.9.2/elementary/utils/ordered_yaml.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/utils/schema.py` & `elementary-data-0.9.2/elementary/utils/schema.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary/utils/time.py` & `elementary-data-0.9.2/elementary/utils/time.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary_data.egg-info/PKG-INFO` & `elementary-data-0.9.2/elementary_data.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elementary-data
-Version: 0.9.1
+Version: 0.9.2
 Summary: Data monitoring and lineage
 Home-page: https://github.com/elementary-data/elementary
 Author: Elementary
 Author-email: or@elementary-data.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
@@ -21,19 +21,19 @@
 Provides-Extra: postgres
 Provides-Extra: databricks
 Provides-Extra: spark
 Provides-Extra: all
 License-File: LICENSE
 
 <p align="center">
-<img alt="Logo" src="static/header_git.png"/ width="1000">
+<img alt="Logo" src="static/github_banner.png"/ width="1000">
 </p>
 
 <h2 align="center">
- Data observability for analytics & data engineers
+ dbt native data observability for analytics & data engineers
 </h2>
 <h4 align="center">
 Monitor your data quality, operation and performance directly from your dbt project.
 </h4>
 
 <p align="center">
 <a href="https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg"><img src="https://img.shields.io/badge/join-Slack-ff69b4"/></a>
@@ -49,98 +49,89 @@
 
 </div>
 
 ## What is Elementary?
 
 Elementary is an open-source data observability solution, built for dbt users. Setup in minutes, gain immediate visibility, detect data issues, send actionable alerts, and understand impact and root cause.
 
-
 <kbd align="center">
         <a href="https://storage.googleapis.com/elementary_static/elementary_demo.html"><img align="center" style="max-width:300px;" src="static/report_ui.gif"> </a>
 </kbd>
 
 <br>
 
 ## Quick start
 
-Step 1 - [Install Elementary dbt package](https://docs.elementary-data.com/quickstart) 
+Step 1 - [Install Elementary dbt package](https://docs.elementary-data.com/quickstart)
 
 Step 2 - [Install Elementary CLI](https://docs.elementary-data.com/quickstart-cli)
 
-   
 ## Features
 
+<img src="static/happy_fire.ico" width="16"/> **Data observability report** - Generate a data observability report, host it or share with your team.
 
- <img src="static/elementary_icon.ico" width="16"/> **Data observability report** - Generate a data observability report, host it or share with your team.
-
- <img src="static/elementary_icon.ico" width="16"/> **Anomaly detection dbt tests** - Collect data quality metrics and detect anomalies, as native dbt tests.
-
- <img src="static/elementary_icon.ico" width="16"/> **Test results** - Enriched with details for fast triage of issues.
+<img src="static/happy_fire.ico" width="16"/> **Anomaly detection dbt tests** - Collect data quality metrics and detect anomalies, as native dbt tests.
 
- <img src="static/elementary_icon.ico" width="16"/> **Models performance** - Visibility of execution times, easy detection of degradation and bottlenecks.
+<img src="static/happy_fire.ico" width="16"/> **Test results** - Enriched with details for fast triage of issues.
 
- <img src="static/elementary_icon.ico" width="16"/> **Data lineage** - Enriched with test results, easy to navigate and filter.
+<img src="static/happy_fire.ico" width="16"/> **Models performance** - Visibility of execution times, easy detection of degradation and bottlenecks.
 
- <img src="static/elementary_icon.ico" width="16"/> **dbt artifacts uploader** - Save metadata and run results as part of your dbt runs. 
+<img src="static/happy_fire.ico" width="16"/> **Data lineage** - Enriched with test results, easy to navigate and filter.
 
- <img src="static/elementary_icon.ico" width="16"/> **Slack alerts** - Actionable alerts, including custom channels and tagging of owners and subscribers.
+<img src="static/happy_fire.ico" width="16"/> **dbt artifacts uploader** - Save metadata and run results as part of your dbt runs.
 
+<img src="static/happy_fire.ico" width="16"/> **Slack alerts** - Actionable alerts, including custom channels and tagging of owners and subscribers.
 
 ##
- 
+
 Join [Slack](https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) to learn more on Elementary.
 
 Our full documentation is [available here](https://docs.elementary-data.com/).
 
-
 ## How it works?
 
-Elementary [dbt package](https://github.com/elementary-data/dbt-data-reliability) creates tables of metadata and test results in your data warehouse, as part of your dbt runs. The CLI tool reads the data from these tables, and is used to generate the UI and alerts. 
+Elementary [dbt package](https://github.com/elementary-data/dbt-data-reliability) creates tables of metadata and test results in your data warehouse, as part of your dbt runs. The CLI tool reads the data from these tables, and is used to generate the UI and alerts.
 
 <img align="center" style="max-width:300px;" src="static/how_elementary_works.png">
 
 ## Community & Support
 
 For additional information and help, you can use one of these channels:
 
-* [Slack](https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) \(Live chat with the team, support, discussions, etc.\)
-* [GitHub issues](https://github.com/elementary-data/elementary/issues) \(Bug reports, feature requests)
-* [Twitter](https://twitter.com/ElementaryData) \(Updates on new releases and stuff)
-
+- [Slack](https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) \(Live chat with the team, support, discussions, etc.\)
+- [GitHub issues](https://github.com/elementary-data/elementary/issues) \(Bug reports, feature requests)
+- [Twitter](https://twitter.com/ElementaryData) \(Updates on new releases and stuff)
 
 ## **Integrations**
 
-* [x] **dbt core (>=1.0.0)** ![](static/dbt-16.png)
-* [x] **dbt cloud**  ![](static/dbt-16.png)
+- [x] **dbt core (>=1.0.0)** ![](static/dbt-16.png)
+- [x] **dbt cloud** ![](static/dbt-16.png)
 
 **Data warehouses:**
-* [x] **Snowflake** ![](static/snowflake-16.png) 
-* [x] **BigQuery**  ![](static/bigquery-16.svg) 
-* [x] **Redshift**  ![](static/redshift-16.png)
-* [x] **Databricks SQL**  ![](static/databricks-16.png)
-* [x] **Postgres**  ![](static/postgres-16.png)
 
-**Operations:**
-
-* [x] **Slack** ![](static/slack-16.png)
-* [x] **GitHub Actions**  ![](static/github-actions-16.png)
-* [x] **Amazon S3**  ![](static/s3-16.svg)
-* [x] **Google Cloud Storage**  ![](static/gcs-16.png)
+- [x] **Snowflake** ![](static/snowflake-16.png)
+- [x] **BigQuery** ![](static/bigquery-16.svg)
+- [x] **Redshift** ![](static/redshift-16.png)
+- [x] **Databricks SQL** ![](static/databricks-16.png)
+- [x] **Postgres** ![](static/postgres-16.png)
 
+**Operations:**
 
+- [x] **Slack** ![](static/slack-16.png)
+- [x] **GitHub Actions** ![](static/github-actions-16.png)
+- [x] **Amazon S3** ![](static/s3-16.svg)
+- [x] **Google Cloud Storage** ![](static/gcs-16.png)
 
 Ask us for integrations on [Slack](https://join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) or as a [GitHub issue](https://github.com/elementary-data/elementary-lineage/issues/new).
 
-
 ## **Contributions**
 
 Thank you :orange_heart: Whether it’s a bug fix, new feature, or additional documentation - we greatly appreciate contributions!
 
-Check out the [contributions guide](https://docs.elementary-data.com/general/contributions) and [open issues](https://github.com/elementary-data/elementary/issues). 
-
+Check out the [contributions guide](https://docs.elementary-data.com/general/contributions) and [open issues](https://github.com/elementary-data/elementary/issues).
 
 **Elementary contributors: ✨**
 
 [//]: contributor-faces
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
@@ -205,12 +196,13 @@
 <a href="https://github.com/will-warner"><img src="https://avatars.githubusercontent.com/u/110092386?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/winzee"><img src="https://avatars.githubusercontent.com/u/1001577?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/vinooganesh"><img src="https://avatars.githubusercontent.com/u/2461070?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/dimoschi"><img src="https://avatars.githubusercontent.com/u/13113025?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/manulpatel"><img src="https://avatars.githubusercontent.com/u/77568048?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/arilmav"><img src="https://avatars.githubusercontent.com/u/60354578?v=4" width="50" height="50" alt=""/></a>
 <a href="https://github.com/kochalex"><img src="https://avatars.githubusercontent.com/u/3217653?v=4" width="50" height="50" alt=""/></a>
+<a href="https://github.com/mossyyy"><img src="https://avatars.githubusercontent.com/u/11269029?v=4" width="50" height="50" alt=""/></a>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: elementary-data Version: 0.9.1 Summary: Data
+Metadata-Version: 2.1 Name: elementary-data Version: 0.9.2 Summary: Data
 monitoring and lineage Home-page: https://github.com/elementary-data/elementary
 Author: Elementary Author-email: or@elementary-data.com Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System ::
 Microsoft :: Windows Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Requires-Python: >=3.6.2 Description-Content-Type: text/markdown
 Provides-Extra: snowflake Provides-Extra: bigquery Provides-Extra: redshift
 Provides-Extra: postgres Provides-Extra: databricks Provides-Extra: spark
 Provides-Extra: all License-File: LICENSE
                                  width="1000">
-         ********** DDaattaa oobbsseerrvvaabbiilliittyy ffoorr aannaallyyttiiccss && ddaattaa eennggiinneeeerrss **********
+   ********** ddbbtt nnaattiivvee ddaattaa oobbsseerrvvaabbiilliittyy ffoorr aannaallyyttiiccss && ddaattaa eennggiinneeeerrss **********
 ****** MMoonniittoorr yyoouurr ddaattaa qquuaalliittyy,, ooppeerraattiioonn aanndd ppeerrffoorrmmaannccee ddiirreeccttllyy ffrroomm yyoouurr ddbbtt
                                  pprroojjeecctt.. ******
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_j_o_i_n_-_S_l_a_c_k_-_f_f_6_9_b_4_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
             _d_o_c_s_-_q_u_i_c_k_s_t_a_r_t_-_o_r_a_n_g_e_][License]left_text=Downloads"/>
   â­ï¸ Star the repo _[_s_t_a_t_i_c_/_s_t_a_r___g_i_t_h_u_b_._p_n_g_]â­ [Demo Â»](https://bit.ly/
  3IAp9wf) | [Docs Â»](https://docs.elementary-data.com/) | [Slack Â»](https://
        join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-
@@ -23,48 +23,47 @@
     ## What is Elementary? Elementary is an open-source data observability
   solution, built for dbt users. Setup in minutes, gain immediate visibility,
   detect data issues, send actionable alerts, and understand impact and root
                          cause. _[_s_t_a_t_i_c_/_r_e_p_o_r_t___u_i_._g_i_f_]
        ## Quick start Step 1 - [Install Elementary dbt package](https://
 docs.elementary-data.com/quickstart) Step 2 - [Install Elementary CLI](https://
          docs.elementary-data.com/quickstart-cli) ## Features [static/
-      elementary_icon.ico]**Data observability report** - Generate a data
-        observability report, host it or share with your team. [static/
-  elementary_icon.ico]**Anomaly detection dbt tests** - Collect data quality
-          metrics and detect anomalies, as native dbt tests. [static/
-elementary_icon.ico]**Test results** - Enriched with details for fast triage of
-  issues. [static/elementary_icon.ico]**Models performance** - Visibility of
-   execution times, easy detection of degradation and bottlenecks. [static/
-  elementary_icon.ico]**Data lineage** - Enriched with test results, easy to
- navigate and filter. [static/elementary_icon.ico]**dbt artifacts uploader** -
-       Save metadata and run results as part of your dbt runs. [static/
-  elementary_icon.ico]**Slack alerts** - Actionable alerts, including custom
-   channels and tagging of owners and subscribers. ## Join [Slack](https://
+ happy_fire.ico]**Data observability report** - Generate a data observability
+   report, host it or share with your team. [static/happy_fire.ico]**Anomaly
+ detection dbt tests** - Collect data quality metrics and detect anomalies, as
+   native dbt tests. [static/happy_fire.ico]**Test results** - Enriched with
+      details for fast triage of issues. [static/happy_fire.ico]**Models
+ performance** - Visibility of execution times, easy detection of degradation
+ and bottlenecks. [static/happy_fire.ico]**Data lineage** - Enriched with test
+ results, easy to navigate and filter. [static/happy_fire.ico]**dbt artifacts
+ uploader** - Save metadata and run results as part of your dbt runs. [static/
+happy_fire.ico]**Slack alerts** - Actionable alerts, including custom channels
+and tagging of owners and subscribers. ## Join [Slack](https://join.slack.com/
+  t/elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) to
+ learn more on Elementary. Our full documentation is [available here](https://
+docs.elementary-data.com/). ## How it works? Elementary [dbt package](https://
+github.com/elementary-data/dbt-data-reliability) creates tables of metadata and
+  test results in your data warehouse, as part of your dbt runs. The CLI tool
+ reads the data from these tables, and is used to generate the UI and alerts.
+    [static/how_elementary_works.png]## Community & Support For additional
+  information and help, you can use one of these channels: - [Slack](https://
        join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-
-zXeVTtXrjYRbdE_V6xq4Rg) to learn more on Elementary. Our full documentation is
-     [available here](https://docs.elementary-data.com/). ## How it works?
-     Elementary [dbt package](https://github.com/elementary-data/dbt-data-
-     reliability) creates tables of metadata and test results in your data
-  warehouse, as part of your dbt runs. The CLI tool reads the data from these
-          tables, and is used to generate the UI and alerts. [static/
-how_elementary_works.png]## Community & Support For additional information and
- help, you can use one of these channels: * [Slack](https://join.slack.com/t/
- elementary-community/shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) \(Live
-  chat with the team, support, discussions, etc.\) * [GitHub issues](https://
-github.com/elementary-data/elementary/issues) \(Bug reports, feature requests)
- * [Twitter](https://twitter.com/ElementaryData) \(Updates on new releases and
-stuff) ## **Integrations** * [x] **dbt core (>=1.0.0)** ![](static/dbt-16.png)
-     * [x] **dbt cloud** ![](static/dbt-16.png) **Data warehouses:** * [x]
-   **Snowflake** ![](static/snowflake-16.png) * [x] **BigQuery** ![](static/
-     bigquery-16.svg) * [x] **Redshift** ![](static/redshift-16.png) * [x]
-**Databricks SQL** ![](static/databricks-16.png) * [x] **Postgres** ![](static/
-postgres-16.png) **Operations:** * [x] **Slack** ![](static/slack-16.png) * [x]
- **GitHub Actions** ![](static/github-actions-16.png) * [x] **Amazon S3** ![]
-(static/s3-16.svg) * [x] **Google Cloud Storage** ![](static/gcs-16.png) Ask us
-  for integrations on [Slack](https://join.slack.com/t/elementary-community/
-shared_invite/zt-uehfrq2f-zXeVTtXrjYRbdE_V6xq4Rg) or as a [GitHub issue](https:
-        //github.com/elementary-data/elementary-lineage/issues/new). ##
-   **Contributions** Thank you :orange_heart: Whether itâs a bug fix, new
-  feature, or additional documentation - we greatly appreciate contributions!
- Check out the [contributions guide](https://docs.elementary-data.com/general/
-contributions) and [open issues](https://github.com/elementary-data/elementary/
-       issues). **Elementary contributors: â¨** [//]: contributor-faces
+zXeVTtXrjYRbdE_V6xq4Rg) \(Live chat with the team, support, discussions, etc.\)
+ - [GitHub issues](https://github.com/elementary-data/elementary/issues) \(Bug
+ reports, feature requests) - [Twitter](https://twitter.com/ElementaryData) \
+   (Updates on new releases and stuff) ## **Integrations** - [x] **dbt core
+ (>=1.0.0)** ![](static/dbt-16.png) - [x] **dbt cloud** ![](static/dbt-16.png)
+  **Data warehouses:** - [x] **Snowflake** ![](static/snowflake-16.png) - [x]
+    **BigQuery** ![](static/bigquery-16.svg) - [x] **Redshift** ![](static/
+ redshift-16.png) - [x] **Databricks SQL** ![](static/databricks-16.png) - [x]
+ **Postgres** ![](static/postgres-16.png) **Operations:** - [x] **Slack** ![]
+   (static/slack-16.png) - [x] **GitHub Actions** ![](static/github-actions-
+    16.png) - [x] **Amazon S3** ![](static/s3-16.svg) - [x] **Google Cloud
+ Storage** ![](static/gcs-16.png) Ask us for integrations on [Slack](https://
+       join.slack.com/t/elementary-community/shared_invite/zt-uehfrq2f-
+ zXeVTtXrjYRbdE_V6xq4Rg) or as a [GitHub issue](https://github.com/elementary-
+     data/elementary-lineage/issues/new). ## **Contributions** Thank you :
+      orange_heart: Whether itâs a bug fix, new feature, or additional
+      documentation - we greatly appreciate contributions! Check out the
+ [contributions guide](https://docs.elementary-data.com/general/contributions)
+   and [open issues](https://github.com/elementary-data/elementary/issues).
+           **Elementary contributors: â¨** [//]: contributor-faces
```

### Comparing `elementary-data-0.9.1/elementary_data.egg-info/SOURCES.txt` & `elementary-data-0.9.2/elementary_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/elementary_data.egg-info/requires.txt` & `elementary-data-0.9.2/elementary_data.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/setup.py` & `elementary-data-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "spark": ["dbt-spark>=0.20,<2.0.0", "dbt-spark[PyHive]>=0.20,<2.0.0"],
 }
 
 
 setup(
     name="elementary-data",
     description="Data monitoring and lineage",
-    version="0.9.1",
+    version="0.9.2",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.6.2",
     entry_points="""
         [console_scripts]
         edr=elementary.cli.cli:cli
     """,
```

### Comparing `elementary-data-0.9.1/tests/integration/monitor/api/alerts/test_alerts_fetcher.py` & `elementary-data-0.9.2/tests/integration/monitor/api/alerts/test_alerts_fetcher.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/tests/integration/monitor/api/tests/test_tests_api.py` & `elementary-data-0.9.2/tests/integration/monitor/api/tests/test_tests_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/tests/mocks/api/alerts_api_mock.py` & `elementary-data-0.9.2/tests/mocks/api/alerts_api_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/tests/mocks/api/tests_api_mock.py` & `elementary-data-0.9.2/tests/mocks/api/tests_api_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/tests/mocks/fetchers/alerts_fetcher_mock.py` & `elementary-data-0.9.2/tests/mocks/fetchers/alerts_fetcher_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/tests/mocks/fetchers/tests_fetcher_mock.py` & `elementary-data-0.9.2/tests/mocks/fetchers/tests_fetcher_mock.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py` & `elementary-data-0.9.2/tests/unit/monitor/alerts/group_alerts_by_table/mock_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,7 +29,8 @@
     env: str = "dev"
 
 
 @dataclass
 class MockDataMonitoringAlerts:
     config: MockConfig
     execution_properties: Dict
+    override_meta_slack_channel: bool
```

### Comparing `elementary-data-0.9.1/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py` & `elementary-data-0.9.2/tests/unit/monitor/alerts/group_alerts_by_table/mock_data.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py` & `elementary-data-0.9.2/tests/unit/monitor/alerts/group_alerts_by_table/test_slack_alerts_group_by.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 @Parametrization.case(
     name="one_warning_goes_to_one_warning",
     list_of_alerts=[AL_WARN_MODEL1_NO_CHANNEL_NO_GROUPING_TS3],
     expected_alert_groups=[
         GroupOfAlertsBySingleAlert(
             alerts=[AL_WARN_MODEL1_NO_CHANNEL_NO_GROUPING_TS3],
             default_channel_destination=DEFAULT_CHANNEL,
+            override_slack_channel=False,
         )
     ],
     expected_execution_properties={
         "had_group_by_alert": True,
         "had_group_by_table": False,
     },
 )
@@ -71,14 +72,15 @@
     name="one_fail_group_by_all_channel_selection_when_alert_is_not_a_model_is_default",
     default_grouping=GroupingType.BY_TABLE.value,
     list_of_alerts=[AL_FAIL_MODEL1_WITH_CHANNEL_NO_GROUPING_TS3],
     expected_alert_groups=[
         GroupOfAlertsByTable(
             alerts=[AL_FAIL_MODEL1_WITH_CHANNEL_NO_GROUPING_TS3],
             default_channel_destination=DEFAULT_CHANNEL,
+            override_slack_channel=False,
         )
     ],
     expected_execution_properties={
         "had_group_by_alert": False,
         "had_group_by_table": True,
     },
 )
@@ -92,14 +94,15 @@
     expected_alert_groups=[
         GroupOfAlertsByTable(
             alerts=[
                 AL_FAIL_MODEL1_WITH_CHANNEL_NO_GROUPING_TS3,
                 AL_WARN_MODEL1_NO_CHANNEL_NO_GROUPING_TS3,
             ],
             default_channel_destination=DEFAULT_CHANNEL,
+            override_slack_channel=False,
         )
     ],
     expected_execution_properties={
         "had_group_by_alert": False,
         "had_group_by_table": True,
     },
 )
@@ -114,18 +117,20 @@
     expected_alert_groups=[
         GroupOfAlertsByTable(
             alerts=[
                 AL_FAIL_MODEL1_WITH_CHANNEL_NO_GROUPING_TS3,
                 AL_WARN_MODEL1_NO_CHANNEL_NO_GROUPING_TS3,
             ],
             default_channel_destination=DEFAULT_CHANNEL,
+            override_slack_channel=False,
         ),
         GroupOfAlertsByTable(
             alerts=[AL_FAIL_MODEL2_NO_CHANNEL_NO_GROUPING_TS3],
             default_channel_destination=DEFAULT_CHANNEL,
+            override_slack_channel=False,
         ),
     ],
     expected_execution_properties={
         "had_group_by_alert": False,
         "had_group_by_table": True,
     },
 )
@@ -138,25 +143,28 @@
         AL_FAIL_MODEL2_NO_CHANNEL_NO_GROUPING_TS3,
         AL_FAIL_MODEL2_NO_CHANNEL_WITH_GROUPING_BY_ALERT_TS2,
     ],
     expected_alert_groups=[
         GroupOfAlertsBySingleAlert(
             alerts=[AL_FAIL_MODEL2_NO_CHANNEL_WITH_GROUPING_BY_ALERT_TS2],
             default_channel_destination=DEFAULT_CHANNEL,
+            override_slack_channel=False,
         ),
         GroupOfAlertsByTable(
             alerts=[
                 AL_FAIL_MODEL1_WITH_CHANNEL_NO_GROUPING_TS3,
                 AL_WARN_MODEL1_NO_CHANNEL_NO_GROUPING_TS3,
             ],
             default_channel_destination=DEFAULT_CHANNEL,
+            override_slack_channel=False,
         ),
         GroupOfAlertsByTable(
             alerts=[AL_FAIL_MODEL2_NO_CHANNEL_NO_GROUPING_TS3],
             default_channel_destination=DEFAULT_CHANNEL,
+            override_slack_channel=False,
         ),
     ],
     expected_execution_properties={
         "had_group_by_alert": True,
         "had_group_by_table": True,
     },
 )
@@ -176,29 +184,33 @@
         GroupOfAlertsByTable(
             alerts=[
                 AL_FAIL_MODEL2_NO_CHANNEL_NO_GROUPING_TS3,
                 AL_FAIL_MODEL2_WITH_CHANNEL_IN_MODEL_META_WITH_GROUPING_BY_TABLE_TS2,
                 AL_ERROR_MODEL2_NO_CHANNEL_WITH_GROUPING_BY_TABLE_TS1,
             ],
             default_channel_destination=DEFAULT_CHANNEL,
+            override_slack_channel=False,
         ),
         GroupOfAlertsBySingleAlert(
             alerts=[AL_ERROR_MODEL3_NO_CHANNEL_WITH_MODEL_META_GROUPING_BY_ALERT_TS1],
             default_channel_destination=DEFAULT_CHANNEL,
+            override_slack_channel=False,
         ),
         GroupOfAlertsBySingleAlert(
             alerts=[AL_FAIL_MODEL2_NO_CHANNEL_WITH_GROUPING_BY_ALERT_TS2],
             default_channel_destination=DEFAULT_CHANNEL,
+            override_slack_channel=False,
         ),
         GroupOfAlertsByTable(
             alerts=[
                 AL_WARN_MODEL1_NO_CHANNEL_NO_GROUPING_TS3,
                 AL_FAIL_MODEL1_WITH_CHANNEL_NO_GROUPING_TS3,
             ],
             default_channel_destination=DEFAULT_CHANNEL,
+            override_slack_channel=False,
         ),
     ],
     expected_execution_properties={
         "had_group_by_alert": True,
         "had_group_by_table": True,
     },
 )
@@ -241,14 +253,15 @@
         )
 
 
 @Parametrization.autodetect_parameters()
 @Parametrization.default_parameters(
     grouping_class=GroupOfAlertsBySingleAlert,
     default_channel=DEFAULT_CHANNEL,
+    override_channel=False,
     default_env="dev",
     expected_owners=None,
     expected_tags=None,
     expected_subs=None,
     expected_warnings=None,
     expected_fails=None,
     expected_errors=None,
@@ -263,14 +276,21 @@
 @Parametrization.case(
     name="single_alert_with_non_default_channel_goes_to_non_default_channel",
     grouping_class=GroupOfAlertsBySingleAlert,
     alerts_list=[AL_FAIL_MODEL1_WITH_CHANNEL_NO_GROUPING_TS3],
     expected_channel=OTHER_CHANNEL,
 )
 @Parametrization.case(
+    name="single alert with non-default channel and override_channel=True goes to default channel",
+    override_channel=True,
+    grouping_class=GroupOfAlertsBySingleAlert,
+    alerts_list=[AL_FAIL_MODEL1_WITH_CHANNEL_NO_GROUPING_TS3],
+    expected_channel=DEFAULT_CHANNEL,
+)
+@Parametrization.case(
     name="group_by_table_forces_use_of_the_model_channel",
     grouping_class=GroupOfAlertsByTable,
     alerts_list=[
         AL_FAIL_MODEL2_WITH_CHANNEL_IN_MODEL_META_WITH_GROUPING_BY_TABLE_TS2,
         AL_ERROR_MODEL2_NO_CHANNEL_WITH_GROUPING_BY_TABLE_TS1,
     ],
     expected_channel=OTHER_CHANNEL,
@@ -281,14 +301,24 @@
     alerts_list=[
         AL_FAIL_MODEL2_WITH_CHANNEL_IN_MODEL_META_WITH_GROUPING_BY_TABLE_TS2,
         AL_ERROR_MODEL2_NO_CHANNEL_WITH_GROUPING_BY_TABLE_TS1,
     ],
     expected_channel=OTHER_CHANNEL,
 )
 @Parametrization.case(
+    name="like previous, but with override_channel - should use the cli (default) channel",
+    grouping_class=GroupOfAlertsByTable,
+    alerts_list=[
+        AL_FAIL_MODEL2_WITH_CHANNEL_IN_MODEL_META_WITH_GROUPING_BY_TABLE_TS2,
+        AL_ERROR_MODEL2_NO_CHANNEL_WITH_GROUPING_BY_TABLE_TS1,
+    ],
+    override_channel=True,
+    expected_channel=DEFAULT_CHANNEL,
+)
+@Parametrization.case(
     name="owners_are_deduplicated",
     grouping_class=GroupOfAlertsByTable,
     alerts_list=[
         AL_WARN_MODEL1_NO_CHANNEL_NO_GROUPING_TS3,
         AL_FAIL_MODEL1_WITH_CHANNEL_NO_GROUPING_TS3,
     ],
     expected_owners=[OWNER_1, OWNER_2, OWNER_3],
@@ -322,25 +352,31 @@
         AL_FAIL_MODEL2_WITH_CHANNEL_IN_MODEL_META_WITH_GROUPING_BY_TABLE_TS2,
     ],
 )
 def test_alert_group_construction(
     grouping_class,
     alerts_list,
     default_channel,
+    override_channel,
     default_env,
     expected_owners,
     expected_tags,
     expected_subs,
     expected_warnings,
     expected_fails,
     expected_errors,
     expected_channel,
 ):
     # business logic
-    alerts_group = grouping_class(alerts_list, default_channel, env=default_env)
+    alerts_group = grouping_class(
+        alerts_list,
+        default_channel,
+        override_slack_channel=override_channel,
+        env=default_env,
+    )
 
     # assertions
     if expected_owners is not None:
         assert sorted(
             alerts_group._components_to_attention_required[OwnersComponent].split(", ")
         ) == sorted(expected_owners)
     if expected_tags is not None:
```

### Comparing `elementary-data-0.9.1/tests/unit/monitor/alerts/test_malformed_alert.py` & `elementary-data-0.9.2/tests/unit/monitor/alerts/test_malformed_alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/tests/unit/monitor/alerts/test_normalized_alert.py` & `elementary-data-0.9.2/tests/unit/monitor/alerts/test_normalized_alert.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/tests/unit/monitor/alerts/test_slack_alert_message_builder.py` & `elementary-data-0.9.2/tests/unit/monitor/alerts/test_slack_alert_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/tests/unit/monitor/api/alerts/test_alert_filters.py` & `elementary-data-0.9.2/tests/unit/monitor/api/alerts/test_alert_filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,72 @@
 from elementary.monitor.alerts.malformed import MalformedAlert
 from elementary.monitor.alerts.model import ModelAlert
 from elementary.monitor.alerts.test import TestAlert
 from elementary.monitor.api.alerts.alert_filters import (
     _filter_alerts_by_model,
     _filter_alerts_by_node_names,
     _filter_alerts_by_owner,
+    _filter_alerts_by_resource_type,
+    _filter_alerts_by_status,
     _filter_alerts_by_tag,
     filter_alerts,
 )
-from elementary.monitor.data_monitoring.schema import SelectorFilterSchema
+from elementary.monitor.data_monitoring.schema import (
+    ResourceType,
+    SelectorFilterSchema,
+    Status,
+)
 
 
 def initial_alerts():
     test_alerts = [
         TestAlert(
             id="1",
             alert_class_id="test_id_1",
             model_unique_id="elementary.model_id_1",
             test_unique_id="test_id_1",
             test_name="test_1",
             test_created_at="2022-10-10 10:10:10",
             tags='["one", "two"]',
             owners='["jeff", "john"]',
+            status="fail",
         ),
         TestAlert(
             id="2",
             alert_class_id="test_id_2",
             model_unique_id="elementary.model_id_1",
             test_unique_id="test_id_2",
             test_name="test_2",
             test_created_at="2022-10-10 09:10:10",
             tags='["three"]',
             owners='["jeff", "john"]',
+            status="fail",
         ),
         TestAlert(
             id="3",
             alert_class_id="test_id_3",
             model_unique_id="elementary.model_id_2",
             test_unique_id="test_id_3",
             test_name="test_3",
             test_created_at="2022-10-10 10:10:10",
             # invalid tag
             tags="one",
             owners='["john"]',
+            status="fail",
         ),
         TestAlert(
             id="4",
             alert_class_id="test_id_4",
             model_unique_id="elementary.model_id_2",
             test_unique_id="test_id_4",
             test_name="test_4",
             test_created_at="2022-10-10 09:10:10",
             tags='["three", "four"]',
             owners='["jeff"]',
+            status="warn",
         ),
     ]
     model_alerts = [
         ModelAlert(
             id="1",
             alert_class_id="elementary.model_id_1",
             model_unique_id="elementary.model_id_1",
@@ -66,14 +76,15 @@
             materialization="table",
             message="",
             full_refresh=False,
             detected_at="2022-10-10 10:00:00",
             alert_suppression_interval=0,
             tags='["one", "two"]',
             owners='["jeff", "john"]',
+            status="error",
         ),
         ModelAlert(
             id="2",
             alert_class_id="elementary.model_id_1",
             model_unique_id="elementary.model_id_1",
             alias="modely",
             path="my/path",
@@ -81,14 +92,15 @@
             materialization="table",
             message="",
             full_refresh=False,
             detected_at="2022-10-10 09:00:00",
             alert_suppression_interval=3,
             tags='["three"]',
             owners='["john"]',
+            status="error",
         ),
         ModelAlert(
             id="3",
             alert_class_id="elementary.model_id_2",
             model_unique_id="elementary.model_id_2",
             alias="model2",
             path="my/path2",
@@ -96,28 +108,30 @@
             materialization="table",
             message="",
             full_refresh=False,
             detected_at="2022-10-10 08:00:00",
             alert_suppression_interval=1,
             tags='["three", "four"]',
             owners='["jeff"]',
+            status="skipped",
         ),
     ]
     malformed_alerts = [
         MalformedAlert(
             id="1",
             data=dict(
                 id="1",
                 alert_class_id="test_id_1",
                 model_unique_id="elementary.model_id_1",
                 test_unique_id="test_id_1",
                 test_name="test_1",
                 test_created_at="2022-10-10 10:10:10",
                 tags='["one", "two"]',
                 owners='["jeff", "john"]',
+                status="fail",
             ),
         ),
         MalformedAlert(
             id="2",
             data=dict(
                 id="2",
                 alert_class_id="elementary.model_id_1",
@@ -128,38 +142,39 @@
                 materialization="table",
                 message="",
                 full_refresh=False,
                 detected_at="2022-10-10 09:00:00",
                 alert_suppression_interval=3,
                 tags='["three"]',
                 owners='["john"]',
+                status="fail",
             ),
         ),
     ]
     return test_alerts, model_alerts, malformed_alerts
 
 
 def test_filter_alerts():
     test_alerts, model_alerts, malformed_alerts = initial_alerts()
 
-    # Test that empty filter returns all of the alerts.
+    # Test that empty filter returns all of the alerts except for skipped.
     filter = SelectorFilterSchema()
     filter_test_alerts = filter_alerts(test_alerts, filter)
     filter_model_alerts = filter_alerts(model_alerts, filter)
     filter_malformed_alerts = filter_alerts(malformed_alerts, filter)
     assert len(filter_test_alerts) == len(test_alerts)
-    assert len(filter_model_alerts) == len(model_alerts)
+    assert len(filter_model_alerts) == len(model_alerts) - 1  # 1 skipped model alert
     assert len(filter_malformed_alerts) == len(malformed_alerts)
 
     # Test that passing no filter returns all of the alerts.
     filter_test_alerts = filter_alerts(test_alerts)
     filter_model_alerts = filter_alerts(model_alerts)
     filter_malformed_alerts = filter_alerts(malformed_alerts)
     assert len(filter_test_alerts) == len(test_alerts)
-    assert len(filter_model_alerts) == len(model_alerts)
+    assert len(filter_model_alerts) == len(model_alerts) - 1  # 1 skipped model alert
     assert len(filter_malformed_alerts) == len(malformed_alerts)
 
     # Test that filter with unsupported selector returns no alert
     filter = SelectorFilterSchema(last_invocation=True, selector="last_invocation")
     filter_test_alerts = filter_alerts(test_alerts, filter)
     filter_model_alerts = filter_alerts(model_alerts, filter)
     filter_malformed_alerts = filter_alerts(malformed_alerts, filter)
@@ -300,7 +315,49 @@
     assert len(filter_model_alerts) == 0
     assert len(filter_malformed_alerts) == 0
 
     filter = SelectorFilterSchema(node_names=["test_1"])
     filter_malformed_alerts = _filter_alerts_by_node_names(malformed_alerts, filter)
     assert len(filter_malformed_alerts) == 1
     assert filter_malformed_alerts[0].id == "1"
+
+
+def test_filter_alerts_by_statuses():
+    test_alerts, model_alerts, malformed_alerts = initial_alerts()
+
+    filter = SelectorFilterSchema(statuses=[Status.WARN])
+    filter_test_alerts = _filter_alerts_by_status(test_alerts, filter)
+    filter_model_alerts = _filter_alerts_by_status(model_alerts, filter)
+    filter_malformed_alerts = _filter_alerts_by_status(malformed_alerts, filter)
+    assert len(filter_test_alerts) == 1
+    assert filter_test_alerts[0].id == "4"
+    assert len(filter_model_alerts) == 0
+    assert len(filter_malformed_alerts) == 0
+
+    filter = SelectorFilterSchema(statuses=[Status.ERROR, Status.SKIPPED])
+    filter_test_alerts = _filter_alerts_by_status(test_alerts, filter)
+    filter_model_alerts = _filter_alerts_by_status(model_alerts, filter)
+    filter_malformed_alerts = _filter_alerts_by_status(malformed_alerts, filter)
+    assert len(filter_test_alerts) == 0
+    assert len(filter_model_alerts) == 3
+    assert len(filter_malformed_alerts) == 0
+
+    filter = SelectorFilterSchema(statuses=[Status.FAIL, Status.WARN])
+    filter_test_alerts = _filter_alerts_by_status(test_alerts, filter)
+    filter_model_alerts = _filter_alerts_by_status(model_alerts, filter)
+    filter_malformed_alerts = _filter_alerts_by_status(malformed_alerts, filter)
+    assert len(filter_test_alerts) == 4
+    assert len(filter_model_alerts) == 0
+    assert len(filter_malformed_alerts) == 2
+
+
+def test_filter_alerts_by_resource_types():
+    test_alerts, model_alerts, malformed_alerts = initial_alerts()
+    all_alerts = test_alerts + model_alerts + malformed_alerts
+
+    filter = SelectorFilterSchema(resource_types=[ResourceType.TEST])
+    filter_test_alerts = _filter_alerts_by_resource_type(all_alerts, filter)
+    assert filter_test_alerts == test_alerts
+
+    filter = SelectorFilterSchema(resource_types=[ResourceType.MODEL])
+    filter_test_alerts = _filter_alerts_by_resource_type(all_alerts, filter)
+    assert filter_test_alerts == model_alerts
```

### Comparing `elementary-data-0.9.1/tests/unit/monitor/api/alerts/test_alerts_api.py` & `elementary-data-0.9.2/tests/unit/monitor/api/alerts/test_alerts_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,20 +17,18 @@
 
     test_alerts = alerts_api_mock.alerts_fetcher.query_pending_test_alerts()
     model_alerts = alerts_api_mock.alerts_fetcher.query_pending_model_alerts()
 
     suppressed_test_alerts = alerts_api_mock._get_suppressed_alerts(
         test_alerts,
         last_test_alert_sent_times,
-        alerts_api_mock.global_suppression_interval,
     )
     suppressed_model_alerts = alerts_api_mock._get_suppressed_alerts(
         model_alerts,
         last_model_alert_sent_times,
-        alerts_api_mock.global_suppression_interval,
     )
 
     assert json.dumps(suppressed_test_alerts, sort_keys=True) == json.dumps(
         ["alert_id_1"], sort_keys=True
     )
     assert json.dumps(suppressed_model_alerts, sort_keys=True) == json.dumps(
         ["alert_id_1"], sort_keys=True
@@ -39,29 +37,41 @@
 
 @Parametrization.autodetect_parameters()
 @Parametrization.case(
     name="meta is none- cli wins",
     cli_interval=1,
     alert_interval=None,
     expected_interval=1,
+    override_suppression_interval=False,
 )
 @Parametrization.case(
     name="meta is not none- meta wins",
     cli_interval=2,
     alert_interval=10,
     expected_interval=10,
+    override_suppression_interval=False,
+)
+@Parametrization.case(
+    name="meta is not none but override is set- cli wins",
+    cli_interval=2,
+    alert_interval=10,
+    expected_interval=2,
+    override_suppression_interval=True,
 )
 def test_get_suppression_interval(
     alerts_api_mock: MockAlertsAPI,
     cli_interval: int,
     alert_interval: Optional[int],
+    override_suppression_interval: bool,
     expected_interval: Optional[int],
 ):
     assert (
-        alerts_api_mock._get_suppression_interval(alert_interval, cli_interval)
+        alerts_api_mock._get_suppression_interval(
+            alert_interval, cli_interval, override_suppression_interval
+        )
         == expected_interval
     )
 
 
 def test_get_latest_alerts(alerts_api_mock: MockAlertsAPI):
     test_alerts = alerts_api_mock.alerts_fetcher.query_pending_test_alerts()
     model_alerts = alerts_api_mock.alerts_fetcher.query_pending_model_alerts()
```

### Comparing `elementary-data-0.9.1/tests/unit/monitor/api/tests/test_tests_api.py` & `elementary-data-0.9.2/tests/unit/monitor/api/tests/test_tests_api.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py` & `elementary-data-0.9.2/tests/unit/monitor/data_monitoring/report/test_slack_report_summary_message_builder.py`

 * *Files identical despite different names*

### Comparing `elementary-data-0.9.1/tests/unit/monitor/data_monitoring/test_selector_filter.py` & `elementary-data-0.9.2/tests/unit/monitor/data_monitoring/test_selector_filter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from unittest import mock
 
 import pytest
 
+from elementary.monitor.data_monitoring.schema import ResourceType, Status
 from elementary.monitor.data_monitoring.selector_filter import SelectorFilter
 from tests.mocks.anonymous_tracking_mock import MockAnonymousTracking
 from tests.mocks.dbt_runner_mock import MockDbtRunner
 
 
 def test_parse_selector_with_user_dbt_runner(dbt_runner_mock, anonymous_tracking_mock):
     dbt_runner_mock.ls = mock.Mock(return_value=[])
@@ -62,14 +63,41 @@
     assert (
         data_monitoring_filter_with_user_dbt_runner.get_filter().model == "mock_model"
     )
     assert (
         data_monitoring_filter_with_user_dbt_runner.get_selector() == "model:mock_model"
     )
 
+    # status selector
+    data_monitoring_filter_with_user_dbt_runner = SelectorFilter(
+        tracking=anonymous_tracking_mock,
+        selector="statuses:fail,error",
+    )
+    assert data_monitoring_filter_with_user_dbt_runner.get_filter().statuses == [
+        Status.FAIL,
+        Status.ERROR,
+    ]
+    assert (
+        data_monitoring_filter_with_user_dbt_runner.get_selector()
+        == "statuses:fail,error"
+    )
+
+    # resource type selector
+    data_monitoring_filter_with_user_dbt_runner = SelectorFilter(
+        tracking=anonymous_tracking_mock,
+        selector="resource_types:model",
+    )
+    assert data_monitoring_filter_with_user_dbt_runner.get_filter().resource_types == [
+        ResourceType.MODEL
+    ]
+    assert (
+        data_monitoring_filter_with_user_dbt_runner.get_selector()
+        == "resource_types:model"
+    )
+
     # invocation_id selector
     data_monitoring_filter_with_user_dbt_runner = SelectorFilter(
         tracking=anonymous_tracking_mock,
         selector="invocation_id:mock_invocation_id",
     )
     assert (
         data_monitoring_filter_with_user_dbt_runner.get_filter().invocation_id
@@ -114,28 +142,25 @@
     )
 
     # unsupported selector
     data_monitoring_filter_with_user_dbt_runner = SelectorFilter(
         tracking=anonymous_tracking_mock,
         selector="blabla:blublu",
     )
-    assert data_monitoring_filter_with_user_dbt_runner.get_filter().tag is None
-    assert data_monitoring_filter_with_user_dbt_runner.get_filter().owner is None
-    assert data_monitoring_filter_with_user_dbt_runner.get_filter().model is None
-    assert (
-        data_monitoring_filter_with_user_dbt_runner.get_filter().last_invocation
-        is False
-    )
-    assert (
-        data_monitoring_filter_with_user_dbt_runner.get_filter().invocation_id is None
-    )
-    assert (
-        data_monitoring_filter_with_user_dbt_runner.get_filter().invocation_time is None
-    )
-    assert data_monitoring_filter_with_user_dbt_runner.get_filter().node_names is None
+    dbt_runner_get_filter = data_monitoring_filter_with_user_dbt_runner.get_filter()
+    assert dbt_runner_get_filter.tag is None
+    assert dbt_runner_get_filter.owner is None
+    assert dbt_runner_get_filter.model is None
+    assert dbt_runner_get_filter.last_invocation is False
+    assert dbt_runner_get_filter.invocation_id is None
+    assert dbt_runner_get_filter.invocation_time is None
+    assert dbt_runner_get_filter.node_names is None
+    assert dbt_runner_get_filter.resource_types is None
+    assert dbt_runner_get_filter.statuses == []
+    assert data_monitoring_filter_with_user_dbt_runner.get_selector() == "blabla:blublu"
 
 
 @pytest.fixture
 def dbt_runner_mock() -> MockDbtRunner:
     return MockDbtRunner()
```

### Comparing `elementary-data-0.9.1/tests/unit/monitor/fetchers/test_alerts_fetcher.py` & `elementary-data-0.9.2/tests/unit/monitor/fetchers/test_alerts_fetcher.py`

 * *Files identical despite different names*

