# Comparing `tmp/systemathics_apis-2.39.0.tar.gz` & `tmp/systemathics_apis-2.39.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systemathics_apis-2.39.0.tar", last modified: Wed May  1 14:47:30 2024, max compression
+gzip compressed data, was "systemathics_apis-2.39.1.tar", last modified: Thu May  2 08:30:12 2024, max compression
```

## Comparing `systemathics_apis-2.39.0.tar` & `systemathics_apis-2.39.1.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.238239 systemathics_apis-2.39.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-01 14:47:30.238239 systemathics_apis-2.39.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:47:30.238239 systemathics_apis-2.39.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 14:47:27.000000 systemathics_apis-2.39.0/systemathics/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/helpers/channel_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/helpers/token_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.206239 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/changes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/changes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/dividends_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/dividends_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/splits_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/splits_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/daily/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.210239 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_bars_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_bars_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_calendars_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_calendars_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_greeks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_greeks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_market_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_market_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_open_interest_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_open_interest_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_prices_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_prices_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_settlement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_settlement_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_vwap_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_vwap_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.210239 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/indices/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.210239 systemathics_apis-2.39.0/systemathics/apis/services/indices/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/indices/v1/components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/indices/v1/components_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/intraday/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.214239 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_bars_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_bars_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_greeks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_greeks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_market_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_market_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_prices_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_prices_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_settlement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_settlement_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_vwap_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_vwap_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.218239 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/reference_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.218239 systemathics_apis-2.39.0/systemathics/apis/services/reference_data/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/reference_data/v1/reference_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/reference_data/v1/reference_data_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/screener_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.218239 systemathics_apis-2.39.0/systemathics/apis/services/screener_data/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/screener_data/v1/screener_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/screener_data/v1/screener_data_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/services/static_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.218239 systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/sector_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/sector_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    41769 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/static_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/static_data_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/services/sustainability/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.218239 systemathics_apis-2.39.0/systemathics/apis/services/sustainability/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/sustainability/v1/sustainability_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/sustainability/v1/sustainability_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/services/tick/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.222239 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_book_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_book_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_quotes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_quotes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_raw_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_raw_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_updates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_updates_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.226239 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/services/tick_conditions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.226239 systemathics_apis-2.39.0/systemathics/apis/services/tick_conditions/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/services/topology/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.226239 systemathics_apis-2.39.0/systemathics/apis/services/topology/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/topology/v1/topologies_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/topology/v1/topologies_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.226239 systemathics_apis-2.39.0/systemathics/apis/services/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/v1/artifacts_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/v1/artifacts_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/type/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/type/shared/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.238239 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/action_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/action_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_updates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_updates_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/condition_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/condition_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/constraints_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/constraints_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/date_interval_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/date_interval_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/field_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/field_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/identifier_and_level_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/identifier_and_level_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/identifier_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/identifier_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/keys_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/keys_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/level_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/level_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/limit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/limit_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mappings_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mappings_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/market_fields_updates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/market_fields_updates_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mbl_market_book_updates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mbl_market_book_updates_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mbo_market_book_updates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mbo_market_book_updates_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/memo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/memo_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/quote_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/quote_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/quotes_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/quotes_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/raw_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/raw_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/sampling_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/sampling_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/side_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/side_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/stream_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/stream_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/time_interval_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/time_interval_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_and_book_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_and_book_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.238239 systemathics_apis-2.39.0/systemathics.apis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-01 14:47:30.000000 systemathics_apis-2.39.0/systemathics.apis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-05-01 14:47:30.000000 systemathics_apis-2.39.0/systemathics.apis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:47:30.000000 systemathics_apis-2.39.0/systemathics.apis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 14:47:30.000000 systemathics_apis-2.39.0/systemathics.apis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 14:47:30.000000 systemathics_apis-2.39.0/systemathics.apis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.088317 systemathics_apis-2.39.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-02 08:30:12.088317 systemathics_apis-2.39.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 08:30:12.088317 systemathics_apis-2.39.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.048316 systemathics_apis-2.39.1/systemathics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.052317 systemathics_apis-2.39.1/systemathics/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 08:30:09.000000 systemathics_apis-2.39.1/systemathics/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.052317 systemathics_apis-2.39.1/systemathics/apis/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/helpers/channel_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/helpers/token_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.052317 systemathics_apis-2.39.1/systemathics/apis/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.048316 systemathics_apis-2.39.1/systemathics/apis/services/corporate_actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.056316 systemathics_apis-2.39.1/systemathics/apis/services/corporate_actions/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/corporate_actions/v1/changes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/corporate_actions/v1/changes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/corporate_actions/v1/dividends_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/corporate_actions/v1/dividends_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/corporate_actions/v1/splits_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/corporate_actions/v1/splits_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.048316 systemathics_apis-2.39.1/systemathics/apis/services/daily/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.060316 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_bars_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_bars_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_calendars_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_calendars_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_greeks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_greeks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_market_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_market_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_open_interest_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_open_interest_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_prices_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_prices_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_settlement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_settlement_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_vwap_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_vwap_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.048316 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.060316 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.048316 systemathics_apis-2.39.1/systemathics/apis/services/indices/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.060316 systemathics_apis-2.39.1/systemathics/apis/services/indices/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/indices/v1/components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/indices/v1/components_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.048316 systemathics_apis-2.39.1/systemathics/apis/services/intraday/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.064317 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_bars_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_bars_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_greeks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_greeks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_market_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_market_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_prices_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_prices_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_settlement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_settlement_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_vwap_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_vwap_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.048316 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.068317 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.048316 systemathics_apis-2.39.1/systemathics/apis/services/reference_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.068317 systemathics_apis-2.39.1/systemathics/apis/services/reference_data/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/reference_data/v1/reference_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/reference_data/v1/reference_data_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.052317 systemathics_apis-2.39.1/systemathics/apis/services/screener_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.068317 systemathics_apis-2.39.1/systemathics/apis/services/screener_data/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/screener_data/v1/screener_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/screener_data/v1/screener_data_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.052317 systemathics_apis-2.39.1/systemathics/apis/services/static_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.068317 systemathics_apis-2.39.1/systemathics/apis/services/static_data/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/static_data/v1/sector_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/static_data/v1/sector_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41769 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/static_data/v1/static_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/static_data/v1/static_data_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.052317 systemathics_apis-2.39.1/systemathics/apis/services/sustainability/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.068317 systemathics_apis-2.39.1/systemathics/apis/services/sustainability/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/sustainability/v1/sustainability_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/sustainability/v1/sustainability_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.052317 systemathics_apis-2.39.1/systemathics/apis/services/tick/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.072317 systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_book_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_book_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_quotes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_quotes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_raw_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_raw_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_trades_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_trades_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_updates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_updates_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.052317 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.076316 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.052317 systemathics_apis-2.39.1/systemathics/apis/services/tick_conditions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.076316 systemathics_apis-2.39.1/systemathics/apis/services/tick_conditions/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.052317 systemathics_apis-2.39.1/systemathics/apis/services/topology/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.076316 systemathics_apis-2.39.1/systemathics/apis/services/topology/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/topology/v1/topologies_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/topology/v1/topologies_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.076316 systemathics_apis-2.39.1/systemathics/apis/services/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/v1/artifacts_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/services/v1/artifacts_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.052317 systemathics_apis-2.39.1/systemathics/apis/type/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.052317 systemathics_apis-2.39.1/systemathics/apis/type/shared/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.088317 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/action_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/action_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/book_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/book_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/book_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/book_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/book_updates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/book_updates_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/condition_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/condition_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/constraints_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/constraints_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/date_interval_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/date_interval_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/field_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/field_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/identifier_and_level_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/identifier_and_level_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/identifier_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/identifier_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/keys_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/keys_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/level_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/level_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/limit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/limit_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/mappings_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/mappings_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/market_fields_updates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/market_fields_updates_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/mbl_market_book_updates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/mbl_market_book_updates_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/mbo_market_book_updates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/mbo_market_book_updates_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/memo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/memo_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/quote_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/quote_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/quotes_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/quotes_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/raw_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/raw_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/sampling_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/sampling_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/side_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/side_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/stream_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/stream_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/time_interval_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/time_interval_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/trade_and_book_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/trade_and_book_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/trade_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/trade_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/trade_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 08:30:02.000000 systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/trade_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:30:12.088317 systemathics_apis-2.39.1/systemathics.apis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-02 08:30:12.000000 systemathics_apis-2.39.1/systemathics.apis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-05-02 08:30:12.000000 systemathics_apis-2.39.1/systemathics.apis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:30:12.000000 systemathics_apis-2.39.1/systemathics.apis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 08:30:12.000000 systemathics_apis-2.39.1/systemathics.apis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 08:30:12.000000 systemathics_apis-2.39.1/systemathics.apis.egg-info/top_level.txt
```

### Comparing `systemathics_apis-2.39.0/LICENSE` & `systemathics_apis-2.39.1/LICENSE`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/PKG-INFO` & `systemathics_apis-2.39.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systemathics.apis
-Version: 2.39.0
+Version: 2.39.1
 Summary: Grpc stub for Systemathics API.
 Author-email: Systemathics <contact@systemathics.com>
 License: MIT License
         
         Copyright (c) 2021 Systemathics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `systemathics_apis-2.39.0/README.md` & `systemathics_apis-2.39.1/README.md`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/pyproject.toml` & `systemathics_apis-2.39.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/helpers/channel_helpers.py` & `systemathics_apis-2.39.1/systemathics/apis/helpers/channel_helpers.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/helpers/token_helpers.py` & `systemathics_apis-2.39.1/systemathics/apis/helpers/token_helpers.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/changes_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/corporate_actions/v1/changes_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/changes_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/corporate_actions/v1/changes_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/dividends_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/corporate_actions/v1/dividends_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/dividends_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/corporate_actions/v1/dividends_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/splits_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/corporate_actions/v1/splits_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/splits_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/corporate_actions/v1/splits_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_bars_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_bars_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_bars_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_bars_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_calendars_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_calendars_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_calendars_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_calendars_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_greeks_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_greeks_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_greeks_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_greeks_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_market_data_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_market_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_market_data_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_market_data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_open_interest_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_open_interest_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_open_interest_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_open_interest_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_prices_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_prices_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_prices_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_prices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_settlement_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_settlement_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_settlement_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_settlement_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_vwap_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_vwap_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_vwap_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily/v1/daily_vwap_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/indices/v1/components_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/indices/v1/components_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/indices/v1/components_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/indices/v1/components_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_bars_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_bars_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_bars_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_bars_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_greeks_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_greeks_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_greeks_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_greeks_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_market_data_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_market_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_market_data_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_market_data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_prices_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_prices_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_prices_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_prices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_settlement_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_settlement_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_settlement_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_settlement_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_vwap_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_vwap_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_vwap_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday/v1/intraday_vwap_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/reference_data/v1/reference_data_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/reference_data/v1/reference_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/reference_data/v1/reference_data_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/reference_data/v1/reference_data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/screener_data/v1/screener_data_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/screener_data/v1/screener_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/screener_data/v1/screener_data_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/screener_data/v1/screener_data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/sector_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/static_data/v1/sector_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/sector_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/static_data/v1/sector_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/static_data_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/static_data/v1/static_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/static_data_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/static_data/v1/static_data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/sustainability/v1/sustainability_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/sustainability/v1/sustainability_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/sustainability/v1/sustainability_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/sustainability/v1/sustainability_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_book_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_book_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_book_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_book_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_quotes_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_quotes_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_quotes_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_quotes_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_raw_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_raw_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_raw_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_raw_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_trades_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_trades_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_updates_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_updates_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_updates_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick/v1/tick_updates_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/topology/v1/topologies_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/topology/v1/topologies_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/topology/v1/topologies_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/topology/v1/topologies_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/v1/artifacts_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/services/v1/artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/services/v1/artifacts_pb2_grpc.py` & `systemathics_apis-2.39.1/systemathics/apis/services/v1/artifacts_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/action_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_data_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/book_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/book_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_updates_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/book_updates_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/condition_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/condition_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/constraints_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/date_interval_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/date_interval_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/field_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/field_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/identifier_and_level_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/identifier_and_level_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/identifier_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/identifier_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/keys_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/level_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/level_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/limit_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/limit_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mappings_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/mappings_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/market_fields_updates_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/market_fields_updates_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mbl_market_book_updates_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/mbl_market_book_updates_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mbo_market_book_updates_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/mbo_market_book_updates_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/memo_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/memo_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/quote_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/quote_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/quotes_data_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/quotes_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/raw_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/raw_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/sampling_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/sampling_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/side_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/side_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/stream_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/stream_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/time_interval_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/time_interval_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_and_book_data_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/trade_and_book_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_data_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/trade_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_pb2.py` & `systemathics_apis-2.39.1/systemathics/apis/type/shared/v1/trade_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.39.0/systemathics.apis.egg-info/PKG-INFO` & `systemathics_apis-2.39.1/systemathics.apis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systemathics.apis
-Version: 2.39.0
+Version: 2.39.1
 Summary: Grpc stub for Systemathics API.
 Author-email: Systemathics <contact@systemathics.com>
 License: MIT License
         
         Copyright (c) 2021 Systemathics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `systemathics_apis-2.39.0/systemathics.apis.egg-info/SOURCES.txt` & `systemathics_apis-2.39.1/systemathics.apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

