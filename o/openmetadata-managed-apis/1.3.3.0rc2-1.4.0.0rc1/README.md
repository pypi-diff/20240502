# Comparing `tmp/openmetadata_managed_apis-1.3.3.0rc2.tar.gz` & `tmp/openmetadata_managed_apis-1.4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmetadata_managed_apis-1.3.3.0rc2.tar", last modified: Tue Apr 16 13:33:08 2024, max compression
+gzip compressed data, was "openmetadata_managed_apis-1.4.0.0rc1.tar", last modified: Thu May  2 07:45:49 2024, max compression
```

## Comparing `openmetadata_managed_apis-1.3.3.0rc2.tar` & `openmetadata_managed_apis-1.4.0.0rc1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:33:08.218746 openmetadata_managed_apis-1.3.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21785 2024-04-16 13:33:08.218746 openmetadata_managed_apis-1.3.3.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:33:08.210746 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:33:08.210746 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/apis_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:33:08.214746 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/disable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/enable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/health_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/kill.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/last_dag_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/run_automation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:33:08.214746 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/kill_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/last_dag_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:33:08.214746 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/resources/dag_runner.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:33:08.214746 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:33:08.214746 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/views/rest_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:33:08.206746 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/views/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:33:08.214746 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/views/templates/rest_api/
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/views/templates/rest_api/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:33:08.214746 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:33:08.218746 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/application.py
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/data_insight.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/dbt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/es_reindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/workflow_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/workflow_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:33:08.218746 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21785 2024-04-16 13:33:08.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-16 13:33:08.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:33:08.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-16 13:33:08.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-16 13:33:08.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-16 13:33:08.000000 openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-16 13:31:43.000000 openmetadata_managed_apis-1.3.3.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:33:08.218746 openmetadata_managed_apis-1.3.3.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:45:49.479345 openmetadata_managed_apis-1.4.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21785 2024-05-02 07:45:49.479345 openmetadata_managed_apis-1.4.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:45:49.463345 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:45:49.467345 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/apis_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:45:49.471345 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/health_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/kill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/last_dag_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/run_automation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:45:49.471345 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/kill_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/last_dag_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:45:49.471345 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/resources/dag_runner.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:45:49.471345 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:45:49.471345 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/views/rest_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:45:49.463345 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/views/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:45:49.471345 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/views/templates/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/views/templates/rest_api/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:45:49.475345 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:45:49.475345 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13442 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/data_insight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/es_reindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/workflow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/workflow_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:45:49.475345 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21785 2024-05-02 07:45:49.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-02 07:45:49.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 07:45:49.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 07:45:49.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 07:45:49.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 07:45:49.000000 openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-02 07:43:33.000000 openmetadata_managed_apis-1.4.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 07:45:49.479345 openmetadata_managed_apis-1.4.0.0rc1/setup.cfg
```

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/LICENSE` & `openmetadata_managed_apis-1.4.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/PKG-INFO` & `openmetadata_managed_apis-1.4.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmetadata_managed_apis
-Version: 1.3.3.0rc2
+Version: 1.4.0.0rc1
 Summary: Airflow REST APIs to create and manage DAGS
 Author: OpenMetadata Committers
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/README.md` & `openmetadata_managed_apis-1.4.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/__init__.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/__init__.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/apis_metadata.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/apis_metadata.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/app.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/app.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/config.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/config.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/error_handlers.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/error_handlers.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/response.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/response.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/delete.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/delete.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/deploy.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/deploy.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/disable.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/disable.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/enable.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/enable.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/health.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/health.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/health_auth.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/health_auth.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/ip.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/ip.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/kill.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/kill.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/last_dag_logs.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/last_dag_logs.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/run_automation.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/run_automation.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/status.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/status.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/routes/trigger.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/routes/trigger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/api/utils.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/api/utils.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/delete.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/delete.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/deploy.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/deploy.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/health.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/health.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/kill_all.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/kill_all.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/last_dag_logs.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/last_dag_logs.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/state.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/state.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/status.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/status.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/operations/trigger.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/operations/trigger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/plugin.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/plugin.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/utils/logger.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/utils/parser.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/utils/parser.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/views/rest_api.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/views/rest_api.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/views/templates/rest_api/index.html` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/views/templates/rest_api/index.html`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/config.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/config.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/application.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/application.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/common.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/common.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/data_insight.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/data_insight.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/dbt.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/dbt.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/es_reindex.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/es_reindex.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/lineage.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/lineage.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/metadata.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/metadata.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/profiler.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/profiler.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/registry.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/registry.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/test_suite.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/test_suite.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/ingestion/usage.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/ingestion/usage.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/workflow_builder.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/workflow_builder.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis/workflows/workflow_factory.py` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis/workflows/workflow_factory.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis.egg-info/PKG-INFO` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmetadata_managed_apis
-Version: 1.3.3.0rc2
+Version: 1.4.0.0rc1
 Summary: Airflow REST APIs to create and manage DAGS
 Author: OpenMetadata Committers
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/openmetadata_managed_apis.egg-info/SOURCES.txt` & `openmetadata_managed_apis-1.4.0.0rc1/openmetadata_managed_apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.3.3.0rc2/pyproject.toml` & `openmetadata_managed_apis-1.4.0.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 # We will keep handling dependencies in setup.py
 # since it helps us organize and isolate version management
 [project]
 name = "openmetadata_managed_apis"
-version = "1.3.3.0-rc2"
+version = "1.4.0.0-rc1"
 readme = "README.md"
 authors = [
     {name = "OpenMetadata Committers"}
 ]
 license = {file = "LICENSE"}
 description = "Airflow REST APIs to create and manage DAGS"
 requires-python = ">=3.8"
```

