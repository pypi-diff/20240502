# Comparing `tmp/hypergo-0.3.8.tar.gz` & `tmp/hypergo-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypergo-0.3.8.tar", last modified: Tue Apr 30 14:54:02 2024, max compression
+gzip compressed data, was "hypergo-0.3.9.tar", last modified: Thu May  2 19:47:54 2024, max compression
```

## Comparing `hypergo-0.3.8.tar` & `hypergo-0.3.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:54:02.616351 hypergo-0.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:54:02.600351 hypergo-0.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:54:02.604351 hypergo-0.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-30 14:53:58.000000 hypergo-0.3.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-30 14:53:58.000000 hypergo-0.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-30 14:53:58.000000 hypergo-0.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-30 14:53:58.000000 hypergo-0.3.8/BACKLOG.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:53:58.000000 hypergo-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-30 14:54:02.616351 hypergo-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 14:53:58.000000 hypergo-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-04-30 14:53:58.000000 hypergo-0.3.8/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-30 14:53:58.000000 hypergo-0.3.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:54:02.608351 hypergo-0.3.8/hypergo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/azure_service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/azure_service_bus_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:54:02.608351 hypergo-0.3.8/hypergo/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/connectors/azure_application_insights.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/hypergo_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/hypergo_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/hypergo_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:54:02.608351 hypergo-0.3.8/hypergo/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/loggers/azure_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/loggers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/loggers/hypergo_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:54:02.612351 hypergo-0.3.8/hypergo/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/metrics/base_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/metrics/custom_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/metrics/hypergo_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/stdio_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-30 14:53:58.000000 hypergo-0.3.8/hypergo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:54:02.616351 hypergo-0.3.8/hypergo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-30 14:54:02.000000 hypergo-0.3.8/hypergo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-30 14:54:02.000000 hypergo-0.3.8/hypergo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:54:02.000000 hypergo-0.3.8/hypergo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-30 14:54:02.000000 hypergo-0.3.8/hypergo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-30 14:54:02.000000 hypergo-0.3.8/hypergo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 14:54:02.000000 hypergo-0.3.8/hypergo.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2851 2024-04-30 14:53:58.000000 hypergo-0.3.8/lint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-30 14:53:58.000000 hypergo-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-30 14:54:02.616351 hypergo-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-30 14:53:58.000000 hypergo-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:54:02.612351 hypergo-0.3.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:54:02.604351 hypergo-0.3.8/tests/integration_pipeline/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:54:02.612351 hypergo-0.3.8/tests/integration_pipeline/input_binder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:54:02.612351 hypergo-0.3.8/tests/integration_pipeline/input_binder/input_binder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/integration_pipeline/input_binder/input_binder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/integration_pipeline/input_binder/input_binder/input_binder.json
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/integration_pipeline/input_binder/input_binder/input_binder.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/integration_pipeline/input_binder/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/integration_pipeline/input_binder/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:54:02.612351 hypergo-0.3.8/tests/integration_pipeline/result_checker/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/integration_pipeline/result_checker/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:54:02.616351 hypergo-0.3.8/tests/integration_pipeline/result_checker/result_checker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/integration_pipeline/result_checker/result_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/integration_pipeline/result_checker/result_checker/result_checker.json
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/integration_pipeline/result_checker/result_checker/result_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/integration_pipeline/result_checker/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/test.json
--rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/test_azure_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/test_azure_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/test_dynamic_input_bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/test_dynamic_routing_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/test_local_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/test_stdio_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-30 14:53:58.000000 hypergo-0.3.8/tests/test_utility_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:54.983234 hypergo-0.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:54.967234 hypergo-0.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:54.971234 hypergo-0.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-02 19:47:47.000000 hypergo-0.3.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-02 19:47:47.000000 hypergo-0.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-02 19:47:47.000000 hypergo-0.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-05-02 19:47:47.000000 hypergo-0.3.9/BACKLOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:47.000000 hypergo-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-02 19:47:54.983234 hypergo-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 19:47:47.000000 hypergo-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-05-02 19:47:47.000000 hypergo-0.3.9/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-02 19:47:47.000000 hypergo-0.3.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:54.975234 hypergo-0.3.9/hypergo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/azure_service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/azure_service_bus_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:54.979234 hypergo-0.3.9/hypergo/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/connectors/azure_application_insights.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/hypergo_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/hypergo_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/hypergo_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:54.979234 hypergo-0.3.9/hypergo/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/loggers/azure_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/loggers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/loggers/hypergo_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:54.979234 hypergo-0.3.9/hypergo/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/metrics/base_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/metrics/custom_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/metrics/hypergo_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/stdio_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-02 19:47:47.000000 hypergo-0.3.9/hypergo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:54.983234 hypergo-0.3.9/hypergo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-02 19:47:54.000000 hypergo-0.3.9/hypergo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-02 19:47:54.000000 hypergo-0.3.9/hypergo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:47:54.000000 hypergo-0.3.9/hypergo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 19:47:54.000000 hypergo-0.3.9/hypergo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-02 19:47:54.000000 hypergo-0.3.9/hypergo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 19:47:54.000000 hypergo-0.3.9/hypergo.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2851 2024-05-02 19:47:47.000000 hypergo-0.3.9/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-02 19:47:47.000000 hypergo-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-02 19:47:54.983234 hypergo-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-02 19:47:47.000000 hypergo-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:54.979234 hypergo-0.3.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:54.971234 hypergo-0.3.9/tests/integration_pipeline/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:54.983234 hypergo-0.3.9/tests/integration_pipeline/input_binder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:54.983234 hypergo-0.3.9/tests/integration_pipeline/input_binder/input_binder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/integration_pipeline/input_binder/input_binder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/integration_pipeline/input_binder/input_binder/input_binder.json
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/integration_pipeline/input_binder/input_binder/input_binder.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/integration_pipeline/input_binder/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/integration_pipeline/input_binder/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:54.983234 hypergo-0.3.9/tests/integration_pipeline/result_checker/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/integration_pipeline/result_checker/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:54.983234 hypergo-0.3.9/tests/integration_pipeline/result_checker/result_checker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/integration_pipeline/result_checker/result_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/integration_pipeline/result_checker/result_checker/result_checker.json
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/integration_pipeline/result_checker/result_checker/result_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/integration_pipeline/result_checker/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/test.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/test_azure_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/test_azure_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/test_dynamic_input_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/test_dynamic_routing_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/test_local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/test_stdio_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-02 19:47:47.000000 hypergo-0.3.9/tests/test_utility_serialization.py
```

### Comparing `hypergo-0.3.8/.github/workflows/python-publish.yml` & `hypergo-0.3.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/.gitignore` & `hypergo-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/BACKLOG.md` & `hypergo-0.3.9/BACKLOG.md`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/PKG-INFO` & `hypergo-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypergo
-Version: 0.3.8
+Version: 0.3.9
 Summary: Project for service bus
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: glom
 Requires-Dist: pydash
 Requires-Dist: azure-servicebus
```

### Comparing `hypergo-0.3.8/RELEASE_NOTES.md` & `hypergo-0.3.9/RELEASE_NOTES.md`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/azure_service_bus_connection.py` & `hypergo-0.3.9/hypergo/azure_service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/config.py` & `hypergo-0.3.9/hypergo/config.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/connection.py` & `hypergo-0.3.9/hypergo/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         executor: Executor = Executor(config, **kwargs)
         self.__send_message(executor=executor, message=message, config=config)
 
     @collect_metrics
     def __send_message(self, executor: Executor, message: MessageType, config: ConfigType) -> None:
         for execution in executor.execute(message):
             message = cast(MessageType, execution)
-            if not message.get("body"):
+            if message.get("body") is None:
                 logger.debug(f"Skipping message with null body. Routingkey: {message.get('routingkey')}")
                 continue
             self.send(message, config["namespace"])
 
     @abstractmethod
     def send(self, message: MessageType, namespace: str) -> None:
         pass
```

### Comparing `hypergo-0.3.8/hypergo/connectors/azure_application_insights.py` & `hypergo-0.3.9/hypergo/connectors/azure_application_insights.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/executor.py` & `hypergo-0.3.9/hypergo/executor.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/graph.py` & `hypergo-0.3.9/hypergo/graph.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/hypergo_cli.py` & `hypergo-0.3.9/hypergo/hypergo_cli.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/hypergo_click.py` & `hypergo-0.3.9/hypergo/hypergo_click.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/hypergo_cmd.py` & `hypergo-0.3.9/hypergo/hypergo_cmd.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/local_storage.py` & `hypergo-0.3.9/hypergo/local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/logger.py` & `hypergo-0.3.9/hypergo/logger.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/loggers/azure_logger.py` & `hypergo-0.3.9/hypergo/loggers/azure_logger.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/loggers/base_logger.py` & `hypergo-0.3.9/hypergo/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/loggers/hypergo_logger.py` & `hypergo-0.3.9/hypergo/loggers/hypergo_logger.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/mapping.py` & `hypergo-0.3.9/hypergo/mapping.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/message.py` & `hypergo-0.3.9/hypergo/message.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/metrics/base_metrics.py` & `hypergo-0.3.9/hypergo/metrics/base_metrics.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/metrics/custom_metrics.py` & `hypergo-0.3.9/hypergo/metrics/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/metrics/hypergo_metrics.py` & `hypergo-0.3.9/hypergo/metrics/hypergo_metrics.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/monitor.py` & `hypergo-0.3.9/hypergo/monitor.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/stdio_connection.py` & `hypergo-0.3.9/hypergo/stdio_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/storage.py` & `hypergo-0.3.9/hypergo/storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/transaction.py` & `hypergo-0.3.9/hypergo/transaction.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/transform.py` & `hypergo-0.3.9/hypergo/transform.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/utility.py` & `hypergo-0.3.9/hypergo/utility.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo/version.py` & `hypergo-0.3.9/hypergo/version.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/hypergo.egg-info/PKG-INFO` & `hypergo-0.3.9/hypergo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypergo
-Version: 0.3.8
+Version: 0.3.9
 Summary: Project for service bus
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: glom
 Requires-Dist: pydash
 Requires-Dist: azure-servicebus
```

### Comparing `hypergo-0.3.8/hypergo.egg-info/SOURCES.txt` & `hypergo-0.3.9/hypergo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/lint.sh` & `hypergo-0.3.9/lint.sh`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/setup.cfg` & `hypergo-0.3.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hypergo
-version = 0.3.8
+version = 0.3.9
 description = Project for service bus
 long_description_content_type = text/markdown
 
 [options]
 packages = find:
 install_requires = 
 	pyyaml
```

### Comparing `hypergo-0.3.8/setup.py` & `hypergo-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 
 
 # Define the setup parameters
 setup(
     name='hypergo',
-    version='0.3.8',  # Enclose the version number in quotes
+    version='0.3.9',  # Enclose the version number in quotes
     description='Project for service bus',
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         "pyyaml",
 	    "glom",
 	    "pydash",
```

### Comparing `hypergo-0.3.8/tests/integration_pipeline/input_binder/input_binder/input_binder.json` & `hypergo-0.3.9/tests/integration_pipeline/input_binder/input_binder/input_binder.json`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/tests/integration_pipeline/result_checker/result_checker/result_checker.json` & `hypergo-0.3.9/tests/integration_pipeline/result_checker/result_checker/result_checker.json`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/tests/test.json` & `hypergo-0.3.9/tests/test.json`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/tests/test.yaml` & `hypergo-0.3.9/tests/test.yaml`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/tests/test_azure_logger.py` & `hypergo-0.3.9/tests/test_azure_logger.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/tests/test_azure_monitor.py` & `hypergo-0.3.9/tests/test_azure_monitor.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/tests/test_dynamic_input_bindings.py` & `hypergo-0.3.9/tests/test_dynamic_input_bindings.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/tests/test_dynamic_routing_key.py` & `hypergo-0.3.9/tests/test_dynamic_routing_key.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/tests/test_local_storage.py` & `hypergo-0.3.9/tests/test_local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/tests/test_message.py` & `hypergo-0.3.9/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/tests/test_stdio_monitor.py` & `hypergo-0.3.9/tests/test_stdio_monitor.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/tests/test_storage.py` & `hypergo-0.3.9/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/tests/test_utility.py` & `hypergo-0.3.9/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.3.8/tests/test_utility_serialization.py` & `hypergo-0.3.9/tests/test_utility_serialization.py`

 * *Files identical despite different names*

