# Comparing `tmp/systemathics_apis-2.38.4.tar.gz` & `tmp/systemathics_apis-2.39.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systemathics_apis-2.38.4.tar", last modified: Thu Apr 25 07:43:24 2024, max compression
+gzip compressed data, was "systemathics_apis-2.39.0.tar", last modified: Wed May  1 14:47:30 2024, max compression
```

## Comparing `systemathics_apis-2.38.4.tar` & `systemathics_apis-2.39.0.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.652109 systemathics_apis-2.38.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-25 07:43:24.652109 systemathics_apis-2.38.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 07:43:24.652109 systemathics_apis-2.38.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.612110 systemathics_apis-2.38.4/systemathics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.616109 systemathics_apis-2.38.4/systemathics/apis/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 07:43:22.000000 systemathics_apis-2.38.4/systemathics/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.616109 systemathics_apis-2.38.4/systemathics/apis/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/helpers/channel_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/helpers/token_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.616109 systemathics_apis-2.38.4/systemathics/apis/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.612110 systemathics_apis-2.38.4/systemathics/apis/services/corporate_actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.616109 systemathics_apis-2.38.4/systemathics/apis/services/corporate_actions/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/corporate_actions/v1/changes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/corporate_actions/v1/changes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/corporate_actions/v1/dividends_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/corporate_actions/v1/dividends_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/corporate_actions/v1/splits_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/corporate_actions/v1/splits_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.612110 systemathics_apis-2.38.4/systemathics/apis/services/daily/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.620109 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_bars_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_bars_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_calendars_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_calendars_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_greeks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_greeks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_market_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_market_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_open_interest_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_open_interest_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_prices_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_prices_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_settlement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_settlement_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_vwap_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_vwap_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.612110 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.624109 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.612110 systemathics_apis-2.38.4/systemathics/apis/services/indices/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.624109 systemathics_apis-2.38.4/systemathics/apis/services/indices/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/indices/v1/components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/indices/v1/components_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.612110 systemathics_apis-2.38.4/systemathics/apis/services/intraday/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.628109 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_bars_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_bars_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_greeks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_greeks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_market_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_market_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_prices_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_prices_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_settlement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_settlement_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_vwap_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_vwap_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.612110 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.632109 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.612110 systemathics_apis-2.38.4/systemathics/apis/services/reference_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.632109 systemathics_apis-2.38.4/systemathics/apis/services/reference_data/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/reference_data/v1/reference_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/reference_data/v1/reference_data_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.612110 systemathics_apis-2.38.4/systemathics/apis/services/screener_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.632109 systemathics_apis-2.38.4/systemathics/apis/services/screener_data/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/screener_data/v1/screener_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/screener_data/v1/screener_data_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.612110 systemathics_apis-2.38.4/systemathics/apis/services/static_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.632109 systemathics_apis-2.38.4/systemathics/apis/services/static_data/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/static_data/v1/sector_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/static_data/v1/sector_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    41769 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/static_data/v1/static_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/static_data/v1/static_data_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.612110 systemathics_apis-2.38.4/systemathics/apis/services/sustainability/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.632109 systemathics_apis-2.38.4/systemathics/apis/services/sustainability/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/sustainability/v1/sustainability_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/sustainability/v1/sustainability_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.612110 systemathics_apis-2.38.4/systemathics/apis/services/tick/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.636109 systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_book_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_book_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_quotes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_quotes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_raw_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_raw_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_trades_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_trades_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_updates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_updates_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.612110 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.640109 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.612110 systemathics_apis-2.38.4/systemathics/apis/services/tick_conditions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.640109 systemathics_apis-2.38.4/systemathics/apis/services/tick_conditions/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.616109 systemathics_apis-2.38.4/systemathics/apis/services/topology/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.640109 systemathics_apis-2.38.4/systemathics/apis/services/topology/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/topology/v1/topologies_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/topology/v1/topologies_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.640109 systemathics_apis-2.38.4/systemathics/apis/services/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/v1/artifacts_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/services/v1/artifacts_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.616109 systemathics_apis-2.38.4/systemathics/apis/type/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.616109 systemathics_apis-2.38.4/systemathics/apis/type/shared/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.652109 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/action_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/action_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/book_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/book_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/book_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/book_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/book_updates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/book_updates_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/condition_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/condition_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/constraints_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/constraints_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/date_interval_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/date_interval_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/field_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/field_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/identifier_and_level_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/identifier_and_level_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/identifier_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/identifier_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/keys_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/keys_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/level_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/level_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/limit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/limit_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/mappings_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/mappings_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/market_fields_updates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/market_fields_updates_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/mbl_market_book_updates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/mbl_market_book_updates_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/mbo_market_book_updates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/mbo_market_book_updates_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/memo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/memo_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/quote_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/quote_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/quotes_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/quotes_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/raw_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/raw_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/sampling_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/sampling_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/side_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/side_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/stream_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/stream_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/time_interval_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/time_interval_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/trade_and_book_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/trade_and_book_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/trade_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/trade_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/trade_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-25 07:43:11.000000 systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/trade_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:43:24.652109 systemathics_apis-2.38.4/systemathics.apis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-25 07:43:24.000000 systemathics_apis-2.38.4/systemathics.apis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-04-25 07:43:24.000000 systemathics_apis-2.38.4/systemathics.apis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:43:24.000000 systemathics_apis-2.38.4/systemathics.apis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-25 07:43:24.000000 systemathics_apis-2.38.4/systemathics.apis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 07:43:24.000000 systemathics_apis-2.38.4/systemathics.apis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.238239 systemathics_apis-2.39.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-01 14:47:30.238239 systemathics_apis-2.39.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 14:47:30.238239 systemathics_apis-2.39.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 14:47:27.000000 systemathics_apis-2.39.0/systemathics/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/helpers/channel_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/helpers/token_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.206239 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/changes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/changes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/dividends_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/dividends_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/splits_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/splits_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/daily/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.210239 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_bars_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_bars_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_calendars_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_calendars_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_greeks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_greeks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_market_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_market_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_open_interest_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_open_interest_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_prices_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_prices_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_settlement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_settlement_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_vwap_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_vwap_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.210239 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/indices/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.210239 systemathics_apis-2.39.0/systemathics/apis/services/indices/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/indices/v1/components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/indices/v1/components_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/intraday/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.214239 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_bars_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_bars_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_greeks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_greeks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_market_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_market_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_prices_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_prices_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_settlement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_settlement_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_vwap_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_vwap_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.218239 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/reference_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.218239 systemathics_apis-2.39.0/systemathics/apis/services/reference_data/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/reference_data/v1/reference_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/reference_data/v1/reference_data_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.198239 systemathics_apis-2.39.0/systemathics/apis/services/screener_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.218239 systemathics_apis-2.39.0/systemathics/apis/services/screener_data/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/screener_data/v1/screener_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/screener_data/v1/screener_data_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/services/static_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.218239 systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/sector_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/sector_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41769 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/static_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/static_data_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/services/sustainability/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.218239 systemathics_apis-2.39.0/systemathics/apis/services/sustainability/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/sustainability/v1/sustainability_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/sustainability/v1/sustainability_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/services/tick/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.222239 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_book_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_book_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_quotes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_quotes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_raw_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_raw_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_updates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_updates_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.226239 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/services/tick_conditions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.226239 systemathics_apis-2.39.0/systemathics/apis/services/tick_conditions/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/services/topology/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.226239 systemathics_apis-2.39.0/systemathics/apis/services/topology/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/topology/v1/topologies_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/topology/v1/topologies_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.226239 systemathics_apis-2.39.0/systemathics/apis/services/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/v1/artifacts_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/services/v1/artifacts_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/type/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.202239 systemathics_apis-2.39.0/systemathics/apis/type/shared/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.238239 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/action_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/action_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_updates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_updates_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/condition_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/condition_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/constraints_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/constraints_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/date_interval_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/date_interval_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/field_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/field_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/identifier_and_level_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/identifier_and_level_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/identifier_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/identifier_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/keys_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/keys_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/level_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/level_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/limit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/limit_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mappings_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mappings_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/market_fields_updates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/market_fields_updates_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mbl_market_book_updates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mbl_market_book_updates_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mbo_market_book_updates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mbo_market_book_updates_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/memo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/memo_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/quote_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/quote_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/quotes_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/quotes_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/raw_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/raw_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/sampling_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/sampling_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/side_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/side_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/stream_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/stream_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/time_interval_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/time_interval_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_and_book_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_and_book_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 14:47:17.000000 systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 14:47:30.238239 systemathics_apis-2.39.0/systemathics.apis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-01 14:47:30.000000 systemathics_apis-2.39.0/systemathics.apis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11373 2024-05-01 14:47:30.000000 systemathics_apis-2.39.0/systemathics.apis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 14:47:30.000000 systemathics_apis-2.39.0/systemathics.apis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 14:47:30.000000 systemathics_apis-2.39.0/systemathics.apis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 14:47:30.000000 systemathics_apis-2.39.0/systemathics.apis.egg-info/top_level.txt
```

### Comparing `systemathics_apis-2.38.4/LICENSE` & `systemathics_apis-2.39.0/LICENSE`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/PKG-INFO` & `systemathics_apis-2.39.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systemathics.apis
-Version: 2.38.4
+Version: 2.39.0
 Summary: Grpc stub for Systemathics API.
 Author-email: Systemathics <contact@systemathics.com>
 License: MIT License
         
         Copyright (c) 2021 Systemathics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `systemathics_apis-2.38.4/README.md` & `systemathics_apis-2.39.0/README.md`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/pyproject.toml` & `systemathics_apis-2.39.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/helpers/channel_helpers.py` & `systemathics_apis-2.39.0/systemathics/apis/helpers/channel_helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,61 +4,54 @@
 
 functions:
     * get_grpc_channel - Get a channel suitable to call Ganymede gRPC API.
     * get_aio_grpc_channel - Get an aio channel suitable to call Ganymede gRPC API.
 """
 
 import os
+from shutil import ExecError
 import grpc
-import urllib.request
-import pathlib
-    
+
 DEFAULT_ENDPOINT = "https://grpc.ganymede.cloud"
 
-def get_grpc_channel(endpoint = "") -> grpc.Channel:
+def get_grpc_channel() -> grpc.Channel:
     """
     Get a channel suitable to call Ganymede gRPC API.
-    If no endpoint parameter is given, try to use GRPC_APIS environment variable or fallback to DEFAULT_ENDPOINT.
+    This uses the GRPC_APIS environment variable in the form http[s]://fdqn[:port] (if no scheme is give, we'll assume https).
+    If none is detected, use DEFAULT_ENDPOINT.
     Note:
-        For secure channels, we'll try to guess the path of CA certificates chain automatically, or download one from Mozilla official site.
+        For secure channels, we'll try to guess the path of CA certificates chain automatically.
+        For windows you need to 'pip install wheel python-certifi-win32' for that to work (it exports Windows CA Store to a PEM file).
         In the event CA certificates cannot be found, or if you want to use a custom file, set the SSL_CERT_FILE environment variable.
     Returns:
-        A channel suitable to call Ganymede gRPC API.
+        An aio channel suitable to call Ganymede gRPC API.
     """
-    endpoint = endpoint if endpoint else os.getenv('GRPC_APIS','')
+    endpoint = os.getenv('GRPC_APIS','')
     endpoint = endpoint if endpoint else DEFAULT_ENDPOINT # if no endpoint was provided, use the default one
     endpoint = endpoint if endpoint.startswith("http") else f"https://{endpoint}" # if no scheme was provided, assume it's https
-    return _get_grpc_channel(endpoint)
-    
-def _get_grpc_channel(endpoint: str) -> grpc.Channel:
-    if not endpoint or not endpoint.startswith("http"):
-        raise "endpoint should have scheme http or https"
     if (endpoint.startswith("https")):
         return grpc.secure_channel(endpoint.replace("https://",""), _get_channel_credentials())
     else:
         return grpc.insecure_channel(endpoint.replace("http://",""))
 
-def get_aio_grpc_channel(endpoint = "") -> grpc.aio.Channel:
+def get_aio_grpc_channel() -> grpc.aio.Channel:
     """
     Get an aio channel suitable to call Ganymede gRPC API.
-    If no endpoint parameter is given, try to use GRPC_APIS environment variable or fallback to DEFAULT_ENDPOINT.
+    This uses the GRPC_APIS environment variable in the form http[s]://fdqn[:port].
+    If none is detected, use DEFAULT_ENDPOINT.
     Note:
-        For secure channels, we'll try to guess the path of CA certificates chain automatically, or download one from Mozilla official site.
+        For secure channels, we'll try to guess the path of CA certificates chain automatically.
+        For windows you need to 'pip install wheel python-certifi-win32' for that to work (it exports Windows CA Store to a PEM file).
         In the event CA certificates cannot be found, or if you want to use a custom file, set the SSL_CERT_FILE environment variable.
     Returns:
         An aio channel suitable to call Ganymede gRPC API.
     """
-    endpoint = endpoint if endpoint else os.getenv('GRPC_APIS','')
+    endpoint = os.getenv('GRPC_APIS','')
     endpoint = endpoint if endpoint else DEFAULT_ENDPOINT # if no endpoint was provided, use the default one
     endpoint = endpoint if endpoint.startswith("http") else f"https://{endpoint}" # if no scheme was provided, assume it's https
-    return _get_aio_grpc_channel(endpoint)
-
-def _get_aio_grpc_channel(endpoint: str) -> grpc.aio.Channel:
-    if not endpoint or not endpoint.startswith("http"):
-        raise "endpoint should have scheme http or https"
     if (endpoint.startswith("https")):
         return grpc.aio.secure_channel(endpoint.replace("https://",""), _get_channel_credentials())
     else:
         return grpc.aio.insecure_channel(endpoint.replace("http://",""))
 
 def _get_channel_credentials() -> grpc.ChannelCredentials:
     # If we have a SSL_CERT_FILE env variable, use it
@@ -71,51 +64,23 @@
     else:
         cabundle = _autodetect_ca_bundle()
 
     with open(cabundle, 'rb') as f:
         credentials = grpc.ssl_channel_credentials(f.read())
         return credentials
 
-def _get_current_mozilla_cacert() -> str:
-    # up to date CA bundle (the official one embedded in Mozilla)
-    url = "http://curl.haxx.se/ca/cacert.pem"
-    
-    # local path for CA bundle
-    cadir = os.path.join(str(pathlib.Path.home()), ".systemathics")
-    cafile = os.path.join(cadir, "cacert.pem")
-    if not os.path.exists(cadir):
-        os.makedirs(cadir)
-    
-    # don't redownload
-    if os.path.exists(cafile):
-        return cafile
-    
-    try:
-        with urllib.request.urlopen(url) as input:
-            with open(cafile, 'wb') as output:
-                output.write(input.read())
-    except urllib.error.URLError as e:
-        print(f"Could not get {url}: {e.reason}")
-           
-    return cafile
-
 def _autodetect_ca_bundle() -> str:
     cabundles = [
 	"/etc/ssl/certs/ca-certificates.crt",                                  # Debian/Ubuntu/Gentoo/etc..
 	"/etc/pki/tls/certs/ca-bundle.crt",                                    # Fedora/RHEL 6
 	"/etc/ssl/ca-bundle.pem",                                              # OpenSUSE
 	"/etc/pki/tls/cacert.pem",                                             # OpenELEC
 	"/etc/pki/ca-trust/extracted/pem/tls-ca-bundle.pem",                   # CentOS/RHEL 7
 	"/etc/ssl/cert.pem",                                                   # Alpine Linux
-    os.path.join(os.getenv('LOCALAPPDATA',''), '.certifi', 'cacert.pem')   # Windows (for those who installed python-certifi-win32, now defunct, e.i: pip install wheel python-certifi-win32)
+    os.path.join(os.getenv('LOCALAPPDATA',''), '.certifi', 'cacert.pem')   # Windows (requires: pip install wheel python-certifi-win32)
     ]
 
-    # probe
     for cabundle in cabundles:
         if (os.path.isfile(cabundle)):
-            print(f"Using CA bundle {cabundle}")
             return cabundle
 
-    # fallback to current mozilla trusted root CA certificate chain
-    cabundle = _get_current_mozilla_cacert()
-    print(f"Using CA bundle {cabundle}")
-    return cabundle
+    raise Exception(f"Could not auto detect trusted root certificates file, tried {cabundles}. Please help by setting SSL_CERT_FILE environment variable")
```

### Comparing `systemathics_apis-2.38.4/systemathics/apis/helpers/token_helpers.py` & `systemathics_apis-2.39.0/systemathics/apis/helpers/token_helpers.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/corporate_actions/v1/changes_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/changes_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/corporate_actions/v1/changes_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/changes_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/corporate_actions/v1/dividends_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/dividends_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/corporate_actions/v1/dividends_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/dividends_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/corporate_actions/v1/splits_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/splits_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/corporate_actions/v1/splits_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/corporate_actions/v1/splits_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_bars_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_bars_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_bars_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_bars_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_calendars_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_calendars_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_calendars_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_calendars_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_greeks_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_greeks_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_greeks_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_greeks_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_implied_volatility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_market_data_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_market_data_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.type import date_pb2 as google_dot_type_dot_date__pb2
 from systemathics.apis.type.shared.v1 import identifier_pb2 as systemathics_dot_apis_dot_type_dot_shared_dot_v1_dot_identifier__pb2
 from systemathics.apis.type.shared.v1 import date_interval_pb2 as systemathics_dot_apis_dot_type_dot_shared_dot_v1_dot_date__interval__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;systemathics/apis/services/daily/v1/daily_market_data.proto\x12#systemathics.apis.services.daily.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x16google/type/date.proto\x1a\x31systemathics/apis/type/shared/v1/identifier.proto\x1a\x34systemathics/apis/type/shared/v1/date_interval.proto\"\xbb\x01\n\x16\x44\x61ilyMarketDataRequest\x12L\n\nidentifier\x18\x01 \x01(\x0b\x32,.systemathics.apis.type.shared.v1.IdentifierR\nidentifier\x12S\n\rdate_interval\x18\x02 \x01(\x0b\x32..systemathics.apis.type.shared.v1.DateIntervalR\x0c\x64\x61teInterval\"c\n\x17\x44\x61ilyMarketDataResponse\x12H\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x34.systemathics.apis.services.daily.v1.DailyMarketDataR\x04\x64\x61ta\"\xfa\x0f\n\x0f\x44\x61ilyMarketData\x12%\n\x04\x64\x61te\x18\x01 \x01(\x0b\x32\x11.google.type.DateR\x04\x64\x61te\x12\x12\n\x04open\x18\x02 \x01(\x01R\x04open\x12\x12\n\x04high\x18\x03 \x01(\x01R\x04high\x12\x10\n\x03low\x18\x04 \x01(\x01R\x03low\x12\x14\n\x05\x63lose\x18\x05 \x01(\x01R\x05\x63lose\x12\x16\n\x06volume\x18\x06 \x01(\x01R\x06volume\x12\x1b\n\tbid_price\x18\x07 \x01(\x01R\x08\x62idPrice\x12\x19\n\x08\x62id_size\x18\x08 \x01(\x01R\x07\x62idSize\x12\x1b\n\task_price\x18\t \x01(\x01R\x08\x61skPrice\x12\x19\n\x08\x61sk_size\x18\n \x01(\x01R\x07\x61skSize\x12\x14\n\x05\x64\x65lta\x18\x0b \x01(\x01R\x05\x64\x65lta\x12\x14\n\x05gamma\x18\x0c \x01(\x01R\x05gamma\x12\x14\n\x05theta\x18\r \x01(\x01R\x05theta\x12\x12\n\x04vega\x18\x0e \x01(\x01R\x04vega\x12\x10\n\x03rho\x18\x0f \x01(\x01R\x03rho\x12-\n\x12implied_volatility\x18\x10 \x01(\x01R\x11impliedVolatility\x12#\n\ropen_interest\x18\x11 \x01(\x01R\x0copenInterest\x12\x1e\n\nunderlying\x18\x12 \x01(\tR\nunderlying\x12;\n\x1aimplied_volatility_30_call\x18\x13 \x01(\x01R\x17impliedVolatility30Call\x12\x39\n\x19implied_volatility_30_put\x18\x14 \x01(\x01R\x16impliedVolatility30Put\x12;\n\x1aimplied_volatility_30_mean\x18\x15 \x01(\x01R\x17impliedVolatility30Mean\x12;\n\x1aimplied_volatility_60_call\x18\x16 \x01(\x01R\x17impliedVolatility60Call\x12\x39\n\x19implied_volatility_60_put\x18\x17 \x01(\x01R\x16impliedVolatility60Put\x12;\n\x1aimplied_volatility_60_mean\x18\x18 \x01(\x01R\x17impliedVolatility60Mean\x12;\n\x1aimplied_volatility_90_call\x18\x19 \x01(\x01R\x17impliedVolatility90Call\x12\x39\n\x19implied_volatility_90_put\x18\x1a \x01(\x01R\x16impliedVolatility90Put\x12;\n\x1aimplied_volatility_90_mean\x18\x1b \x01(\x01R\x17impliedVolatility90Mean\x12=\n\x1bimplied_volatility_120_call\x18\x1c \x01(\x01R\x18impliedVolatility120Call\x12;\n\x1aimplied_volatility_120_put\x18\x1d \x01(\x01R\x17impliedVolatility120Put\x12=\n\x1bimplied_volatility_120_mean\x18\x1e \x01(\x01R\x18impliedVolatility120Mean\x12=\n\x1bimplied_volatility_150_call\x18\x1f \x01(\x01R\x18impliedVolatility150Call\x12;\n\x1aimplied_volatility_150_put\x18  \x01(\x01R\x17impliedVolatility150Put\x12=\n\x1bimplied_volatility_150_mean\x18! \x01(\x01R\x18impliedVolatility150Mean\x12=\n\x1bimplied_volatility_180_call\x18\" \x01(\x01R\x18impliedVolatility180Call\x12;\n\x1aimplied_volatility_180_put\x18# \x01(\x01R\x17impliedVolatility180Put\x12=\n\x1bimplied_volatility_180_mean\x18$ \x01(\x01R\x18impliedVolatility180Mean\x12=\n\x1bimplied_volatility_360_call\x18% \x01(\x01R\x18impliedVolatility360Call\x12;\n\x1aimplied_volatility_360_put\x18& \x01(\x01R\x17impliedVolatility360Put\x12=\n\x1bimplied_volatility_360_mean\x18\' \x01(\x01R\x18impliedVolatility360Mean\x12\x1f\n\x0b\x63\x61ll_volume\x18( \x01(\x01R\ncallVolume\x12\x1d\n\nput_volume\x18) \x01(\x01R\tputVolume\x12!\n\x0ctotal_volume\x18* \x01(\x01R\x0btotalVolume\x12,\n\x12\x63\x61ll_open_interest\x18+ \x01(\x01R\x10\x63\x61llOpenInterest\x12*\n\x11put_open_interest\x18, \x01(\x01R\x0fputOpenInterest\x12.\n\x13total_open_interest\x18- \x01(\x01R\x11totalOpenInterest\x12\x14\n\x05score\x18. \x01(\x01R\x05score2\xc5\x01\n\x16\x44\x61ilyMarketDataService\x12\xaa\x01\n\x0f\x44\x61ilyMarketData\x12;.systemathics.apis.services.daily.v1.DailyMarketDataRequest\x1a<.systemathics.apis.services.daily.v1.DailyMarketDataResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/daily/marketdataB\xf0\x01\n\'com.systemathics.apis.services.daily.v1B\x14\x44\x61ilyMarketDataProtoP\x01\xa2\x02\x04SASD\xaa\x02#Systemathics.Apis.Services.Daily.V1\xca\x02#Systemathics\\Apis\\Services\\Daily\\V1\xe2\x02/Systemathics\\Apis\\Services\\Daily\\V1\\GPBMetadata\xea\x02\'Systemathics::Apis::Services::Daily::V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n;systemathics/apis/services/daily/v1/daily_market_data.proto\x12#systemathics.apis.services.daily.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x16google/type/date.proto\x1a\x31systemathics/apis/type/shared/v1/identifier.proto\x1a\x34systemathics/apis/type/shared/v1/date_interval.proto\"\xbb\x01\n\x16\x44\x61ilyMarketDataRequest\x12L\n\nidentifier\x18\x01 \x01(\x0b\x32,.systemathics.apis.type.shared.v1.IdentifierR\nidentifier\x12S\n\rdate_interval\x18\x02 \x01(\x0b\x32..systemathics.apis.type.shared.v1.DateIntervalR\x0c\x64\x61teInterval\"c\n\x17\x44\x61ilyMarketDataResponse\x12H\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x34.systemathics.apis.services.daily.v1.DailyMarketDataR\x04\x64\x61ta\"\xf6\x0f\n\x0f\x44\x61ilyMarketData\x12%\n\x04\x64\x61te\x18\x01 \x01(\x0b\x32\x11.google.type.DateR\x04\x64\x61te\x12\x12\n\x04open\x18\x02 \x01(\x01R\x04open\x12\x12\n\x04high\x18\x03 \x01(\x01R\x04high\x12\x10\n\x03low\x18\x04 \x01(\x01R\x03low\x12\x14\n\x05\x63lose\x18\x05 \x01(\x01R\x05\x63lose\x12\x16\n\x06volume\x18\x06 \x01(\x01R\x06volume\x12\x1a\n\x08\x42idPrice\x18\x07 \x01(\x01R\x08\x42idPrice\x12\x18\n\x07\x42idSize\x18\x08 \x01(\x01R\x07\x42idSize\x12\x1a\n\x08\x41skPrice\x18\t \x01(\x01R\x08\x41skPrice\x12\x18\n\x07\x41skSize\x18\n \x01(\x01R\x07\x41skSize\x12\x14\n\x05\x64\x65lta\x18\x0b \x01(\x01R\x05\x64\x65lta\x12\x14\n\x05gamma\x18\x0c \x01(\x01R\x05gamma\x12\x14\n\x05theta\x18\r \x01(\x01R\x05theta\x12\x12\n\x04vega\x18\x0e \x01(\x01R\x04vega\x12\x10\n\x03rho\x18\x0f \x01(\x01R\x03rho\x12-\n\x12implied_volatility\x18\x10 \x01(\x01R\x11impliedVolatility\x12#\n\ropen_interest\x18\x11 \x01(\x01R\x0copenInterest\x12\x1e\n\nunderlying\x18\x12 \x01(\x01R\nunderlying\x12;\n\x1aimplied_volatility_30_call\x18\x13 \x01(\x01R\x17impliedVolatility30Call\x12\x39\n\x19implied_volatility_30_put\x18\x14 \x01(\x01R\x16impliedVolatility30Put\x12;\n\x1aimplied_volatility_30_mean\x18\x15 \x01(\x01R\x17impliedVolatility30Mean\x12;\n\x1aimplied_volatility_60_call\x18\x16 \x01(\x01R\x17impliedVolatility60Call\x12\x39\n\x19implied_volatility_60_put\x18\x17 \x01(\x01R\x16impliedVolatility60Put\x12;\n\x1aimplied_volatility_60_mean\x18\x18 \x01(\x01R\x17impliedVolatility60Mean\x12;\n\x1aimplied_volatility_90_call\x18\x19 \x01(\x01R\x17impliedVolatility90Call\x12\x39\n\x19implied_volatility_90_put\x18\x1a \x01(\x01R\x16impliedVolatility90Put\x12;\n\x1aimplied_volatility_90_mean\x18\x1b \x01(\x01R\x17impliedVolatility90Mean\x12=\n\x1bimplied_volatility_120_call\x18\x1c \x01(\x01R\x18impliedVolatility120Call\x12;\n\x1aimplied_volatility_120_put\x18\x1d \x01(\x01R\x17impliedVolatility120Put\x12=\n\x1bimplied_volatility_120_mean\x18\x1e \x01(\x01R\x18impliedVolatility120Mean\x12=\n\x1bimplied_volatility_150_call\x18\x1f \x01(\x01R\x18impliedVolatility150Call\x12;\n\x1aimplied_volatility_150_put\x18  \x01(\x01R\x17impliedVolatility150Put\x12=\n\x1bimplied_volatility_150_mean\x18! \x01(\x01R\x18impliedVolatility150Mean\x12=\n\x1bimplied_volatility_180_call\x18\" \x01(\x01R\x18impliedVolatility180Call\x12;\n\x1aimplied_volatility_180_put\x18# \x01(\x01R\x17impliedVolatility180Put\x12=\n\x1bimplied_volatility_180_mean\x18$ \x01(\x01R\x18impliedVolatility180Mean\x12=\n\x1bimplied_volatility_360_call\x18% \x01(\x01R\x18impliedVolatility360Call\x12;\n\x1aimplied_volatility_360_put\x18& \x01(\x01R\x17impliedVolatility360Put\x12=\n\x1bimplied_volatility_360_mean\x18\' \x01(\x01R\x18impliedVolatility360Mean\x12\x1f\n\x0b\x63\x61ll_volume\x18( \x01(\x01R\ncallVolume\x12\x1d\n\nput_volume\x18) \x01(\x01R\tputVolume\x12!\n\x0ctotal_volume\x18* \x01(\x01R\x0btotalVolume\x12,\n\x12\x63\x61ll_open_interest\x18+ \x01(\x01R\x10\x63\x61llOpenInterest\x12*\n\x11put_open_interest\x18, \x01(\x01R\x0fputOpenInterest\x12.\n\x13total_open_interest\x18- \x01(\x01R\x11totalOpenInterest\x12\x14\n\x05score\x18. \x01(\x01R\x05score2\xc5\x01\n\x16\x44\x61ilyMarketDataService\x12\xaa\x01\n\x0f\x44\x61ilyMarketData\x12;.systemathics.apis.services.daily.v1.DailyMarketDataRequest\x1a<.systemathics.apis.services.daily.v1.DailyMarketDataResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/daily/marketdataB\xf0\x01\n\'com.systemathics.apis.services.daily.v1B\x14\x44\x61ilyMarketDataProtoP\x01\xa2\x02\x04SASD\xaa\x02#Systemathics.Apis.Services.Daily.V1\xca\x02#Systemathics\\Apis\\Services\\Daily\\V1\xe2\x02/Systemathics\\Apis\\Services\\Daily\\V1\\GPBMetadata\xea\x02\'Systemathics::Apis::Services::Daily::V1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'systemathics.apis.services.daily.v1.daily_market_data_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\'com.systemathics.apis.services.daily.v1B\024DailyMarketDataProtoP\001\242\002\004SASD\252\002#Systemathics.Apis.Services.Daily.V1\312\002#Systemathics\\Apis\\Services\\Daily\\V1\342\002/Systemathics\\Apis\\Services\\Daily\\V1\\GPBMetadata\352\002\'Systemathics::Apis::Services::Daily::V1'
   _globals['_DAILYMARKETDATASERVICE'].methods_by_name['DailyMarketData']._loaded_options = None
   _globals['_DAILYMARKETDATASERVICE'].methods_by_name['DailyMarketData']._serialized_options = b'\202\323\344\223\002\026\022\024/v1/daily/marketdata'
   _globals['_DAILYMARKETDATAREQUEST']._serialized_start=260
   _globals['_DAILYMARKETDATAREQUEST']._serialized_end=447
   _globals['_DAILYMARKETDATARESPONSE']._serialized_start=449
   _globals['_DAILYMARKETDATARESPONSE']._serialized_end=548
   _globals['_DAILYMARKETDATA']._serialized_start=551
-  _globals['_DAILYMARKETDATA']._serialized_end=2593
-  _globals['_DAILYMARKETDATASERVICE']._serialized_start=2596
-  _globals['_DAILYMARKETDATASERVICE']._serialized_end=2793
+  _globals['_DAILYMARKETDATA']._serialized_end=2589
+  _globals['_DAILYMARKETDATASERVICE']._serialized_start=2592
+  _globals['_DAILYMARKETDATASERVICE']._serialized_end=2789
 # @@protoc_insertion_point(module_scope)
```

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_market_data_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_market_data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_open_interest_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_open_interest_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_open_interest_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_open_interest_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_prices_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_prices_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_prices_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_prices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_settlement_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_settlement_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_settlement_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_settlement_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_vwap_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_vwap_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily/v1/daily_vwap_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily/v1/daily_vwap_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_bollinger_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_cma_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_ema_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_macd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_rsi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_sma_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/daily_analytics/v1/daily_volatility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/indices/v1/components_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/indices/v1/components_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/indices/v1/components_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/indices/v1/components_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_bars_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_bars_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_bars_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_bars_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_best_limit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_greeks_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_greeks_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_greeks_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_greeks_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_implied_volatility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_market_data_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_market_data_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from systemathics.apis.type.shared.v1 import identifier_pb2 as systemathics_dot_apis_dot_type_dot_shared_dot_v1_dot_identifier__pb2
 from systemathics.apis.type.shared.v1 import date_interval_pb2 as systemathics_dot_apis_dot_type_dot_shared_dot_v1_dot_date__interval__pb2
 from systemathics.apis.type.shared.v1 import sampling_pb2 as systemathics_dot_apis_dot_type_dot_shared_dot_v1_dot_sampling__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nAsystemathics/apis/services/intraday/v1/intraday_market_data.proto\x12&systemathics.apis.services.intraday.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x31systemathics/apis/type/shared/v1/identifier.proto\x1a\x34systemathics/apis/type/shared/v1/date_interval.proto\x1a/systemathics/apis/type/shared/v1/sampling.proto\"\x86\x02\n\x19IntradayMarketDataRequest\x12L\n\nidentifier\x18\x01 \x01(\x0b\x32,.systemathics.apis.type.shared.v1.IdentifierR\nidentifier\x12\x46\n\x08sampling\x18\x02 \x01(\x0e\x32*.systemathics.apis.type.shared.v1.SamplingR\x08sampling\x12S\n\rdate_interval\x18\x03 \x01(\x0b\x32..systemathics.apis.type.shared.v1.DateIntervalR\x0c\x64\x61teInterval\"l\n\x1aIntradayMarketDataResponse\x12N\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32:.systemathics.apis.services.intraday.v1.IntradayMarketDataR\x04\x64\x61ta\"\x99\x04\n\x12IntradayMarketData\x12\x39\n\ntime_stamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ttimeStamp\x12\x12\n\x04open\x18\x02 \x01(\x01R\x04open\x12\x12\n\x04high\x18\x03 \x01(\x01R\x04high\x12\x10\n\x03low\x18\x04 \x01(\x01R\x03low\x12\x14\n\x05\x63lose\x18\x05 \x01(\x01R\x05\x63lose\x12\x16\n\x06volume\x18\x06 \x01(\x01R\x06volume\x12\x1b\n\tbid_price\x18\x07 \x01(\x01R\x08\x62idPrice\x12\x19\n\x08\x62id_size\x18\x08 \x01(\x01R\x07\x62idSize\x12\x1b\n\task_price\x18\t \x01(\x01R\x08\x61skPrice\x12\x19\n\x08\x61sk_size\x18\n \x01(\x01R\x07\x61skSize\x12\x14\n\x05\x64\x65lta\x18\x0b \x01(\x01R\x05\x64\x65lta\x12\x14\n\x05gamma\x18\x0c \x01(\x01R\x05gamma\x12\x14\n\x05theta\x18\r \x01(\x01R\x05theta\x12\x12\n\x04vega\x18\x0e \x01(\x01R\x04vega\x12\x10\n\x03rho\x18\x0f \x01(\x01R\x03rho\x12-\n\x12implied_volatility\x18\x10 \x01(\x01R\x11impliedVolatility\x12#\n\ropen_interest\x18\x11 \x01(\x01R\x0copenInterest\x12\x1e\n\nunderlying\x18\x12 \x01(\x01R\nunderlying\x12\x14\n\x05score\x18\x13 \x01(\x01R\x05score2\xda\x01\n\x19IntradayMarketDataService\x12\xbc\x01\n\x12IntradayMarketData\x12\x41.systemathics.apis.services.intraday.v1.IntradayMarketDataRequest\x1a\x42.systemathics.apis.services.intraday.v1.IntradayMarketDataResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/v1/intraday/marketdataB\x82\x02\n*com.systemathics.apis.services.intraday.v1B\x17IntradayMarketDataProtoP\x01\xa2\x02\x04SASI\xaa\x02&Systemathics.Apis.Services.Intraday.V1\xca\x02&Systemathics\\Apis\\Services\\Intraday\\V1\xe2\x02\x32Systemathics\\Apis\\Services\\Intraday\\V1\\GPBMetadata\xea\x02*Systemathics::Apis::Services::Intraday::V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nAsystemathics/apis/services/intraday/v1/intraday_market_data.proto\x12&systemathics.apis.services.intraday.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x31systemathics/apis/type/shared/v1/identifier.proto\x1a\x34systemathics/apis/type/shared/v1/date_interval.proto\x1a/systemathics/apis/type/shared/v1/sampling.proto\"\x86\x02\n\x19IntradayMarketDataRequest\x12L\n\nidentifier\x18\x01 \x01(\x0b\x32,.systemathics.apis.type.shared.v1.IdentifierR\nidentifier\x12\x46\n\x08sampling\x18\x02 \x01(\x0e\x32*.systemathics.apis.type.shared.v1.SamplingR\x08sampling\x12S\n\rdate_interval\x18\x03 \x01(\x0b\x32..systemathics.apis.type.shared.v1.DateIntervalR\x0c\x64\x61teInterval\"l\n\x1aIntradayMarketDataResponse\x12N\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32:.systemathics.apis.services.intraday.v1.IntradayMarketDataR\x04\x64\x61ta\"\x95\x04\n\x12IntradayMarketData\x12\x39\n\ntime_stamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ttimeStamp\x12\x12\n\x04open\x18\x02 \x01(\x01R\x04open\x12\x12\n\x04high\x18\x03 \x01(\x01R\x04high\x12\x10\n\x03low\x18\x04 \x01(\x01R\x03low\x12\x14\n\x05\x63lose\x18\x05 \x01(\x01R\x05\x63lose\x12\x16\n\x06volume\x18\x06 \x01(\x01R\x06volume\x12\x1a\n\x08\x42idPrice\x18\x07 \x01(\x01R\x08\x42idPrice\x12\x18\n\x07\x42idSize\x18\x08 \x01(\x01R\x07\x42idSize\x12\x1a\n\x08\x41skPrice\x18\t \x01(\x01R\x08\x41skPrice\x12\x18\n\x07\x41skSize\x18\n \x01(\x01R\x07\x41skSize\x12\x14\n\x05\x64\x65lta\x18\x0b \x01(\x01R\x05\x64\x65lta\x12\x14\n\x05gamma\x18\x0c \x01(\x01R\x05gamma\x12\x14\n\x05theta\x18\r \x01(\x01R\x05theta\x12\x12\n\x04vega\x18\x0e \x01(\x01R\x04vega\x12\x10\n\x03rho\x18\x0f \x01(\x01R\x03rho\x12-\n\x12implied_volatility\x18\x10 \x01(\x01R\x11impliedVolatility\x12#\n\ropen_interest\x18\x11 \x01(\x01R\x0copenInterest\x12\x1e\n\nunderlying\x18\x12 \x01(\x01R\nunderlying\x12\x14\n\x05score\x18\x13 \x01(\x01R\x05score2\xda\x01\n\x19IntradayMarketDataService\x12\xbc\x01\n\x12IntradayMarketData\x12\x41.systemathics.apis.services.intraday.v1.IntradayMarketDataRequest\x1a\x42.systemathics.apis.services.intraday.v1.IntradayMarketDataResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/v1/intraday/marketdataB\x82\x02\n*com.systemathics.apis.services.intraday.v1B\x17IntradayMarketDataProtoP\x01\xa2\x02\x04SASI\xaa\x02&Systemathics.Apis.Services.Intraday.V1\xca\x02&Systemathics\\Apis\\Services\\Intraday\\V1\xe2\x02\x32Systemathics\\Apis\\Services\\Intraday\\V1\\GPBMetadata\xea\x02*Systemathics::Apis::Services::Intraday::V1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'systemathics.apis.services.intraday.v1.intraday_market_data_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n*com.systemathics.apis.services.intraday.v1B\027IntradayMarketDataProtoP\001\242\002\004SASI\252\002&Systemathics.Apis.Services.Intraday.V1\312\002&Systemathics\\Apis\\Services\\Intraday\\V1\342\0022Systemathics\\Apis\\Services\\Intraday\\V1\\GPBMetadata\352\002*Systemathics::Apis::Services::Intraday::V1'
   _globals['_INTRADAYMARKETDATASERVICE'].methods_by_name['IntradayMarketData']._loaded_options = None
   _globals['_INTRADAYMARKETDATASERVICE'].methods_by_name['IntradayMarketData']._serialized_options = b'\202\323\344\223\002\031\022\027/v1/intraday/marketdata'
   _globals['_INTRADAYMARKETDATAREQUEST']._serialized_start=327
   _globals['_INTRADAYMARKETDATAREQUEST']._serialized_end=589
   _globals['_INTRADAYMARKETDATARESPONSE']._serialized_start=591
   _globals['_INTRADAYMARKETDATARESPONSE']._serialized_end=699
   _globals['_INTRADAYMARKETDATA']._serialized_start=702
-  _globals['_INTRADAYMARKETDATA']._serialized_end=1239
-  _globals['_INTRADAYMARKETDATASERVICE']._serialized_start=1242
-  _globals['_INTRADAYMARKETDATASERVICE']._serialized_end=1460
+  _globals['_INTRADAYMARKETDATA']._serialized_end=1235
+  _globals['_INTRADAYMARKETDATASERVICE']._serialized_start=1238
+  _globals['_INTRADAYMARKETDATASERVICE']._serialized_end=1456
 # @@protoc_insertion_point(module_scope)
```

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_market_data_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_market_data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_open_interest_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_prices_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_prices_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_prices_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_prices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_settlement_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_settlement_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_settlement_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_settlement_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_vwap_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_vwap_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday/v1/intraday_vwap_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday/v1/intraday_vwap_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_bollinger_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_cma_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_ema_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_macd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_rsi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_sma_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/intraday_analytics/v1/intraday_volatility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/reference_data/v1/reference_data_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/reference_data/v1/reference_data_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,29 +18,28 @@
 from systemathics.apis.services.daily.v1 import daily_prices_pb2 as systemathics_dot_apis_dot_services_dot_daily_dot_v1_dot_daily__prices__pb2
 from systemathics.apis.services.daily.v1 import daily_vwap_pb2 as systemathics_dot_apis_dot_services_dot_daily_dot_v1_dot_daily__vwap__pb2
 from systemathics.apis.services.daily.v1 import daily_calendars_pb2 as systemathics_dot_apis_dot_services_dot_daily_dot_v1_dot_daily__calendars__pb2
 from systemathics.apis.services.daily.v1 import daily_open_interest_pb2 as systemathics_dot_apis_dot_services_dot_daily_dot_v1_dot_daily__open__interest__pb2
 from systemathics.apis.services.daily.v1 import daily_implied_volatility_pb2 as systemathics_dot_apis_dot_services_dot_daily_dot_v1_dot_daily__implied__volatility__pb2
 from systemathics.apis.services.daily.v1 import daily_settlement_pb2 as systemathics_dot_apis_dot_services_dot_daily_dot_v1_dot_daily__settlement__pb2
 from systemathics.apis.services.daily.v1 import daily_greeks_pb2 as systemathics_dot_apis_dot_services_dot_daily_dot_v1_dot_daily__greeks__pb2
-from systemathics.apis.services.daily.v1 import daily_market_data_pb2 as systemathics_dot_apis_dot_services_dot_daily_dot_v1_dot_daily__market__data__pb2
 from systemathics.apis.services.corporate_actions.v1 import dividends_pb2 as systemathics_dot_apis_dot_services_dot_corporate__actions_dot_v1_dot_dividends__pb2
 from systemathics.apis.services.corporate_actions.v1 import splits_pb2 as systemathics_dot_apis_dot_services_dot_corporate__actions_dot_v1_dot_splits__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nAsystemathics/apis/services/reference_data/v1/reference_data.proto\x12,systemathics.apis.services.reference_data.v1\x1a\x1cgoogle/api/annotations.proto\x1a;systemathics/apis/services/static_data/v1/static_data.proto\x1a\x34systemathics/apis/services/daily/v1/daily_bars.proto\x1a\x36systemathics/apis/services/daily/v1/daily_prices.proto\x1a\x34systemathics/apis/services/daily/v1/daily_vwap.proto\x1a\x39systemathics/apis/services/daily/v1/daily_calendars.proto\x1a=systemathics/apis/services/daily/v1/daily_open_interest.proto\x1a\x42systemathics/apis/services/daily/v1/daily_implied_volatility.proto\x1a:systemathics/apis/services/daily/v1/daily_settlement.proto\x1a\x36systemathics/apis/services/daily/v1/daily_greeks.proto\x1a;systemathics/apis/services/daily/v1/daily_market_data.proto\x1a?systemathics/apis/services/corporate_actions/v1/dividends.proto\x1a<systemathics/apis/services/corporate_actions/v1/splits.proto\"\x9b\x01\n\x10ReferenceRequest\x12S\n\nasset_type\x18\x01 \x01(\x0e\x32\x34.systemathics.apis.services.static_data.v1.AssetTypeR\tassetType\x12\x16\n\x06ticker\x18\x02 \x01(\tR\x06ticker\x12\x1a\n\x08\x65xchange\x18\x03 \x01(\tR\x08\x65xchange\"\x94\x07\n\x11ReferenceResponse\x12?\n\x03\x62\x61r\x18\x01 \x01(\x0b\x32-.systemathics.apis.services.daily.v1.DailyBarR\x03\x62\x61r\x12\x45\n\x05price\x18\x02 \x01(\x0b\x32/.systemathics.apis.services.daily.v1.DailyPriceR\x05price\x12\x42\n\x04vwap\x18\x03 \x01(\x0b\x32..systemathics.apis.services.daily.v1.DailyVwapR\x04vwap\x12N\n\x08\x63\x61lendar\x18\x04 \x01(\x0b\x32\x32.systemathics.apis.services.daily.v1.DailyCalendarR\x08\x63\x61lendar\x12T\n\nsettlement\x18\x05 \x01(\x0b\x32\x34.systemathics.apis.services.daily.v1.DailySettlementR\nsettlement\x12[\n\ropen_interest\x18\x06 \x01(\x0b\x32\x36.systemathics.apis.services.daily.v1.DailyOpenInterestR\x0copenInterest\x12j\n\x12implied_volatility\x18\x07 \x01(\x0b\x32;.systemathics.apis.services.daily.v1.DailyImpliedVolatilityR\x11impliedVolatility\x12H\n\x06greeks\x18\x08 \x01(\x0b\x32\x30.systemathics.apis.services.daily.v1.DailyGreeksR\x06greeks\x12U\n\x08\x64ividend\x18\t \x01(\x0b\x32\x39.systemathics.apis.services.corporate_actions.v1.DividendR\x08\x64ividend\x12L\n\x05split\x18\n \x01(\x0b\x32\x36.systemathics.apis.services.corporate_actions.v1.SplitR\x05split\x12U\n\x0bmarket_data\x18\x0b \x01(\x0b\x32\x34.systemathics.apis.services.daily.v1.DailyMarketDataR\nmarketData2\xbc\x01\n\x10ReferenceService\x12\xa7\x01\n\tReference\x12>.systemathics.apis.services.reference_data.v1.ReferenceRequest\x1a?.systemathics.apis.services.reference_data.v1.ReferenceResponse\"\x19\x82\xd3\xe4\x93\x02\x13\x12\x11/v1/referencedataB\x97\x02\n0com.systemathics.apis.services.reference_data.v1B\x12ReferenceDataProtoP\x01\xa2\x02\x04SASR\xaa\x02+Systemathics.Apis.Services.ReferenceData.V1\xca\x02+Systemathics\\Apis\\Services\\ReferenceData\\V1\xe2\x02\x37Systemathics\\Apis\\Services\\ReferenceData\\V1\\GPBMetadata\xea\x02/Systemathics::Apis::Services::ReferenceData::V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nAsystemathics/apis/services/reference_data/v1/reference_data.proto\x12,systemathics.apis.services.reference_data.v1\x1a\x1cgoogle/api/annotations.proto\x1a;systemathics/apis/services/static_data/v1/static_data.proto\x1a\x34systemathics/apis/services/daily/v1/daily_bars.proto\x1a\x36systemathics/apis/services/daily/v1/daily_prices.proto\x1a\x34systemathics/apis/services/daily/v1/daily_vwap.proto\x1a\x39systemathics/apis/services/daily/v1/daily_calendars.proto\x1a=systemathics/apis/services/daily/v1/daily_open_interest.proto\x1a\x42systemathics/apis/services/daily/v1/daily_implied_volatility.proto\x1a:systemathics/apis/services/daily/v1/daily_settlement.proto\x1a\x36systemathics/apis/services/daily/v1/daily_greeks.proto\x1a?systemathics/apis/services/corporate_actions/v1/dividends.proto\x1a<systemathics/apis/services/corporate_actions/v1/splits.proto\"\x9b\x01\n\x10ReferenceRequest\x12S\n\nasset_type\x18\x01 \x01(\x0e\x32\x34.systemathics.apis.services.static_data.v1.AssetTypeR\tassetType\x12\x16\n\x06ticker\x18\x02 \x01(\tR\x06ticker\x12\x1a\n\x08\x65xchange\x18\x03 \x01(\tR\x08\x65xchange\"\xbd\x06\n\x11ReferenceResponse\x12?\n\x03\x62\x61r\x18\x01 \x01(\x0b\x32-.systemathics.apis.services.daily.v1.DailyBarR\x03\x62\x61r\x12\x45\n\x05price\x18\x02 \x01(\x0b\x32/.systemathics.apis.services.daily.v1.DailyPriceR\x05price\x12\x42\n\x04vwap\x18\x03 \x01(\x0b\x32..systemathics.apis.services.daily.v1.DailyVwapR\x04vwap\x12N\n\x08\x63\x61lendar\x18\x04 \x01(\x0b\x32\x32.systemathics.apis.services.daily.v1.DailyCalendarR\x08\x63\x61lendar\x12T\n\nsettlement\x18\x05 \x01(\x0b\x32\x34.systemathics.apis.services.daily.v1.DailySettlementR\nsettlement\x12[\n\ropen_interest\x18\x06 \x01(\x0b\x32\x36.systemathics.apis.services.daily.v1.DailyOpenInterestR\x0copenInterest\x12j\n\x12implied_volatility\x18\x07 \x01(\x0b\x32;.systemathics.apis.services.daily.v1.DailyImpliedVolatilityR\x11impliedVolatility\x12H\n\x06greeks\x18\x08 \x01(\x0b\x32\x30.systemathics.apis.services.daily.v1.DailyGreeksR\x06greeks\x12U\n\x08\x64ividend\x18\t \x01(\x0b\x32\x39.systemathics.apis.services.corporate_actions.v1.DividendR\x08\x64ividend\x12L\n\x05split\x18\n \x01(\x0b\x32\x36.systemathics.apis.services.corporate_actions.v1.SplitR\x05split2\xbc\x01\n\x10ReferenceService\x12\xa7\x01\n\tReference\x12>.systemathics.apis.services.reference_data.v1.ReferenceRequest\x1a?.systemathics.apis.services.reference_data.v1.ReferenceResponse\"\x19\x82\xd3\xe4\x93\x02\x13\x12\x11/v1/referencedataB\x97\x02\n0com.systemathics.apis.services.reference_data.v1B\x12ReferenceDataProtoP\x01\xa2\x02\x04SASR\xaa\x02+Systemathics.Apis.Services.ReferenceData.V1\xca\x02+Systemathics\\Apis\\Services\\ReferenceData\\V1\xe2\x02\x37Systemathics\\Apis\\Services\\ReferenceData\\V1\\GPBMetadata\xea\x02/Systemathics::Apis::Services::ReferenceData::V1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'systemathics.apis.services.reference_data.v1.reference_data_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n0com.systemathics.apis.services.reference_data.v1B\022ReferenceDataProtoP\001\242\002\004SASR\252\002+Systemathics.Apis.Services.ReferenceData.V1\312\002+Systemathics\\Apis\\Services\\ReferenceData\\V1\342\0027Systemathics\\Apis\\Services\\ReferenceData\\V1\\GPBMetadata\352\002/Systemathics::Apis::Services::ReferenceData::V1'
   _globals['_REFERENCESERVICE'].methods_by_name['Reference']._loaded_options = None
   _globals['_REFERENCESERVICE'].methods_by_name['Reference']._serialized_options = b'\202\323\344\223\002\023\022\021/v1/referencedata'
-  _globals['_REFERENCEREQUEST']._serialized_start=865
-  _globals['_REFERENCEREQUEST']._serialized_end=1020
-  _globals['_REFERENCERESPONSE']._serialized_start=1023
-  _globals['_REFERENCERESPONSE']._serialized_end=1939
-  _globals['_REFERENCESERVICE']._serialized_start=1942
-  _globals['_REFERENCESERVICE']._serialized_end=2130
+  _globals['_REFERENCEREQUEST']._serialized_start=804
+  _globals['_REFERENCEREQUEST']._serialized_end=959
+  _globals['_REFERENCERESPONSE']._serialized_start=962
+  _globals['_REFERENCERESPONSE']._serialized_end=1791
+  _globals['_REFERENCESERVICE']._serialized_start=1794
+  _globals['_REFERENCESERVICE']._serialized_end=1982
 # @@protoc_insertion_point(module_scope)
```

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/reference_data/v1/reference_data_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/reference_data/v1/reference_data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/screener_data/v1/screener_data_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/screener_data/v1/screener_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/screener_data/v1/screener_data_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/screener_data/v1/screener_data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/static_data/v1/sector_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/sector_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/static_data/v1/sector_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/sector_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/static_data/v1/static_data_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/static_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/static_data/v1/static_data_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/static_data/v1/static_data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/sustainability/v1/sustainability_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/sustainability/v1/sustainability_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/sustainability/v1/sustainability_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/sustainability/v1/sustainability_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_book_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_book_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_book_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_book_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_quotes_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_quotes_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_quotes_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_quotes_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_raw_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_raw_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_raw_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_raw_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_and_book_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_trades_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_trades_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_trades_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_updates_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_updates_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick/v1/tick_updates_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick/v1/tick_updates_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bars_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_bollinger_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_cma_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_ema_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_batch_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_priips_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_sma_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_spread_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_condition_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_trade_conditions_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_analytics/v1/tick_vwap_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/tick_conditions/v1/tick_conditions_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/topology/v1/topologies_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/topology/v1/topologies_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/topology/v1/topologies_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/topology/v1/topologies_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/v1/artifacts_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/services/v1/artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/services/v1/artifacts_pb2_grpc.py` & `systemathics_apis-2.39.0/systemathics/apis/services/v1/artifacts_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/action_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/book_data_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/book_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/book_updates_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/book_updates_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/condition_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/condition_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/constraints_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/date_interval_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/date_interval_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/field_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/field_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/identifier_and_level_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/identifier_and_level_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/identifier_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/identifier_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/keys_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/keys_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/level_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/level_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/limit_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/limit_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/mappings_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mappings_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/market_fields_updates_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/market_fields_updates_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/mbl_market_book_updates_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mbl_market_book_updates_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/mbo_market_book_updates_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/mbo_market_book_updates_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/memo_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/memo_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/quote_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/quote_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/quotes_data_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/quotes_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/raw_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/raw_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/sampling_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/sampling_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/side_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/side_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/stream_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/stream_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/time_interval_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/time_interval_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/trade_and_book_data_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_and_book_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/trade_data_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_data_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics/apis/type/shared/v1/trade_pb2.py` & `systemathics_apis-2.39.0/systemathics/apis/type/shared/v1/trade_pb2.py`

 * *Files identical despite different names*

### Comparing `systemathics_apis-2.38.4/systemathics.apis.egg-info/PKG-INFO` & `systemathics_apis-2.39.0/systemathics.apis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systemathics.apis
-Version: 2.38.4
+Version: 2.39.0
 Summary: Grpc stub for Systemathics API.
 Author-email: Systemathics <contact@systemathics.com>
 License: MIT License
         
         Copyright (c) 2021 Systemathics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `systemathics_apis-2.38.4/systemathics.apis.egg-info/SOURCES.txt` & `systemathics_apis-2.39.0/systemathics.apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

