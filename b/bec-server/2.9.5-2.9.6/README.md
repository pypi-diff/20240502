# Comparing `tmp/bec_server-2.9.5.tar.gz` & `tmp/bec_server-2.9.6.tar.gz`

## Comparing `bec_server-2.9.5.tar` & `bec_server-2.9.6.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.5/README.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/bec_server_utils/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/bec_server_utils/launch.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/bec_server_utils/service_handler.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/bec_server_utils/subprocess_launch.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/bec_server_utils/tmux_launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/data_processing/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/data_processing/dap_server.py
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/data_processing/dap_service.py
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/data_processing/dap_service_manager.py
--rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/data_processing/lmfit1d_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/data_processing/cli/__init__.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/data_processing/cli/launch.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/device_server/__init__.py
--rw-r--r--   0        0        0    18918 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/device_server/device_server.py
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/device_server/rpc_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/device_server/cli/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/device_server/cli/launch.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/device_server/devices/__init__.py
--rw-r--r--   0        0        0     5525 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/device_server/devices/config_update_handler.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/device_server/devices/device_serializer.py
--rw-r--r--   0        0        0    22491 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/device_server/devices/devicemanager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/device_server/tests/__init__.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/device_server/tests/utils.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/file_writer/__init__.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/file_writer/default_writer.py
--rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/file_writer/file_writer.py
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/file_writer/file_writer_manager.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/file_writer/merged_dicts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/file_writer/cli/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/file_writer/cli/launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/file_writer_plugins/__init__.py
--rw-r--r--   0        0        0    22190 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/file_writer_plugins/cSAXS.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_bundler/__init__.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_bundler/bec_emitter.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_bundler/bluesky_emitter.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_bundler/emitter.py
--rw-r--r--   0        0        0    15950 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_bundler/scan_bundler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_bundler/cli/__init__.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_bundler/cli/launch.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/__init__.py
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/device_validation.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/errors.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/path_optimization.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/scan_assembler.py
--rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/scan_guard.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/scan_manager.py
--rw-r--r--   0        0        0    34904 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/scan_queue.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/scan_server.py
--rw-r--r--   0        0        0    18406 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/scan_stubs.py
--rw-r--r--   0        0        0    35666 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/scan_worker.py
--rw-r--r--   0        0        0    52578 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/scans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/cli/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/cli/launch.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/scan_plugins/__init__.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/scan_plugins/otf_scan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/tests/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/tests/fixtures.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scan_server/tests/utils.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scihub/__init__.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scihub/repeated_timer.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scihub/scihub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scihub/cli/__init__.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scihub/cli/launch.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scihub/scibec/__init__.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scihub/scibec/config_handler.py
--rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scihub/scibec/scibec_connector.py
--rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scihub/scibec/scibec_metadata_handler.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scihub/scilog/__init__.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 bec_server-2.9.5/bec_server/scihub/scilog/scilog.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_bec_server_utils/test_main.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_bec_server_utils/test_service_handler.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_bec_server_utils/test_tmux_launch.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_data_processing/conftest.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_data_processing/test_dap_cli_launch.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_data_processing/test_dap_server.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_data_processing/test_dap_service_manager.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_data_processing/test_lmfit1d_service.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_device_server/conftest.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_device_server/test_config_handler.py
--rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_device_server/test_device_manager_ds.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_device_server/test_device_serializer.py
--rw-r--r--   0        0        0    28297 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_device_server/test_device_server.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_device_server/test_device_server_cli_launch.py
--rw-r--r--   0        0        0     9555 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_device_server/test_rpc_mixin.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_file_writer/conftest.py
--rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_file_writer/test_file_writer.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_file_writer/test_file_writer_cli_launch.py
--rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_file_writer/test_file_writer_manager.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scan_bundler/conftest.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scan_bundler/test_bec_emitter.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scan_bundler/test_bluesky_emitter.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scan_bundler/test_emitter.py
--rw-r--r--   0        0        0    25388 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scan_bundler/test_scan_bundler.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scan_server/conftest.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scan_server/test_path_optimization.py
--rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scan_server/test_scan_guard.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scan_server/test_scan_server_cli_launch.py
--rw-r--r--   0        0        0    27483 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scan_server/test_scan_server_queue.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scan_server/test_scan_stubs.py
--rw-r--r--   0        0        0    54003 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scan_server/test_scan_worker.py
--rw-r--r--   0        0        0    87794 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scan_server/test_scans.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scihub/conftest.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scihub/test_repeated_timer.py
--rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scihub/test_scibec_config_handler.py
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scihub/test_scibec_connector.py
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scihub/test_scibec_metadata_handler.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scihub/test_scihub_cli_launch.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bec_server-2.9.5/tests/tests_scihub/test_scilog_connector.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_server-2.9.5/.gitignore
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 bec_server-2.9.5/pyproject.toml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bec_server-2.9.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.6/README.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/bec_server_utils/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/bec_server_utils/launch.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/bec_server_utils/service_handler.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/bec_server_utils/subprocess_launch.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/bec_server_utils/tmux_launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/data_processing/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/data_processing/dap_server.py
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/data_processing/dap_service.py
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/data_processing/dap_service_manager.py
+-rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/data_processing/lmfit1d_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/data_processing/cli/__init__.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/data_processing/cli/launch.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/device_server/__init__.py
+-rw-r--r--   0        0        0    18918 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/device_server/device_server.py
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/device_server/rpc_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/device_server/cli/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/device_server/cli/launch.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/device_server/devices/__init__.py
+-rw-r--r--   0        0        0     5525 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/device_server/devices/config_update_handler.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/device_server/devices/device_serializer.py
+-rw-r--r--   0        0        0    22491 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/device_server/devices/devicemanager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/device_server/tests/__init__.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/device_server/tests/utils.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/file_writer/__init__.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/file_writer/default_writer.py
+-rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/file_writer/file_writer.py
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/file_writer/file_writer_manager.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/file_writer/merged_dicts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/file_writer/cli/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/file_writer/cli/launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/file_writer_plugins/__init__.py
+-rw-r--r--   0        0        0    22190 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/file_writer_plugins/cSAXS.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_bundler/__init__.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_bundler/bec_emitter.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_bundler/bluesky_emitter.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_bundler/emitter.py
+-rw-r--r--   0        0        0    15950 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_bundler/scan_bundler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_bundler/cli/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_bundler/cli/launch.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/__init__.py
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/device_validation.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/errors.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/path_optimization.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/scan_assembler.py
+-rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/scan_guard.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/scan_manager.py
+-rw-r--r--   0        0        0    34904 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/scan_queue.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/scan_server.py
+-rw-r--r--   0        0        0    18406 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/scan_stubs.py
+-rw-r--r--   0        0        0    35666 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/scan_worker.py
+-rw-r--r--   0        0        0    52578 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/scans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/cli/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/cli/launch.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/scan_plugins/__init__.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/scan_plugins/otf_scan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/tests/__init__.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/tests/fixtures.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scan_server/tests/utils.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scihub/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scihub/repeated_timer.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scihub/scihub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scihub/cli/__init__.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scihub/cli/launch.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scihub/scibec/__init__.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scihub/scibec/config_handler.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scihub/scibec/scibec_connector.py
+-rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scihub/scibec/scibec_metadata_handler.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scihub/scilog/__init__.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 bec_server-2.9.6/bec_server/scihub/scilog/scilog.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_bec_server_utils/test_main.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_bec_server_utils/test_service_handler.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_bec_server_utils/test_tmux_launch.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_data_processing/conftest.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_data_processing/test_dap_cli_launch.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_data_processing/test_dap_server.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_data_processing/test_dap_service_manager.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_data_processing/test_lmfit1d_service.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_device_server/conftest.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_device_server/test_config_handler.py
+-rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_device_server/test_device_manager_ds.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_device_server/test_device_serializer.py
+-rw-r--r--   0        0        0    28297 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_device_server/test_device_server.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_device_server/test_device_server_cli_launch.py
+-rw-r--r--   0        0        0     9555 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_device_server/test_rpc_mixin.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_file_writer/conftest.py
+-rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_file_writer/test_file_writer.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_file_writer/test_file_writer_cli_launch.py
+-rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_file_writer/test_file_writer_manager.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scan_bundler/conftest.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scan_bundler/test_bec_emitter.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scan_bundler/test_bluesky_emitter.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scan_bundler/test_emitter.py
+-rw-r--r--   0        0        0    25388 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scan_bundler/test_scan_bundler.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scan_server/conftest.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scan_server/test_path_optimization.py
+-rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scan_server/test_scan_guard.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scan_server/test_scan_server_cli_launch.py
+-rw-r--r--   0        0        0    27483 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scan_server/test_scan_server_queue.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scan_server/test_scan_stubs.py
+-rw-r--r--   0        0        0    54003 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scan_server/test_scan_worker.py
+-rw-r--r--   0        0        0    87794 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scan_server/test_scans.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scihub/conftest.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scihub/test_repeated_timer.py
+-rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scihub/test_scibec_config_handler.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scihub/test_scibec_connector.py
+-rw-r--r--   0        0        0     8242 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scihub/test_scibec_metadata_handler.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scihub/test_scihub_cli_launch.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bec_server-2.9.6/tests/tests_scihub/test_scilog_connector.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_server-2.9.6/.gitignore
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 bec_server-2.9.6/pyproject.toml
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bec_server-2.9.6/PKG-INFO
```

### Comparing `bec_server-2.9.5/bec_server/bec_server_utils/launch.py` & `bec_server-2.9.6/bec_server/bec_server_utils/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/bec_server_utils/service_handler.py` & `bec_server-2.9.6/bec_server/bec_server_utils/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/bec_server_utils/subprocess_launch.py` & `bec_server-2.9.6/bec_server/bec_server_utils/subprocess_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/bec_server_utils/tmux_launch.py` & `bec_server-2.9.6/bec_server/bec_server_utils/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/data_processing/dap_server.py` & `bec_server-2.9.6/bec_server/data_processing/dap_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/data_processing/dap_service.py` & `bec_server-2.9.6/bec_server/data_processing/dap_service.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/data_processing/dap_service_manager.py` & `bec_server-2.9.6/bec_server/data_processing/dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/data_processing/lmfit1d_service.py` & `bec_server-2.9.6/bec_server/data_processing/lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/data_processing/cli/launch.py` & `bec_server-2.9.6/bec_server/data_processing/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/device_server/device_server.py` & `bec_server-2.9.6/bec_server/device_server/device_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/device_server/rpc_mixin.py` & `bec_server-2.9.6/bec_server/device_server/rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/device_server/cli/launch.py` & `bec_server-2.9.6/bec_server/device_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/device_server/devices/config_update_handler.py` & `bec_server-2.9.6/bec_server/device_server/devices/config_update_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/device_server/devices/device_serializer.py` & `bec_server-2.9.6/bec_server/device_server/devices/device_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/device_server/devices/devicemanager.py` & `bec_server-2.9.6/bec_server/device_server/devices/devicemanager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/device_server/tests/utils.py` & `bec_server-2.9.6/bec_server/device_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/file_writer/default_writer.py` & `bec_server-2.9.6/bec_server/file_writer/default_writer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/file_writer/file_writer.py` & `bec_server-2.9.6/bec_server/file_writer/file_writer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/file_writer/file_writer_manager.py` & `bec_server-2.9.6/bec_server/file_writer/file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/file_writer/merged_dicts.py` & `bec_server-2.9.6/bec_server/file_writer/merged_dicts.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/file_writer/cli/launch.py` & `bec_server-2.9.6/bec_server/file_writer/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/file_writer_plugins/cSAXS.py` & `bec_server-2.9.6/bec_server/file_writer_plugins/cSAXS.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_bundler/bec_emitter.py` & `bec_server-2.9.6/bec_server/scan_bundler/bec_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_bundler/bluesky_emitter.py` & `bec_server-2.9.6/bec_server/scan_bundler/bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_bundler/emitter.py` & `bec_server-2.9.6/bec_server/scan_bundler/emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_bundler/scan_bundler.py` & `bec_server-2.9.6/bec_server/scan_bundler/scan_bundler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_bundler/cli/launch.py` & `bec_server-2.9.6/bec_server/scan_bundler/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_server/device_validation.py` & `bec_server-2.9.6/bec_server/scan_server/device_validation.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_server/path_optimization.py` & `bec_server-2.9.6/bec_server/scan_server/path_optimization.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_server/scan_assembler.py` & `bec_server-2.9.6/bec_server/scan_server/scan_assembler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_server/scan_guard.py` & `bec_server-2.9.6/bec_server/scan_server/scan_guard.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_server/scan_manager.py` & `bec_server-2.9.6/bec_server/scan_server/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_server/scan_queue.py` & `bec_server-2.9.6/bec_server/scan_server/scan_queue.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_server/scan_server.py` & `bec_server-2.9.6/bec_server/scan_server/scan_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_server/scan_stubs.py` & `bec_server-2.9.6/bec_server/scan_server/scan_stubs.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_server/scan_worker.py` & `bec_server-2.9.6/bec_server/scan_server/scan_worker.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_server/scans.py` & `bec_server-2.9.6/bec_server/scan_server/scans.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_server/cli/launch.py` & `bec_server-2.9.6/bec_server/scan_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_server/scan_plugins/otf_scan.py` & `bec_server-2.9.6/bec_server/scan_server/scan_plugins/otf_scan.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scan_server/tests/utils.py` & `bec_server-2.9.6/bec_server/scan_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scihub/repeated_timer.py` & `bec_server-2.9.6/bec_server/scihub/repeated_timer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scihub/scihub.py` & `bec_server-2.9.6/bec_server/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scihub/cli/launch.py` & `bec_server-2.9.6/bec_server/scihub/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scihub/scibec/config_handler.py` & `bec_server-2.9.6/bec_server/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/bec_server/scihub/scibec/scibec_connector.py` & `bec_server-2.9.6/bec_server/scihub/scibec/scibec_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import os
 from typing import TYPE_CHECKING
 
+import py_scibec
 from dotenv import dotenv_values
 from py_scibec import SciBecCore
 
 from bec_lib import MessageEndpoints, bec_logger, messages
 from bec_lib.connector import ConnectorBase
 from bec_server.scihub.repeated_timer import RepeatedTimer
 
@@ -172,37 +173,32 @@
 
     def _update_scibec_instance(self):
         logger.info(f"Connecting to SciBec on {self.host}")
         self.scibec = SciBecCore(host=self.host)
         self.scibec.login(username=self.ingestor, password=self.ingestor_secret)
 
     def _update_experiment_info(self):
-        beamline_info = self.scibec.beamline.beamline_controller_find(
-            query_params={"filter": {"where": {"name": self.target_bl}}}
-        )
-        if not beamline_info.body:
+        bl_filter = py_scibec.bec.BeamlineFilterWhere(where={"name": self.target_bl})
+        beamline_info = self.scibec.beamline.beamline_controller_find(bl_filter)
+        if not beamline_info:
             raise SciBecConnectorError(f"Could not find a beamline with the name {self.target_bl}")
-        beamline_info = beamline_info.body[0]
-        self.scibec_info["beamline"] = beamline_info
-        experiment_id = beamline_info.get("activeExperiment")
+        self.scibec_info["beamline"] = beamline_info[0]
+        experiment_id = beamline_info[0].active_experiment
 
         if not experiment_id:
             raise SciBecConnectorError(f"Could not find an active experiment on {self.target_bl}")
 
-        experiment = self.scibec.experiment.experiment_controller_find_by_id(
-            path_params={"id": experiment_id}
-        )
+        experiment = self.scibec.experiment.experiment_controller_find_by_id(experiment_id)
 
         if not experiment:
             raise SciBecConnectorError(f"Could not find an experiment with the id {experiment_id}")
-        experiment = experiment.body
         self.scibec_info["activeExperiment"] = experiment
 
     def _update_eaccount_in_redis(self):
-        write_account = self.scibec_info["activeExperiment"]["writeAccount"]
+        write_account = self.scibec_info["activeExperiment"].write_account
         if write_account[0] == "p":
             write_account = write_account.replace("p", "e")
         msg = messages.VariableMessage(value=write_account)
         self.connector.set(MessageEndpoints.account(), msg)
 
     def shutdown(self):
         """
```

### Comparing `bec_server-2.9.5/bec_server/scihub/scibec/scibec_metadata_handler.py` & `bec_server-2.9.6/bec_server/scihub/scibec/scibec_metadata_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import json
 import time
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
+import py_scibec
+import py_scibec_openapi_client.models as py_scibec_models
 
 from bec_lib import MessageEndpoints, bec_logger
 from bec_lib.serialization import json_ext
 
 logger = bec_logger.logger
 
 if TYPE_CHECKING:
@@ -63,67 +65,68 @@
         Returns:
             dict: The updated scan data
         """
         scibec = self.scibec_connector.scibec
         if not scibec:
             return
         scibec_info = self.scibec_connector.scibec_info
-        experiment_id = scibec_info["activeExperiment"]["id"]
+        experiment_id = scibec_info["activeExperiment"].id
         # session_id = scibec_info["activeSession"][0]["id"]
         # experiment_id = scibec_info["activeSession"][0]["experimentId"]
         logger.debug(f"Received new scan status {msg}")
-        scan = scibec.scan.scan_controller_find(
-            query_params={"filter": {"where": {"scanId": msg.content["scan_id"]}}}
-        ).body
+        scan_filter = py_scibec.bec.ScanFilterWhere(where={"scanId": msg.content["scan_id"]})
+        scan = scibec.scan.scan_controller_find(scan_filter)
         if not scan:
             info = msg.content["info"]
             dataset_number = info.get("dataset_number")
-            dataset = scibec.dataset.dataset_controller_find(
-                query_params={
-                    "filter": {"where": {"number": dataset_number, "experimentId": experiment_id}}
-                }
-            ).body
+            dataset_filter = py_scibec.bec.DatasetFilterWhere(
+                where={"number": dataset_number, "experimentId": experiment_id}
+            )
+            dataset = scibec.dataset.dataset_controller_find(dataset_filter)
             if dataset:
                 dataset = dataset[0]
             else:
-                dataset = scibec.dataset.dataset_controller_create(
-                    body=scibec.models.Dataset(
-                        **{
-                            "readACL": scibec_info["activeExperiment"]["readACL"],
-                            "writeACL": scibec_info["activeExperiment"]["readACL"],
-                            "owner": scibec_info["activeExperiment"]["owner"],
-                            "number": dataset_number,
-                            "experimentId": experiment_id,
-                            "name": info.get("dataset_name", ""),
-                        }
-                    )
-                ).body
-
-            scan_data = {
-                "readACL": scibec_info["activeExperiment"]["readACL"],
-                "writeACL": scibec_info["activeExperiment"]["readACL"],
-                "owner": scibec_info["activeExperiment"]["owner"],
-                "scanType": info.get("scan_name", ""),
-                "scanId": info.get("scan_id", ""),
-                "queueId": info.get("queue_id", ""),
-                "requestId": info.get("RID", ""),
-                "exitStatus": msg.content["status"],
-                # "queue": info.get("stream", ""),
-                "metadata": info,
-                # "sessionId": session_id,
-                "datasetId": dataset["id"],
-                "scanNumber": info.get("scan_number", 0),
-            }
-            scan = scibec.scan.scan_controller_create(body=scibec.models.Scan(**scan_data)).body
+                new_dataset = py_scibec.bec.NewDataset(
+                    **{
+                        "readACL": scibec_info["activeExperiment"].read_acl,
+                        "writeACL": scibec_info["activeExperiment"].read_acl,
+                        "owner": scibec_info["activeExperiment"].owner,
+                        "number": dataset_number,
+                        "experimentId": experiment_id,
+                        "name": info.get("dataset_name", ""),
+                    }
+                )
+                dataset = scibec.dataset.dataset_controller_create(new_dataset)
+
+            new_scan = py_scibec.bec.NewScan(
+                **{
+                    "readACL": scibec_info["activeExperiment"].read_acl,
+                    "writeACL": scibec_info["activeExperiment"].read_acl,
+                    "owner": scibec_info["activeExperiment"].owner,
+                    "scanType": info.get("scan_name", ""),
+                    "scanId": info.get("scan_id", ""),
+                    "queueId": info.get("queue_id", ""),
+                    "requestId": info.get("RID", ""),
+                    "exitStatus": msg.content["status"],
+                    # "queue": info.get("stream", ""),
+                    "metadata": info,
+                    # "sessionId": session_id,
+                    "datasetId": dataset.id,
+                    "scanNumber": info.get("scan_number", 0),
+                }
+            )
+            scan = scibec.scan.scan_controller_create(new_scan)
             # scan = scibec.add_scan(scan_data)
         else:
             info = msg.content["info"]
             scan = scibec.scan.scan_controller_update_by_id(
-                path_params={"id": scan[0]["id"]},
-                body={"metadata": info, "exitStatus": msg.content["status"]},
+                id=scan[0].id,
+                scan_partial=py_scibec.bec.ScanPartial(
+                    metadata=info, exitStatus=msg.content["status"]
+                ),
             )
         return scan
 
     @staticmethod
     def _handle_file_content(msg, *, parent, **_kwargs) -> None:
         msg = msg.value
         try:
@@ -170,17 +173,16 @@
         Args:
             file_path(str): The path to the original NeXuS file
             data(dict): The scan data
         """
         scibec = self.scibec_connector.scibec
         if not scibec:
             return
-        scan = scibec.scan.scan_controller_find(
-            query_params={"filter": {"where": {"scanId": data["metadata"]["scan_id"]}}}
-        ).body
+        scan_filter = py_scibec.bec.ScanFilterWhere(where={"scanId": data["metadata"]["scan_id"]})
+        scan = scibec.scan.scan_controller_find(scan_filter)
         if not scan:
             logger.warning(
                 f"Could not find scan with scan_id {data['metadata']['scan_id']}. Cannot write scan"
                 " data to SciBec."
             )
             return
         scan = scan[0]
@@ -191,32 +193,32 @@
         logger.info(f"Data size: {data_size} MB")
         if data_size > 1:
             logger.info(
                 f"Data size is larger than {self.MAX_DATA_SIZE/1e6} MB. Splitting data into chunks."
             )
             self._write_scan_data_chunks(file_path, data_bec, scan)
         else:
-
-            scibec.scan_data.scan_data_controller_create_many(
-                body=scibec.models.ScanData(
-                    **{
-                        "readACL": scan["readACL"],
-                        "writeACL": scan["readACL"],
-                        "owner": scan["owner"],
-                        "scanId": scan["id"],
-                        "filePath": file_path,
-                        "data": data_bec,
-                    }
-                )
+            new_scan_data = py_scibec.bec.NewScanData(
+                **{
+                    "readACL": scan.read_acl,
+                    "writeACL": scan.read_acl,
+                    "owner": scan.owner,
+                    "scanId": scan.id,
+                    "filePath": file_path,
+                    "data": data_bec,
+                }
             )
+            scibec.scan_data.scan_data_controller_create_many(new_scan_data)
         logger.info(
             f"Wrote scan data to SciBec for scan_id {data['metadata']['scan_id']} in {time.time() - start} seconds."
         )
 
-    def _write_scan_data_chunks(self, file_path: str, data_bec: dict, scan: dict):
+    def _write_scan_data_chunks(
+        self, file_path: str, data_bec: dict, scan: py_scibec_models.ScanWithRelations
+    ):
         """
         Write the scan data to SciBec in chunks. This method is called if the scan data is larger
         than 1 MB. The method loops through all keys in the data dictionary and creates chunks of
         max 1 MB size. The chunks are then written to SciBec.
 
         Args:
             file_path(str): The path to the original NeXuS file
@@ -230,43 +232,41 @@
         for key, value in data_bec.items():
             if len(json.dumps({key: value})) > self.MAX_DATA_SIZE:
                 logger.warning(
                     f"Data size of key {key} is larger than {self.MAX_DATA_SIZE/1e6} MB. Cannot write this key to SciBec."
                 )
                 continue
             if len(json.dumps(chunk)) + len(json.dumps({key: value})) > self.MAX_DATA_SIZE:
-                scibec.scan_data.scan_data_controller_create_many(
-                    body=scibec.models.ScanData(
-                        **{
-                            "readACL": scan["readACL"],
-                            "writeACL": scan["readACL"],
-                            "owner": scan["owner"],
-                            "scanId": scan["id"],
-                            "filePath": file_path,
-                            "data": chunk,
-                        }
-                    )
+                new_scan_data = py_scibec.bec.NewScanData(
+                    **{
+                        "readACL": scan.read_acl,
+                        "writeACL": scan.read_acl,
+                        "owner": scan.owner,
+                        "scanId": scan.id,
+                        "filePath": file_path,
+                        "data": chunk,
+                    }
                 )
+                scibec.scan_data.scan_data_controller_create_many(new_scan_data)
                 chunk = {}
             chunk[key] = value
 
         # Write the last chunk
         if chunk:
-            scibec.scan_data.scan_data_controller_create_many(
-                body=scibec.models.ScanData(
-                    **{
-                        "readACL": scan["readACL"],
-                        "writeACL": scan["readACL"],
-                        "owner": scan["owner"],
-                        "scanId": scan["id"],
-                        "filePath": file_path,
-                        "data": chunk,
-                    }
-                )
+            new_scan_data = py_scibec.bec.NewScanData(
+                **{
+                    "readACL": scan.read_acl,
+                    "writeACL": scan.read_acl,
+                    "owner": scan.owner,
+                    "scanId": scan.id,
+                    "filePath": file_path,
+                    "data": chunk,
+                }
             )
+            scibec.scan_data.scan_data_controller_create_many(new_scan_data)
 
     def shutdown(self):
         """
         Shutdown the metadata handler
         """
         if self._scan_status_register:
             self._scan_status_register.shutdown()
```

### Comparing `bec_server-2.9.5/bec_server/scihub/scilog/scilog.py` & `bec_server-2.9.6/bec_server/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_bec_server_utils/test_main.py` & `bec_server-2.9.6/tests/tests_bec_server_utils/test_main.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_bec_server_utils/test_service_handler.py` & `bec_server-2.9.6/tests/tests_bec_server_utils/test_service_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_bec_server_utils/test_tmux_launch.py` & `bec_server-2.9.6/tests/tests_bec_server_utils/test_tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_data_processing/test_dap_cli_launch.py` & `bec_server-2.9.6/tests/tests_data_processing/test_dap_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_data_processing/test_dap_service_manager.py` & `bec_server-2.9.6/tests/tests_data_processing/test_dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_data_processing/test_lmfit1d_service.py` & `bec_server-2.9.6/tests/tests_data_processing/test_lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_device_server/conftest.py` & `bec_server-2.9.6/tests/tests_device_server/conftest.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_device_server/test_config_handler.py` & `bec_server-2.9.6/tests/tests_device_server/test_config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_device_server/test_device_manager_ds.py` & `bec_server-2.9.6/tests/tests_device_server/test_device_manager_ds.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_device_server/test_device_serializer.py` & `bec_server-2.9.6/tests/tests_device_server/test_device_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_device_server/test_device_server.py` & `bec_server-2.9.6/tests/tests_device_server/test_device_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_device_server/test_device_server_cli_launch.py` & `bec_server-2.9.6/tests/tests_device_server/test_device_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_device_server/test_rpc_mixin.py` & `bec_server-2.9.6/tests/tests_device_server/test_rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_file_writer/test_file_writer.py` & `bec_server-2.9.6/tests/tests_file_writer/test_file_writer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_file_writer/test_file_writer_cli_launch.py` & `bec_server-2.9.6/tests/tests_file_writer/test_file_writer_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_file_writer/test_file_writer_manager.py` & `bec_server-2.9.6/tests/tests_file_writer/test_file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scan_bundler/conftest.py` & `bec_server-2.9.6/tests/tests_scan_bundler/conftest.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scan_bundler/test_bec_emitter.py` & `bec_server-2.9.6/tests/tests_scan_bundler/test_bec_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scan_bundler/test_bluesky_emitter.py` & `bec_server-2.9.6/tests/tests_scan_bundler/test_bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scan_bundler/test_emitter.py` & `bec_server-2.9.6/tests/tests_scan_bundler/test_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scan_bundler/test_scan_bundler.py` & `bec_server-2.9.6/tests/tests_scan_bundler/test_scan_bundler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py` & `bec_server-2.9.6/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scan_server/test_path_optimization.py` & `bec_server-2.9.6/tests/tests_scan_server/test_path_optimization.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scan_server/test_scan_guard.py` & `bec_server-2.9.6/tests/tests_scan_server/test_scan_guard.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scan_server/test_scan_server_cli_launch.py` & `bec_server-2.9.6/tests/tests_scan_server/test_scan_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scan_server/test_scan_server_queue.py` & `bec_server-2.9.6/tests/tests_scan_server/test_scan_server_queue.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scan_server/test_scan_stubs.py` & `bec_server-2.9.6/tests/tests_scan_server/test_scan_stubs.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scan_server/test_scan_worker.py` & `bec_server-2.9.6/tests/tests_scan_server/test_scan_worker.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scan_server/test_scans.py` & `bec_server-2.9.6/tests/tests_scan_server/test_scans.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scihub/test_repeated_timer.py` & `bec_server-2.9.6/tests/tests_scihub/test_repeated_timer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scihub/test_scibec_config_handler.py` & `bec_server-2.9.6/tests/tests_scihub/test_scibec_config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scihub/test_scibec_connector.py` & `bec_server-2.9.6/tests/tests_scihub/test_scibec_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from unittest import mock
 
 import pytest
 
 from bec_lib import MessageEndpoints, ServiceConfig, messages
-from bec_lib.logger import bec_logger
 from bec_lib.messages import BECStatus
 from bec_lib.tests.utils import ConnectorMock
 from bec_server.scihub import SciHub
 from bec_server.scihub.scibec import SciBecConnector
 
 
 class SciHubMocked(SciHub):
@@ -110,42 +109,24 @@
                 ) as mock_update_eaccount_in_redis:
                     SciBecMock.connect_to_scibec()
                     mock_update_scibec_instance.assert_called_once()
                     mock_update_experiment_info.assert_called_once()
                     mock_update_eaccount_in_redis.assert_called_once()
 
 
-class ServerResponseMock:
-    def __init__(self, body):
-        self.body = body
-
-
-def test_scibec_update_experiment_info(SciBecMock):
+def test_scibec_update_experiment_info(SciBecMock, active_experiment, beamline_document):
     with mock.patch.object(SciBecMock, "scibec") as mock_scibec:
-        beamline_document = {
-            "name": "dummy_bl",
-            "activeExperiment": "dummy_experiment",
-            "id": "dummy_id",
-        }
-        mock_scibec.beamline.beamline_controller_find.return_value = ServerResponseMock(
-            (beamline_document,)
-        )
-        experiment_document = {
-            "name": "dummy_experiment",
-            "writeAccount": "dummy_write_account",
-            "id": "dummy_experiment_id",
-        }
-        mock_scibec.experiment.experiment_controller_find_by_id.return_value = ServerResponseMock(
-            experiment_document
-        )
+        mock_scibec.beamline.beamline_controller_find.return_value = (beamline_document,)
+        experiment_document = active_experiment
+        mock_scibec.experiment.experiment_controller_find_by_id.return_value = experiment_document
         SciBecMock._update_experiment_info()
         assert SciBecMock.scibec_info["activeExperiment"] == experiment_document
         assert SciBecMock.scibec_info["beamline"] == beamline_document
 
 
-def test_update_eaccount_in_redis(SciBecMock):
-    SciBecMock.scibec_info = {"activeExperiment": {"writeAccount": "p12345"}}
+def test_update_eaccount_in_redis(SciBecMock, active_experiment):
+    SciBecMock.scibec_info = {"activeExperiment": active_experiment}
     with mock.patch.object(SciBecMock, "connector") as mock_connector:
         SciBecMock._update_eaccount_in_redis()
         mock_connector.set.assert_called_once_with(
             MessageEndpoints.account(), messages.VariableMessage(value="e12345")
         )
```

### Comparing `bec_server-2.9.5/tests/tests_scihub/test_scibec_metadata_handler.py` & `bec_server-2.9.6/tests/tests_scihub/test_scibec_metadata_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from unittest import mock
 
 import numpy as np
 import pytest
+from py_scibec_openapi_client.models import NewScanData, ScanPartial
 
 from bec_lib import messages
 from bec_lib.redis_connector import MessageObject
 from bec_server.scihub.scibec.scibec_metadata_handler import SciBecMetadataHandler
 
 
 @pytest.fixture
@@ -42,56 +43,41 @@
 def test_update_scan_status_returns_without_scibec(md_handler):
     # pylint: disable=protected-access
     msg = messages.ScanStatusMessage(scan_id="scan_id", status="open", info={})
     md_handler.scibec_connector.scibec = None
     md_handler.update_scan_status(msg)
 
 
-def test_update_scan_status(md_handler):
+def test_update_scan_status(md_handler, active_experiment, dataset_document):
     # pylint: disable=protected-access
     msg = messages.ScanStatusMessage(scan_id="scan_id", status="open", info={"dataset_number": 12})
     scibec = mock.Mock()
     md_handler.scibec_connector.scibec = scibec
-    scibec_info = {
-        "activeExperiment": {
-            "id": "id",
-            "readACL": ["readACL"],
-            "writeACL": ["writeACL"],
-            "owner": "owner",
-        }
-    }
+    scibec_info = {"activeExperiment": active_experiment}
     md_handler.scibec_connector.scibec_info = scibec_info
-    type(scibec.scan.scan_controller_find()).body = mock.PropertyMock(return_value=[])
-    type(scibec.dataset.dataset_controller_find()).body = mock.PropertyMock(return_value=[])
-    type(scibec.dataset.dataset_controller_create()).body = mock.PropertyMock(
-        return_value={"id": "id"}
-    )
+    scibec.scan.scan_controller_find = mock.MagicMock(return_value=[])
+    scibec.dataset.dataset_controller_find = mock.MagicMock(return_value=[])
+    scibec.dataset.dataset_controller_create = mock.MagicMock(return_value=dataset_document)
     md_handler.update_scan_status(msg)
 
 
-def test_update_scan_status_patch(md_handler):
+def test_update_scan_status_patch(md_handler, active_experiment, scan_document):
     # pylint: disable=protected-access
     msg = messages.ScanStatusMessage(
         scan_id="scan_id", status="closed", info={"dataset_number": 12}
     )
     scibec = mock.Mock()
     md_handler.scibec_connector.scibec = scibec
-    scibec_info = {
-        "activeExperiment": {
-            "id": "id",
-            "readACL": ["readACL"],
-            "writeACL": ["writeACL"],
-            "owner": "owner",
-        }
-    }
+    scibec_info = {"activeExperiment": active_experiment}
     md_handler.scibec_connector.scibec_info = scibec_info
-    type(scibec.scan.scan_controller_find()).body = mock.PropertyMock(return_value=[{"id": "id"}])
+    scibec.scan.scan_controller_find = mock.MagicMock(return_value=[scan_document])
     md_handler.update_scan_status(msg)
     scibec.scan.scan_controller_update_by_id.assert_called_once_with(
-        path_params={"id": "id"}, body={"metadata": {"dataset_number": 12}, "exitStatus": "closed"}
+        id="dummy_id",
+        scan_partial=ScanPartial(exit_status="closed", metadata={"dataset_number": 12}),
     )
 
 
 def test_handle_file_content(md_handler):
     # pylint: disable=protected-access
     msg = messages.FileContentMessage(file_path="my_file.h5", data={"data": {}})
     msg_raw = MessageObject(value=msg, topic="file_content")
@@ -120,56 +106,48 @@
     md_handler.update_scan_data(file_path="my_file.h5", data={"data": {}})
 
 
 def test_update_scan_data_without_scan(md_handler):
     # pylint: disable=protected-access
     scibec = mock.Mock()
     md_handler.scibec_connector.scibec = scibec
-    type(scibec.scan.scan_controller_find()).body = mock.PropertyMock(return_value=[])
+    scibec.scan.scan_controller_find = mock.MagicMock(return_value=[])
     md_handler.update_scan_data(
         file_path="my_file.h5", data={"data": {}, "metadata": {"scan_id": "scan_id"}}
     )
 
 
-def test_update_scan_data(md_handler):
+def test_update_scan_data(md_handler, scan_document):
     # pylint: disable=protected-access
     scibec = mock.Mock()
     md_handler.scibec_connector.scibec = scibec
-    type(scibec.scan.scan_controller_find()).body = mock.PropertyMock(
-        return_value=[
-            {"id": "id", "readACL": ["readACL"], "writeACL": ["writeACL"], "owner": "owner"}
-        ]
-    )
+    scibec.scan.scan_controller_find = mock.MagicMock(return_value=[scan_document])
     md_handler.update_scan_data(
         file_path="my_file.h5", data={"data": {}, "metadata": {"scan_id": "scan_id"}}
     )
     scibec.scan_data.scan_data_controller_create_many.assert_called_once_with(
-        body=scibec.models.ScanData(
+        NewScanData(
             **{
-                "readACL": "readACL",
-                "writeACL": "readACL",
-                "owner": "owner",
-                "scanId": "id",
+                "readACL": ["readACL"],
+                "writeACL": ["readACL"],
+                "owner": ["owner"],
+                "scanId": "dummy_id",
                 "filePath": "my_file.h5",
                 "data": {"data": {}, "metadata": {"scan_id": "scan_id"}},
             }
         )
     )
 
 
-def test_update_scan_data_exceeding_limit(md_handler):
+def test_update_scan_data_exceeding_limit(md_handler, scan_document):
     # pylint: disable=protected-access
     scibec = mock.Mock()
     md_handler.MAX_DATA_SIZE = 1000
     md_handler.scibec_connector.scibec = scibec
-    type(scibec.scan.scan_controller_find()).body = mock.PropertyMock(
-        return_value=[
-            {"id": "id", "readACL": ["readACL"], "writeACL": ["writeACL"], "owner": "owner"}
-        ]
-    )
+    scibec.scan.scan_controller_find = mock.MagicMock(return_value=[scan_document])
     data_block = {f"key_{i}": {"signal": list(range(100))} for i in range(10)}
     data_block.update({"metadata": {"scan_id": "scan_id"}})
     md_handler.update_scan_data(file_path="my_file.h5", data=data_block)
     num_calls = scibec.scan_data.scan_data_controller_create_many.call_count
     assert num_calls == 5
```

### Comparing `bec_server-2.9.5/tests/tests_scihub/test_scihub_cli_launch.py` & `bec_server-2.9.6/tests/tests_scihub/test_scihub_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/tests/tests_scihub/test_scilog_connector.py` & `bec_server-2.9.6/tests/tests_scihub/test_scilog_connector.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/.gitignore` & `bec_server-2.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.5/pyproject.toml` & `bec_server-2.9.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec-server"
-version = "2.9.5"
+version = "2.9.6"
 description = "BEC server"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
```

### Comparing `bec_server-2.9.5/PKG-INFO` & `bec_server-2.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bec-server
-Version: 2.9.5
+Version: 2.9.6
 Summary: BEC server
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/bec
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```

