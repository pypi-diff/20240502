# Comparing `tmp/frequenz-sdk-1.0.0rc6.tar.gz` & `tmp/frequenz-sdk-1.0.0rc6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-sdk-1.0.0rc6.tar", last modified: Fri Apr 12 14:04:26 2024, max compression
+gzip compressed data, was "frequenz-sdk-1.0.0rc6.post1.tar", last modified: Thu May  2 11:27:48 2024, max compression
```

## Comparing `frequenz-sdk-1.0.0rc6.tar` & `frequenz-sdk-1.0.0rc6.post1.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.515937 frequenz-sdk-1.0.0rc6/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-12 14:04:26.515937 frequenz-sdk-1.0.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.495938 frequenz-sdk-1.0.0rc6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/examples/battery_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:04:26.515937 frequenz-sdk-1.0.0rc6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.495938 frequenz-sdk-1.0.0rc6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.491938 frequenz-sdk-1.0.0rc6/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.495938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.495938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_singleton_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.495938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/
--rw-r--r--   0 runner    (1001) docker     (127)    23225 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_background_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_channel_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_config_managing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.499938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/_component_metric_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17214 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.499938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_matryoshka.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_power_managing_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_sorted_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_resampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_run_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.499938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.499938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_battery_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_component_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.499938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19277 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_ev_charger_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.499938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_pv_inverter_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_pv_inverter_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_pv_inverter_manager/_pv_inverter_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_pool_status_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.499938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18069 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_battery_status_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_blocking_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_component_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_ev_charger_status_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8031 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_pv_inverter_status_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.503938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29217 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/_battery_distribution_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/power_distributing.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.503938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/config/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.503938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24626 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/_data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/_power_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    36983 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/component_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.503938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_base_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_grid_frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_moving_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    38921 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_quantities.py
--rw-r--r--   0 runner    (1001) docker     (127)    30181 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_resampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.503938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_ringbuffer/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_ringbuffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24318 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_voltage_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.507938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18069 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_battery_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_battery_pool_reference_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    21524 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_result_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.507938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9565 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool_reference_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_result_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_system_bounds_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.507938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    40624 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_engine_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.507938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_battery_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_chp_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_consumer_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_current_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_formula_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_current_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_3_phase_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_producer_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_pv_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_resampled_formula_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.511937 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/logical_meter/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/logical_meter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.511937 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/_pv_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/_pv_pool_reference_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/_result_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/_system_bounds_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.511937 frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-12 14:04:26.000000 frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-12 14:04:26.000000 frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:04:26.000000 frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-12 14:04:26.000000 frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 14:04:26.000000 frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.260773 frequenz-sdk-1.0.0rc6.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-02 11:27:48.260773 frequenz-sdk-1.0.0rc6.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.236773 frequenz-sdk-1.0.0rc6.post1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/examples/battery_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 11:27:48.260773 frequenz-sdk-1.0.0rc6.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.236773 frequenz-sdk-1.0.0rc6.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.232773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.236773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.236773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/_internal/_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/_internal/_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/_internal/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/_internal/_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/_internal/_singleton_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.240773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/
+-rw-r--r--   0 runner    (1001) docker     (127)    23225 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_background_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_channel_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_config_managing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.240773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_data_sourcing/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_data_sourcing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_data_sourcing/_component_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18369 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.240773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_power_managing/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_power_managing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_power_managing/_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_power_managing/_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_power_managing/_matryoshka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_power_managing/_power_managing_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_power_managing/_sorted_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_run_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.240773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.240773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_battery_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_component_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.240773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19277 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_ev_charger_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.244773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_pv_inverter_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_pv_inverter_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_pv_inverter_manager/_pv_inverter_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_pool_status_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.244773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_status/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18069 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_status/_battery_status_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_status/_blocking_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_status/_component_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_status/_ev_charger_status_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8032 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_status/_pv_inverter_status_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.244773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29217 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/_battery_distribution_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/power_distributing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.244773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/config/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.244773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/microgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24626 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/microgrid/_data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/microgrid/_power_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36983 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/microgrid/component_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/microgrid/connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.248773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_base_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_grid_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_moving_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38921 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30181 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_resampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.248773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_ringbuffer/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_ringbuffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24318 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_voltage_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.248773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18069 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/_battery_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/_battery_pool_reference_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21524 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/_result_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.248773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/ev_charger_pool/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/ev_charger_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9565 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool_reference_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/ev_charger_pool/_result_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/ev_charger_pool/_system_bounds_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.252773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40624 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_engine_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.252773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_battery_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_chp_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_consumer_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_current_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_formula_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_current_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_3_phase_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_producer_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_pv_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_resampled_formula_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.252773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/logical_meter/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/logical_meter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.252773 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/pv_pool/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/pv_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/pv_pool/_pv_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/pv_pool/_pv_pool_reference_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/pv_pool/_result_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-02 11:27:35.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/pv_pool/_system_bounds_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:48.252773 frequenz-sdk-1.0.0rc6.post1/src/frequenz_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-02 11:27:48.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-02 11:27:48.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 11:27:48.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-02 11:27:48.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 11:27:48.000000 frequenz-sdk-1.0.0rc6.post1/src/frequenz_sdk.egg-info/top_level.txt
```

### Comparing `frequenz-sdk-1.0.0rc6/LICENSE` & `frequenz-sdk-1.0.0rc6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/PKG-INFO` & `frequenz-sdk-1.0.0rc6.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-sdk
-Version: 1.0.0rc6
+Version: 1.0.0rc6.post1
 Summary: A development kit to interact with the Frequenz development platform
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-sdk-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-sdk-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-sdk-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-sdk-python
@@ -37,50 +37,50 @@
 Provides-Extra: dev-flake8
 Requires-Dist: flake8==7.0.0; extra == "dev-flake8"
 Requires-Dist: flake8-docstrings==1.7.0; extra == "dev-flake8"
 Requires-Dist: flake8-pyproject==1.2.3; extra == "dev-flake8"
 Requires-Dist: pydoclint==0.4.1; extra == "dev-flake8"
 Requires-Dist: pydocstyle==6.3.0; extra == "dev-flake8"
 Provides-Extra: dev-examples
-Requires-Dist: polars==0.20.18; extra == "dev-examples"
+Requires-Dist: polars==0.20.23; extra == "dev-examples"
 Provides-Extra: dev-formatting
-Requires-Dist: black==24.3.0; extra == "dev-formatting"
+Requires-Dist: black==24.4.2; extra == "dev-formatting"
 Requires-Dist: isort==5.13.2; extra == "dev-formatting"
 Provides-Extra: dev-mkdocs
-Requires-Dist: black==24.3.0; extra == "dev-mkdocs"
+Requires-Dist: black==24.4.2; extra == "dev-mkdocs"
 Requires-Dist: Markdown==3.6; extra == "dev-mkdocs"
-Requires-Dist: mike==2.0.0; extra == "dev-mkdocs"
+Requires-Dist: mike==2.1.0; extra == "dev-mkdocs"
 Requires-Dist: mkdocs-gen-files==0.5.0; extra == "dev-mkdocs"
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == "dev-mkdocs"
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == "dev-mkdocs"
-Requires-Dist: mkdocs-material==9.5.16; extra == "dev-mkdocs"
-Requires-Dist: mkdocstrings[python]==0.24.1; extra == "dev-mkdocs"
-Requires-Dist: frequenz-repo-config[lib]==0.9.1; extra == "dev-mkdocs"
+Requires-Dist: mkdocs-material==9.5.20; extra == "dev-mkdocs"
+Requires-Dist: mkdocstrings[python]==0.25.0; extra == "dev-mkdocs"
+Requires-Dist: frequenz-repo-config[lib]==0.9.2; extra == "dev-mkdocs"
 Provides-Extra: dev-mypy
-Requires-Dist: mypy==1.9.0; extra == "dev-mypy"
+Requires-Dist: mypy==1.10.0; extra == "dev-mypy"
 Requires-Dist: grpc-stubs==1.24.12; extra == "dev-mypy"
 Requires-Dist: types-Markdown==3.6.0.20240316; extra == "dev-mypy"
 Requires-Dist: types-protobuf==4.24.0.20240129; extra == "dev-mypy"
-Requires-Dist: types-setuptools==69.2.0.20240317; extra == "dev-mypy"
+Requires-Dist: types-setuptools==69.5.0.20240423; extra == "dev-mypy"
 Requires-Dist: frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]; extra == "dev-mypy"
 Provides-Extra: dev-noxfile
-Requires-Dist: nox==2023.4.22; extra == "dev-noxfile"
-Requires-Dist: frequenz-repo-config[lib]==0.9.1; extra == "dev-noxfile"
+Requires-Dist: nox==2024.4.15; extra == "dev-noxfile"
+Requires-Dist: frequenz-repo-config[lib]==0.9.2; extra == "dev-noxfile"
 Provides-Extra: dev-pylint
 Requires-Dist: pylint==3.1.0; extra == "dev-pylint"
 Requires-Dist: frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]; extra == "dev-pylint"
 Provides-Extra: dev-pytest
-Requires-Dist: pytest==8.1.1; extra == "dev-pytest"
-Requires-Dist: frequenz-repo-config[extra-lint-examples]==0.9.1; extra == "dev-pytest"
+Requires-Dist: pytest==8.2.0; extra == "dev-pytest"
+Requires-Dist: frequenz-repo-config[extra-lint-examples]==0.9.2; extra == "dev-pytest"
 Requires-Dist: pytest-mock==3.14.0; extra == "dev-pytest"
 Requires-Dist: pytest-asyncio==0.23.6; extra == "dev-pytest"
 Requires-Dist: time-machine==2.12.0; extra == "dev-pytest"
 Requires-Dist: async-solipsism==0.6; extra == "dev-pytest"
 Requires-Dist: frequenz-sdk[dev-examples]; extra == "dev-pytest"
-Requires-Dist: hypothesis==6.100.0; extra == "dev-pytest"
+Requires-Dist: hypothesis==6.100.2; extra == "dev-pytest"
 Provides-Extra: dev
 Requires-Dist: frequenz-sdk[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]; extra == "dev"
 
 # Frequenz Python SDK
 
 [![Build Status](https://github.com/frequenz-floss/frequenz-sdk-python/actions/workflows/ci.yaml/badge.svg)](https://github.com/frequenz-floss/frequenz-sdk-python/actions/workflows/ci.yaml)
 [![PyPI Package](https://img.shields.io/pypi/v/frequenz-sdk)](https://pypi.org/project/frequenz-sdk/)
```

### Comparing `frequenz-sdk-1.0.0rc6/README.md` & `frequenz-sdk-1.0.0rc6.post1/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/examples/battery_pool.py` & `frequenz-sdk-1.0.0rc6.post1/examples/battery_pool.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/pyproject.toml` & `frequenz-sdk-1.0.0rc6.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 [build-system]
 requires = [
   "setuptools == 69.0.3",
   "setuptools_scm[toml] == 8.0.4",
-  "frequenz-repo-config[lib] == 0.9.1",
+  "frequenz-repo-config[lib] == 0.9.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-sdk"
 description = "A development kit to interact with the Frequenz development platform"
 readme = "README.md"
@@ -54,52 +54,52 @@
 dev-flake8 = [
   "flake8 == 7.0.0",
   "flake8-docstrings == 1.7.0",
   "flake8-pyproject == 1.2.3",  # For reading the flake8 config from pyproject.toml
   "pydoclint == 0.4.1",
   "pydocstyle == 6.3.0",
 ]
-dev-examples = ["polars == 0.20.18"]
-dev-formatting = ["black == 24.3.0", "isort == 5.13.2"]
+dev-examples = ["polars == 0.20.23"]
+dev-formatting = ["black == 24.4.2", "isort == 5.13.2"]
 dev-mkdocs = [
-  "black == 24.3.0",
+  "black == 24.4.2",
   "Markdown==3.6",
-  "mike == 2.0.0",
+  "mike == 2.1.0",
   "mkdocs-gen-files == 0.5.0",
   "mkdocs-literate-nav == 0.6.1",
   "mkdocs-macros-plugin == 1.0.5",
-  "mkdocs-material == 9.5.16",
-  "mkdocstrings[python] == 0.24.1",
-  "frequenz-repo-config[lib] == 0.9.1",
+  "mkdocs-material == 9.5.20",
+  "mkdocstrings[python] == 0.25.0",
+  "frequenz-repo-config[lib] == 0.9.2",
 ]
 dev-mypy = [
-  "mypy == 1.9.0",
+  "mypy == 1.10.0",
   "grpc-stubs == 1.24.12",               # This dependency introduces breaking changes in patch releases
   "types-Markdown == 3.6.0.20240316",
   "types-protobuf == 4.24.0.20240129",
-  "types-setuptools == 69.2.0.20240317",
+  "types-setuptools == 69.5.0.20240423",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
-dev-noxfile = ["nox == 2023.4.22", "frequenz-repo-config[lib] == 0.9.1"]
+dev-noxfile = ["nox == 2024.4.15", "frequenz-repo-config[lib] == 0.9.2"]
 dev-pylint = [
   "pylint == 3.1.0",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 dev-pytest = [
-  "pytest == 8.1.1",
-  "frequenz-repo-config[extra-lint-examples] == 0.9.1",
+  "pytest == 8.2.0",
+  "frequenz-repo-config[extra-lint-examples] == 0.9.2",
   "pytest-mock == 3.14.0",
   "pytest-asyncio == 0.23.6",
   "time-machine == 2.12.0",
   "async-solipsism == 0.6",
   # For checking docstring code examples
   "frequenz-sdk[dev-examples]",
-  "hypothesis == 6.100.0",
+  "hypothesis == 6.100.2",
 ]
 dev = [
   "frequenz-sdk[dev-mkdocs,dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
 
 [project.urls]
 Documentation = "https://frequenz-floss.github.io/frequenz-sdk-python/"
```

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_asyncio.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/_internal/_asyncio.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_channels.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/_internal/_channels.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_constants.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/_internal/_constants.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_math.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/_internal/_math.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_singleton_meta.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/_internal/_singleton_meta.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/__init__.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_actor.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_actor.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_background_service.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_background_service.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_channel_registry.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_channel_registry.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_config_managing.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_config_managing.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/_component_metric_request.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_data_sourcing/_component_metric_request.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,24 @@
     ComponentMetricId.CURRENT_PHASE_1: lambda msg: msg.current_per_phase[0],
     ComponentMetricId.CURRENT_PHASE_2: lambda msg: msg.current_per_phase[1],
     ComponentMetricId.CURRENT_PHASE_3: lambda msg: msg.current_per_phase[2],
     ComponentMetricId.VOLTAGE_PHASE_1: lambda msg: msg.voltage_per_phase[0],
     ComponentMetricId.VOLTAGE_PHASE_2: lambda msg: msg.voltage_per_phase[1],
     ComponentMetricId.VOLTAGE_PHASE_3: lambda msg: msg.voltage_per_phase[2],
     ComponentMetricId.FREQUENCY: lambda msg: msg.frequency,
+    ComponentMetricId.REACTIVE_POWER: lambda msg: msg.reactive_power,
+    ComponentMetricId.REACTIVE_POWER_PHASE_1: lambda msg: msg.reactive_power_per_phase[
+        0
+    ],
+    ComponentMetricId.REACTIVE_POWER_PHASE_2: lambda msg: msg.reactive_power_per_phase[
+        1
+    ],
+    ComponentMetricId.REACTIVE_POWER_PHASE_3: lambda msg: msg.reactive_power_per_phase[
+        2
+    ],
 }
 
 _BatteryDataMethods: dict[ComponentMetricId, Callable[[BatteryData], float]] = {
     ComponentMetricId.SOC: lambda msg: msg.soc,
     ComponentMetricId.SOC_LOWER_BOUND: lambda msg: msg.soc_lower_bound,
     ComponentMetricId.SOC_UPPER_BOUND: lambda msg: msg.soc_upper_bound,
     ComponentMetricId.CAPACITY: lambda msg: msg.capacity,
@@ -80,28 +90,48 @@
     ComponentMetricId.CURRENT_PHASE_1: lambda msg: msg.current_per_phase[0],
     ComponentMetricId.CURRENT_PHASE_2: lambda msg: msg.current_per_phase[1],
     ComponentMetricId.CURRENT_PHASE_3: lambda msg: msg.current_per_phase[2],
     ComponentMetricId.VOLTAGE_PHASE_1: lambda msg: msg.voltage_per_phase[0],
     ComponentMetricId.VOLTAGE_PHASE_2: lambda msg: msg.voltage_per_phase[1],
     ComponentMetricId.VOLTAGE_PHASE_3: lambda msg: msg.voltage_per_phase[2],
     ComponentMetricId.FREQUENCY: lambda msg: msg.frequency,
+    ComponentMetricId.REACTIVE_POWER: lambda msg: msg.reactive_power,
+    ComponentMetricId.REACTIVE_POWER_PHASE_1: lambda msg: msg.reactive_power_per_phase[
+        0
+    ],
+    ComponentMetricId.REACTIVE_POWER_PHASE_2: lambda msg: msg.reactive_power_per_phase[
+        1
+    ],
+    ComponentMetricId.REACTIVE_POWER_PHASE_3: lambda msg: msg.reactive_power_per_phase[
+        2
+    ],
 }
 
 _EVChargerDataMethods: dict[ComponentMetricId, Callable[[EVChargerData], float]] = {
     ComponentMetricId.ACTIVE_POWER: lambda msg: msg.active_power,
     ComponentMetricId.ACTIVE_POWER_PHASE_1: lambda msg: msg.active_power_per_phase[0],
     ComponentMetricId.ACTIVE_POWER_PHASE_2: lambda msg: msg.active_power_per_phase[1],
     ComponentMetricId.ACTIVE_POWER_PHASE_3: lambda msg: msg.active_power_per_phase[2],
     ComponentMetricId.CURRENT_PHASE_1: lambda msg: msg.current_per_phase[0],
     ComponentMetricId.CURRENT_PHASE_2: lambda msg: msg.current_per_phase[1],
     ComponentMetricId.CURRENT_PHASE_3: lambda msg: msg.current_per_phase[2],
     ComponentMetricId.VOLTAGE_PHASE_1: lambda msg: msg.voltage_per_phase[0],
     ComponentMetricId.VOLTAGE_PHASE_2: lambda msg: msg.voltage_per_phase[1],
     ComponentMetricId.VOLTAGE_PHASE_3: lambda msg: msg.voltage_per_phase[2],
     ComponentMetricId.FREQUENCY: lambda msg: msg.frequency,
+    ComponentMetricId.REACTIVE_POWER: lambda msg: msg.reactive_power,
+    ComponentMetricId.REACTIVE_POWER_PHASE_1: lambda msg: msg.reactive_power_per_phase[
+        0
+    ],
+    ComponentMetricId.REACTIVE_POWER_PHASE_2: lambda msg: msg.reactive_power_per_phase[
+        1
+    ],
+    ComponentMetricId.REACTIVE_POWER_PHASE_3: lambda msg: msg.reactive_power_per_phase[
+        2
+    ],
 }
 
 
 class MicrogridApiSource:
     """Fetches requested metrics from the Microgrid API.
 
     Used by the DataSourcingActor.
```

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_base_classes.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_power_managing/_base_classes.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_bounds.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_power_managing/_bounds.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_matryoshka.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_power_managing/_matryoshka.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_power_managing_actor.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_power_managing/_power_managing_actor.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_sorted_set.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_power_managing/_sorted_set.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_resampling.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_resampling.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_run_utils.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/_run_utils.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/__init__.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_battery_manager.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_battery_manager.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_component_manager.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_component_manager.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_config.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_config.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_ev_charger_manager.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_ev_charger_manager.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_states.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_states.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_pv_inverter_manager/_pv_inverter_manager.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_managers/_pv_inverter_manager/_pv_inverter_manager.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_pool_status_tracker.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_pool_status_tracker.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/__init__.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_status/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_battery_status_tracker.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_status/_battery_status_tracker.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_blocking_status.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_status/_blocking_status.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_component_status.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_status/_component_status.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_ev_charger_status_tracker.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_status/_ev_charger_status_tracker.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_pv_inverter_status_tracker.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_component_status/_pv_inverter_status_tracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
                 self._blocking_status.is_blocked()
                 and new_status != ComponentStatusEnum.NOT_WORKING
             ):
                 new_status = ComponentStatusEnum.UNCERTAIN
 
             if new_status != self._last_status:
                 _logger.info(
-                    "EV charger %s status changed from %s to %s",
+                    "PV inverter %s status changed from %s to %s",
                     self._component_id,
                     self._last_status,
                     new_status,
                 )
                 self._last_status = new_status
                 await self._status_sender.send(
                     ComponentStatus(self._component_id, new_status)
```

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/_battery_distribution_algorithm.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/_battery_distribution_algorithm.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/power_distributing.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/power_distributing.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/request.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/request.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/result.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/actor/power_distributing/result.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/config/_config.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/config/_config.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/__init__.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/microgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/_data_pipeline.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/microgrid/_data_pipeline.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/_power_wrapper.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/microgrid/_power_wrapper.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/component_graph.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/microgrid/component_graph.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/connection_manager.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/microgrid/connection_manager.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/__init__.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_base_types.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_base_types.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_grid_frequency.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_grid_frequency.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_moving_window.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_moving_window.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_quantities.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_quantities.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_resampling.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_resampling.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_voltage_streamer.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/_voltage_streamer.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_battery_pool.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/_battery_pool.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_battery_pool_reference_store.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/_battery_pool_reference_store.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_methods.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/_methods.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_result_types.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/battery_pool/_result_types.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/consumer.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/consumer.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool_reference_store.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool_reference_store.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_result_types.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/ev_charger_pool/_result_types.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_system_bounds_tracker.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/ev_charger_pool/_system_bounds_tracker.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_engine.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_engine.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_engine_pool.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_engine_pool.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_evaluator.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_evaluator.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_formatter.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_formatter.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/__init__.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_battery_power_formula.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_battery_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_chp_power_formula.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_chp_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_consumer_power_formula.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_consumer_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_current_formula.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_current_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_power_formula.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_formula_generator.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_formula_generator.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_current_formula.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_current_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_3_phase_formula.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_3_phase_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_formula.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_producer_power_formula.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_producer_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_pv_power_formula.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_pv_power_formula.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_steps.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_formula_steps.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_resampled_formula_builder.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_resampled_formula_builder.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_tokenizer.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/formula_engine/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/grid.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/grid.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/producer.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/producer.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/_pv_pool.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/pv_pool/_pv_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,27 +126,27 @@
         Returns:
             Set of managed component IDs.
         """
         return self._pv_pool_ref.component_ids
 
     @property
     def power(self) -> FormulaEngine[Power]:
-        """Fetch the total power for the EV Chargers in the pool.
+        """Fetch the total power for the PV Inverters in the pool.
 
         This formula produces values that are in the Passive Sign Convention (PSC).
 
-        If a formula engine to calculate EV Charger power is not already running, it
+        If a formula engine to calculate PV Inverter power is not already running, it
         will be started.
 
         A receiver from the formula engine can be created using the `new_receiver`
         method.
 
         Returns:
-            A FormulaEngine that will calculate and stream the total power of all EV
-                Chargers.
+            A FormulaEngine that will calculate and stream the total power of all PV
+                Inverters.
         """
         engine = self._pv_pool_ref.formula_pool.from_power_formula_generator(
             "pv_power",
             PVPowerFormula,
             FormulaGeneratorConfig(
                 component_ids=self._pv_pool_ref.component_ids,
             ),
```

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/_pv_pool_reference_store.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/pv_pool/_pv_pool_reference_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,10 +94,10 @@
             self.component_ids,
             self.status_receiver,
             self.bounds_channel.new_sender(),
         )
         self.bounds_tracker.start()
 
     async def stop(self) -> None:
-        """Stop all tasks and channels owned by the EVChargerPool."""
+        """Stop all tasks and channels owned by the PVInverterPool."""
         await self.formula_pool.stop()
         await self.bounds_tracker.stop()
```

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/_result_types.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/pv_pool/_result_types.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/_system_bounds_tracker.py` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz/sdk/timeseries/pv_pool/_system_bounds_tracker.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/PKG-INFO` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-sdk
-Version: 1.0.0rc6
+Version: 1.0.0rc6.post1
 Summary: A development kit to interact with the Frequenz development platform
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-sdk-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-sdk-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-sdk-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-sdk-python
@@ -37,50 +37,50 @@
 Provides-Extra: dev-flake8
 Requires-Dist: flake8==7.0.0; extra == "dev-flake8"
 Requires-Dist: flake8-docstrings==1.7.0; extra == "dev-flake8"
 Requires-Dist: flake8-pyproject==1.2.3; extra == "dev-flake8"
 Requires-Dist: pydoclint==0.4.1; extra == "dev-flake8"
 Requires-Dist: pydocstyle==6.3.0; extra == "dev-flake8"
 Provides-Extra: dev-examples
-Requires-Dist: polars==0.20.18; extra == "dev-examples"
+Requires-Dist: polars==0.20.23; extra == "dev-examples"
 Provides-Extra: dev-formatting
-Requires-Dist: black==24.3.0; extra == "dev-formatting"
+Requires-Dist: black==24.4.2; extra == "dev-formatting"
 Requires-Dist: isort==5.13.2; extra == "dev-formatting"
 Provides-Extra: dev-mkdocs
-Requires-Dist: black==24.3.0; extra == "dev-mkdocs"
+Requires-Dist: black==24.4.2; extra == "dev-mkdocs"
 Requires-Dist: Markdown==3.6; extra == "dev-mkdocs"
-Requires-Dist: mike==2.0.0; extra == "dev-mkdocs"
+Requires-Dist: mike==2.1.0; extra == "dev-mkdocs"
 Requires-Dist: mkdocs-gen-files==0.5.0; extra == "dev-mkdocs"
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == "dev-mkdocs"
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == "dev-mkdocs"
-Requires-Dist: mkdocs-material==9.5.16; extra == "dev-mkdocs"
-Requires-Dist: mkdocstrings[python]==0.24.1; extra == "dev-mkdocs"
-Requires-Dist: frequenz-repo-config[lib]==0.9.1; extra == "dev-mkdocs"
+Requires-Dist: mkdocs-material==9.5.20; extra == "dev-mkdocs"
+Requires-Dist: mkdocstrings[python]==0.25.0; extra == "dev-mkdocs"
+Requires-Dist: frequenz-repo-config[lib]==0.9.2; extra == "dev-mkdocs"
 Provides-Extra: dev-mypy
-Requires-Dist: mypy==1.9.0; extra == "dev-mypy"
+Requires-Dist: mypy==1.10.0; extra == "dev-mypy"
 Requires-Dist: grpc-stubs==1.24.12; extra == "dev-mypy"
 Requires-Dist: types-Markdown==3.6.0.20240316; extra == "dev-mypy"
 Requires-Dist: types-protobuf==4.24.0.20240129; extra == "dev-mypy"
-Requires-Dist: types-setuptools==69.2.0.20240317; extra == "dev-mypy"
+Requires-Dist: types-setuptools==69.5.0.20240423; extra == "dev-mypy"
 Requires-Dist: frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]; extra == "dev-mypy"
 Provides-Extra: dev-noxfile
-Requires-Dist: nox==2023.4.22; extra == "dev-noxfile"
-Requires-Dist: frequenz-repo-config[lib]==0.9.1; extra == "dev-noxfile"
+Requires-Dist: nox==2024.4.15; extra == "dev-noxfile"
+Requires-Dist: frequenz-repo-config[lib]==0.9.2; extra == "dev-noxfile"
 Provides-Extra: dev-pylint
 Requires-Dist: pylint==3.1.0; extra == "dev-pylint"
 Requires-Dist: frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]; extra == "dev-pylint"
 Provides-Extra: dev-pytest
-Requires-Dist: pytest==8.1.1; extra == "dev-pytest"
-Requires-Dist: frequenz-repo-config[extra-lint-examples]==0.9.1; extra == "dev-pytest"
+Requires-Dist: pytest==8.2.0; extra == "dev-pytest"
+Requires-Dist: frequenz-repo-config[extra-lint-examples]==0.9.2; extra == "dev-pytest"
 Requires-Dist: pytest-mock==3.14.0; extra == "dev-pytest"
 Requires-Dist: pytest-asyncio==0.23.6; extra == "dev-pytest"
 Requires-Dist: time-machine==2.12.0; extra == "dev-pytest"
 Requires-Dist: async-solipsism==0.6; extra == "dev-pytest"
 Requires-Dist: frequenz-sdk[dev-examples]; extra == "dev-pytest"
-Requires-Dist: hypothesis==6.100.0; extra == "dev-pytest"
+Requires-Dist: hypothesis==6.100.2; extra == "dev-pytest"
 Provides-Extra: dev
 Requires-Dist: frequenz-sdk[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]; extra == "dev"
 
 # Frequenz Python SDK
 
 [![Build Status](https://github.com/frequenz-floss/frequenz-sdk-python/actions/workflows/ci.yaml/badge.svg)](https://github.com/frequenz-floss/frequenz-sdk-python/actions/workflows/ci.yaml)
 [![PyPI Package](https://img.shields.io/pypi/v/frequenz-sdk)](https://pypi.org/project/frequenz-sdk/)
```

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/SOURCES.txt` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/requires.txt` & `frequenz-sdk-1.0.0rc6.post1/src/frequenz_sdk.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,56 +13,56 @@
 typing_extensions<5,>=4.6.1
 watchfiles>=0.15.0
 
 [dev]
 frequenz-sdk[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
 
 [dev-examples]
-polars==0.20.18
+polars==0.20.23
 
 [dev-flake8]
 flake8==7.0.0
 flake8-docstrings==1.7.0
 flake8-pyproject==1.2.3
 pydoclint==0.4.1
 pydocstyle==6.3.0
 
 [dev-formatting]
-black==24.3.0
+black==24.4.2
 isort==5.13.2
 
 [dev-mkdocs]
-black==24.3.0
+black==24.4.2
 Markdown==3.6
-mike==2.0.0
+mike==2.1.0
 mkdocs-gen-files==0.5.0
 mkdocs-literate-nav==0.6.1
 mkdocs-macros-plugin==1.0.5
-mkdocs-material==9.5.16
-mkdocstrings[python]==0.24.1
-frequenz-repo-config[lib]==0.9.1
+mkdocs-material==9.5.20
+mkdocstrings[python]==0.25.0
+frequenz-repo-config[lib]==0.9.2
 
 [dev-mypy]
-mypy==1.9.0
+mypy==1.10.0
 grpc-stubs==1.24.12
 types-Markdown==3.6.0.20240316
 types-protobuf==4.24.0.20240129
-types-setuptools==69.2.0.20240317
+types-setuptools==69.5.0.20240423
 frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]
 
 [dev-noxfile]
-nox==2023.4.22
-frequenz-repo-config[lib]==0.9.1
+nox==2024.4.15
+frequenz-repo-config[lib]==0.9.2
 
 [dev-pylint]
 pylint==3.1.0
 frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]
 
 [dev-pytest]
-pytest==8.1.1
-frequenz-repo-config[extra-lint-examples]==0.9.1
+pytest==8.2.0
+frequenz-repo-config[extra-lint-examples]==0.9.2
 pytest-mock==3.14.0
 pytest-asyncio==0.23.6
 time-machine==2.12.0
 async-solipsism==0.6
 frequenz-sdk[dev-examples]
-hypothesis==6.100.0
+hypothesis==6.100.2
```

