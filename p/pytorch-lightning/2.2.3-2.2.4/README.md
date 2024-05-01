# Comparing `tmp/pytorch-lightning-2.2.3.tar.gz` & `tmp/pytorch-lightning-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-lightning-2.2.3.tar", last modified: Tue Apr 23 18:47:23 2024, max compression
+gzip compressed data, was "pytorch-lightning-2.2.4.tar", last modified: Wed May  1 22:53:03 2024, max compression
```

## Comparing `pytorch-lightning-2.2.3.tar` & `pytorch-lightning-2.2.4.tar`

### file list

```diff
@@ -1,343 +1,343 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.697496 pytorch-lightning-2.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.653496 pytorch-lightning-2.2.3/.actions/
--rw-r--r--   0 runner    (1001) docker     (127)    20994 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-04-23 18:47:23.697496 pytorch-lightning-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.649496 pytorch-lightning-2.2.3/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.657496 pytorch-lightning-2.2.3/requirements/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/requirements/fabric/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/requirements/fabric/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/requirements/fabric/examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/requirements/fabric/strategies.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/requirements/fabric/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.657496 pytorch-lightning-2.2.3/requirements/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/requirements/pytorch/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/requirements/pytorch/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/requirements/pytorch/examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/requirements/pytorch/extra.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/requirements/pytorch/strategies.txt
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/requirements/pytorch/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:47:23.697496 pytorch-lightning-2.2.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     7935 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.657496 pytorch-lightning-2.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.657496 pytorch-lightning-2.2.3/src/lightning_fabric/
--rw-r--r--   0 runner    (1001) docker     (127)    31993 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/src/lightning_fabric/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/src/lightning_fabric/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/src/lightning_fabric/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.657496 pytorch-lightning-2.2.3/src/lightning_fabric/_graveyard/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/_graveyard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/_graveyard/tpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.657496 pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/mps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    51173 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/fabric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.661496 pytorch-lightning-2.2.3/src/lightning_fabric/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/loggers/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.661496 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.661496 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/collectives/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/collectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/collectives/collective.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/collectives/single_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/collectives/torch_collective.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.661496 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/cluster_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/kubeflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/torchelastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.661496 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/io/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/io/checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/io/torch_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/io/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.665496 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/amp.py
--rw-r--r--   0 runner    (1001) docker     (127)    21109 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/bitsandbytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/double.py
--rw-r--r--   0 runner    (1001) docker     (127)     7066 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/half.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/transformer_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.665496 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/dp.py
--rw-r--r--   0 runner    (1001) docker     (127)    44201 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.665496 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/launchers/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/launchers/subprocess_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/launchers/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/single_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/single_xla.py
--rw-r--r--   0 runner    (1001) docker     (127)    18446 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)    30495 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/strategies/xla_fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.669496 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/apply_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/consolidate_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/device_dtype_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/device_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/init.py
--rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/spike.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.669496 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/testing/_runif.py
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/throughput.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/src/lightning_fabric/version.info
--rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/lightning_fabric/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.669496 pytorch-lightning-2.2.3/src/pytorch_lightning/
--rw-r--r--   0 runner    (1001) docker     (127)   455300 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16138 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.673496 pytorch-lightning-2.2.3/src/pytorch_lightning/_graveyard/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/_graveyard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/_graveyard/_torchmetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/_graveyard/hpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/_graveyard/ipu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/_graveyard/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/_graveyard/tpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.673496 pytorch-lightning-2.2.3/src/pytorch_lightning/accelerators/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/accelerators/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/accelerators/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/accelerators/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/accelerators/mps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/accelerators/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.677496 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/batch_size_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11022 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/device_stats_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)    19095 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/finetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/gradient_accumulation_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/lambda_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/lr_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    38519 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/model_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/on_exception_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/prediction_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.677496 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/progress/
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/progress/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (127)    25511 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/progress/rich_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/progress/tqdm_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/pruning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/rich_model_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/spike.py
--rw-r--r--   0 runner    (1001) docker     (127)    17922 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/stochastic_weight_avg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/throughput_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    36431 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.677496 pytorch-lightning-2.2.3/src/pytorch_lightning/core/
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/core/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)    27024 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/core/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.677496 pytorch-lightning-2.2.3/src/pytorch_lightning/core/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/core/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/core/mixins/hparams_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    71246 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/core/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    18344 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/core/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/core/saving.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.677496 pytorch-lightning-2.2.3/src/pytorch_lightning/demos/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/demos/boring_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/demos/mnist_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/demos/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.681496 pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15769 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/comet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    14391 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    23695 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/neptune.py
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    24970 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.681496 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25464 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/evaluation_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/fetchers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19179 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/fit_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.681496 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/optimization/automatic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/optimization/closure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/optimization/manual.py
--rw-r--r--   0 runner    (1001) docker     (127)    18682 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/prediction_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    23209 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/training_epoch_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/loops/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.681496 pytorch-lightning-2.2.3/src/pytorch_lightning/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/overrides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/overrides/distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.681496 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.681496 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/environments/
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/environments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.685496 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/io/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/io/async_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/io/checkpoint_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/io/torch_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/io/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/io/xla_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/layer_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.685496 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/amp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/bitsandbytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/double.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/half.py
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/transformer_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.685496 pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    23778 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.685496 pytorch-lightning-2.2.3/src/pytorch_lightning/serve/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/serve/servable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/serve/servable_module_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.689496 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19061 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)    40964 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)    31015 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.689496 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/launchers/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/launchers/subprocess_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/launchers/xla.py
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/single_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/single_xla.py
--rw-r--r--   0 runner    (1001) docker     (127)    25739 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.689496 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/configuration_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.689496 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34278 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/accelerator_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10663 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/callback_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    24486 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/checkpoint_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    23249 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/data_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.693496 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/logger_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/logger_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/logger_connector/fx_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/logger_connector/logger_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    20934 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/logger_connector/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/signal_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/states.py
--rw-r--r--   0 runner    (1001) docker     (127)    73384 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.693496 pytorch-lightning-2.2.3/src/pytorch_lightning/tuner/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/tuner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12868 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/tuner/batch_size_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/tuner/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/tuner/tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.697496 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/_pytree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/combined_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/consolidate_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/grads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.697496 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/migration/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/migration/migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/migration/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/model_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.697496 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/model_summary/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/model_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/model_summary/model_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/model_summary/model_summary_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/parameter_tying.py
--rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/signature_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.697496 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/testing/_runif.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/upgrade_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-23 18:47:22.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/src/pytorch_lightning/version.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:47:23.673496 pytorch-lightning-2.2.3/src/pytorch_lightning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/pytorch_lightning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/pytorch_lightning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/pytorch_lightning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/pytorch_lightning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/pytorch_lightning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-23 18:47:23.000000 pytorch-lightning-2.2.3/src/pytorch_lightning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 18:46:57.000000 pytorch-lightning-2.2.3/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.114273 pytorch-lightning-2.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.066273 pytorch-lightning-2.2.4/.actions/
+-rw-r--r--   0 runner    (1001) docker     (127)    20994 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-05-01 22:53:03.114273 pytorch-lightning-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.062273 pytorch-lightning-2.2.4/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.070273 pytorch-lightning-2.2.4/requirements/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/requirements/fabric/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/requirements/fabric/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/requirements/fabric/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/requirements/fabric/strategies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/requirements/fabric/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.070273 pytorch-lightning-2.2.4/requirements/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/requirements/pytorch/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/requirements/pytorch/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/requirements/pytorch/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/requirements/pytorch/extra.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/requirements/pytorch/strategies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/requirements/pytorch/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 22:53:03.114273 pytorch-lightning-2.2.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7935 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.070273 pytorch-lightning-2.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.070273 pytorch-lightning-2.2.4/src/lightning_fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)    31993 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/src/lightning_fabric/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/src/lightning_fabric/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/src/lightning_fabric/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.070273 pytorch-lightning-2.2.4/src/lightning_fabric/_graveyard/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/_graveyard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/_graveyard/tpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.074273 pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27849 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51173 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/fabric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.074273 pytorch-lightning-2.2.4/src/lightning_fabric/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/loggers/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.074273 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.074273 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/collectives/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/collectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/collectives/collective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/collectives/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/collectives/torch_collective.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.074273 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/cluster_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/kubeflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/torchelastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.078273 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/io/checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/io/torch_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/io/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.078273 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/amp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21109 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/bitsandbytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7066 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/half.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/transformer_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.078273 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9838 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/dp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44201 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.082273 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/launchers/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/launchers/subprocess_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/launchers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/single_xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18446 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30495 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/strategies/xla_fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.086273 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/apply_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/consolidate_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23129 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/device_dtype_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/device_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11766 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/spike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.086273 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/testing/_runif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/throughput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/src/lightning_fabric/version.info
+-rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/lightning_fabric/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.086273 pytorch-lightning-2.2.4/src/pytorch_lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)   455300 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16138 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.090273 pytorch-lightning-2.2.4/src/pytorch_lightning/_graveyard/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/_graveyard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/_graveyard/_torchmetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/_graveyard/hpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/_graveyard/ipu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/_graveyard/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/_graveyard/tpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.090273 pytorch-lightning-2.2.4/src/pytorch_lightning/accelerators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/accelerators/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/accelerators/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/accelerators/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/accelerators/mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/accelerators/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.094273 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/batch_size_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11022 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/device_stats_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19095 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/finetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/gradient_accumulation_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/lr_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38519 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/model_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/on_exception_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/prediction_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.094273 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/progress/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/progress/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25511 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/progress/rich_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/progress/tqdm_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/pruning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/rich_model_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/spike.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17922 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/stochastic_weight_avg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/throughput_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36431 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.094273 pytorch-lightning-2.2.4/src/pytorch_lightning/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/core/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27024 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/core/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.094273 pytorch-lightning-2.2.4/src/pytorch_lightning/core/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/core/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/core/mixins/hparams_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71246 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18344 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/core/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/core/saving.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.094273 pytorch-lightning-2.2.4/src/pytorch_lightning/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7818 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/demos/boring_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9243 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/demos/mnist_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/demos/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.098273 pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15769 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/comet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14391 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23695 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24970 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.098273 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25464 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/evaluation_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/fetchers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19179 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/fit_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.098273 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/optimization/automatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/optimization/closure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/optimization/manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18682 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/prediction_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23209 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/training_epoch_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/loops/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.098273 pytorch-lightning-2.2.4/src/pytorch_lightning/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/overrides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11202 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/overrides/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.098273 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.098273 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/environments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.102273 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/io/async_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/io/checkpoint_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/io/torch_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/io/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/io/xla_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/layer_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.102273 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/amp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/bitsandbytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/half.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/transformer_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.102273 pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23778 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.102273 pytorch-lightning-2.2.4/src/pytorch_lightning/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/serve/servable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/serve/servable_module_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.106273 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19061 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40964 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31015 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.106273 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14256 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/launchers/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7009 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/launchers/subprocess_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7502 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/launchers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/single_xla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25739 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.106273 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/configuration_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.110273 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34278 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/accelerator_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10663 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/callback_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24486 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/checkpoint_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23249 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/data_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.110273 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/logger_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/logger_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/logger_connector/fx_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/logger_connector/logger_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20934 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/logger_connector/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/signal_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73384 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.110273 pytorch-lightning-2.2.4/src/pytorch_lightning/tuner/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/tuner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12868 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/tuner/batch_size_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19672 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/tuner/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11471 2024-05-01 22:53:01.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/tuner/tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.114273 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/_pytree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/combined_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/consolidate_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/grads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.114273 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/migration/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/migration/migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/migration/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/model_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.114273 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/model_summary/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/model_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/model_summary/model_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/model_summary/model_summary_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/parameter_tying.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11822 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/signature_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.114273 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/testing/_runif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/upgrade_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/src/pytorch_lightning/version.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:53:03.086273 pytorch-lightning-2.2.4/src/pytorch_lightning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-05-01 22:53:03.000000 pytorch-lightning-2.2.4/src/pytorch_lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-01 22:53:02.000000 pytorch-lightning-2.2.4/src/pytorch_lightning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 22:52:43.000000 pytorch-lightning-2.2.4/src/version.info
```

### Comparing `pytorch-lightning-2.2.3/.actions/assistant.py` & `pytorch-lightning-2.2.4/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/CITATION.cff` & `pytorch-lightning-2.2.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/LICENSE` & `pytorch-lightning-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/PKG-INFO` & `pytorch-lightning-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-lightning
-Version: 2.2.3
+Version: 2.2.4
 Summary: PyTorch Lightning is the lightweight PyTorch wrapper for ML researchers. Scale your models. Write less boilerplate.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -62,15 +62,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytorch-lightning)](https://pypi.org/project/pytorch-lightning/)
 [![PyPI Status](https://badge.fury.io/py/pytorch-lightning.svg)](https://badge.fury.io/py/pytorch-lightning)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pytorch-lightning)](https://pepy.tech/project/pytorch-lightning)
 [![Conda](https://img.shields.io/conda/v/conda-forge/pytorch-lightning?label=conda&color=success)](https://anaconda.org/conda-forge/pytorch-lightning)
 [![DockerHub](https://img.shields.io/docker/pulls/pytorchlightning/pytorch_lightning.svg)](https://hub.docker.com/r/pytorchlightning/pytorch_lightning)
 [![codecov](https://codecov.io/gh/Lightning-AI/pytorch-lightning/graph/badge.svg?token=SmzX8mnKlA)](https://codecov.io/gh/Lightning-AI/pytorch-lightning)
 
-[![ReadTheDocs](https://readthedocs.org/projects/pytorch-lightning/badge/?version=2.2.3)](https://lightning.ai/docs/pytorch/stable/)[![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
+[![ReadTheDocs](https://readthedocs.org/projects/pytorch-lightning/badge/?version=2.2.4)](https://lightning.ai/docs/pytorch/stable/)[![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/lightning/blob/master/LICENSE)
 
 <!--
 [![CodeFactor](https://www.codefactor.io/repository/github/Lightning-AI/lightning/badge)](https://www.codefactor.io/repository/github/Lightning-AI/lightning)
 -->
 
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytorch-lightning Version: 2.2.3 Summary: PyTorch
+Metadata-Version: 2.1 Name: pytorch-lightning Version: 2.2.4 Summary: PyTorch
 Lightning is the lightweight PyTorch wrapper for ML researchers. Scale your
 models. Write less boilerplate. Home-page: https://github.com/Lightning-AI/
 lightning Author: Lightning AI et al. Author-email: pytorch@lightning.ai
 License: Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
 Project-URL: Documentation, https://pytorch-lightning.rtfd.io/en/latest/
 Project-URL: Source Code, https://github.com/Lightning-AI/lightning Keywords:
@@ -34,15 +34,15 @@
                   img.shields.io/conda/v/conda-forge/pytorch-
 lightning?label=conda&color=success)](https://anaconda.org/conda-forge/pytorch-
 lightning) [![DockerHub](https://img.shields.io/docker/pulls/pytorchlightning/
       pytorch_lightning.svg)](https://hub.docker.com/r/pytorchlightning/
   pytorch_lightning) [![codecov](https://codecov.io/gh/Lightning-AI/pytorch-
  lightning/graph/badge.svg?token=SmzX8mnKlA)](https://codecov.io/gh/Lightning-
 AI/pytorch-lightning) [![ReadTheDocs](https://readthedocs.org/projects/pytorch-
- lightning/badge/?version=2.2.3)](https://lightning.ai/docs/pytorch/stable/)[!
+ lightning/badge/?version=2.2.4)](https://lightning.ai/docs/pytorch/stable/)[!
  [Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)]
    (https://discord.gg/VptPCZkGNa) [![license](https://img.shields.io/badge/
 License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/lightning/blob/
                                 master/LICENSE)
 ###### \*Codecov is > 90%+ but build delays may show less
 ______________________________________________________________________ ##
 PyTorch Lightning is just organized PyTorch Lightning disentangles PyTorch code
```

### Comparing `pytorch-lightning-2.2.3/README.md` & `pytorch-lightning-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/pyproject.toml` & `pytorch-lightning-2.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/requirements/fabric/strategies.txt` & `pytorch-lightning-2.2.4/requirements/fabric/strategies.txt`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/requirements/pytorch/base.txt` & `pytorch-lightning-2.2.4/requirements/pytorch/base.txt`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/requirements/pytorch/extra.txt` & `pytorch-lightning-2.2.4/requirements/pytorch/extra.txt`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/requirements/pytorch/test.txt` & `pytorch-lightning-2.2.4/requirements/pytorch/test.txt`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/setup.py` & `pytorch-lightning-2.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/CHANGELOG.md` & `pytorch-lightning-2.2.4/src/lightning_fabric/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/__init__.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/__setup__.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/__setup__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/_graveyard/__init__.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/_graveyard/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/_graveyard/tpu.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/_graveyard/tpu.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/__init__.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/accelerator.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/accelerator.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/cpu.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/cpu.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/cuda.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/cuda.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/mps.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/mps.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/registry.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/registry.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/accelerators/xla.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/accelerators/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/cli.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/cli.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/connector.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/connector.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/fabric.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/fabric.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/loggers/__init__.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/loggers/csv_logs.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/loggers/csv_logs.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/loggers/logger.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/loggers/tensorboard.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/__init__.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/collectives/collective.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/collectives/collective.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/collectives/single_device.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/collectives/single_device.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/collectives/torch_collective.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/collectives/torch_collective.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/__init__.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/cluster_environment.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/cluster_environment.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/kubeflow.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/kubeflow.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/lightning.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/lightning.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/lsf.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/lsf.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/mpi.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/mpi.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/slurm.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/slurm.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/torchelastic.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/torchelastic.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/environments/xla.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/environments/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/io/__init__.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/io/checkpoint_io.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/io/checkpoint_io.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/io/torch_io.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/io/torch_io.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/io/xla.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/io/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/__init__.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/amp.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/amp.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/bitsandbytes.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/bitsandbytes.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/deepspeed.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/deepspeed.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/double.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/double.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/fsdp.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/fsdp.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/half.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/half.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/precision.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/transformer_engine.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/transformer_engine.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/utils.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/plugins/precision/xla.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/plugins/precision/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/__init__.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/ddp.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/ddp.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/deepspeed.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/deepspeed.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/dp.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/dp.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/fsdp.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/fsdp.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/launchers/__init__.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/launchers/launcher.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/launchers/multiprocessing.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/launchers/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/launchers/subprocess_script.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/launchers/subprocess_script.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/launchers/xla.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/launchers/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/parallel.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/registry.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/registry.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/single_device.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/single_device.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/single_xla.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/single_xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/strategy.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/xla.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/strategies/xla_fsdp.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/strategies/xla_fsdp.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/__init__.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/apply_func.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/apply_func.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/cloud_io.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/cloud_io.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/consolidate_checkpoint.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/consolidate_checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/data.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/data.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/device_dtype_mixin.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/device_dtype_mixin.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/device_parser.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/device_parser.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/distributed.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/enums.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/exceptions.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/imports.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/init.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/init.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/load.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/load.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/logger.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/optimizer.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/optimizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/rank_zero.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/rank_zero.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/registry.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/registry.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/seed.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/seed.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/spike.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/spike.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/testing/_runif.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/testing/_runif.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/throughput.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/throughput.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/types.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/types.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/utilities/warnings.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/lightning_fabric/wrappers.py` & `pytorch-lightning-2.2.4/src/lightning_fabric/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/CHANGELOG.md` & `pytorch-lightning-2.2.4/src/pytorch_lightning/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/README.md` & `pytorch-lightning-2.2.4/src/pytorch_lightning/README.md`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/__about__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/__about__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/__setup__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/__setup__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/_graveyard/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/_graveyard/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/_graveyard/_torchmetrics.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/_graveyard/_torchmetrics.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/_graveyard/hpu.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/_graveyard/hpu.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/_graveyard/ipu.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/_graveyard/ipu.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/_graveyard/precision.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/_graveyard/precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/_graveyard/tpu.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/_graveyard/tpu.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/accelerators/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/accelerators/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/accelerators/accelerator.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/accelerators/accelerator.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/accelerators/cpu.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/accelerators/cpu.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/accelerators/cuda.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/accelerators/cuda.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/accelerators/mps.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/accelerators/mps.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/accelerators/xla.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/accelerators/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/batch_size_finder.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/batch_size_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/callback.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/device_stats_monitor.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/device_stats_monitor.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/early_stopping.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/finetuning.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/finetuning.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/gradient_accumulation_scheduler.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/gradient_accumulation_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/lambda_function.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/lr_finder.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/lr_monitor.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/lr_monitor.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/model_checkpoint.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/model_summary.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/model_summary.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/on_exception_checkpoint.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/on_exception_checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/prediction_writer.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/prediction_writer.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/progress/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/progress/progress_bar.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/progress/progress_bar.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/progress/rich_progress.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/progress/rich_progress.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/progress/tqdm_progress.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/progress/tqdm_progress.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/pruning.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/pruning.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/rich_model_summary.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/rich_model_summary.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/spike.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/spike.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/stochastic_weight_avg.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/stochastic_weight_avg.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/throughput_monitor.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/throughput_monitor.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/callbacks/timer.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/callbacks/timer.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/cli.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/cli.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/core/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/core/datamodule.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/core/datamodule.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/core/hooks.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/core/hooks.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/core/mixins/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/core/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/core/mixins/hparams_mixin.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/core/mixins/hparams_mixin.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/core/module.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/core/module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/core/optimizer.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/core/optimizer.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/core/saving.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/core/saving.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/demos/boring_classes.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/demos/boring_classes.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/demos/mnist_datamodule.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/demos/mnist_datamodule.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/demos/transformer.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/demos/transformer.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/comet.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/comet.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/csv_logs.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/csv_logs.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/logger.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/mlflow.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/mlflow.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/neptune.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/neptune.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/tensorboard.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/utilities.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/utilities.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loggers/wandb.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loggers/wandb.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loops/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loops/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loops/evaluation_loop.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loops/evaluation_loop.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loops/fetchers.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loops/fetchers.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loops/fit_loop.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loops/fit_loop.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loops/loop.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loops/loop.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loops/optimization/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loops/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loops/optimization/automatic.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loops/optimization/automatic.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loops/optimization/closure.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loops/optimization/closure.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loops/optimization/manual.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loops/optimization/manual.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loops/prediction_loop.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loops/prediction_loop.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loops/progress.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loops/progress.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loops/training_epoch_loop.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loops/training_epoch_loop.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/loops/utilities.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/loops/utilities.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/overrides/distributed.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/overrides/distributed.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/environments/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/io/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/io/async_plugin.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/io/async_plugin.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/io/checkpoint_plugin.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/io/checkpoint_plugin.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/io/torch_plugin.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/io/torch_plugin.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/io/wrapper.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/io/wrapper.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/io/xla_plugin.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/io/xla_plugin.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/layer_sync.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/layer_sync.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/amp.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/amp.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/bitsandbytes.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/bitsandbytes.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/deepspeed.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/deepspeed.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/double.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/double.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/fsdp.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/fsdp.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/half.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/half.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/precision.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/transformer_engine.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/transformer_engine.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/plugins/precision/xla.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/plugins/precision/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/advanced.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/advanced.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/base.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/base.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/profiler.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/profiler.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/pytorch.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/pytorch.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/simple.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/simple.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/profilers/xla.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/profilers/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/serve/servable_module.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/serve/servable_module.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/serve/servable_module_validator.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/serve/servable_module_validator.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/ddp.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/ddp.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/deepspeed.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/deepspeed.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/fsdp.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/fsdp.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/launchers/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/launchers/launcher.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/launchers/multiprocessing.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/launchers/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/launchers/subprocess_script.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/launchers/subprocess_script.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/launchers/xla.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/launchers/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/parallel.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/single_device.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/single_device.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/single_xla.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/single_xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/strategy.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/strategies/xla.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/strategies/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/call.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/call.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/configuration_validator.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/configuration_validator.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/accelerator_connector.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/accelerator_connector.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/callback_connector.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/callback_connector.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/checkpoint_connector.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/checkpoint_connector.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/data_connector.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/data_connector.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/logger_connector/fx_validator.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/logger_connector/fx_validator.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/logger_connector/logger_connector.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/logger_connector/logger_connector.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/logger_connector/result.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/logger_connector/result.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/connectors/signal_connector.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/connectors/signal_connector.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/setup.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/setup.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/states.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/states.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/trainer/trainer.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/tuner/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/tuner/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/tuner/batch_size_scaling.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/tuner/batch_size_scaling.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/tuner/lr_finder.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/tuner/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/tuner/tuning.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/tuner/tuning.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/_pytree.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/_pytree.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/argparse.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/argparse.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/combined_loader.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/combined_loader.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/compile.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/compile.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/consolidate_checkpoint.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/consolidate_checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/data.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/data.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/deepspeed.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/deepspeed.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/enums.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/exceptions.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/grads.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/grads.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/imports.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/memory.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/memory.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/migration/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/migration/migration.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/migration/migration.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/migration/utils.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/migration/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/model_helpers.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/model_helpers.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/model_summary/__init__.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/model_summary/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/model_summary/model_summary.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/model_summary/model_summary.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/model_summary/model_summary_deepspeed.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/model_summary/model_summary_deepspeed.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/parameter_tying.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/parameter_tying.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/parsing.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/parsing.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/rank_zero.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/rank_zero.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/seed.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/seed.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/signature_utils.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/signature_utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/testing/_runif.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/testing/_runif.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/types.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/types.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/upgrade_checkpoint.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/upgrade_checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning/utilities/warnings.py` & `pytorch-lightning-2.2.4/src/pytorch_lightning/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning.egg-info/PKG-INFO` & `pytorch-lightning-2.2.4/src/pytorch_lightning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-lightning
-Version: 2.2.3
+Version: 2.2.4
 Summary: PyTorch Lightning is the lightweight PyTorch wrapper for ML researchers. Scale your models. Write less boilerplate.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -62,15 +62,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytorch-lightning)](https://pypi.org/project/pytorch-lightning/)
 [![PyPI Status](https://badge.fury.io/py/pytorch-lightning.svg)](https://badge.fury.io/py/pytorch-lightning)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pytorch-lightning)](https://pepy.tech/project/pytorch-lightning)
 [![Conda](https://img.shields.io/conda/v/conda-forge/pytorch-lightning?label=conda&color=success)](https://anaconda.org/conda-forge/pytorch-lightning)
 [![DockerHub](https://img.shields.io/docker/pulls/pytorchlightning/pytorch_lightning.svg)](https://hub.docker.com/r/pytorchlightning/pytorch_lightning)
 [![codecov](https://codecov.io/gh/Lightning-AI/pytorch-lightning/graph/badge.svg?token=SmzX8mnKlA)](https://codecov.io/gh/Lightning-AI/pytorch-lightning)
 
-[![ReadTheDocs](https://readthedocs.org/projects/pytorch-lightning/badge/?version=2.2.3)](https://lightning.ai/docs/pytorch/stable/)[![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
+[![ReadTheDocs](https://readthedocs.org/projects/pytorch-lightning/badge/?version=2.2.4)](https://lightning.ai/docs/pytorch/stable/)[![Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)](https://discord.gg/VptPCZkGNa)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/lightning/blob/master/LICENSE)
 
 <!--
 [![CodeFactor](https://www.codefactor.io/repository/github/Lightning-AI/lightning/badge)](https://www.codefactor.io/repository/github/Lightning-AI/lightning)
 -->
 
 </div>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytorch-lightning Version: 2.2.3 Summary: PyTorch
+Metadata-Version: 2.1 Name: pytorch-lightning Version: 2.2.4 Summary: PyTorch
 Lightning is the lightweight PyTorch wrapper for ML researchers. Scale your
 models. Write less boilerplate. Home-page: https://github.com/Lightning-AI/
 lightning Author: Lightning AI et al. Author-email: pytorch@lightning.ai
 License: Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
 Project-URL: Documentation, https://pytorch-lightning.rtfd.io/en/latest/
 Project-URL: Source Code, https://github.com/Lightning-AI/lightning Keywords:
@@ -34,15 +34,15 @@
                   img.shields.io/conda/v/conda-forge/pytorch-
 lightning?label=conda&color=success)](https://anaconda.org/conda-forge/pytorch-
 lightning) [![DockerHub](https://img.shields.io/docker/pulls/pytorchlightning/
       pytorch_lightning.svg)](https://hub.docker.com/r/pytorchlightning/
   pytorch_lightning) [![codecov](https://codecov.io/gh/Lightning-AI/pytorch-
  lightning/graph/badge.svg?token=SmzX8mnKlA)](https://codecov.io/gh/Lightning-
 AI/pytorch-lightning) [![ReadTheDocs](https://readthedocs.org/projects/pytorch-
- lightning/badge/?version=2.2.3)](https://lightning.ai/docs/pytorch/stable/)[!
+ lightning/badge/?version=2.2.4)](https://lightning.ai/docs/pytorch/stable/)[!
  [Discord](https://img.shields.io/discord/1077906959069626439?style=plastic)]
    (https://discord.gg/VptPCZkGNa) [![license](https://img.shields.io/badge/
 License-Apache%202.0-blue.svg)](https://github.com/Lightning-AI/lightning/blob/
                                 master/LICENSE)
 ###### \*Codecov is > 90%+ but build delays may show less
 ______________________________________________________________________ ##
 PyTorch Lightning is just organized PyTorch Lightning disentangles PyTorch code
```

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning.egg-info/SOURCES.txt` & `pytorch-lightning-2.2.4/src/pytorch_lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch-lightning-2.2.3/src/pytorch_lightning.egg-info/requires.txt` & `pytorch-lightning-2.2.4/src/pytorch_lightning.egg-info/requires.txt`

 * *Files identical despite different names*

