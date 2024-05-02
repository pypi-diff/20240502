# Comparing `tmp/prediction_market_agent_tooling-0.9.1.tar.gz` & `tmp/prediction_market_agent_tooling-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prediction_market_agent_tooling-0.9.1.tar", max compression
+gzip compressed data, was "prediction_market_agent_tooling-0.9.3.tar", max compression
```

## Comparing `prediction_market_agent_tooling-0.9.1.tar` & `prediction_market_agent_tooling-0.9.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     7650 2024-04-05 08:50:05.815609 prediction_market_agent_tooling-0.9.1/LICENSE
--rw-r--r--   0        0        0     2992 2024-04-05 08:50:05.815609 prediction_market_agent_tooling-0.9.1/README.md
--rw-r--r--   0        0        0     9578 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_dxdao.abi.json
--rw-r--r--   0        0        0    11406 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_fpmm.abi.json
--rw-r--r--   0        0        0     9841 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json
--rw-r--r--   0        0        0     4777 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json
--rw-r--r--   0        0        0     7315 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_kleros.abi.json
--rw-r--r--   0        0        0     1775 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_oracle.abi.json
--rw-r--r--   0        0        0    15953 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_realitio.abi.json
--rw-r--r--   0        0        0     6055 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/wxdai.abi.json
--rw-r--r--   0        0        0        0 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/benchmark/__init__.py
--rw-r--r--   0        0        0     3737 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/benchmark/agents.py
--rw-r--r--   0        0        0    21237 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/benchmark/benchmark.py
--rw-r--r--   0        0        0     2748 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/benchmark/utils.py
--rw-r--r--   0        0        0     2596 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/config.py
--rw-r--r--   0        0        0     7621 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/agent.py
--rw-r--r--   0        0        0      621 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/agent_example.py
--rw-r--r--   0        0        0       82 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/constants.py
--rw-r--r--   0        0        0     3739 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/gcp/deploy.py
--rw-r--r--   0        0        0     5255 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/gcp/utils.py
--rw-r--r--   0        0        0     2526 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/gtypes.py
--rw-r--r--   0        0        0     4488 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/agent_market.py
--rw-r--r--   0        0        0     1026 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/categorize.py
--rw-r--r--   0        0        0      763 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/data_models.py
--rw-r--r--   0        0        0        0 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/__init__.py
--rw-r--r--   0        0        0     6882 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/api.py
--rw-r--r--   0        0        0     5357 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/data_models.py
--rw-r--r--   0        0        0     3402 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/manifold.py
--rw-r--r--   0        0        0      513 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/utils.py
--rw-r--r--   0        0        0     1550 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/markets.py
--rw-r--r--   0        0        0        0 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/__init__.py
--rw-r--r--   0        0        0    10800 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/data_models.py
--rw-r--r--   0        0        0    27589 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen.py
--rw-r--r--   0        0        0    19354 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_contracts.py
--rw-r--r--   0        0        0     7399 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_replicate.py
--rw-r--r--   0        0        0    11382 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_resolve_replicated.py
--rw-r--r--   0        0        0    15716 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_subgraph_handler.py
--rw-r--r--   0        0        0     4188 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/api.py
--rw-r--r--   0        0        0     4199 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/data_models.py
--rw-r--r--   0        0        0    10863 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/data_models_web.py
--rw-r--r--   0        0        0     2652 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/polymarket.py
--rw-r--r--   0        0        0     1960 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/utils.py
--rw-r--r--   0        0        0     2503 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/markets/manifold.py
--rw-r--r--   0        0        0     2419 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/markets/omen.py
--rw-r--r--   0        0        0     2413 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/markets/polymarket.py
--rw-r--r--   0        0        0    11465 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/monitor.py
--rw-r--r--   0        0        0     4045 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/monitor_app.py
--rw-r--r--   0        0        0        0 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/py.typed
--rw-r--r--   0        0        0      625 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/balances.py
--rw-r--r--   0        0        0     3520 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py
--rw-r--r--   0        0        0     4367 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py
--rw-r--r--   0        0        0      422 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/betting_strategies/minimum_bet_to_win.py
--rw-r--r--   0        0        0      429 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/betting_strategies/stretch_bet_between.py
--rw-r--r--   0        0        0      499 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/cache.py
--rw-r--r--   0        0        0     5879 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/contract.py
--rw-r--r--   0        0        0      660 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/gnosis_rpc.py
--rw-r--r--   0        0        0     1761 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/google.py
--rw-r--r--   0        0        0     2037 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/hexbytes_custom.py
--rw-r--r--   0        0        0     2613 2024-04-05 08:50:05.819609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/is_predictable.py
--rw-r--r--   0        0        0      733 2024-04-05 08:50:05.823609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/parallelism.py
--rw-r--r--   0        0        0      729 2024-04-05 08:50:05.823609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/singleton.py
--rw-r--r--   0        0        0     4674 2024-04-05 08:50:05.823609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/utils.py
--rw-r--r--   0        0        0     5314 2024-04-05 08:50:05.823609 prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/web3_utils.py
--rw-r--r--   0        0        0     1355 2024-04-05 08:50:05.823609 prediction_market_agent_tooling-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 prediction_market_agent_tooling-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     7650 2024-04-05 15:25:06.768929 prediction_market_agent_tooling-0.9.3/LICENSE
+-rw-r--r--   0        0        0     2992 2024-04-05 15:25:06.768929 prediction_market_agent_tooling-0.9.3/README.md
+-rw-r--r--   0        0        0     9578 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/omen_dxdao.abi.json
+-rw-r--r--   0        0        0    11406 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/omen_fpmm.abi.json
+-rw-r--r--   0        0        0     9841 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json
+-rw-r--r--   0        0        0     4777 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json
+-rw-r--r--   0        0        0     7315 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/omen_kleros.abi.json
+-rw-r--r--   0        0        0     1775 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/omen_oracle.abi.json
+-rw-r--r--   0        0        0    15953 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/omen_realitio.abi.json
+-rw-r--r--   0        0        0     6055 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/wxdai.abi.json
+-rw-r--r--   0        0        0        0 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/benchmark/__init__.py
+-rw-r--r--   0        0        0     3737 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/benchmark/agents.py
+-rw-r--r--   0        0        0    21237 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/benchmark/benchmark.py
+-rw-r--r--   0        0        0     2748 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/benchmark/utils.py
+-rw-r--r--   0        0        0     2596 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/config.py
+-rw-r--r--   0        0        0     7771 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/deploy/agent.py
+-rw-r--r--   0        0        0      621 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/deploy/agent_example.py
+-rw-r--r--   0        0        0       82 2024-04-05 15:25:06.772929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/deploy/constants.py
+-rw-r--r--   0        0        0     3739 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/deploy/gcp/deploy.py
+-rw-r--r--   0        0        0     5255 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/deploy/gcp/utils.py
+-rw-r--r--   0        0        0     2526 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/gtypes.py
+-rw-r--r--   0        0        0     4488 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/agent_market.py
+-rw-r--r--   0        0        0     1026 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/categorize.py
+-rw-r--r--   0        0        0      763 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/data_models.py
+-rw-r--r--   0        0        0        0 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/manifold/__init__.py
+-rw-r--r--   0        0        0     6882 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/manifold/api.py
+-rw-r--r--   0        0        0     5357 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/manifold/data_models.py
+-rw-r--r--   0        0        0     3402 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/manifold/manifold.py
+-rw-r--r--   0        0        0      513 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/manifold/utils.py
+-rw-r--r--   0        0        0     1550 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/markets.py
+-rw-r--r--   0        0        0        0 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/omen/__init__.py
+-rw-r--r--   0        0        0    11454 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/omen/data_models.py
+-rw-r--r--   0        0        0    26859 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/omen/omen.py
+-rw-r--r--   0        0        0    19354 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/omen/omen_contracts.py
+-rw-r--r--   0        0        0     7403 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/omen/omen_replicate.py
+-rw-r--r--   0        0        0    11382 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/omen/omen_resolve_replicated.py
+-rw-r--r--   0        0        0    17077 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/omen/omen_subgraph_handler.py
+-rw-r--r--   0        0        0     4188 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/polymarket/api.py
+-rw-r--r--   0        0        0     4199 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/polymarket/data_models.py
+-rw-r--r--   0        0        0    10863 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/polymarket/data_models_web.py
+-rw-r--r--   0        0        0     2652 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/polymarket/polymarket.py
+-rw-r--r--   0        0        0     1960 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/polymarket/utils.py
+-rw-r--r--   0        0        0     2503 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/monitor/markets/manifold.py
+-rw-r--r--   0        0        0     2419 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/monitor/markets/omen.py
+-rw-r--r--   0        0        0     2413 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/monitor/markets/polymarket.py
+-rw-r--r--   0        0        0    11465 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/monitor/monitor.py
+-rw-r--r--   0        0        0     4045 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/monitor/monitor_app.py
+-rw-r--r--   0        0        0        0 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/py.typed
+-rw-r--r--   0        0        0      625 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/balances.py
+-rw-r--r--   0        0        0     3520 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py
+-rw-r--r--   0        0        0     4367 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py
+-rw-r--r--   0        0        0      422 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/betting_strategies/minimum_bet_to_win.py
+-rw-r--r--   0        0        0      429 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/betting_strategies/stretch_bet_between.py
+-rw-r--r--   0        0        0      499 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/cache.py
+-rw-r--r--   0        0        0     5879 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/contract.py
+-rw-r--r--   0        0        0      660 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/gnosis_rpc.py
+-rw-r--r--   0        0        0     1761 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/google.py
+-rw-r--r--   0        0        0     2037 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/hexbytes_custom.py
+-rw-r--r--   0        0        0     2613 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/is_predictable.py
+-rw-r--r--   0        0        0      733 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/parallelism.py
+-rw-r--r--   0        0        0      729 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/singleton.py
+-rw-r--r--   0        0        0     4674 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/utils.py
+-rw-r--r--   0        0        0     5314 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/web3_utils.py
+-rw-r--r--   0        0        0     1355 2024-04-05 15:25:06.776929 prediction_market_agent_tooling-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     4660 1970-01-01 00:00:00.000000 prediction_market_agent_tooling-0.9.3/PKG-INFO
```

### Comparing `prediction_market_agent_tooling-0.9.1/LICENSE` & `prediction_market_agent_tooling-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/README.md` & `prediction_market_agent_tooling-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_dxdao.abi.json` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/omen_dxdao.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_fpmm.abi.json` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/omen_fpmm.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/omen_fpmm_conditionaltokens.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/omen_fpmm_factory.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_kleros.abi.json` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/omen_kleros.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_oracle.abi.json` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/omen_oracle.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/omen_realitio.abi.json` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/omen_realitio.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/abis/wxdai.abi.json` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/abis/wxdai.abi.json`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/benchmark/agents.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/benchmark/agents.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/benchmark/benchmark.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/benchmark/utils.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/config.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/config.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/agent.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/deploy/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     AgentMarket,
     FilterBy,
     SortBy,
 )
 from prediction_market_agent_tooling.markets.data_models import BetAmount
 from prediction_market_agent_tooling.markets.markets import MarketType
 from prediction_market_agent_tooling.markets.omen.omen import (
-    redeem_positions_from_all_user_bets,
+    redeem_from_all_user_positions,
 )
 from prediction_market_agent_tooling.monitor.monitor_app import (
     MARKET_TYPE_TO_DEPLOYED_AGENT,
 )
 from prediction_market_agent_tooling.tools.utils import DatetimeWithTimezone, utcnow
 
 MAX_AVAILABLE_MARKETS = 20
@@ -178,17 +178,19 @@
         )
         return available_markets
 
     def before(self, market_type: MarketType) -> None:
         """
         Executes actions that occur before bets are placed.
         """
+        keys = APIKeys()
 
         if market_type == MarketType.OMEN:
-            redeem_positions_from_all_user_bets()
+            # Omen is specific, because the user (agent) needs to manually withdraw winnings from the market.
+            redeem_from_all_user_positions(keys.bet_from_private_key)
 
     def process_bets(self, market_type: MarketType, _place_bet: bool = True) -> None:
         """
         Processes bets placed by agents on a given market.
         """
         available_markets = self.get_markets(market_type)
         markets = self.pick_markets(available_markets)
```

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/agent_example.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/deploy/agent_example.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/gcp/deploy.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/deploy/gcp/deploy.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/deploy/gcp/utils.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/deploy/gcp/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/gtypes.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/gtypes.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/agent_market.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/agent_market.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/categorize.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/categorize.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/data_models.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/data_models.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/api.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/manifold/api.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/data_models.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/manifold/data_models.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/manifold.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/manifold/manifold.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/manifold/utils.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/manifold/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/markets.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/markets.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/data_models.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/omen/data_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,40 +82,52 @@
 class OmenUserPosition(BaseModel):
     id: HexBytes
     position: OmenPosition
     balance: Wei
     wrappedBalance: Wei
     totalBalance: Wei
 
+    @property
+    def redeemable(self) -> bool:
+        return self.totalBalance > 0
+
 
 class OmenMarket(BaseModel):
     """
     https://aiomen.eth.limo
     """
 
     BET_AMOUNT_CURRENCY: t.ClassVar[Currency] = Currency.xDai
 
     id: HexAddress
     title: str
     creator: HexAddress
     category: str
     collateralVolume: Wei
-    liquidityMeasure: Wei
+    # Note: there are two similar parameters relating to liquidity:
+    # liquidityParameter and liquidityMeasure. The former appears to match most
+    # closely with the liquidity returned when calling the contract directly
+    # (see OmenAgentMarket.get_liquidity). So we can use it e.g. for filtering
+    # markets, but until better understood, please call the contract directly.
+    liquidityParameter: Wei
     usdVolume: USD
     collateralToken: HexAddress
     outcomes: list[str]
     outcomeTokenAmounts: list[OmenOutcomeToken]
     outcomeTokenMarginalPrices: t.Optional[list[xDai]]
     fee: t.Optional[Wei]
     resolutionTimestamp: t.Optional[int] = None
     answerFinalizedTimestamp: t.Optional[int] = None
     currentAnswer: t.Optional[str] = None
     creationTimestamp: t.Optional[int] = None
     condition: Condition
     question: Question
+    openingTimestamp: t.Optional[
+        int
+    ] = None  # Don't be fooled - this is the time that the market closes for trading, and the market question is opened on reality.eth!
 
     @property
     def answer_index(self) -> t.Optional[int]:
         return int(self.currentAnswer, 16) if self.currentAnswer else None
 
     @property
     def has_valid_answer(self) -> bool:
```

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/omen/omen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import typing as t
-from collections import defaultdict
 from datetime import datetime
 from decimal import Decimal
 
 from loguru import logger
 from web3 import Web3
 from web3.constants import HASH_ZERO
 
 from prediction_market_agent_tooling.config import APIKeys
 from prediction_market_agent_tooling.gtypes import (
     ChecksumAddress,
     HexAddress,
+    HexBytes,
     HexStr,
     PrivateKey,
     Wei,
     wei_type,
     xDai,
     xdai_type,
 )
@@ -42,14 +42,15 @@
     OmenOracleContract,
     OmenRealitioContract,
 )
 from prediction_market_agent_tooling.markets.omen.omen_subgraph_handler import (
     OmenSubgraphHandler,
 )
 from prediction_market_agent_tooling.tools.balances import get_balances
+from prediction_market_agent_tooling.tools.utils import check_not_none
 from prediction_market_agent_tooling.tools.web3_utils import (
     add_fraction,
     private_key_to_public_key,
     remove_fraction,
     wei_to_xdai,
     xdai_to_wei,
 )
@@ -66,14 +67,15 @@
     currency: t.ClassVar[Currency] = Currency.xDai
     base_url: t.ClassVar[str] = OMEN_BASE_URL
     creator: HexAddress
 
     collateral_token_contract_address_checksummed: ChecksumAddress
     market_maker_contract_address_checksummed: ChecksumAddress
     condition: Condition
+    finalized_time: datetime | None
 
     INVALID_MARKET_ANSWER: HexStr = HexStr(
         "0xFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF"
     )
 
     def get_liquidity(self) -> Wei:
         return self.get_contract().totalSupply()
@@ -95,101 +97,113 @@
             amount=amount_xdai,
             from_private_key=keys.bet_from_private_key,
             market=self,
             binary_outcome=outcome,
             auto_deposit=omen_auto_deposit,
         )
 
-    def was_bet_outcome_correct(self, resolved_omen_bets: t.List[OmenBet]) -> bool:
+    def was_any_bet_outcome_correct(self, resolved_omen_bets: t.List[OmenBet]) -> bool:
         resolved_bets_for_market = [
             bet for bet in resolved_omen_bets if bet.fpmm.id == self.id
         ]
 
         # If there were no bets for this market, we conservatively say that
         # this method was called incorrectly, hence we raise an Error.
         if not resolved_bets_for_market:
             raise ValueError(f"No resolved bets provided for market {self.id}")
 
         # We iterate through bets since agent could have placed bets on multiple outcomes.
         # If one of the bets was correct, we return true since there is a redeemable amount to be retrieved.
         for bet in resolved_bets_for_market:
             # We only handle markets that are already finalized AND have a final answer
-            if (
-                bet.fpmm.question.answerFinalizedTimestamp is None
-                or bet.fpmm.question.currentAnswer is None
-            ):
+            if not bet.fpmm.is_resolved:
                 continue
 
             # Like Olas, we assert correctness by matching index OR invalid market answer
             if bet.outcomeIndex == int(
-                bet.fpmm.question.currentAnswer, 16
+                check_not_none(
+                    bet.fpmm.question.currentAnswer,
+                    "Shouldn't be None if the market is resolved",
+                ),
+                16,
             ) or bet.outcomeIndex == int(self.INVALID_MARKET_ANSWER, 16):
                 return True
 
         return False
 
-    def check_if_position_was_already_redeemed(self) -> bool:
+    def market_redeemable_by(self, user: ChecksumAddress) -> bool:
         """
-        Olas solves this problem (see https://github.com/valory-xyz/trader/blob/033ad88998fe0dc16457cd312b32f9e3b2d9a25f/packages/valory/skills/decision_maker_abci/behaviours/reedem.py#L487) by keeping state of the conditionIDs that were already claimed.
-        Since we currently use stateless functions to redeem positions, it's not possible to query state. Hence we proceed by not tracking the positions already redeemed.
-        Note that this has no major consequences from a gas perspective, it only incurs extra subgraph queries and RPC reads, no writes hence no gas costs.
+        Will return true if given user placed a bet on this market and that bet has a balance.
+        If the user never placed a bet on this market, this corretly return False.
         """
-        return False
-
-    def redeem_positions(self, bets_on_market: t.List[OmenBet]) -> None:
-        keys = APIKeys()
-
-        bet_was_correct = self.was_bet_outcome_correct(bets_on_market)
-        if not bet_was_correct:
-            logger.debug(f"Bet placed on market {self.id} was incorrect.")
-            return None
-
-        position_already_redeemed = self.check_if_position_was_already_redeemed()
-        if position_already_redeemed:
-            logger.debug(f"Position on market {self.id} was already redeemed.")
+        positions = OmenSubgraphHandler().get_positions(condition_id=self.condition.id)
+        user_positions = OmenSubgraphHandler().get_user_positions(
+            better_address=user,
+            position_id_in=[p.id for p in positions],
+            # After redeem, this will became zero.
+            total_balance_bigger_than=wei_type(0),
+        )
+        return len(user_positions) > 0
+
+    def redeem_positions(self, for_private_key: PrivateKey) -> None:
+        for_public_key = private_key_to_public_key(for_private_key)
+        market_is_redeemable = self.market_redeemable_by(user=for_public_key)
+        if not market_is_redeemable:
+            logger.debug(
+                f"Position on market {self.id} was already redeemed or no bets were placed at all by {for_public_key=}."
+            )
             return None
 
-        return omen_redeem_full_position_tx(
-            market=self, from_private_key=keys.bet_from_private_key
-        )
+        omen_redeem_full_position_tx(market=self, from_private_key=for_private_key)
 
     @staticmethod
     def from_data_model(model: OmenMarket) -> "OmenAgentMarket":
         return OmenAgentMarket(
             id=model.id,
             question=model.title,
             creator=model.creator,
             outcomes=model.outcomes,
             collateral_token_contract_address_checksummed=model.collateral_token_contract_address_checksummed,
             market_maker_contract_address_checksummed=model.market_maker_contract_address_checksummed,
             resolution=model.get_resolution_enum(),
             created_time=model.creation_datetime,
-            close_time=model.finalized_datetime,
+            finalized_time=model.finalized_datetime,
             p_yes=model.p_yes,
             condition=model.condition,
             url=model.url,
             volume=wei_to_xdai(model.collateralVolume),
+            close_time=datetime.fromtimestamp(model.openingTimestamp)
+            if model.openingTimestamp
+            else None,
         )
 
     @staticmethod
     def get_binary_markets(
         limit: int,
         sort_by: SortBy,
         filter_by: FilterBy = FilterBy.OPEN,
         created_after: t.Optional[datetime] = None,
         excluded_questions: set[str] | None = None,
     ) -> list[AgentMarket]:
+        if filter_by == FilterBy.OPEN:
+            # We assume here that we are only interested in markets that
+            # we can trade on, i.e. ones with non-zero liquidity.
+            liquidity_bigger_than = wei_type(0)
+        else:
+            liquidity_bigger_than = None
+
         return [
             OmenAgentMarket.from_data_model(m)
             for m in get_omen_binary_markets(
                 limit=limit,
                 sort_by=sort_by,
                 created_after=created_after,
                 filter_by=filter_by,
                 excluded_questions=excluded_questions,
+                liquidity_bigger_than=liquidity_bigger_than,
             )
         ]
 
     def get_contract(self) -> OmenFixedProductMarketMakerContract:
         return OmenFixedProductMarketMakerContract(
             address=self.market_maker_contract_address_checksummed
         )
@@ -215,14 +229,15 @@
     opened_before: t.Optional[datetime] = None,
     opened_after: t.Optional[datetime] = None,
     finalized_before: t.Optional[datetime] = None,
     finalized: bool | None = None,
     resolved: bool | None = None,
     creator: t.Optional[HexAddress] = None,
     liquidity_bigger_than: Wei | None = None,
+    condition_id_in: list[HexBytes] | None = None,
     excluded_questions: set[str] | None = None,
 ) -> list[OmenMarket]:
     subgraph_handler = OmenSubgraphHandler()
     return subgraph_handler.get_omen_binary_markets(
         limit=limit,
         sort_by=sort_by,
         created_after=created_after,
@@ -230,14 +245,15 @@
         opened_after=opened_after,
         finalized_before=finalized_before,
         finalized=finalized,
         resolved=resolved,
         filter_by=filter_by,
         creator=creator,
         liquidity_bigger_than=liquidity_bigger_than,
+        condition_id_in=condition_id_in,
         excluded_questions=excluded_questions,
     )
 
 
 def pick_binary_market(
     sort_by: SortBy = SortBy.CLOSING_SOONEST, filter_by: FilterBy = FilterBy.OPEN
 ) -> OmenMarket:
@@ -696,37 +712,7 @@
             web3=web3,
         )
         new_balances = get_balances(public_key)
 
         logger.info(
             f"Redeemed {new_balances.wxdai - original_balances.wxdai} wxDai from position {user_position.id=}."
         )
-
-
-def redeem_positions_from_all_user_bets() -> None:
-    """
-    Redeems positions from all resolved Omen markets where the user placed a bet.
-
-    Note: This function is very similar to `redeem_from_all_user_positions`, but it will redeem only positions obtained from bets, not from liquidity withdrawals.
-    """
-    keys = APIKeys()
-    omen_subgraph_handler = OmenSubgraphHandler()
-    resolved_omen_bets = omen_subgraph_handler.get_resolved_bets(
-        better_address=keys.bet_from_address,
-        start_time=datetime(2020, 1, 1),
-    )
-
-    bets_per_market_id: t.Dict[HexAddress, t.List[OmenBet]] = defaultdict(list)
-    market_id_to_market: t.Dict[HexAddress, OmenMarket] = {}
-
-    for bet in resolved_omen_bets:
-        bets_per_market_id[bet.fpmm.id].append(bet)
-        # We keep track of the unique markets
-        if bet.fpmm.id not in market_id_to_market:
-            market_id_to_market[bet.fpmm.id] = bet.fpmm
-
-    # We redeem positions for each unique resolved market where the
-    # agent has placed bets.
-    for market_id, omen_bets in bets_per_market_id.items():
-        market_data_model = market_id_to_market[market_id]
-        market = OmenAgentMarket.from_data_model(market_data_model)
-        market.redeem_positions(omen_bets)
```

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_contracts.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/omen/omen_contracts.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_replicate.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/omen/omen_replicate.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,18 +174,18 @@
             and not market.is_resolved
             and not (
                 market.p_yes > saturation_above_threshold
                 or market.p_no > saturation_above_threshold
             )
         ):
             logger.info(
-                f"[{idx+1}/{len(markets)}] Skipping unfunding of `{market.liquidityMeasure=} {market.question=}  {market.url=}`, because it's not saturated yet, `{market.p_yes=}`."
+                f"[{idx+1}/{len(markets)}] Skipping unfunding of `{market.liquidityParameter=} {market.question=}  {market.url=}`, because it's not saturated yet, `{market.p_yes=}`."
             )
             continue
         logger.info(
-            f"[{idx+1}/{len(markets)}] Unfunding market `{market.liquidityMeasure=} {market.question=} {market.url=}`."
+            f"[{idx+1}/{len(markets)}] Unfunding market `{market.liquidityParameter=} {market.question=} {market.url=}`."
         )
         omen_remove_fund_market_tx(
             market=OmenAgentMarket.from_data_model(market),
             shares=None,
             from_private_key=from_private_key,
         )
```

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_resolve_replicated.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/omen/omen_resolve_replicated.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/omen/omen_subgraph_handler.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/omen/omen_subgraph_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from prediction_market_agent_tooling.gtypes import HexAddress, HexBytes, Wei
 from prediction_market_agent_tooling.markets.agent_market import FilterBy, SortBy
 from prediction_market_agent_tooling.markets.omen.data_models import (
     OMEN_FALSE_OUTCOME,
     OMEN_TRUE_OUTCOME,
     OmenBet,
     OmenMarket,
+    OmenPosition,
     OmenUserPosition,
     RealityAnswer,
     RealityQuestion,
 )
 from prediction_market_agent_tooling.tools.singleton import SingletonMeta
 from prediction_market_agent_tooling.tools.utils import to_int_timestamp, utcnow
 from prediction_market_agent_tooling.tools.web3_utils import ZERO_BYTES
@@ -92,15 +93,15 @@
         # Since it's still not working, we hardcode the schema to be fetched below.
         return [
             markets_field.id,
             markets_field.title,
             markets_field.creator,
             markets_field.collateralVolume,
             markets_field.usdVolume,
-            markets_field.liquidityMeasure,
+            markets_field.liquidityParameter,
             markets_field.collateralToken,
             markets_field.outcomes,
             markets_field.outcomeTokenAmounts,
             markets_field.outcomeTokenMarginalPrices,
             markets_field.fee,
             markets_field.answerFinalizedTimestamp,
             markets_field.resolutionTimestamp,
@@ -148,15 +149,15 @@
         if created_after:
             where_stms["creationTimestamp_gt"] = to_int_timestamp(created_after)
 
         if opened_before:
             where_stms["openingTimestamp_lt"] = to_int_timestamp(opened_before)
 
         if liquidity_bigger_than is not None:
-            where_stms["liquidityMeasure_gt"] = liquidity_bigger_than
+            where_stms["liquidityParameter_gt"] = liquidity_bigger_than
 
         if condition_id_in is not None:
             where_stms["condition_"]["id_in"] = [x.hex() for x in condition_id_in]
 
         if filter_by == FilterBy.RESOLVED:
             finalized = True
             resolved = True
@@ -168,14 +169,15 @@
             pass
         else:
             raise ValueError(f"Unknown filter_by: {filter_by}")
 
         if resolved is not None:
             if resolved:
                 where_stms["resolutionTimestamp_not"] = None
+                where_stms["currentAnswer_not"] = self.INVALID_ANSWER
             else:
                 where_stms["resolutionTimestamp"] = None
 
         if finalized is not None:
             if finalized:
                 where_stms["answerFinalizedTimestamp_not"] = None
             else:
@@ -192,27 +194,35 @@
         excluded_question_titles = [""]
         if excluded_questions is not None:
             excluded_question_titles = [i for i in excluded_questions]
 
         where_stms["question_"]["title_not_in"] = excluded_question_titles
         return where_stms
 
-    def _build_sort_direction(self, sort_by: SortBy) -> str:
+    def _build_sort_params(self, sort_by: SortBy) -> tuple[str, FieldPath]:
         match sort_by:
             case SortBy.NEWEST:
                 sort_direction = "desc"
+                sort_by_field = (
+                    self.trades_subgraph.FixedProductMarketMaker.creationTimestamp
+                )
             case SortBy.CLOSING_SOONEST:
-                # `desc` feel unintuitive, but really if we use `asc`, we are getting markets closing in 2030, 2026, etc.
-                sort_direction = "desc"
+                sort_direction = "asc"
+                sort_by_field = (
+                    self.trades_subgraph.FixedProductMarketMaker.openingTimestamp
+                )
             case SortBy.NONE:
                 sort_direction = "desc"
+                sort_by_field = (
+                    self.trades_subgraph.FixedProductMarketMaker.creationTimestamp
+                )
             case _:
                 raise ValueError(f"Unknown sort_by: {sort_by}")
 
-        return sort_direction
+        return sort_direction, sort_by_field
 
     def get_omen_binary_markets(
         self,
         limit: t.Optional[int],
         sort_by: SortBy,
         filter_by: FilterBy,
         created_after: t.Optional[datetime] = None,
@@ -238,17 +248,18 @@
             finalized=finalized,
             resolved=resolved,
             condition_id_in=condition_id_in,
             excluded_questions=excluded_questions,
             liquidity_bigger_than=liquidity_bigger_than,
         )
 
-        sort_direction = self._build_sort_direction(sort_by)
+        sort_direction, sort_by_field = self._build_sort_params(sort_by)
+
         markets = self.trades_subgraph.Query.fixedProductMarketMakers(
-            orderBy=self.trades_subgraph.FixedProductMarketMaker.creationTimestamp,
+            orderBy=sort_by_field,
             orderDirection=sort_direction,
             first=(
                 limit if limit else sys.maxsize
             ),  # if not limit, we fetch all possible markets
             where=where_stms,
         )
 
@@ -285,38 +296,66 @@
                 # subgrounds might pack all items as a list, indexed by a key, or pack it as a dictionary (if one single element)
                 if isinstance(v, dict):
                     items.extend([v])
                 else:
                     items.extend(v)
         return items
 
-    def _get_fields_for_user_positions(self, positions: FieldPath) -> list[FieldPath]:
+    def _get_fields_for_user_positions(
+        self, user_positions: FieldPath
+    ) -> list[FieldPath]:
+        return [
+            user_positions.id,
+            user_positions.balance,
+            user_positions.wrappedBalance,
+            user_positions.totalBalance,
+        ] + self._get_fields_for_positions(user_positions.position)
+
+    def _get_fields_for_positions(self, positions: FieldPath) -> list[FieldPath]:
         return [
             positions.id,
-            positions.position.id,
-            positions.position.conditionIds,
-            positions.position.collateralTokenAddress,
-            positions.position.indexSets,
-            positions.balance,
-            positions.wrappedBalance,
-            positions.totalBalance,
+            positions.conditionIds,
+            positions.collateralTokenAddress,
+            positions.indexSets,
         ]
 
+    def get_positions(
+        self,
+        condition_id: HexBytes | None = None,
+    ) -> list[OmenPosition]:
+        where_stms: dict[str, t.Any] = {}
+
+        if condition_id is not None:
+            where_stms["conditionIds_contains"] = [condition_id.hex()]
+
+        positions = self.conditional_tokens_subgraph.Query.positions(
+            first=sys.maxsize, where=where_stms
+        )
+        fields = self._get_fields_for_positions(positions)
+        result = self.sg.query_json(fields)
+        items = self._parse_items_from_json(result)
+        return [OmenPosition.model_validate(i) for i in items]
+
     def get_user_positions(
         self,
         better_address: ChecksumAddress,
+        position_id_in: list[HexBytes] | None = None,
         total_balance_bigger_than: Wei | None = None,
     ) -> list[OmenUserPosition]:
         where_stms: dict[str, t.Any] = {
             "user": better_address.lower(),
+            "position_": {},
         }
 
         if total_balance_bigger_than is not None:
             where_stms["totalBalance_gt"] = total_balance_bigger_than
 
+        if position_id_in is not None:
+            where_stms["position_"]["positionId_in"] = [x.hex() for x in position_id_in]
+
         positions = self.conditional_tokens_subgraph.Query.userPositions(
             first=sys.maxsize, where=where_stms
         )
         fields = self._get_fields_for_user_positions(positions)
         result = self.sg.query_json(fields)
         items = self._parse_items_from_json(result)
         return [OmenUserPosition.model_validate(i) for i in items]
```

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/api.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/polymarket/api.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/data_models.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/polymarket/data_models.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/data_models_web.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/polymarket/data_models_web.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/polymarket.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/polymarket/polymarket.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/markets/polymarket/utils.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/markets/polymarket/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/markets/manifold.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/monitor/markets/manifold.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/markets/omen.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/monitor/markets/omen.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/markets/polymarket.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/monitor/markets/polymarket.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/monitor.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/monitor/monitor_app.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/monitor/monitor_app.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/balances.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/balances.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/betting_strategies/kelly_criterion.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/betting_strategies/market_moving.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/contract.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/contract.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/gnosis_rpc.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/gnosis_rpc.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/google.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/google.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/hexbytes_custom.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/hexbytes_custom.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/is_predictable.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/is_predictable.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/parallelism.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/parallelism.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/singleton.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/singleton.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/utils.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/prediction_market_agent_tooling/tools/web3_utils.py` & `prediction_market_agent_tooling-0.9.3/prediction_market_agent_tooling/tools/web3_utils.py`

 * *Files identical despite different names*

### Comparing `prediction_market_agent_tooling-0.9.1/pyproject.toml` & `prediction_market_agent_tooling-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prediction-market-agent-tooling"
-version = "0.9.1"
+version = "0.9.3"
 description = "Tools to benchmark, deploy and monitor prediction market agents."
 authors = ["Gnosis"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 buy_omen = "scripts.bet_omen:buy"
 sell_omen = "scripts.bet_omen:sell"
```

### Comparing `prediction_market_agent_tooling-0.9.1/PKG-INFO` & `prediction_market_agent_tooling-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prediction-market-agent-tooling
-Version: 0.9.1
+Version: 0.9.3
 Summary: Tools to benchmark, deploy and monitor prediction market agents.
 Author: Gnosis
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: google
```

