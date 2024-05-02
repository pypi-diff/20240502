# Comparing `tmp/dagster-cloud-1.7.3.tar.gz` & `tmp/dagster-cloud-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-1.7.3.tar", last modified: Thu Apr 25 20:21:35 2024, max compression
+gzip compressed data, was "dagster-cloud-1.7.4.tar", last modified: Thu May  2 20:44:01 2024, max compression
```

## Comparing `dagster-cloud-1.7.3.tar` & `dagster-cloud-1.7.4.tar`

### file list

```diff
@@ -1,140 +1,138 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.897462 dagster-cloud-1.7.3/
--rw-r--r--   0 root         (0) root         (0)     4562 2024-04-25 20:21:35.897462 dagster-cloud-1.7.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.833463 dagster-cloud-1.7.3/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      160 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.833463 dagster-cloud-1.7.3/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)      796 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.837463 dagster-cloud-1.7.3/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7584 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45467 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1770 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.841463 dagster-cloud-1.7.3/dagster_cloud/anomaly_detection/
--rw-r--r--   0 root         (0) root         (0)      279 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/anomaly_detection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9296 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/anomaly_detection/defs.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/anomaly_detection/mutation.py
--rw-r--r--   0 root         (0) root         (0)     1986 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/anomaly_detection/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.841463 dagster-cloud-1.7.3/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19251 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.841463 dagster-cloud-1.7.3/dagster_cloud/artifacts/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/artifacts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.841463 dagster-cloud-1.7.3/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      248 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1242 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/auth/constants.py
--rw-r--r--   0 root         (0) root         (0)      455 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.845463 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/
--rw-r--r--   0 root         (0) root         (0)     1873 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.845463 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)      816 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py
--rw-r--r--   0 root         (0) root         (0)     7964 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     3234 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py
--rw-r--r--   0 root         (0) root         (0)      138 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/errors.py
--rw-r--r--   0 root         (0) root         (0)     2524 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/insights_utils.py
--rw-r--r--   0 root         (0) root         (0)    10835 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/metrics_utils.py
--rw-r--r--   0 root         (0) root         (0)     1403 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.849463 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5611 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py
--rw-r--r--   0 root         (0) root         (0)     5185 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     7064 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/definitions.py
--rw-r--r--   0 root         (0) root         (0)     9358 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py
--rw-r--r--   0 root         (0) root         (0)     3808 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.849463 dagster-cloud-1.7.3/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.853463 dagster-cloud-1.7.3/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3098 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.853463 dagster-cloud-1.7.3/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    17256 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.853463 dagster-cloud-1.7.3/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.857463 dagster-cloud-1.7.3/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    22345 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.857463 dagster-cloud-1.7.3/dagster_cloud/metrics/
--rw-r--r--   0 root         (0) root         (0)    10090 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/metrics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.857463 dagster-cloud-1.7.3/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.857463 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.861463 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3907 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9301 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5251 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3790 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.865463 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.865463 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     2115 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17843 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)    12797 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    15703 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     3322 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.865463 dagster-cloud-1.7.3/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1620 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.865463 dagster-cloud-1.7.3/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4247 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.869463 dagster-cloud-1.7.3/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1690 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.869463 dagster-cloud-1.7.3/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4753 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.873463 dagster-cloud-1.7.3/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16377 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    46580 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.873463 dagster-cloud-1.7.3/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6446 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    18839 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.873463 dagster-cloud-1.7.3/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1930 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     7575 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.877463 dagster-cloud-1.7.3/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2778 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4693 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/util/container_resources.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.877463 dagster-cloud-1.7.3/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.881463 dagster-cloud-1.7.3/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)    10918 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     6575 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     5319 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.881463 dagster-cloud-1.7.3/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12977 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      352 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.885463 dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28818 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    28623 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      534 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4126 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     2746 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.889463 dagster-cloud-1.7.3/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26248 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)     9825 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/kubernetes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.897462 dagster-cloud-1.7.3/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14248 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    83997 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1209 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:35.833463 dagster-cloud-1.7.3/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4562 2024-04-25 20:21:35.000000 dagster-cloud-1.7.3/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4274 2024-04-25 20:21:35.000000 dagster-cloud-1.7.3/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:21:35.000000 dagster-cloud-1.7.3/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      509 2024-04-25 20:21:35.000000 dagster-cloud-1.7.3/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-25 20:21:35.000000 dagster-cloud-1.7.3/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 20:21:35.897462 dagster-cloud-1.7.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3078 2024-04-25 20:08:52.000000 dagster-cloud-1.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.758723 dagster-cloud-1.7.4/
+-rw-r--r--   0 root         (0) root         (0)     4562 2024-05-02 20:44:01.758723 dagster-cloud-1.7.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.690724 dagster-cloud-1.7.4/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      316 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.694724 dagster-cloud-1.7.4/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)      796 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.694724 dagster-cloud-1.7.4/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45582 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.694724 dagster-cloud-1.7.4/dagster_cloud/anomaly_detection/
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/anomaly_detection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9296 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/anomaly_detection/defs.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/anomaly_detection/mutation.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/anomaly_detection/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.698724 dagster-cloud-1.7.4/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19251 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.698724 dagster-cloud-1.7.4/dagster_cloud/artifacts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/artifacts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.702724 dagster-cloud-1.7.4/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      248 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/auth/constants.py
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.706724 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/
+-rw-r--r--   0 root         (0) root         (0)     1873 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.706724 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7964 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     3234 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/insights_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4194 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/metrics_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.710724 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5611 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py
+-rw-r--r--   0 root         (0) root         (0)     5185 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/definitions.py
+-rw-r--r--   0 root         (0) root         (0)    10624 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.710724 dagster-cloud-1.7.4/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.714724 dagster-cloud-1.7.4/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.714724 dagster-cloud-1.7.4/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    17294 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.714724 dagster-cloud-1.7.4/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.718724 dagster-cloud-1.7.4/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    22345 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.718724 dagster-cloud-1.7.4/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.718724 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.722724 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3907 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9301 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.726724 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.726724 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17844 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)    12797 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    15703 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.730723 dagster-cloud-1.7.4/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.730723 dagster-cloud-1.7.4/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.730723 dagster-cloud-1.7.4/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.734723 dagster-cloud-1.7.4/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4753 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.738723 dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16377 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    46580 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.738723 dagster-cloud-1.7.4/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6446 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    18839 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.742723 dagster-cloud-1.7.4/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7575 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.742723 dagster-cloud-1.7.4/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/util/container_resources.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.742723 dagster-cloud-1.7.4/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.746723 dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)    10918 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     6575 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     5319 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.746723 dagster-cloud-1.7.4/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12977 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      352 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.750723 dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28818 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    28623 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.754723 dagster-cloud-1.7.4/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26248 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)     9825 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/kubernetes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.758723 dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14248 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    83997 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.690724 dagster-cloud-1.7.4/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4562 2024-05-02 20:44:01.000000 dagster-cloud-1.7.4/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4240 2024-05-02 20:44:01.000000 dagster-cloud-1.7.4/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:44:01.000000 dagster-cloud-1.7.4/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      509 2024-05-02 20:44:01.000000 dagster-cloud-1.7.4/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-02 20:44:01.000000 dagster-cloud-1.7.4/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 20:44:01.758723 dagster-cloud-1.7.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/setup.py
```

### Comparing `dagster-cloud-1.7.3/PKG-INFO` & `dagster-cloud-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.7.3
+Version: 1.7.4
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster-cloud-1.7.3/README.md` & `dagster-cloud-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/agent/__init__.py` & `dagster-cloud-1.7.4/dagster_cloud/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/agent/cli/__init__.py` & `dagster-cloud-1.7.4/dagster_cloud/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster-cloud-1.7.4/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,16 +309,17 @@
         if (
             self._last_heartbeat_time
             and (curr_time - self._last_heartbeat_time).total_seconds() < heartbeat_interval_seconds
         ):
             return
 
         errors = [
-            TimestampedError(timestamp.float_timestamp, error)
+            TimestampedError(timestamp.timestamp(), error)
             for (error, timestamp) in self._errors
+            if timestamp.timestamp() > curr_time.timestamp() - 60 * 60 * 24
         ]
 
         run_worker_statuses_dict = instance.user_code_launcher.get_cloud_run_worker_statuses(
             self._active_deployment_names
         )
 
         code_server_heartbeats_dict = instance.user_code_launcher.get_grpc_server_heartbeats()
@@ -333,15 +334,14 @@
                         agent_id=agent_uuid,
                         agent_label=instance.dagster_cloud_api_agent_label,
                         agent_type=(
                             type(instance.user_code_launcher).__name__
                             if instance.user_code_launcher
                             else None
                         ),
-                        errors=errors,
                         metadata=merge_dicts(
                             {AGENT_VERSION_LABEL: __version__},
                             {"image_tag": agent_image_tag} if agent_image_tag else {},
                             {
                                 "utilization_metrics": self._utilization_metrics
                                 if instance.user_code_launcher.agent_metrics_enabled
                                 else {}
@@ -368,14 +368,15 @@
 
         self._last_heartbeat_time = curr_time
 
         instance.organization_scoped_graphql_client().execute(
             ADD_AGENT_HEARTBEATS_MUTATION,
             variable_values={
                 "serializedAgentHeartbeats": serialized_agent_heartbeats,
+                "serializedErrors": [serialize_value(error) for error in errors],
             },
             idempotent_mutation=True,
         )
 
     @property
     def executor(self) -> ThreadPoolExecutor:
         return self._executor
```

### Comparing `dagster-cloud-1.7.3/dagster_cloud/agent/queries.py` & `dagster-cloud-1.7.4/dagster_cloud/agent/queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,17 +34,17 @@
             }
         }
     }
 """
 
 
 ADD_AGENT_HEARTBEATS_MUTATION = """
-    mutation AddAgentHeartbeats($serializedAgentHeartbeats: [AgentHeartbeatInput!]) {
+    mutation AddAgentHeartbeats($serializedAgentHeartbeats: [AgentHeartbeatInput!], $serializedErrors: [String!]) {
         userCloudAgent {
-            addAgentHeartbeats (serializedAgentHeartbeats: $serializedAgentHeartbeats) {
+            addAgentHeartbeats (serializedAgentHeartbeats: $serializedAgentHeartbeats, serializedErrors: $serializedErrors) {
                 ok
             }
         }
     }
 """
 
 GET_AGENTS_QUERY = """
```

### Comparing `dagster-cloud-1.7.3/dagster_cloud/anomaly_detection/defs.py` & `dagster-cloud-1.7.4/dagster_cloud/anomaly_detection/defs.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/anomaly_detection/types.py` & `dagster-cloud-1.7.4/dagster_cloud/anomaly_detection/types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/api/dagster_cloud_api.py` & `dagster-cloud-1.7.4/dagster_cloud/api/dagster_cloud_api.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/auth/constants.py` & `dagster-cloud-1.7.4/dagster_cloud/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/dagster_insights/__init__.py` & `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py` & `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py` & `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py` & `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/dagster_insights/insights_utils.py` & `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/insights_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/dagster_insights/metrics_utils.py` & `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,307 +1,292 @@
-import os
-import tempfile
-from typing import Any, Dict, Generator, List, NamedTuple, Optional, Tuple, Union
-
-import dagster._check as check
-import requests
-from dagster import AssetExecutionContext, DagsterInstance, OpExecutionContext
-from dagster._annotations import experimental
-from dagster_cloud_cli.core.errors import raise_http_error
-from dagster_cloud_cli.core.headers.auth import DagsterCloudInstanceScope
-from gql import Client, gql
-from gql.transport.requests import RequestsHTTPTransport
-
-from dagster_cloud.instance import DagsterCloudAgentInstance
-
-from .query import PUT_CLOUD_METRICS_MUTATION, PUT_COST_INFORMATION_MUTATION
-
-
-def _chunks(chunk_list: List[Any], length: int):
-    """Yield successive n-sized chunks from lst."""
-    for i in range(0, len(chunk_list), length):
-        yield chunk_list[i : i + length]
+import warnings
+from contextlib import contextmanager
+from io import StringIO
+from typing import (
+    Any,
+    Generator,
+    Iterable,
+    Iterator,
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
+
+import snowflake.connector
+from dagster import (
+    AssetExecutionContext,
+    AssetKey,
+    DagsterInvariantViolationError,
+    OpExecutionContext,
+    get_dagster_logger,
+)
+from dagster._annotations import experimental, public
+from dagster._check import CheckError
+from dagster._core.errors import DagsterInvalidPropertyError
+from dagster._core.storage.event_log.sql_event_log import SqlDbConnection
+from dagster_snowflake import SnowflakeConnection, SnowflakeResource
+from snowflake.connector.cursor import SnowflakeCursor
+
+from dagster_cloud.dagster_insights.insights_utils import (
+    get_current_context_and_asset_key,
+)
 
+from .snowflake_utils import meter_snowflake_query
 
-@experimental
-class DagsterMetric(NamedTuple):
-    """Experimental: This class gives information about a Metric.
-
-    Args:
-        metric_name (str): name of the metric
-        metric_value (float): value of the metric
-    """
 
-    metric_name: str
-    metric_value: float
+def get_current_context_and_asset_key_or_warn() -> (
+    Tuple[Union[OpExecutionContext, AssetExecutionContext, None], Optional[AssetKey]]
+):
+    try:
+        return get_current_context_and_asset_key()
+    except (DagsterInvalidPropertyError, DagsterInvariantViolationError, CheckError):
+        warnings.warn(
+            "Accessed InsightsSnowflakeResource outside of an Op or Asset context."
+            " This query may not be properly attributed."
+        )
+        return None, None
 
 
-def query_graphql_from_instance(
-    instance: DagsterInstance, query_text: str, variables=None
-) -> Dict[str, Any]:
-    headers = {}
+class InsightsSnowflakeCursor(SnowflakeCursor):
+    def __init__(self, *args, **kwargs) -> None:
+        self._asset_key = None
+        super().__init__(*args, **kwargs)
 
-    url, cloud_token = get_url_and_token_from_instance(instance)
+    def set_asset_key(self, asset_key: Optional[AssetKey]):
+        self._asset_key = asset_key
 
-    headers["Dagster-Cloud-API-Token"] = cloud_token
+    def execute(self, command: str, *args, **kwargs):
+        context, inferred_asset_key = get_current_context_and_asset_key_or_warn()
+        if not context:
+            return super().execute(command, *args, **kwargs)
 
-    transport = RequestsHTTPTransport(
-        url=url,
-        use_json=True,
-        timeout=300,
-        headers={"Dagster-Cloud-Api-Token": cloud_token},
-    )
-    client = Client(transport=transport, fetch_schema_from_transport=True)
-    return client.execute(gql(query_text), variable_values=variables or dict())
+        associated_asset_key = self._asset_key or inferred_asset_key
 
+        return super().execute(
+            meter_snowflake_query(context, command, associated_asset_key=associated_asset_key),
+            *args,
+            **kwargs,
+        )
 
-def get_url_and_token_from_instance(instance: DagsterInstance) -> Tuple[str, str]:
-    if not isinstance(instance, DagsterCloudAgentInstance):
-        raise RuntimeError("This asset only functions in a running Dagster Cloud instance")
 
-    return f"{instance.dagit_url}graphql", instance.dagster_cloud_agent_token
+class WrappedSnowflakeConnection(snowflake.connector.SnowflakeConnection):
+    def __init__(self, *args, asset_key: Optional[AssetKey] = None, **kwargs) -> None:
+        self._asset_key = asset_key
+        super().__init__(*args, **kwargs)
+
+    def execute_string(
+        self,
+        sql_text: str,
+        remove_comments: bool = False,
+        return_cursors: bool = True,
+        cursor_class: Type[SnowflakeCursor] = InsightsSnowflakeCursor,
+        **kwargs,
+    ) -> Iterable[SnowflakeCursor]:
+        return super().execute_string(
+            sql_text,
+            remove_comments,
+            return_cursors,
+            cursor_class,  # type: ignore  # (bad stubs)
+            **kwargs,
+        )
 
+    def execute_stream(
+        self,
+        stream: StringIO,
+        remove_comments: bool = False,
+        cursor_class: Type[SnowflakeCursor] = InsightsSnowflakeCursor,
+        **kwargs,
+    ) -> Generator[SnowflakeCursor, None, None]:
+        return super().execute_stream(stream, remove_comments, cursor_class, **kwargs)  # type: ignore  # (bad stubs)
+
+    def cursor(self, cursor_class=None) -> SnowflakeCursor:
+        if cursor_class is None:
+            cursor = cast(InsightsSnowflakeCursor, super().cursor(InsightsSnowflakeCursor))
+            cursor.set_asset_key(self._asset_key)
+        else:
+            cursor = super().cursor(cursor_class)
 
-def _cost_information_chunk_size() -> int:
-    return 10000
+        return cursor
 
 
-def chunk_by_opaque_id(
-    chunk_list: List[Tuple[str, float]], length: int
-) -> Generator[List[Tuple[str, float]], None, None]:
-    """Yield chunks of data. Groups by opaque_id so that
-    all metrics for a given opaque_id are in the same chunk.
-    Chunks will be of size `length` or less unless a single
-    opaque_id has more than `length` metrics.
+@experimental
+class InsightsSnowflakeResource(SnowflakeResource):
+    """A wrapper around :py:class:`SnowflakeResource` which automatically tags
+    Snowflake queries with comments which can be used to attribute Snowflake
+    query costs to Dagster jobs and assets.
+
+    If connector configuration is not set, InsightsSnowflakeResource.get_connection() will return a
+    `snowflake.connector.Connection <https://docs.snowflake.com/en/developer-guide/python-connector/python-connector-api#object-connection>`__
+    object. If connector="sqlalchemy" configuration is set, then InsightsSnowflakeResource.get_connection() will
+    return a `SQLAlchemy Connection <https://docs.sqlalchemy.org/en/20/core/connections.html#sqlalchemy.engine.Connection>`__
+    or a `SQLAlchemy raw connection <https://docs.sqlalchemy.org/en/20/core/connections.html#sqlalchemy.engine.Engine.raw_connection>`__.
+
+    A simple example of loading data into Snowflake and subsequently querying that data is shown below:
+
+    Examples:
+        .. code-block:: python
+
+            from dagster import job, op
+            from dagster_insights import InsightsSnowflakeResource
+
+            @op
+            def get_one(snowflake_resource: InsightsSnowflakeResource):
+                with snowflake_resource.get_connection() as conn:
+                    # conn is a snowflake.connector.Connection object
+                    conn.cursor().execute("SELECT 1")
+
+            @job
+            def my_snowflake_job():
+                get_one()
+
+            my_snowflake_job.execute_in_process(
+                resources={
+                    'snowflake_resource': InsightsSnowflakeResource(
+                        account=EnvVar("SNOWFLAKE_ACCOUNT"),
+                        user=EnvVar("SNOWFLAKE_USER"),
+                        password=EnvVar("SNOWFLAKE_PASSWORD")
+                        database="MY_DATABASE",
+                        schema="MY_SCHEMA",
+                        warehouse="MY_WAREHOUSE"
+                    )
+                }
+            )
     """
-    sorted_chunk_list = sorted(chunk_list, key=lambda x: x[0]) + [("marker", 0.0)]
-
-    current_opaque_id = None
-    last_opaque_id_boundary = 0
-    last_chunk_boundary = 0
-    for i, (opaque_id, _) in enumerate(sorted_chunk_list):
-        # If we've seen enough metrics to fill a chunk, yield the chunk minus the
-        # current opaque_id, and start a new chunk
-        if i - last_chunk_boundary > length:
-            yield sorted_chunk_list[last_chunk_boundary:last_opaque_id_boundary]
-            last_chunk_boundary = last_opaque_id_boundary
-
-        if opaque_id != current_opaque_id:
-            current_opaque_id = opaque_id
-            last_opaque_id_boundary = i
-
-    sorted_chunk_list = sorted_chunk_list[:-1]
-    if last_chunk_boundary < len(sorted_chunk_list):
-        yield sorted_chunk_list[last_chunk_boundary:]
-
-
-def get_post_request_params(
-    instance: DagsterInstance,
-) -> Tuple[requests.Session, str, Dict[str, str], int, Optional[Dict[str, str]]]:
-    if not isinstance(instance, DagsterCloudAgentInstance):
-        raise RuntimeError("This asset only functions in a running Dagster Cloud instance")
-
-    return (
-        instance.requests_managed_retries_session,
-        instance.dagster_cloud_gen_insights_url_url,
-        instance.dagster_cloud_api_headers(DagsterCloudInstanceScope.DEPLOYMENT),
-        instance.dagster_cloud_api_timeout,
-        instance.dagster_cloud_api_proxies,
-    )
-
-
-def upload_cost_information(
-    context: Union[OpExecutionContext, AssetExecutionContext],
-    metric_name: str,
-    cost_information: List[Tuple[str, float, str]],
-):
-    import pyarrow as pa
-    import pyarrow.parquet as pq
 
-    with tempfile.TemporaryDirectory() as temp_dir:
-        opaque_ids = pa.array([opaque_id for opaque_id, _, _ in cost_information])
-        costs = pa.array([cost for _, cost, _ in cost_information])
-        query_ids = pa.array([query_id for _, _, query_id in cost_information])
-        metric_names = pa.array([metric_name for _, _, _ in cost_information])
-
-        cost_pq_file = os.path.join(temp_dir, "cost.parquet")
-        pq.write_table(
-            pa.Table.from_arrays(
-                [opaque_ids, costs, metric_names, query_ids],
-                ["opaque_id", "cost", "metric_name", "query_id"],
-            ),
-            cost_pq_file,
+    def get_object_to_set_on_execution_context(self) -> Any:
+        # Directly create a SnowflakeConnection here for backcompat since the SnowflakeConnection
+        # has methods this resource does not have
+        return SnowflakeConnection(
+            config=self._resolved_config_dict,
+            log=get_dagster_logger(),
+            snowflake_connection_resource=self,
         )
 
-        instance = context.instance
-        session, url, headers, timeout, proxies = get_post_request_params(instance)
-
-        resp = session.post(url, headers=headers, timeout=timeout, proxies=proxies)
-        raise_http_error(resp)
-        resp_data = resp.json()
-
-        assert "url" in resp_data and "fields" in resp_data, resp_data
-
-        with open(cost_pq_file, "rb") as f:
-            session.post(
-                resp_data["url"],
-                data=resp_data["fields"],
-                files={"file": f},
+    @public
+    @contextmanager
+    def get_connection(
+        self, raw_conn: bool = True
+    ) -> Iterator[Union[SqlDbConnection, WrappedSnowflakeConnection]]:
+        if self.connector == "sqlalchemy":
+            from snowflake.sqlalchemy import URL
+            from sqlalchemy import create_engine, event
+
+            engine = create_engine(
+                URL(**self._sqlalchemy_connection_args),
+                connect_args=self._sqlalchemy_engine_args,
             )
 
+            # Attach a listener to the connection which will add a comment to any SQL query
+            # executed through the connection. This comment will be used to identify the query
+            # when later attributing cost.
+            @event.listens_for(engine, "before_cursor_execute", retval=True)
+            def comment_sql(conn, cursor, statement, parameters, context, executemany):
+                context, asset_key = get_current_context_and_asset_key_or_warn()
+                if not context:
+                    return statement, parameters
+
+                statement = meter_snowflake_query(
+                    context, statement, associated_asset_key=asset_key
+                )
+                return statement, parameters
+
+            conn = engine.raw_connection() if raw_conn else engine.connect()
+
+            yield conn
+            conn.close()
+            engine.dispose()
+        else:
+            conn = WrappedSnowflakeConnection(**self._connection_args)
+
+            yield conn
+            if not self.autocommit:
+                conn.commit()
+            conn.close()
+
+    @public
+    @contextmanager
+    def get_connection_for_asset(
+        self, asset_key: AssetKey, raw_conn: bool = True
+    ) -> Iterator[Union[SqlDbConnection, WrappedSnowflakeConnection]]:
+        if self.connector == "sqlalchemy":
+            from snowflake.sqlalchemy import URL
+            from sqlalchemy import create_engine, event
+
+            engine = create_engine(
+                URL(**self._sqlalchemy_connection_args),
+                connect_args=self._sqlalchemy_engine_args,
+            )
 
-@experimental
-def put_cost_information(
-    context: Union[OpExecutionContext, AssetExecutionContext],
-    metric_name: str,
-    cost_information: List[Tuple[str, float, str]],
-    start: float,
-    end: float,
-    submit_gql: bool = True,
-) -> None:
-    chunk_size = _cost_information_chunk_size()
-
-    try:
-        import pyarrow as pyarrow  # pylint: disable=import-error
-
-        try:
-            upload_cost_information(context, metric_name, cost_information)
-        except Exception:
-            context.log.warn("Failed to upload cost information to S3.", exc_info=True)
-            # if we're not submitting via GQL API as well, raise the exception more loudly
-            if not submit_gql:
-                raise
-    except ImportError:
-        context.log.warn(
-            "Dagster insights dependencies not installed. In the future, you will need to install dagster-cloud[insights] to use this feature."
-        )
-        # if we're not submitting via GQL API as well, raise the exception more loudly
-        if not submit_gql:
-            raise
-
-    # early exit if we're not submitting via GQL API as well
-    if not submit_gql:
-        return
-
-    cost_info_input = [
-        {
-            "opaqueId": opaque_id,
-            "cost": float(cost),
-        }
-        for opaque_id, cost, _ in cost_information
-    ]
-
-    # Chunk the cost information & keep each opaque id in the same chunk
-    # to avoid the cost information for a single asset being split across
-    # multiple steps
-    for chunk in chunk_by_opaque_id(
-        [(opaque_id, cost) for opaque_id, cost, _ in cost_information], chunk_size
+            # Attach a listener to the connection which will add a comment to any SQL query
+            # executed through the connection. This comment will be used to identify the query
+            # when later attributing cost.
+            @event.listens_for(engine, "before_cursor_execute", retval=True)
+            def comment_sql(conn, cursor, statement, parameters, context, executemany):
+                context, _ = get_current_context_and_asset_key_or_warn()
+                if not context:
+                    return statement, parameters
+
+                statement = meter_snowflake_query(
+                    context, statement, associated_asset_key=asset_key
+                )
+                return statement, parameters
+
+            conn = engine.raw_connection() if raw_conn else engine.connect()
+
+            yield conn
+            conn.close()
+            engine.dispose()
+        else:
+            conn = WrappedSnowflakeConnection(asset_key=asset_key, **self._connection_args)
+
+            yield conn
+            if not self.autocommit:
+                conn.commit()
+            conn.close()
+
+
+class InsightsSnowflakeConnection(SnowflakeConnection):
+    def execute_query(
+        self,
+        sql: str,
+        parameters: Union[Sequence[Any], Mapping[Any, Any], None] = None,
+        fetch_results: bool = False,
+        use_pandas_result: bool = False,
     ):
-        cost_info_input = [
-            {
-                "opaqueId": opaque_id,
-                "cost": float(cost),
-            }
-            for opaque_id, cost in chunk
-        ]
-
-        result = query_graphql_from_instance(
-            context.instance,
-            PUT_COST_INFORMATION_MUTATION,
-            variables={
-                "costInfo": cost_info_input,
-                "metricName": metric_name,
-                "start": start,
-                "end": end,
-            },
+        context, asset_key = get_current_context_and_asset_key_or_warn()
+        if not context:
+            return super().execute_query(sql, parameters, fetch_results, use_pandas_result)
+
+        return super().execute_query(
+            meter_snowflake_query(context, sql, associated_asset_key=asset_key),
+            parameters,
+            fetch_results,
+            use_pandas_result,
         )
-        if (
-            result["submitCostInformationForMetrics"]["__typename"]
-            != "CreateOrUpdateMetricsSuccess"
-        ):
-            raise RuntimeError("Failed to submit cost information", result)
 
+    def execute_queries(
+        self,
+        sql_queries: Sequence[str],
+        parameters: Union[Sequence[Any], Mapping[Any, Any], None] = None,
+        fetch_results: bool = False,
+        use_pandas_result: bool = False,
+    ) -> Union[Sequence[Any], None]:
+        context, asset_key = get_current_context_and_asset_key_or_warn()
+
+        if not context:
+            return super().execute_queries(
+                sql_queries, parameters, fetch_results, use_pandas_result
+            )
 
-@experimental
-def put_metrics(
-    context: Union[OpExecutionContext, AssetExecutionContext],
-    run_id: str,
-    step_key: str,
-    metrics: List[DagsterMetric],
-    asset_key: Optional[str] = None,
-    partition: Optional[str] = None,
-) -> Dict[str, Any]:
-    """Experimental: Store metrics in the dagster cloud metrics store. This method is useful when you would like to
-    store run, asset or asset group materialization metric data to view in the insights UI.
-
-    To associate a metric with an asset, you must provide the asset_key and partition arguments. If you do not provide
-    these arguments, the metric will be associated with the job. Often you will want to store both job and asset
-    metrics, in which case you should call this method twice, once with the asset_key and partition arguments, and
-    once without.
-
-    Currently only supported in Dagster Cloud.
-
-    Args:
-        context (Union[OpExecutionContext, AssetExecutionContext]): the execution context used to query Cloud
-        run_id (str): id of the dagster run
-        step_key (str): key of the step
-        code_location_name (str): name of the code location
-        repository_name (str): name of the repository
-        metrics (List[DagsterMetric]): metrics to store in the dagster metrics store
-        asset_key (Optional[str]): key of the asset, if storing an asset metric
-        partition (Optional[str]): partition of the asset, if storing an asset metric
-    """
-    check.list_param(metrics, "metrics", of_type=DagsterMetric)
-    check.str_param(run_id, "run_id", run_id)
-    check.str_param(step_key, "step_key", step_key)
-    check.opt_str_param(asset_key, "asset_key", asset_key)
-    check.opt_str_param(partition, "partition", partition)
-
-    url, token = get_url_and_token_from_instance(context.instance)
-
-    transport = RequestsHTTPTransport(
-        url=url,
-        use_json=True,
-        timeout=300,
-        headers={"Dagster-Cloud-Api-Token": token},
-    )
-    Client(transport=transport, fetch_schema_from_transport=True)
-
-    metric_graphql_input = {
-        "runId": run_id,
-        "stepKey": step_key,
-        "assetMetricDefinitions": [],
-        "jobMetricDefinitions": [],
-    }
-
-    if asset_key is not None:
-        metric_graphql_input["assetMetricDefinitions"].append(
-            {
-                "assetKey": asset_key,
-                "partition": partition,
-                "metricValues": [
-                    {
-                        "metricValue": metric_def.metric_value,
-                        "metricName": metric_def.metric_name,
-                    }
-                    for metric_def in metrics
-                ],
-            }
-        )
-    else:
-        metric_graphql_input["jobMetricDefinitions"].append(
-            {
-                "metricValues": [
-                    {
-                        "metricValue": metric_def.metric_value,
-                        "metricName": metric_def.metric_name,
-                    }
-                    for metric_def in metrics
-                ],
-            }
+        return super().execute_queries(
+            [
+                meter_snowflake_query(context, sql, associated_asset_key=asset_key)
+                for sql in sql_queries
+            ],
+            parameters,
+            fetch_results,
+            use_pandas_result,
         )
-
-    return query_graphql_from_instance(
-        context.instance,
-        PUT_CLOUD_METRICS_MUTATION,
-        variables={"metrics": [metric_graphql_input]},
-    )
```

### Comparing `dagster-cloud-1.7.3/dagster_cloud/dagster_insights/query.py` & `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/query.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py` & `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py` & `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/definitions.py` & `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from dataclasses import dataclass
 from datetime import date, datetime, timedelta, timezone
 from pprint import pprint
 from typing import (
     TYPE_CHECKING,
     Optional,
     Sequence,
@@ -47,15 +48,15 @@
     job_name: str = "snowflake_insights_import",
     dry_run=False,
     allow_partial_partitions=True,
     snowflake_resource_key: str = "snowflake",
     snowflake_usage_latency: int = SNOWFLAKE_QUERY_HISTORY_LATENCY_SLA_MINS,
     partition_end_offset_hrs: int = 1,
     schedule_batch_size_hrs: int = 1,
-    submit_to_s3_only: bool = False,
+    submit_to_s3_only: bool = True,  # DEPRECATED
 ) -> SnowflakeInsightsDefinitions:
     """Generates a pre-defined Dagster asset and schedule that can be used to import Snowflake cost
     data into Dagster Insights.
 
     The schedule will run hourly, and will query the Snowflake query_history table for all queries
     that ran in the hour starting at the scheduled time. It will then submit the cost data to
     Dagster Insights.
@@ -78,14 +79,19 @@
             run. For example, if this is set to 2, the schedule will run every 2 hours and process
             2 hours of data. Defaults to 1.
     """
     # for backcompat, this used to take `date`
     if isinstance(start_date, date):
         start_date = start_date.strftime("%Y-%m-%d-%H:%M")
 
+    if submit_to_s3_only is False:
+        warnings.warn(
+            "The `submit_to_s3_only` parameter is now deprecated. Insights cost data will now always be uploaded to Dagster Insights via S3."
+        )
+
     partition_end_offset_hrs = -abs(partition_end_offset_hrs)
 
     partitions_def = HourlyPartitionsDefinition(
         start_date=start_date, end_offset=partition_end_offset_hrs
     )
 
     @asset(
@@ -138,15 +144,14 @@
             )
             put_cost_information(
                 context=context,
                 metric_name="snowflake_credits",
                 cost_information=costs,
                 start=start_hour.timestamp(),
                 end=end_hour.timestamp(),
-                submit_gql=not submit_to_s3_only,
             )
 
     insights_job = define_asset_job(
         job_name,
         AssetSelection.assets(poll_snowflake_query_history_hour),
         partitions_def=partitions_def,
     )
```

### Comparing `dagster-cloud-1.7.3/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py` & `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/execution/cloud_run_launcher/process.py` & `dagster-cloud-1.7.4/dagster_cloud/execution/cloud_run_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/execution/monitoring/__init__.py` & `dagster-cloud-1.7.4/dagster_cloud/execution/monitoring/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 import sys
 import threading
 from enum import Enum
 from typing import (
     Any,
     Dict,
     Iterable,
@@ -105,14 +106,19 @@
             ),
         )
 
     def get_code_server_utilization_metrics(self) -> Optional[CloudCodeServerUtilizationMetrics]:
         return self.metadata.get("utilization_metrics")
 
 
+RUN_WORKER_STATUS_MESSAGE_LIMIT = int(
+    os.getenv("DAGSTER_CLOUD_RUN_WORKER_STATUS_MESSAGE_SIZE_LIMIT", "1000")
+)
+
+
 @whitelist_for_serdes
 class CloudRunWorkerStatus(
     NamedTuple(
         "_CloudRunWorkerStatus",
         [
             ("run_id", str),
             ("status_type", WorkerStatus),
@@ -146,18 +152,19 @@
     def from_check_run_health_result(
         cls,
         run_id: str,
         result: CheckRunHealthResult,
         run_worker_debug_info: Optional[str] = None,
     ) -> "CloudRunWorkerStatus":
         check.inst_param(result, "result", CheckRunHealthResult)
+        msg = (result.msg or "") + (f"\n{run_worker_debug_info}" if run_worker_debug_info else "")
         return CloudRunWorkerStatus(
             run_id,
             result.status,
-            (result.msg or "") + (f"\n{run_worker_debug_info}" if run_worker_debug_info else ""),
+            msg[:RUN_WORKER_STATUS_MESSAGE_LIMIT],
             transient=result.transient,
             run_worker_id=result.run_worker_id,
         )
 
 
 @whitelist_for_serdes
 class CloudRunWorkerStatuses(
@@ -273,16 +280,15 @@
                         except Exception:
                             logger.exception("Failure fetching debug info for failed run worker")
 
                     statuses_for_deployment.append(
                         CloudRunWorkerStatus.from_check_run_health_result(
                             run.run_id,
                             run_worker_health,
-                            # Truncate to ensure that the debug info doesn't hit a size upload limit
-                            run_worker_debug_info[:1000] if run_worker_debug_info else None,
+                            run_worker_debug_info,
                         )
                     )
                 else:
                     if scoped_instance.is_using_isolated_agents:  # type: ignore  # (instance subclass)
                         # Not currently supported for non isolated run monitoring
                         continue
```

### Comparing `dagster-cloud-1.7.3/dagster_cloud/execution/utils/process.py` & `dagster-cloud-1.7.4/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/instance/__init__.py` & `dagster-cloud-1.7.4/dagster_cloud/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/pex/grpc/client.py` & `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/pex/grpc/compile.py` & `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/manager.py` & `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,15 @@
                 pex_server = self._pex_servers.get(handle_id)
                 if not pex_server:
                     # still in _pending_startup_pex_servers
                     logging.info("Server %s not up yet, will request shutdown later", handle_id)
                     continue
 
                 if isinstance(pex_server, PexErrorEntry):
-                    logging.info("Server %s was in an error state, no shutdown needed", handle_id)
+                    logging.debug("Server %s was in an error state, no shutdown needed", handle_id)
                     continue
 
                 if pex_server.heartbeat_shutdown_event.is_set():
                     # already requested shutdown
                     logging.info("Already requested shutdown for server %s", handle_id)
                     continue
```

### Comparing `dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/registry.py` & `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/pex/grpc/server/server.py` & `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/pex/grpc/types.py` & `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/secrets/loader.py` & `dagster-cloud-1.7.4/dagster_cloud/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/serverless/io_manager.py` & `dagster-cloud-1.7.4/dagster_cloud/serverless/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/storage/client.py` & `dagster-cloud-1.7.4/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster-cloud-1.7.4/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/storage/event_logs/queries.py` & `dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/storage/event_logs/storage.py` & `dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/storage/event_logs/utils.py` & `dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/storage/runs/queries.py` & `dagster-cloud-1.7.4/dagster_cloud/storage/runs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/storage/runs/storage.py` & `dagster-cloud-1.7.4/dagster_cloud/storage/runs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/storage/schedules/queries.py` & `dagster-cloud-1.7.4/dagster_cloud/storage/schedules/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/storage/schedules/storage.py` & `dagster-cloud-1.7.4/dagster_cloud/storage/schedules/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/util/__init__.py` & `dagster-cloud-1.7.4/dagster_cloud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/util/container_resources.py` & `dagster-cloud-1.7.4/dagster_cloud/util/container_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/config_schema/__init__.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/config_schema/docker.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/config_schema/ecs.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/docker/__init__.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/client.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/launcher.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/run_launcher.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/service.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/service.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/ecs/utils.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/kubernetes/utils.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.3/dagster_cloud.egg-info/PKG-INFO` & `dagster-cloud-1.7.4/dagster_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.7.3
+Version: 1.7.4
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster-cloud-1.7.3/dagster_cloud.egg-info/SOURCES.txt` & `dagster-cloud-1.7.4/dagster_cloud.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 dagster_cloud/execution/cloud_run_launcher/__init__.py
 dagster_cloud/execution/cloud_run_launcher/k8s.py
 dagster_cloud/execution/cloud_run_launcher/process.py
 dagster_cloud/execution/monitoring/__init__.py
 dagster_cloud/execution/utils/__init__.py
 dagster_cloud/execution/utils/process.py
 dagster_cloud/instance/__init__.py
-dagster_cloud/metrics/__init__.py
 dagster_cloud/pex/__init__.py
 dagster_cloud/pex/grpc/__init__.py
 dagster_cloud/pex/grpc/client.py
 dagster_cloud/pex/grpc/compile.py
 dagster_cloud/pex/grpc/types.py
 dagster_cloud/pex/grpc/__generated__/__init__.py
 dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
```

### Comparing `dagster-cloud-1.7.3/setup.py` & `dagster-cloud-1.7.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.7.3",
-        "dagster-cloud-cli==1.7.3",
+        "dagster==1.7.4",
+        "dagster-cloud-cli==1.7.4",
         "pex>=2.1.132,<3",
         "questionary",
         "requests",
         "typer[all]",
     ],
     extras_require={
         "tests": [
@@ -62,21 +62,21 @@
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
             "dbt-core",
             "dbt-snowflake",
             "dbt-postgres",
             "dbt-duckdb",
-            "dagster-dbt==0.23.3",
-            "dagster_k8s==0.23.3",
+            "dagster-dbt==0.23.4",
+            "dagster_k8s==0.23.4",
         ],
         "insights": ["pyarrow"],
-        "docker": ["docker", "dagster_docker==0.23.3"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.23.3"],
-        "ecs": ["dagster_aws==0.23.3", "boto3"],
+        "docker": ["docker", "dagster_docker==0.23.4"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.23.4"],
+        "ecs": ["dagster_aws==0.23.4", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```

