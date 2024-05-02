# Comparing `tmp/numalogic-0.9.1a7.tar.gz` & `tmp/numalogic-0.9.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic-0.9.1a7.tar", max compression
+gzip compressed data, was "numalogic-0.9.1a8.tar", max compression
```

## Comparing `numalogic-0.9.1a7.tar` & `numalogic-0.9.1a8.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0    11357 2024-04-29 22:43:18.338402 numalogic-0.9.1a7/LICENSE
--rw-r--r--   0        0        0     5244 2024-04-29 22:43:18.338402 numalogic-0.9.1a7/README.md
--rw-r--r--   0        0        0      676 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/__init__.py
--rw-r--r--   0        0        0     1016 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/_constants.py
--rw-r--r--   0        0        0      413 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/backtest/__init__.py
--rw-r--r--   0        0        0      248 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/backtest/_constants.py
--rw-r--r--   0        0        0    16031 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/backtest/_prom.py
--rw-r--r--   0        0        0     1636 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/base.py
--rw-r--r--   0        0        0     1102 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/blocks/__init__.py
--rw-r--r--   0        0        0     4672 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/blocks/_base.py
--rw-r--r--   0        0        0     3229 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/blocks/_nn.py
--rw-r--r--   0        0        0     3906 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/blocks/_transform.py
--rw-r--r--   0        0        0     5776 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/blocks/pipeline.py
--rw-r--r--   0        0        0     1271 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/config/__init__.py
--rw-r--r--   0        0        0     4818 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/config/_config.py
--rw-r--r--   0        0        0     7543 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/config/factory.py
--rw-r--r--   0        0        0      550 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/__init__.py
--rw-r--r--   0        0        0      689 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/_base.py
--rw-r--r--   0        0        0     1709 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/_config.py
--rw-r--r--   0        0        0      157 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/druid/__init__.py
--rw-r--r--   0        0        0     9647 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/druid/_druid.py
--rw-r--r--   0        0        0      765 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/druid/aggregators.py
--rw-r--r--   0        0        0      696 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/druid/postaggregator.py
--rw-r--r--   0        0        0    10150 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/prometheus.py
--rw-r--r--   0        0        0       79 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/rds/__init__.py
--rw-r--r--   0        0        0     5022 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/rds/_base.py
--rw-r--r--   0        0        0     2608 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/rds/_rds.py
--rw-r--r--   0        0        0        0 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/rds/db/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/rds/db/factory.py
--rw-r--r--   0        0        0     4193 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/rds/db/mysql_fetcher.py
--rw-r--r--   0        0        0     2734 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/redis.py
--rw-r--r--   0        0        0        0 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/utils/aws/__init__.py
--rw-r--r--   0        0        0     5637 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/utils/aws/boto3_client_manager.py
--rw-r--r--   0        0        0     4636 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/utils/aws/config.py
--rw-r--r--   0        0        0     1265 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/utils/aws/db_configurations.py
--rw-r--r--   0        0        0     1738 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/utils/aws/exceptions.py
--rw-r--r--   0        0        0     3346 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/utils/aws/sts_client_manager.py
--rw-r--r--   0        0        0     2181 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/connectors/utils/enum.py
--rw-r--r--   0        0        0        0 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/models/__init__.py
--rw-r--r--   0        0        0      668 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/models/autoencoder/__init__.py
--rw-r--r--   0        0        0     3419 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/models/autoencoder/base.py
--rw-r--r--   0        0        0      581 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/models/autoencoder/variants/__init__.py
--rw-r--r--   0        0        0    11705 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/models/autoencoder/variants/conv.py
--rw-r--r--   0        0        0     6599 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/models/autoencoder/variants/lstm.py
--rw-r--r--   0        0        0    14335 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/models/autoencoder/variants/transformer.py
--rw-r--r--   0        0        0     8562 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/models/autoencoder/variants/vanilla.py
--rw-r--r--   0        0        0        0 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/models/forecast/__init__.py
--rw-r--r--   0        0        0      158 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/models/forecast/variants/__init__.py
--rw-r--r--   0        0        0     4289 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/models/forecast/variants/naive.py
--rw-r--r--   0        0        0      489 2024-04-29 22:43:18.362402 numalogic-0.9.1a7/numalogic/models/threshold/__init__.py
--rw-r--r--   0        0        0     7531 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/models/threshold/_mahalanobis.py
--rw-r--r--   0        0        0     2943 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/models/threshold/_median.py
--rw-r--r--   0        0        0     4720 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/models/threshold/_static.py
--rw-r--r--   0        0        0     2462 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/models/threshold/_std.py
--rw-r--r--   0        0        0       77 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/models/vae/__init__.py
--rw-r--r--   0        0        0     2046 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/models/vae/base.py
--rw-r--r--   0        0        0     1536 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/models/vae/layer.py
--rw-r--r--   0        0        0       82 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/models/vae/variants/__init__.py
--rw-r--r--   0        0        0     7916 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/models/vae/variants/conv.py
--rw-r--r--   0        0        0      975 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/monitoring/__init__.py
--rw-r--r--   0        0        0     3906 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/monitoring/metrics.py
--rw-r--r--   0        0        0     1282 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/registry/__init__.py
--rw-r--r--   0        0        0      651 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/registry/_serialize.py
--rw-r--r--   0        0        0     6734 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/registry/artifact.py
--rw-r--r--   0        0        0    15564 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/registry/dynamodb_registry.py
--rw-r--r--   0        0        0     3334 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/registry/localcache.py
--rw-r--r--   0        0        0    13536 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/registry/mlflow_registry.py
--rw-r--r--   0        0        0    16600 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/registry/redis_registry.py
--rw-r--r--   0        0        0      841 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/synthetic/__init__.py
--rw-r--r--   0        0        0    12457 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/synthetic/anomalies.py
--rw-r--r--   0        0        0     1637 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/synthetic/sparsity.py
--rw-r--r--   0        0        0     4739 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/synthetic/timeseries.py
--rw-r--r--   0        0        0        0 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/tools/__init__.py
--rw-r--r--   0        0        0      631 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/tools/aggregators.py
--rw-r--r--   0        0        0     3615 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/tools/callbacks.py
--rw-r--r--   0        0        0    10279 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/tools/data.py
--rw-r--r--   0        0        0     2545 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/tools/exceptions.py
--rw-r--r--   0        0        0     3168 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/tools/trainer.py
--rw-r--r--   0        0        0     2237 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/tools/types.py
--rw-r--r--   0        0        0     1418 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/transforms/__init__.py
--rw-r--r--   0        0        0     4006 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/transforms/_movavg.py
--rw-r--r--   0        0        0     2252 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/transforms/_postprocess.py
--rw-r--r--   0        0        0     4772 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/transforms/_scaler.py
--rw-r--r--   0        0        0     5178 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/transforms/_stateless.py
--rw-r--r--   0        0        0     3560 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/README.md
--rw-r--r--   0        0        0     1232 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/__init__.py
--rw-r--r--   0        0        0     1937 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/__main__.py
--rw-r--r--   0        0        0     5192 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/_base.py
--rw-r--r--   0        0        0     3711 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/_config.py
--rw-r--r--   0        0        0     1060 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/_logger.py
--rw-r--r--   0        0        0     4923 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/_metrics.py
--rw-r--r--   0        0        0     3376 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/entities.py
--rw-r--r--   0        0        0     4298 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/factory.py
--rw-r--r--   0        0        0     7317 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/inference.py
--rw-r--r--   0        0        0     2196 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/payloadtx.py
--rw-r--r--   0        0        0    15827 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/postprocess.py
--rw-r--r--   0        0        0     9286 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/preprocess.py
--rw-r--r--   0        0        0     5581 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/staticthresh.py
--rw-r--r--   0        0        0    14920 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/tools.py
--rw-r--r--   0        0        0      229 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/trainer/__init__.py
--rw-r--r--   0        0        0    14056 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/trainer/_base.py
--rw-r--r--   0        0        0     5187 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/trainer/_druid.py
--rw-r--r--   0        0        0     3816 2024-04-29 22:43:18.366402 numalogic-0.9.1a7/numalogic/udfs/trainer/_prom.py
--rw-r--r--   0        0        0     3032 2024-04-29 22:43:18.370402 numalogic-0.9.1a7/pyproject.toml
--rw-r--r--   0        0        0     6954 1970-01-01 00:00:00.000000 numalogic-0.9.1a7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-02 00:48:04.298230 numalogic-0.9.1a8/LICENSE
+-rw-r--r--   0        0        0     5244 2024-05-02 00:48:04.298230 numalogic-0.9.1a8/README.md
+-rw-r--r--   0        0        0      676 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/__init__.py
+-rw-r--r--   0        0        0     1016 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/_constants.py
+-rw-r--r--   0        0        0      413 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/backtest/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/backtest/_constants.py
+-rw-r--r--   0        0        0    16031 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/backtest/_prom.py
+-rw-r--r--   0        0        0     1636 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/base.py
+-rw-r--r--   0        0        0     1102 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/blocks/__init__.py
+-rw-r--r--   0        0        0     4672 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/blocks/_base.py
+-rw-r--r--   0        0        0     3229 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/blocks/_nn.py
+-rw-r--r--   0        0        0     3906 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/blocks/_transform.py
+-rw-r--r--   0        0        0     5776 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/blocks/pipeline.py
+-rw-r--r--   0        0        0     1271 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/config/__init__.py
+-rw-r--r--   0        0        0     4818 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/config/_config.py
+-rw-r--r--   0        0        0     7543 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/config/factory.py
+-rw-r--r--   0        0        0      550 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/__init__.py
+-rw-r--r--   0        0        0      689 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/_base.py
+-rw-r--r--   0        0        0     1890 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/_config.py
+-rw-r--r--   0        0        0      157 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/druid/__init__.py
+-rw-r--r--   0        0        0    10789 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/druid/_druid.py
+-rw-r--r--   0        0        0      765 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/druid/aggregators.py
+-rw-r--r--   0        0        0      696 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/druid/postaggregator.py
+-rw-r--r--   0        0        0    10150 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/prometheus.py
+-rw-r--r--   0        0        0       79 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/rds/__init__.py
+-rw-r--r--   0        0        0     5022 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/rds/_base.py
+-rw-r--r--   0        0        0     2608 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/rds/_rds.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/rds/db/__init__.py
+-rw-r--r--   0        0        0     1061 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/rds/db/factory.py
+-rw-r--r--   0        0        0     4193 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/rds/db/mysql_fetcher.py
+-rw-r--r--   0        0        0     2734 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/redis.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/utils/aws/__init__.py
+-rw-r--r--   0        0        0     5637 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/utils/aws/boto3_client_manager.py
+-rw-r--r--   0        0        0     4636 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/utils/aws/config.py
+-rw-r--r--   0        0        0     1265 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/utils/aws/db_configurations.py
+-rw-r--r--   0        0        0     1738 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/utils/aws/exceptions.py
+-rw-r--r--   0        0        0     3346 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/utils/aws/sts_client_manager.py
+-rw-r--r--   0        0        0     2181 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/connectors/utils/enum.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/__init__.py
+-rw-r--r--   0        0        0      668 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/autoencoder/__init__.py
+-rw-r--r--   0        0        0     3419 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/autoencoder/base.py
+-rw-r--r--   0        0        0      581 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/autoencoder/variants/__init__.py
+-rw-r--r--   0        0        0    11705 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/autoencoder/variants/conv.py
+-rw-r--r--   0        0        0     6599 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/autoencoder/variants/lstm.py
+-rw-r--r--   0        0        0    14335 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/autoencoder/variants/transformer.py
+-rw-r--r--   0        0        0     8562 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/autoencoder/variants/vanilla.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/forecast/__init__.py
+-rw-r--r--   0        0        0      158 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/forecast/variants/__init__.py
+-rw-r--r--   0        0        0     4289 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/forecast/variants/naive.py
+-rw-r--r--   0        0        0      489 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/threshold/__init__.py
+-rw-r--r--   0        0        0     7531 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/threshold/_mahalanobis.py
+-rw-r--r--   0        0        0     2943 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/threshold/_median.py
+-rw-r--r--   0        0        0     4720 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/threshold/_static.py
+-rw-r--r--   0        0        0     2462 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/threshold/_std.py
+-rw-r--r--   0        0        0       77 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/vae/__init__.py
+-rw-r--r--   0        0        0     2046 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/vae/base.py
+-rw-r--r--   0        0        0     1536 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/vae/layer.py
+-rw-r--r--   0        0        0       82 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/vae/variants/__init__.py
+-rw-r--r--   0        0        0     7916 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/models/vae/variants/conv.py
+-rw-r--r--   0        0        0      975 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/monitoring/__init__.py
+-rw-r--r--   0        0        0     3906 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/monitoring/metrics.py
+-rw-r--r--   0        0        0     1282 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/registry/__init__.py
+-rw-r--r--   0        0        0      651 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/registry/_serialize.py
+-rw-r--r--   0        0        0     6734 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/registry/artifact.py
+-rw-r--r--   0        0        0    15564 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/registry/dynamodb_registry.py
+-rw-r--r--   0        0        0     3334 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/registry/localcache.py
+-rw-r--r--   0        0        0    13536 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/registry/mlflow_registry.py
+-rw-r--r--   0        0        0    16600 2024-05-02 00:48:04.322230 numalogic-0.9.1a8/numalogic/registry/redis_registry.py
+-rw-r--r--   0        0        0      841 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/synthetic/__init__.py
+-rw-r--r--   0        0        0    12457 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/synthetic/anomalies.py
+-rw-r--r--   0        0        0     1637 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/synthetic/sparsity.py
+-rw-r--r--   0        0        0     4739 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/synthetic/timeseries.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/tools/__init__.py
+-rw-r--r--   0        0        0      631 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/tools/aggregators.py
+-rw-r--r--   0        0        0     3615 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/tools/callbacks.py
+-rw-r--r--   0        0        0    10279 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/tools/data.py
+-rw-r--r--   0        0        0     2545 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/tools/exceptions.py
+-rw-r--r--   0        0        0     3168 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/tools/trainer.py
+-rw-r--r--   0        0        0     2237 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/tools/types.py
+-rw-r--r--   0        0        0     1418 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/transforms/__init__.py
+-rw-r--r--   0        0        0     4006 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/transforms/_movavg.py
+-rw-r--r--   0        0        0     2252 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/transforms/_postprocess.py
+-rw-r--r--   0        0        0     4772 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/transforms/_scaler.py
+-rw-r--r--   0        0        0     5178 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/transforms/_stateless.py
+-rw-r--r--   0        0        0     3560 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/README.md
+-rw-r--r--   0        0        0     1232 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/__init__.py
+-rw-r--r--   0        0        0     1937 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/__main__.py
+-rw-r--r--   0        0        0     5192 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/_base.py
+-rw-r--r--   0        0        0     3711 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/_config.py
+-rw-r--r--   0        0        0     1060 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/_logger.py
+-rw-r--r--   0        0        0     4923 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/_metrics.py
+-rw-r--r--   0        0        0     3376 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/entities.py
+-rw-r--r--   0        0        0     4298 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/factory.py
+-rw-r--r--   0        0        0     7317 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/inference.py
+-rw-r--r--   0        0        0     2196 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/payloadtx.py
+-rw-r--r--   0        0        0    15827 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/postprocess.py
+-rw-r--r--   0        0        0     9286 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/preprocess.py
+-rw-r--r--   0        0        0     5581 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/staticthresh.py
+-rw-r--r--   0        0        0    14920 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/tools.py
+-rw-r--r--   0        0        0      229 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/trainer/__init__.py
+-rw-r--r--   0        0        0    14056 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/trainer/_base.py
+-rw-r--r--   0        0        0     5248 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/trainer/_druid.py
+-rw-r--r--   0        0        0     3816 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/numalogic/udfs/trainer/_prom.py
+-rw-r--r--   0        0        0     3032 2024-05-02 00:48:04.326230 numalogic-0.9.1a8/pyproject.toml
+-rw-r--r--   0        0        0     6954 1970-01-01 00:00:00.000000 numalogic-0.9.1a8/PKG-INFO
```

### Comparing `numalogic-0.9.1a7/LICENSE` & `numalogic-0.9.1a8/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/README.md` & `numalogic-0.9.1a8/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/__init__.py` & `numalogic-0.9.1a8/numalogic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/_constants.py` & `numalogic-0.9.1a8/numalogic/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/backtest/_prom.py` & `numalogic-0.9.1a8/numalogic/backtest/_prom.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/base.py` & `numalogic-0.9.1a8/numalogic/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/blocks/__init__.py` & `numalogic-0.9.1a8/numalogic/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/blocks/_base.py` & `numalogic-0.9.1a8/numalogic/blocks/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/blocks/_nn.py` & `numalogic-0.9.1a8/numalogic/blocks/_nn.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/blocks/_transform.py` & `numalogic-0.9.1a8/numalogic/blocks/_transform.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/blocks/pipeline.py` & `numalogic-0.9.1a8/numalogic/blocks/pipeline.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/config/__init__.py` & `numalogic-0.9.1a8/numalogic/config/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/config/_config.py` & `numalogic-0.9.1a8/numalogic/config/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/config/factory.py` & `numalogic-0.9.1a8/numalogic/config/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/__init__.py` & `numalogic-0.9.1a8/numalogic/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/_base.py` & `numalogic-0.9.1a8/numalogic/connectors/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/_config.py` & `numalogic-0.9.1a8/numalogic/connectors/_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,16 +33,23 @@
 class Pivot:
     index: str = "timestamp"
     columns: list[str] = field(default_factory=list)
     value: list[str] = field(default_factory=lambda: ["count"])
 
 
 @dataclass
+class FilterConf:
+    inclusion_filters: Optional[list[dict]] = None
+    exclusion_filters: Optional[list[dict]] = None
+
+
+@dataclass
 class DruidFetcherConf:
     datasource: str
+    static_filters: Optional[FilterConf] = None
     dimensions: list[str] = field(default_factory=list)
     aggregations: dict = field(default_factory=dict)
     group_by: list[str] = field(default_factory=list)
     pivot: Pivot = field(default_factory=lambda: Pivot())
     granularity: str = "minute"
 
     def __post_init__(self):
```

### Comparing `numalogic-0.9.1a7/numalogic/connectors/druid/_druid.py` & `numalogic-0.9.1a8/numalogic/connectors/druid/_druid.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pandas as pd
 import pytz
 from pydruid.client import PyDruid
 from pydruid.utils.dimensions import DimensionSpec
 from pydruid.utils.filters import Filter
 
 from numalogic.connectors._base import DataFetcher
-from numalogic.connectors._config import Pivot
+from numalogic.connectors._config import Pivot, FilterConf
 from typing import Optional, Final
 
 from numalogic.tools.exceptions import DruidFetcherError
 
 _LOGGER = logging.getLogger(__name__)
 TIMEOUT: Final[int] = 10000
 _MAX_CONCURRENCY: Final[int] = 16
@@ -30,32 +30,50 @@
 
     Returns: a dict of key value pairs
 
     """
     return dict(zip(filter_keys, filter_values))
 
 
+def _combine_in_filters(filters_list) -> Filter:
+    return Filter(type="and", fields=[Filter(**item) for item in filters_list])
+
+
+def _combine_ex_filters(filters_list) -> Filter:
+    filters = _combine_in_filters(filters_list)
+    return Filter(type="not", field=filters)
+
+
+def _make_static_filters(filters: FilterConf) -> Filter:
+    in_filters, ex_filters = _combine_in_filters(filters.inclusion_filters), _combine_ex_filters(
+        filters.exclusion_filters
+    )
+    return Filter(type="and", fields=[in_filters, ex_filters])
+
+
 def build_params(
     datasource: str,
     dimensions: list[str],
     filter_pairs: dict,
     granularity: str,
     hours: float,
     delay: float,
+    static_filters: Optional[FilterConf] = None,
     aggregations: Optional[list[str]] = None,
     post_aggregations: Optional[list[str]] = None,
     reference_dt: Optional[datetime] = None,
 ) -> dict:
     """
 
     Args:
         datasource: Data source to query
         dimensions: The dimensions to group by
         filter_pairs: Indicates which rows of
           data to include in the query
+        static_filters: Static filters passed from config
         granularity: Time bucket to aggregate data by hour, day, minute, etc.,
         hours: Hours from now to skip training.
         delay: Added delay to the fetch query from current time.
         aggregations: A map from aggregator name to one of the
           ``pydruid.utils.aggregators`` e.g., ``doublesum``
         post_aggregations: A map from post aggregator name to one of the
           ``pydruid.utils.postaggregator`` e.g., ``QuantilesDoublesSketchToQuantile``.
@@ -65,14 +83,19 @@
     Returns: a dict of parameters
 
     """
     _filter = Filter(
         type="and",
         fields=[Filter(type="selector", dimension=k, value=v) for k, v in filter_pairs.items()],
     )
+    if static_filters:
+        _LOGGER.debug("Static Filters are present!")
+        _static_filters = _make_static_filters(static_filters)
+        _filter = Filter(type="and", fields=[_static_filters, _filter])
+
     reference_dt = reference_dt or datetime.now(pytz.utc)
     end_dt = reference_dt - timedelta(hours=delay)
     _LOGGER.debug("Querying with end_dt: %s, that is with delay of %s hrs", end_dt, delay)
 
     start_dt = end_dt - timedelta(hours=hours)
 
     intervals = [f"{start_dt.isoformat()}/{end_dt.isoformat()}"]
@@ -114,14 +137,15 @@
         self,
         datasource: str,
         filter_keys: list[str],
         filter_values: list[str],
         dimensions: list[str],
         delay: float = 3.0,
         granularity: str = "minute",
+        static_filters: Optional[FilterConf] = None,
         aggregations: Optional[dict] = None,
         post_aggregations: Optional[dict] = None,
         group_by: Optional[list[str]] = None,
         pivot: Optional[Pivot] = None,
         hours: float = 24,
     ) -> pd.DataFrame:
         """
@@ -131,14 +155,15 @@
         ------
             datasource: Data source to query
             filter_keys: keys
             filter_values: values
             dimensions: The dimensions to group by
             delay: Added delay to the fetch query from current time.
             granularity: Time bucket to aggregate data by hour, day, minute, etc.
+            static_filters: user defined filters
             aggregations: A map from aggregator name to one of the
                 ``pydruid.utils.aggregators`` e.g., ``doublesum``
             post_aggregations: postaggregations map
             group_by: List of columns to group by
             pivot: Pivot configuration
             hours: Hours from now to fetch.
 
@@ -148,14 +173,15 @@
         """
         _start_time = time.perf_counter()
         filter_pairs = make_filter_pairs(filter_keys, filter_values)
         query_params = build_params(
             datasource=datasource,
             dimensions=dimensions,
             filter_pairs=filter_pairs,
+            static_filters=static_filters,
             granularity=granularity,
             hours=hours,
             delay=delay,
             aggregations=aggregations,
             post_aggregations=post_aggregations,
         )
         df = self._fetch(**query_params)
@@ -189,14 +215,15 @@
         self,
         datasource: str,
         filter_keys: list[str],
         filter_values: list[str],
         dimensions: list[str],
         delay: float = 3.0,
         granularity: str = "minute",
+        static_filter: Optional[FilterConf] = None,
         aggregations: Optional[dict] = None,
         post_aggregations: Optional[dict] = None,
         group_by: Optional[list[str]] = None,
         pivot: Optional[Pivot] = None,
         hours: int = 24,
         chunked_hours: int = 6,
     ) -> pd.DataFrame:
@@ -209,14 +236,15 @@
             filter_keys: keys
             filter_values: values
             dimensions: The dimensions to group by
             delay: Added delay to the fetch query from current time.
             granularity: Time bucket to aggregate data by hour, day, minute, etc.
             aggregations: A map from aggregator name to one of the
                 ``pydruid.utils.aggregators`` e.g., ``doublesum``
+            static_filter: user defined filters
             post_aggregations: postaggregations map
             group_by: List of columns to group by
             pivot: Pivot configuration
             hours: Hours from now to skip training.
             chunked_hours: Hours to fetch in each chunk
 
         Returns
@@ -241,31 +269,30 @@
         while hours_elapsed < hours:
             ref_dt = curr_time - timedelta(hours=hours_elapsed)
             qparams.append(
                 build_params(
                     datasource=datasource,
                     dimensions=dimensions,
                     filter_pairs=filter_pairs,
+                    static_filter=static_filter,
                     granularity=granularity,
                     hours=min(chunked_hours, hours - hours_elapsed),
                     delay=delay,
                     aggregations=aggregations,
                     post_aggregations=post_aggregations,
                     reference_dt=ref_dt,
                 )
             )
             hours_elapsed += chunked_hours
 
         max_threads = min(_MAX_CONCURRENCY, len(qparams))
         _LOGGER.debug("Fetching data concurrently with %s threads", max_threads)
         with ThreadPoolExecutor(max_workers=max_threads) as executor:
             futures = [executor.submit(self._fetch, **params) for params in qparams]
-            for future in futures:
-                chunked_dfs.append(future.result())
-
+            chunked_dfs.extend(future.result() for future in futures)
         df = pd.concat(chunked_dfs, axis=0, ignore_index=True)
         df["timestamp"] = pd.to_datetime(df["timestamp"]).astype("int64") // 10**6
 
         if group_by:
             df = df.groupby(by=group_by).sum().reset_index()
 
         if pivot and pivot.columns:
```

### Comparing `numalogic-0.9.1a7/numalogic/connectors/druid/aggregators.py` & `numalogic-0.9.1a8/numalogic/connectors/druid/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/druid/postaggregator.py` & `numalogic-0.9.1a8/numalogic/connectors/druid/postaggregator.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/prometheus.py` & `numalogic-0.9.1a8/numalogic/connectors/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/rds/_base.py` & `numalogic-0.9.1a8/numalogic/connectors/rds/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/rds/_rds.py` & `numalogic-0.9.1a8/numalogic/connectors/rds/_rds.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/rds/db/factory.py` & `numalogic-0.9.1a8/numalogic/connectors/rds/db/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/rds/db/mysql_fetcher.py` & `numalogic-0.9.1a8/numalogic/connectors/rds/db/mysql_fetcher.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/redis.py` & `numalogic-0.9.1a8/numalogic/connectors/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/utils/aws/boto3_client_manager.py` & `numalogic-0.9.1a8/numalogic/connectors/utils/aws/boto3_client_manager.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/utils/aws/config.py` & `numalogic-0.9.1a8/numalogic/connectors/utils/aws/config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/utils/aws/db_configurations.py` & `numalogic-0.9.1a8/numalogic/connectors/utils/aws/db_configurations.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/utils/aws/exceptions.py` & `numalogic-0.9.1a8/numalogic/connectors/utils/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/utils/aws/sts_client_manager.py` & `numalogic-0.9.1a8/numalogic/connectors/utils/aws/sts_client_manager.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/connectors/utils/enum.py` & `numalogic-0.9.1a8/numalogic/connectors/utils/enum.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/autoencoder/__init__.py` & `numalogic-0.9.1a8/numalogic/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/autoencoder/base.py` & `numalogic-0.9.1a8/numalogic/models/autoencoder/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/autoencoder/variants/__init__.py` & `numalogic-0.9.1a8/numalogic/models/autoencoder/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/autoencoder/variants/conv.py` & `numalogic-0.9.1a8/numalogic/models/autoencoder/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/autoencoder/variants/lstm.py` & `numalogic-0.9.1a8/numalogic/models/autoencoder/variants/lstm.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/autoencoder/variants/transformer.py` & `numalogic-0.9.1a8/numalogic/models/autoencoder/variants/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/autoencoder/variants/vanilla.py` & `numalogic-0.9.1a8/numalogic/models/autoencoder/variants/vanilla.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/forecast/variants/naive.py` & `numalogic-0.9.1a8/numalogic/models/forecast/variants/naive.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/threshold/_mahalanobis.py` & `numalogic-0.9.1a8/numalogic/models/threshold/_mahalanobis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/threshold/_median.py` & `numalogic-0.9.1a8/numalogic/models/threshold/_median.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/threshold/_static.py` & `numalogic-0.9.1a8/numalogic/models/threshold/_static.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/threshold/_std.py` & `numalogic-0.9.1a8/numalogic/models/threshold/_std.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/vae/base.py` & `numalogic-0.9.1a8/numalogic/models/vae/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/vae/layer.py` & `numalogic-0.9.1a8/numalogic/models/vae/layer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/models/vae/variants/conv.py` & `numalogic-0.9.1a8/numalogic/models/vae/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/monitoring/__init__.py` & `numalogic-0.9.1a8/numalogic/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/monitoring/metrics.py` & `numalogic-0.9.1a8/numalogic/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/registry/__init__.py` & `numalogic-0.9.1a8/numalogic/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/registry/_serialize.py` & `numalogic-0.9.1a8/numalogic/registry/_serialize.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/registry/artifact.py` & `numalogic-0.9.1a8/numalogic/registry/artifact.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/registry/dynamodb_registry.py` & `numalogic-0.9.1a8/numalogic/registry/dynamodb_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/registry/localcache.py` & `numalogic-0.9.1a8/numalogic/registry/localcache.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/registry/mlflow_registry.py` & `numalogic-0.9.1a8/numalogic/registry/mlflow_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/registry/redis_registry.py` & `numalogic-0.9.1a8/numalogic/registry/redis_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/synthetic/__init__.py` & `numalogic-0.9.1a8/numalogic/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/synthetic/anomalies.py` & `numalogic-0.9.1a8/numalogic/synthetic/anomalies.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/synthetic/sparsity.py` & `numalogic-0.9.1a8/numalogic/synthetic/sparsity.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/synthetic/timeseries.py` & `numalogic-0.9.1a8/numalogic/synthetic/timeseries.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/tools/aggregators.py` & `numalogic-0.9.1a8/numalogic/tools/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/tools/callbacks.py` & `numalogic-0.9.1a8/numalogic/tools/callbacks.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/tools/data.py` & `numalogic-0.9.1a8/numalogic/tools/data.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/tools/exceptions.py` & `numalogic-0.9.1a8/numalogic/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/tools/trainer.py` & `numalogic-0.9.1a8/numalogic/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/tools/types.py` & `numalogic-0.9.1a8/numalogic/tools/types.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/transforms/__init__.py` & `numalogic-0.9.1a8/numalogic/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/transforms/_movavg.py` & `numalogic-0.9.1a8/numalogic/transforms/_movavg.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/transforms/_postprocess.py` & `numalogic-0.9.1a8/numalogic/transforms/_postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/transforms/_scaler.py` & `numalogic-0.9.1a8/numalogic/transforms/_scaler.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/transforms/_stateless.py` & `numalogic-0.9.1a8/numalogic/transforms/_stateless.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/README.md` & `numalogic-0.9.1a8/numalogic/udfs/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/__init__.py` & `numalogic-0.9.1a8/numalogic/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/__main__.py` & `numalogic-0.9.1a8/numalogic/udfs/__main__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/_base.py` & `numalogic-0.9.1a8/numalogic/udfs/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/_config.py` & `numalogic-0.9.1a8/numalogic/udfs/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/_logger.py` & `numalogic-0.9.1a8/numalogic/udfs/_logger.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/_metrics.py` & `numalogic-0.9.1a8/numalogic/udfs/_metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/entities.py` & `numalogic-0.9.1a8/numalogic/udfs/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/factory.py` & `numalogic-0.9.1a8/numalogic/udfs/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/inference.py` & `numalogic-0.9.1a8/numalogic/udfs/inference.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/payloadtx.py` & `numalogic-0.9.1a8/numalogic/udfs/payloadtx.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/postprocess.py` & `numalogic-0.9.1a8/numalogic/udfs/postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/preprocess.py` & `numalogic-0.9.1a8/numalogic/udfs/preprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/staticthresh.py` & `numalogic-0.9.1a8/numalogic/udfs/staticthresh.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/tools.py` & `numalogic-0.9.1a8/numalogic/udfs/tools.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/trainer/_base.py` & `numalogic-0.9.1a8/numalogic/udfs/trainer/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/numalogic/udfs/trainer/_druid.py` & `numalogic-0.9.1a8/numalogic/udfs/trainer/_druid.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
             )
 
         try:
             _df = self.data_fetcher.fetch(
                 datasource=_fetcher_conf.datasource,
                 filter_keys=_stream_conf.composite_keys,
                 filter_values=payload.composite_keys,
+                static_filters=_fetcher_conf.static_filters,
                 dimensions=list(_fetcher_conf.dimensions),
                 delay=self.dataconn_conf.delay_hrs,
                 granularity=_fetcher_conf.granularity,
                 aggregations=dict(_fetcher_conf.aggregations),
                 group_by=list(_fetcher_conf.group_by),
                 pivot=_fetcher_conf.pivot,
                 hours=_conf.numalogic_conf.trainer.train_hours,
```

### Comparing `numalogic-0.9.1a7/numalogic/udfs/trainer/_prom.py` & `numalogic-0.9.1a8/numalogic/udfs/trainer/_prom.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a7/pyproject.toml` & `numalogic-0.9.1a8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic"
-version = "0.9.1a7"
+version = "0.9.1a8"
 description = "Collection of operational Machine Learning models and tools."
 authors = ["Numalogic Developers"]
 packages = [{ include = "numalogic" }]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
```

### Comparing `numalogic-0.9.1a7/PKG-INFO` & `numalogic-0.9.1a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic
-Version: 0.9.1a7
+Version: 0.9.1a8
 Summary: Collection of operational Machine Learning models and tools.
 Home-page: https://numalogic.numaproj.io/
 License: Apache-2.0
 Author: Numalogic Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.9,<3.12
```

