# Comparing `tmp/lightning-fabric-2.2.3.tar.gz` & `tmp/lightning-fabric-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-fabric-2.2.3.tar", last modified: Tue Apr 23 18:46:41 2024, max compression
+gzip compressed data, was "lightning-fabric-2.2.4.tar", last modified: Wed May  1 22:52:28 2024, max compression
```

## Comparing `lightning-fabric-2.2.3.tar` & `lightning-fabric-2.2.4.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.776931 lightning-fabric-2.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.756931 lightning-fabric-2.2.3/.actions/
--rw-r--r--   0 runner    (1001) docker     (127)    20994 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-04-23 18:46:41.776931 lightning-fabric-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.756931 lightning-fabric-2.2.3/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.756931 lightning-fabric-2.2.3/requirements/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/requirements/fabric/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/requirements/fabric/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/requirements/fabric/examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/requirements/fabric/strategies.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/requirements/fabric/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:46:41.776931 lightning-fabric-2.2.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     7935 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.760931 lightning-fabric-2.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.760931 lightning-fabric-2.2.3/src/lightning_fabric/
--rw-r--r--   0 runner    (1001) docker     (127)    31993 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/src/lightning_fabric/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13372 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/src/lightning_fabric/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/src/lightning_fabric/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/src/lightning_fabric/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/src/lightning_fabric/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.760931 lightning-fabric-2.2.3/src/lightning_fabric/_graveyard/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/_graveyard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/_graveyard/tpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.764931 lightning-fabric-2.2.3/src/lightning_fabric/accelerators/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/accelerators/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/accelerators/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/accelerators/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/accelerators/mps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/accelerators/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/accelerators/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    51173 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/fabric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.764931 lightning-fabric-2.2.3/src/lightning_fabric/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/loggers/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.764931 lightning-fabric-2.2.3/src/lightning_fabric/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.764931 lightning-fabric-2.2.3/src/lightning_fabric/plugins/collectives/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/collectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/collectives/collective.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/collectives/single_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/collectives/torch_collective.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.764931 lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/cluster_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/kubeflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/torchelastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.768931 lightning-fabric-2.2.3/src/lightning_fabric/plugins/io/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/io/checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/io/torch_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/io/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.768931 lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/amp.py
--rw-r--r--   0 runner    (1001) docker     (127)    21109 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/bitsandbytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/double.py
--rw-r--r--   0 runner    (1001) docker     (127)     7066 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/half.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/transformer_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/src/lightning_fabric/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.772931 lightning-fabric-2.2.3/src/lightning_fabric/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/dp.py
--rw-r--r--   0 runner    (1001) docker     (127)    44201 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.772931 lightning-fabric-2.2.3/src/lightning_fabric/strategies/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/launchers/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/launchers/subprocess_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/launchers/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/single_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/single_xla.py
--rw-r--r--   0 runner    (1001) docker     (127)    18446 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)    30495 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/strategies/xla_fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.776931 lightning-fabric-2.2.3/src/lightning_fabric/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/apply_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/consolidate_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/device_dtype_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/device_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/init.py
--rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/spike.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.776931 lightning-fabric-2.2.3/src/lightning_fabric/utilities/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/testing/_runif.py
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/throughput.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/src/lightning_fabric/version.info
--rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:41.760931 lightning-fabric-2.2.3/src/lightning_fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 18:46:41.000000 lightning-fabric-2.2.3/src/lightning_fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 18:46:20.000000 lightning-fabric-2.2.3/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.617006 lightning-fabric-2.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.597006 lightning-fabric-2.2.4/.actions/
+-rw-r--r--   0 runner    (1001) docker     (127)    20994 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-01 22:52:28.613006 lightning-fabric-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.593006 lightning-fabric-2.2.4/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.597006 lightning-fabric-2.2.4/requirements/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/requirements/fabric/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/requirements/fabric/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/requirements/fabric/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/requirements/fabric/strategies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/requirements/fabric/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 22:52:28.617006 lightning-fabric-2.2.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7935 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.597006 lightning-fabric-2.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.601006 lightning-fabric-2.2.4/src/lightning_fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)    31993 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/src/lightning_fabric/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13372 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/src/lightning_fabric/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/src/lightning_fabric/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/src/lightning_fabric/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/src/lightning_fabric/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.601006 lightning-fabric-2.2.4/src/lightning_fabric/_graveyard/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/_graveyard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/_graveyard/tpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.601006 lightning-fabric-2.2.4/src/lightning_fabric/accelerators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/accelerators/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/accelerators/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/accelerators/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/accelerators/mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/accelerators/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/accelerators/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51173 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/fabric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.605006 lightning-fabric-2.2.4/src/lightning_fabric/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/loggers/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.605006 lightning-fabric-2.2.4/src/lightning_fabric/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.605006 lightning-fabric-2.2.4/src/lightning_fabric/plugins/collectives/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/collectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/collectives/collective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/collectives/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/collectives/torch_collective.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.605006 lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/cluster_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/kubeflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/torchelastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.605006 lightning-fabric-2.2.4/src/lightning_fabric/plugins/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/io/checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/io/torch_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/io/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.609006 lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/amp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21109 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/bitsandbytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7066 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/half.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/transformer_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/src/lightning_fabric/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.609006 lightning-fabric-2.2.4/src/lightning_fabric/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/dp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44201 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.609006 lightning-fabric-2.2.4/src/lightning_fabric/strategies/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/launchers/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/launchers/subprocess_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/launchers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/single_xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18446 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30495 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/strategies/xla_fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.613006 lightning-fabric-2.2.4/src/lightning_fabric/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/apply_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/consolidate_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/device_dtype_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/device_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/spike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.613006 lightning-fabric-2.2.4/src/lightning_fabric/utilities/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/testing/_runif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/throughput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/src/lightning_fabric/version.info
+-rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:28.601006 lightning-fabric-2.2.4/src/lightning_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 22:52:28.000000 lightning-fabric-2.2.4/src/lightning_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 22:52:08.000000 lightning-fabric-2.2.4/src/version.info
```

### Comparing `lightning-fabric-2.2.3/.actions/assistant.py` & `lightning-fabric-2.2.4/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/LICENSE` & `lightning-fabric-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/PKG-INFO` & `lightning-fabric-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-fabric
-Version: 2.2.3
+Version: 2.2.4
 Summary: UNKNOWN
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
```

### Comparing `lightning-fabric-2.2.3/README.md` & `lightning-fabric-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/pyproject.toml` & `lightning-fabric-2.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/requirements/fabric/strategies.txt` & `lightning-fabric-2.2.4/requirements/fabric/strategies.txt`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/setup.py` & `lightning-fabric-2.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/CHANGELOG.md` & `lightning-fabric-2.2.4/src/lightning_fabric/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/README.md` & `lightning-fabric-2.2.4/src/lightning_fabric/README.md`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/__init__.py` & `lightning-fabric-2.2.4/src/lightning_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/__setup__.py` & `lightning-fabric-2.2.4/src/lightning_fabric/__setup__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/_graveyard/__init__.py` & `lightning-fabric-2.2.4/src/lightning_fabric/_graveyard/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/_graveyard/tpu.py` & `lightning-fabric-2.2.4/src/lightning_fabric/_graveyard/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/accelerators/__init__.py` & `lightning-fabric-2.2.4/src/lightning_fabric/accelerators/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/accelerators/accelerator.py` & `lightning-fabric-2.2.4/src/lightning_fabric/accelerators/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/accelerators/cpu.py` & `lightning-fabric-2.2.4/src/lightning_fabric/accelerators/cpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/accelerators/cuda.py` & `lightning-fabric-2.2.4/src/lightning_fabric/accelerators/cuda.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/accelerators/mps.py` & `lightning-fabric-2.2.4/src/lightning_fabric/accelerators/mps.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/accelerators/registry.py` & `lightning-fabric-2.2.4/src/lightning_fabric/accelerators/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/accelerators/xla.py` & `lightning-fabric-2.2.4/src/lightning_fabric/accelerators/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/cli.py` & `lightning-fabric-2.2.4/src/lightning_fabric/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/connector.py` & `lightning-fabric-2.2.4/src/lightning_fabric/connector.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/fabric.py` & `lightning-fabric-2.2.4/src/lightning_fabric/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/loggers/__init__.py` & `lightning-fabric-2.2.4/src/lightning_fabric/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/loggers/csv_logs.py` & `lightning-fabric-2.2.4/src/lightning_fabric/loggers/csv_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/loggers/logger.py` & `lightning-fabric-2.2.4/src/lightning_fabric/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/loggers/tensorboard.py` & `lightning-fabric-2.2.4/src/lightning_fabric/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/__init__.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/collectives/collective.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/collectives/collective.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/collectives/single_device.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/collectives/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/collectives/torch_collective.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/collectives/torch_collective.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/__init__.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/cluster_environment.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/cluster_environment.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/kubeflow.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/kubeflow.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/lightning.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/lightning.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/lsf.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/lsf.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/mpi.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/mpi.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/slurm.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/slurm.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/torchelastic.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/torchelastic.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/environments/xla.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/environments/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/io/__init__.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/io/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/io/checkpoint_io.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/io/checkpoint_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/io/torch_io.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/io/torch_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/io/xla.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/io/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/__init__.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/amp.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/amp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/bitsandbytes.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/bitsandbytes.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/deepspeed.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/double.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/double.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/fsdp.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/half.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/half.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/precision.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/transformer_engine.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/transformer_engine.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/utils.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/plugins/precision/xla.py` & `lightning-fabric-2.2.4/src/lightning_fabric/plugins/precision/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/__init__.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/ddp.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/ddp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/deepspeed.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/dp.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/dp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/fsdp.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/launchers/__init__.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/launchers/launcher.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/launchers/multiprocessing.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/launchers/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/launchers/subprocess_script.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/launchers/subprocess_script.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/launchers/xla.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/launchers/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/parallel.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/registry.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/single_device.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/single_xla.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/single_xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/strategy.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/xla.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/strategies/xla_fsdp.py` & `lightning-fabric-2.2.4/src/lightning_fabric/strategies/xla_fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/__init__.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/apply_func.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/apply_func.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/cloud_io.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/cloud_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/consolidate_checkpoint.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/consolidate_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/data.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/data.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/device_dtype_mixin.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/device_dtype_mixin.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/device_parser.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/device_parser.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/distributed.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/enums.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/exceptions.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/imports.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/init.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/init.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/load.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/load.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/logger.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/optimizer.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/optimizer.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/rank_zero.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/rank_zero.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/registry.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/seed.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/seed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/spike.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/spike.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/testing/_runif.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/testing/_runif.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/throughput.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/throughput.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/types.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/utilities/warnings.py` & `lightning-fabric-2.2.4/src/lightning_fabric/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric/wrappers.py` & `lightning-fabric-2.2.4/src/lightning_fabric/wrappers.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric.egg-info/PKG-INFO` & `lightning-fabric-2.2.4/src/lightning_fabric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-fabric
-Version: 2.2.3
+Version: 2.2.4
 Summary: UNKNOWN
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
```

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric.egg-info/SOURCES.txt` & `lightning-fabric-2.2.4/src/lightning_fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.2.3/src/lightning_fabric.egg-info/requires.txt` & `lightning-fabric-2.2.4/src/lightning_fabric.egg-info/requires.txt`

 * *Files identical despite different names*

