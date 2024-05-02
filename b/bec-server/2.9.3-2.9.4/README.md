# Comparing `tmp/bec_server-2.9.3.tar.gz` & `tmp/bec_server-2.9.4.tar.gz`

## Comparing `bec_server-2.9.3.tar` & `bec_server-2.9.4.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.3/README.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/bec_server_utils/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/bec_server_utils/launch.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/bec_server_utils/service_handler.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/bec_server_utils/subprocess_launch.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/bec_server_utils/tmux_launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/data_processing/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/data_processing/dap_server.py
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/data_processing/dap_service.py
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/data_processing/dap_service_manager.py
--rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/data_processing/lmfit1d_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/data_processing/cli/__init__.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/data_processing/cli/launch.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/device_server/__init__.py
--rw-r--r--   0        0        0    18918 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/device_server/device_server.py
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/device_server/rpc_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/device_server/cli/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/device_server/cli/launch.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/device_server/devices/__init__.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/device_server/devices/config_update_handler.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/device_server/devices/device_serializer.py
--rw-r--r--   0        0        0    22519 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/device_server/devices/devicemanager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/device_server/tests/__init__.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/device_server/tests/utils.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/file_writer/__init__.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/file_writer/default_writer.py
--rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/file_writer/file_writer.py
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/file_writer/file_writer_manager.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/file_writer/merged_dicts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/file_writer/cli/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/file_writer/cli/launch.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/file_writer_plugins/__init__.py
--rw-r--r--   0        0        0    22190 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/file_writer_plugins/cSAXS.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_bundler/__init__.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_bundler/bec_emitter.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_bundler/bluesky_emitter.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_bundler/emitter.py
--rw-r--r--   0        0        0    15950 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_bundler/scan_bundler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_bundler/cli/__init__.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_bundler/cli/launch.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/__init__.py
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/device_validation.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/errors.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/path_optimization.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/scan_assembler.py
--rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/scan_guard.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/scan_manager.py
--rw-r--r--   0        0        0    34887 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/scan_queue.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/scan_server.py
--rw-r--r--   0        0        0    18416 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/scan_stubs.py
--rw-r--r--   0        0        0    35666 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/scan_worker.py
--rw-r--r--   0        0        0    52578 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/scans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/cli/__init__.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/cli/launch.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/scan_plugins/__init__.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/scan_plugins/otf_scan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/tests/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/tests/fixtures.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scan_server/tests/utils.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scihub/__init__.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scihub/repeated_timer.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scihub/scihub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scihub/cli/__init__.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scihub/cli/launch.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scihub/scibec/__init__.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scihub/scibec/config_handler.py
--rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scihub/scibec/scibec_connector.py
--rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scihub/scibec/scibec_metadata_handler.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scihub/scilog/__init__.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 bec_server-2.9.3/bec_server/scihub/scilog/scilog.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_bec_server_utils/test_main.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_bec_server_utils/test_service_handler.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_bec_server_utils/test_tmux_launch.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_data_processing/conftest.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_data_processing/test_dap_cli_launch.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_data_processing/test_dap_server.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_data_processing/test_dap_service_manager.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_data_processing/test_lmfit1d_service.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_device_server/conftest.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_device_server/test_config_handler.py
--rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_device_server/test_device_manager_ds.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_device_server/test_device_serializer.py
--rw-r--r--   0        0        0    28297 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_device_server/test_device_server.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_device_server/test_device_server_cli_launch.py
--rw-r--r--   0        0        0     9555 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_device_server/test_rpc_mixin.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_file_writer/conftest.py
--rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_file_writer/test_file_writer.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_file_writer/test_file_writer_cli_launch.py
--rw-r--r--   0        0        0    11233 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_file_writer/test_file_writer_manager.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scan_bundler/conftest.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scan_bundler/test_bec_emitter.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scan_bundler/test_bluesky_emitter.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scan_bundler/test_emitter.py
--rw-r--r--   0        0        0    25541 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scan_bundler/test_scan_bundler.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scan_server/conftest.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scan_server/test_path_optimization.py
--rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scan_server/test_scan_guard.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scan_server/test_scan_server_cli_launch.py
--rw-r--r--   0        0        0    26475 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scan_server/test_scan_server_queue.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scan_server/test_scan_stubs.py
--rw-r--r--   0        0        0    54003 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scan_server/test_scan_worker.py
--rw-r--r--   0        0        0    87804 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scan_server/test_scans.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scihub/conftest.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scihub/test_repeated_timer.py
--rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scihub/test_scibec_config_handler.py
--rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scihub/test_scibec_connector.py
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scihub/test_scibec_metadata_handler.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scihub/test_scihub_cli_launch.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bec_server-2.9.3/tests/tests_scihub/test_scilog_connector.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_server-2.9.3/.gitignore
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 bec_server-2.9.3/pyproject.toml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bec_server-2.9.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.4/README.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/bec_server_utils/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/bec_server_utils/launch.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/bec_server_utils/service_handler.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/bec_server_utils/subprocess_launch.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/bec_server_utils/tmux_launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/data_processing/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/data_processing/dap_server.py
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/data_processing/dap_service.py
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/data_processing/dap_service_manager.py
+-rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/data_processing/lmfit1d_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/data_processing/cli/__init__.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/data_processing/cli/launch.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/device_server/__init__.py
+-rw-r--r--   0        0        0    18918 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/device_server/device_server.py
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/device_server/rpc_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/device_server/cli/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/device_server/cli/launch.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/device_server/devices/__init__.py
+-rw-r--r--   0        0        0     5525 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/device_server/devices/config_update_handler.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/device_server/devices/device_serializer.py
+-rw-r--r--   0        0        0    22491 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/device_server/devices/devicemanager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/device_server/tests/__init__.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/device_server/tests/utils.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/file_writer/__init__.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/file_writer/default_writer.py
+-rw-r--r--   0        0        0     8713 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/file_writer/file_writer.py
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/file_writer/file_writer_manager.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/file_writer/merged_dicts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/file_writer/cli/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/file_writer/cli/launch.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/file_writer_plugins/__init__.py
+-rw-r--r--   0        0        0    22190 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/file_writer_plugins/cSAXS.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_bundler/__init__.py
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_bundler/bec_emitter.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_bundler/bluesky_emitter.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_bundler/emitter.py
+-rw-r--r--   0        0        0    15950 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_bundler/scan_bundler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_bundler/cli/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_bundler/cli/launch.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/__init__.py
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/device_validation.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/errors.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/path_optimization.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/scan_assembler.py
+-rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/scan_guard.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/scan_manager.py
+-rw-r--r--   0        0        0    34887 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/scan_queue.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/scan_server.py
+-rw-r--r--   0        0        0    18406 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/scan_stubs.py
+-rw-r--r--   0        0        0    35666 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/scan_worker.py
+-rw-r--r--   0        0        0    52578 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/scans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/cli/__init__.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/cli/launch.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/scan_plugins/__init__.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/scan_plugins/otf_scan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/tests/__init__.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/tests/fixtures.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scan_server/tests/utils.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scihub/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scihub/repeated_timer.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scihub/scihub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scihub/cli/__init__.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scihub/cli/launch.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scihub/scibec/__init__.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scihub/scibec/config_handler.py
+-rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scihub/scibec/scibec_connector.py
+-rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scihub/scibec/scibec_metadata_handler.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scihub/scilog/__init__.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 bec_server-2.9.4/bec_server/scihub/scilog/scilog.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_bec_server_utils/test_main.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_bec_server_utils/test_service_handler.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_bec_server_utils/test_tmux_launch.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_data_processing/conftest.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_data_processing/test_dap_cli_launch.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_data_processing/test_dap_server.py
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_data_processing/test_dap_service_manager.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_data_processing/test_lmfit1d_service.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_device_server/conftest.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_device_server/test_config_handler.py
+-rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_device_server/test_device_manager_ds.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_device_server/test_device_serializer.py
+-rw-r--r--   0        0        0    28297 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_device_server/test_device_server.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_device_server/test_device_server_cli_launch.py
+-rw-r--r--   0        0        0     9555 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_device_server/test_rpc_mixin.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_file_writer/conftest.py
+-rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_file_writer/test_file_writer.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_file_writer/test_file_writer_cli_launch.py
+-rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_file_writer/test_file_writer_manager.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scan_bundler/conftest.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scan_bundler/test_bec_emitter.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scan_bundler/test_bluesky_emitter.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scan_bundler/test_emitter.py
+-rw-r--r--   0        0        0    25388 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scan_bundler/test_scan_bundler.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scan_server/conftest.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scan_server/test_path_optimization.py
+-rw-r--r--   0        0        0    11602 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scan_server/test_scan_guard.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scan_server/test_scan_server_cli_launch.py
+-rw-r--r--   0        0        0    26475 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scan_server/test_scan_server_queue.py
+-rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scan_server/test_scan_stubs.py
+-rw-r--r--   0        0        0    54003 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scan_server/test_scan_worker.py
+-rw-r--r--   0        0        0    87794 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scan_server/test_scans.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scihub/conftest.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scihub/test_repeated_timer.py
+-rw-r--r--   0        0        0    16951 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scihub/test_scibec_config_handler.py
+-rw-r--r--   0        0        0     5641 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scihub/test_scibec_connector.py
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scihub/test_scibec_metadata_handler.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scihub/test_scihub_cli_launch.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 bec_server-2.9.4/tests/tests_scihub/test_scilog_connector.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 bec_server-2.9.4/.gitignore
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 bec_server-2.9.4/pyproject.toml
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 bec_server-2.9.4/PKG-INFO
```

### Comparing `bec_server-2.9.3/bec_server/bec_server_utils/launch.py` & `bec_server-2.9.4/bec_server/bec_server_utils/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/bec_server_utils/service_handler.py` & `bec_server-2.9.4/bec_server/bec_server_utils/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/bec_server_utils/subprocess_launch.py` & `bec_server-2.9.4/bec_server/bec_server_utils/subprocess_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/bec_server_utils/tmux_launch.py` & `bec_server-2.9.4/bec_server/bec_server_utils/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/data_processing/dap_server.py` & `bec_server-2.9.4/bec_server/data_processing/dap_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/data_processing/dap_service.py` & `bec_server-2.9.4/bec_server/data_processing/dap_service.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/data_processing/dap_service_manager.py` & `bec_server-2.9.4/bec_server/data_processing/dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/data_processing/lmfit1d_service.py` & `bec_server-2.9.4/bec_server/data_processing/lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/data_processing/cli/launch.py` & `bec_server-2.9.4/bec_server/data_processing/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/device_server/device_server.py` & `bec_server-2.9.4/bec_server/device_server/device_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/device_server/rpc_mixin.py` & `bec_server-2.9.4/bec_server/device_server/rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/device_server/cli/launch.py` & `bec_server-2.9.4/bec_server/device_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/device_server/devices/config_update_handler.py` & `bec_server-2.9.4/bec_server/device_server/devices/config_update_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,16 @@
                     self.device_manager.update_config(device.obj, dev_config["deviceConfig"])
                 except Exception as exc:
                     self.device_manager.update_config(device.obj, old_config)
                     raise DeviceConfigError(f"Error during object update. {exc}")
 
                 if "limits" in dev_config["deviceConfig"]:
                     limits = {
-                        "low": device.obj.low_limit_travel.get(),
-                        "high": device.obj.high_limit_travel.get(),
+                        "low": {"value": device.obj.low_limit_travel.get()},
+                        "high": {"value": device.obj.high_limit_travel.get()},
                     }
                     self.device_manager.connector.set_and_publish(
                         MessageEndpoints.device_limits(device.name),
                         messages.DeviceMessage(signals=limits),
                     )
 
             if "enabled" in dev_config:
```

### Comparing `bec_server-2.9.3/bec_server/device_server/devices/device_serializer.py` & `bec_server-2.9.4/bec_server/device_server/devices/device_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/device_server/devices/devicemanager.py` & `bec_server-2.9.4/bec_server/device_server/devices/devicemanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,16 @@
 
     def initialize_device_buffer(self, connector):
         """initialize the device read and readback buffer on redis with a new reading"""
         dev_msg = messages.DeviceMessage(signals=self.obj.read(), metadata={})
         dev_config_msg = messages.DeviceMessage(signals=self.obj.read_configuration(), metadata={})
         if hasattr(self.obj, "low_limit_travel") and hasattr(self.obj, "high_limit_travel"):
             limits = {
-                "low": self.obj.low_limit_travel.get(),
-                "high": self.obj.high_limit_travel.get(),
+                "low": {"value": self.obj.low_limit_travel.get()},
+                "high": {"value": self.obj.high_limit_travel.get()},
             }
         else:
             limits = None
         pipe = connector.pipeline()
         connector.set_and_publish(MessageEndpoints.device_readback(self.name), dev_msg, pipe=pipe)
         connector.set_and_publish(
             topic=MessageEndpoints.device_read(self.name), msg=dev_msg, pipe=pipe
@@ -527,17 +527,15 @@
         bundle = messages.BundleMessage()
         for ii in range(emitted_points, max_points):
             timestamp = time.time()
             signals = {}
             for key, val in data.items():
                 signals[key] = {"value": val[ii], "timestamp": timestamp}
             bundle.append(
-                messages.DeviceMessage(
-                    signals={obj.name: signals}, metadata={"point_id": ii, **metadata}
-                )
+                messages.DeviceMessage(signals=signals, metadata={"point_id": ii, **metadata})
             )
         ds_obj.emitted_points[metadata["scan_id"]] = max_points
         pipe = self.connector.pipeline()
         self.connector.send(MessageEndpoints.device_read(obj.root.name), bundle, pipe=pipe)
         msg = messages.DeviceStatusMessage(
             device=obj.root.name, status=max_points, metadata=metadata
         )
```

### Comparing `bec_server-2.9.3/bec_server/device_server/tests/utils.py` & `bec_server-2.9.4/bec_server/device_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/file_writer/default_writer.py` & `bec_server-2.9.4/bec_server/file_writer/default_writer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/file_writer/file_writer.py` & `bec_server-2.9.4/bec_server/file_writer/file_writer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/file_writer/file_writer_manager.py` & `bec_server-2.9.4/bec_server/file_writer/file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/file_writer/merged_dicts.py` & `bec_server-2.9.4/bec_server/file_writer/merged_dicts.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/file_writer/cli/launch.py` & `bec_server-2.9.4/bec_server/file_writer/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/file_writer_plugins/cSAXS.py` & `bec_server-2.9.4/bec_server/file_writer_plugins/cSAXS.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_bundler/bec_emitter.py` & `bec_server-2.9.4/bec_server/scan_bundler/bec_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_bundler/bluesky_emitter.py` & `bec_server-2.9.4/bec_server/scan_bundler/bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_bundler/emitter.py` & `bec_server-2.9.4/bec_server/scan_bundler/emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_bundler/scan_bundler.py` & `bec_server-2.9.4/bec_server/scan_bundler/scan_bundler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_bundler/cli/launch.py` & `bec_server-2.9.4/bec_server/scan_bundler/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_server/device_validation.py` & `bec_server-2.9.4/bec_server/scan_server/device_validation.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_server/path_optimization.py` & `bec_server-2.9.4/bec_server/scan_server/path_optimization.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_server/scan_assembler.py` & `bec_server-2.9.4/bec_server/scan_server/scan_assembler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_server/scan_guard.py` & `bec_server-2.9.4/bec_server/scan_server/scan_guard.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_server/scan_manager.py` & `bec_server-2.9.4/bec_server/scan_server/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_server/scan_queue.py` & `bec_server-2.9.4/bec_server/scan_server/scan_queue.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_server/scan_server.py` & `bec_server-2.9.4/bec_server/scan_server/scan_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_server/scan_stubs.py` & `bec_server-2.9.4/bec_server/scan_server/scan_stubs.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,15 +394,15 @@
         Returns:
             Generator[None, None, None]: Generator that yields a device message.
         """
         metadata = {"point_id": point_id}
         yield self._device_msg(
             device=device,
             action="publish_data_as_read",
-            parameter={"data": {device: data}},
+            parameter={"data": data},
             metadata=metadata,
         )
 
     def trigger(self, *, group: str, point_id: int) -> Generator[None, None, None]:
         """Trigger a device group
 
         Args:
```

### Comparing `bec_server-2.9.3/bec_server/scan_server/scan_worker.py` & `bec_server-2.9.4/bec_server/scan_server/scan_worker.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_server/scans.py` & `bec_server-2.9.4/bec_server/scan_server/scans.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_server/cli/launch.py` & `bec_server-2.9.4/bec_server/scan_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_server/scan_plugins/otf_scan.py` & `bec_server-2.9.4/bec_server/scan_server/scan_plugins/otf_scan.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scan_server/tests/utils.py` & `bec_server-2.9.4/bec_server/scan_server/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scihub/repeated_timer.py` & `bec_server-2.9.4/bec_server/scihub/repeated_timer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scihub/scihub.py` & `bec_server-2.9.4/bec_server/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scihub/cli/launch.py` & `bec_server-2.9.4/bec_server/scihub/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scihub/scibec/config_handler.py` & `bec_server-2.9.4/bec_server/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scihub/scibec/scibec_connector.py` & `bec_server-2.9.4/bec_server/scihub/scibec/scibec_connector.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scihub/scibec/scibec_metadata_handler.py` & `bec_server-2.9.4/bec_server/scihub/scibec/scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/bec_server/scihub/scilog/scilog.py` & `bec_server-2.9.4/bec_server/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_bec_server_utils/test_main.py` & `bec_server-2.9.4/tests/tests_bec_server_utils/test_main.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_bec_server_utils/test_service_handler.py` & `bec_server-2.9.4/tests/tests_bec_server_utils/test_service_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_bec_server_utils/test_tmux_launch.py` & `bec_server-2.9.4/tests/tests_bec_server_utils/test_tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_data_processing/test_dap_cli_launch.py` & `bec_server-2.9.4/tests/tests_data_processing/test_dap_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_data_processing/test_dap_service_manager.py` & `bec_server-2.9.4/tests/tests_data_processing/test_dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_data_processing/test_lmfit1d_service.py` & `bec_server-2.9.4/tests/tests_data_processing/test_lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_device_server/conftest.py` & `bec_server-2.9.4/tests/tests_device_server/conftest.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_device_server/test_config_handler.py` & `bec_server-2.9.4/tests/tests_device_server/test_config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_device_server/test_device_manager_ds.py` & `bec_server-2.9.4/tests/tests_device_server/test_device_manager_ds.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_device_server/test_device_serializer.py` & `bec_server-2.9.4/tests/tests_device_server/test_device_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_device_server/test_device_server.py` & `bec_server-2.9.4/tests/tests_device_server/test_device_server.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_device_server/test_device_server_cli_launch.py` & `bec_server-2.9.4/tests/tests_device_server/test_device_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_device_server/test_rpc_mixin.py` & `bec_server-2.9.4/tests/tests_device_server/test_rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_file_writer/test_file_writer.py` & `bec_server-2.9.4/tests/tests_file_writer/test_file_writer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_file_writer/test_file_writer_cli_launch.py` & `bec_server-2.9.4/tests/tests_file_writer/test_file_writer_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_file_writer/test_file_writer_manager.py` & `bec_server-2.9.4/tests/tests_file_writer/test_file_writer_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 # pylint: skip-file
-import contextlib
 import os
 from unittest import mock
 
 import numpy as np
 import pytest
-import yaml
 
 import bec_lib
-from bec_lib import DeviceManagerBase, MessageEndpoints, ServiceConfig, messages
+from bec_lib import MessageEndpoints, ServiceConfig, messages
 from bec_lib.logger import bec_logger
-from bec_lib.messages import BECStatus
 from bec_lib.redis_connector import MessageObject
 from bec_lib.tests.utils import ConnectorMock
 from bec_server.file_writer import FileWriterManager
 from bec_server.file_writer.file_writer import FileWriter
 from bec_server.file_writer.file_writer_manager import ScanStorage
 
 # pylint: disable=missing-function-docstring
@@ -29,17 +26,18 @@
     config = ServiceConfig(
         redis={"host": "dummy", "port": 6379},
         config={
             "file_writer": {"plugin": "default_NeXus_format", "base_path": "./"},
             "log_writer": {"base_path": "./"},
         },
     )
-    with mock.patch.object(
-        FileWriterManager, "_start_device_manager", return_value=None
-    ), mock.patch.object(FileWriterManager, "wait_for_service"):
+    with (
+        mock.patch.object(FileWriterManager, "_start_device_manager", return_value=None),
+        mock.patch.object(FileWriterManager, "wait_for_service"),
+    ):
         file_writer_manager_mock = FileWriterManager(config=config, connector_cls=connector_cls)
         try:
             yield file_writer_manager_mock
         finally:
             file_writer_manager_mock.shutdown()
             bec_logger.logger.remove()
             bec_logger._reset_singleton()
@@ -191,18 +189,18 @@
             mock_connector.xrange.assert_called_once_with(key, min="-", max="+")
             mock_process.assert_called_once_with(data, "scan_id", "dev1")
 
 
 def test_process_async_data_single_entry(file_writer_manager_mock):
     file_manager = file_writer_manager_mock
     file_manager.scan_storage["scan_id"] = ScanStorage(10, "scan_id")
-    data = [{"data": messages.DeviceMessage(signals={"data": np.zeros((10, 10))})}]
+    data = [{"data": messages.DeviceMessage(signals={"data": {"value": np.zeros((10, 10))}})}]
     file_manager._process_async_data(data, "scan_id", "dev1")
     assert np.isclose(
-        file_manager.scan_storage["scan_id"].async_data["dev1"]["data"], np.zeros((10, 10))
+        file_manager.scan_storage["scan_id"].async_data["dev1"]["data"]["value"], np.zeros((10, 10))
     ).all()
 
 
 def test_process_async_data_extend(file_writer_manager_mock):
     file_manager = file_writer_manager_mock
     file_manager.scan_storage["scan_id"] = ScanStorage(10, "scan_id")
     data = [
```

### Comparing `bec_server-2.9.3/tests/tests_scan_bundler/conftest.py` & `bec_server-2.9.4/tests/tests_scan_bundler/conftest.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scan_bundler/test_bec_emitter.py` & `bec_server-2.9.4/tests/tests_scan_bundler/test_bec_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scan_bundler/test_bluesky_emitter.py` & `bec_server-2.9.4/tests/tests_scan_bundler/test_bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scan_bundler/test_emitter.py` & `bec_server-2.9.4/tests/tests_scan_bundler/test_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scan_bundler/test_scan_bundler.py` & `bec_server-2.9.4/tests/tests_scan_bundler/test_scan_bundler.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,32 @@
 from bec_lib import MessageEndpoints, messages
 from bec_lib.connector import MessageObject
 
 # pylint: disable=missing-function-docstring
 # pylint: disable=protected-access
 
 
-def test_device_read_callback(scan_bundler_mock):
+@pytest.fixture()
+def dummy_signal_data():
+    return {
+        "samx": {"value": 0.51, "timestamp": 1234.56},
+        "samx_setpoint": {"value": 0.51, "timestamp": 1234.56},
+    }
+
+
+@pytest.fixture()
+def dummy_device_data_message(dummy_signal_data):
+    return messages.DeviceMessage(
+        signals=dummy_signal_data, metadata={"scan_id": "scan_id", "readout_priority": "monitored"}
+    )
+
+
+def test_device_read_callback(scan_bundler_mock, dummy_signal_data):
     dev_msg = messages.DeviceMessage(
-        signals={"samx": {"samx": 0.51, "setpoint": 0.5, "motor_is_moving": 0}},
-        metadata={"scan_id": "laksjd", "readout_priority": "monitored"},
+        signals=dummy_signal_data, metadata={"scan_id": "laksjd", "readout_priority": "monitored"}
     )
     msg = MessageObject(MessageEndpoints.device_read("samx").endpoint, dev_msg)
 
     with mock.patch.object(scan_bundler_mock, "_add_device_to_storage") as add_dev:
         scan_bundler_mock._device_read_callback(msg)
         add_dev.assert_called_once_with([dev_msg], "samx")
 
@@ -64,18 +78,17 @@
         if not storageID and not scan_msg:
             with pytest.raises(TimeoutError):
                 sb._wait_for_scan_id(scan_id, 1)
             return
         sb._wait_for_scan_id(scan_id)
 
 
-def test_add_device_to_storage_returns_without_scan_id(scan_bundler_mock):
+def test_add_device_to_storage_returns_without_scan_id(scan_bundler_mock, dummy_signal_data):
     msg = messages.DeviceMessage(
-        signals={"samx": {"samx": 0.51, "setpoint": 0.5, "motor_is_moving": 0}},
-        metadata={"readout_priority": "monitored"},
+        signals=dummy_signal_data, metadata={"readout_priority": "monitored"}
     )
     sb = scan_bundler_mock
     sb._add_device_to_storage([msg], "samx", timeout_time=1)
     assert "samx" not in sb.device_storage
 
 
 def test_add_device_to_storage_returns_without_signal(scan_bundler_mock):
@@ -83,64 +96,47 @@
         signals={}, metadata={"scan_id": "scan_id", "readout_priority": "monitored"}
     )
     sb = scan_bundler_mock
     sb._add_device_to_storage([msg], "samx", timeout_time=1)
     assert "samx" not in sb.device_storage
 
 
-def test_add_device_to_storage_returns_on_timeout(scan_bundler_mock):
+def test_add_device_to_storage_returns_on_timeout(scan_bundler_mock, dummy_signal_data):
     msg = messages.DeviceMessage(
-        signals={"samx": {"samx": 0.51, "setpoint": 0.5, "motor_is_moving": 0}},
-        metadata={"scan_id": "scan_id", "readout_priority": "monitored"},
+        signals=dummy_signal_data, metadata={"scan_id": "scan_id", "readout_priority": "monitored"}
     )
     sb = scan_bundler_mock
     sb._add_device_to_storage([msg], "samx", timeout_time=1)
     assert "samx" not in sb.device_storage
 
 
 @pytest.mark.parametrize("scan_status", ["aborted", "closed"])
-def test_add_device_to_storage_returns_without_scan_info(scan_bundler_mock, scan_status):
+def test_add_device_to_storage_returns_without_scan_info(
+    scan_bundler_mock, scan_status, dummy_signal_data
+):
     msg = messages.DeviceMessage(
-        signals={"samx": {"samx": 0.51, "setpoint": 0.5, "motor_is_moving": 0}},
-        metadata={"scan_id": "scan_id", "readout_priority": "monitored"},
+        signals=dummy_signal_data, metadata={"scan_id": "scan_id", "readout_priority": "monitored"}
     )
     sb = scan_bundler_mock
     sb.sync_storage["scan_id"] = {"info": {}}
     sb.sync_storage["scan_id"]["status"] = scan_status
     sb._add_device_to_storage([msg], "samx", timeout_time=1)
     assert "samx" not in sb.device_storage
 
 
 @pytest.mark.parametrize(
     "msg,scan_type",
     [
-        (
-            messages.DeviceMessage(
-                signals={"samx": {"samx": 0.51, "setpoint": 0.5, "motor_is_moving": 0}},
-                metadata={"scan_id": "scan_id", "readout_priority": "monitored"},
-            ),
-            "step",
-        ),
-        (
-            messages.DeviceMessage(
-                signals={"samx": {"samx": 0.51, "setpoint": 0.5, "motor_is_moving": 0}},
-                metadata={"scan_id": "scan_id", "readout_priority": "monitored"},
-            ),
-            "fly",
-        ),
-        (
-            messages.DeviceMessage(
-                signals={"samx": {"samx": 0.51, "setpoint": 0.5, "motor_is_moving": 0}},
-                metadata={"scan_id": "scan_id", "readout_priority": "monitored"},
-            ),
-            "wrong",
-        ),
+        ("dummy_device_data_message", "step"),
+        ("dummy_device_data_message", "fly"),
+        ("dummy_device_data_message", "wrong"),
     ],
 )
-def test_add_device_to_storage_primary(scan_bundler_mock, msg, scan_type):
+def test_add_device_to_storage_primary(scan_bundler_mock, msg, scan_type, request):
+    msg = request.getfixturevalue(msg)
     sb = scan_bundler_mock
     sb.sync_storage["scan_id"] = {"info": {"scan_type": scan_type, "monitor_sync": "bec"}}
     sb.sync_storage["scan_id"]["status"] = "open"
     sb.monitored_devices["scan_id"] = {"devices": [sb.device_manager.devices.samx]}
     sb.storage_initialized.add("scan_id")
     if scan_type == "step":
         with mock.patch.object(sb, "_step_scan_update") as step_update:
@@ -161,23 +157,29 @@
 
 
 @pytest.mark.parametrize(
     "msg,scan_type",
     [
         (
             messages.DeviceMessage(
-                signals={"samx": {"samx": 0.51, "setpoint": 0.5, "motor_is_moving": 0}},
+                signals={
+                    "samx": {"value": 0.51},
+                    "setpoint": {"value": 0.5},
+                    "motor_is_moving": {"value": 0},
+                },
                 metadata={"scan_id": "scan_id"},
             ),
             "fly",
         ),
         (
             messages.DeviceMessage(
                 signals={
-                    "flyer": {"flyer": 0.51, "flyer_setpoint": 0.5, "flyer_motor_is_moving": 0}
+                    "flyer": {"value": 0.51},
+                    "flyer_setpoint": {"value": 0.5},
+                    "flyer_motor_is_moving": {"value": 0},
                 },
                 metadata={"scan_id": "scan_id"},
             ),
             "fly",
         ),
     ],
 )
@@ -200,15 +202,19 @@
 
 
 @pytest.mark.parametrize(
     "msg,scan_type",
     [
         (
             messages.DeviceMessage(
-                signals={"samx": {"samx": 0.51, "setpoint": 0.5, "motor_is_moving": 0}},
+                signals={
+                    "samx": {"value": 0.51},
+                    "setpoint": {"value": 0.5},
+                    "motor_is_moving": {"value": 0},
+                },
                 metadata={"scan_id": "scan_id", "readout_priority": "baseline"},
             ),
             "step",
         )
     ],
 )
 def test_add_device_to_storage_baseline(scan_bundler_mock, msg, scan_type):
@@ -398,15 +404,14 @@
 @pytest.mark.parametrize(
     "scan_msg",
     [
         messages.ScanStatusMessage(
             scan_id="6ff7a89a-79e5-43ad-828b-c1e1aeed5803",
             status="closed",
             info={
-                "readout_priority": "monitored",
                 "DIID": 4,
                 "RID": "a53538b4-79f3-4132-91b5-d044e438f460",
                 "scan_id": "3ea07f69-b0ee-44fa-8451-b85824a37397",
                 "queue_id": "84e5bc19-e2fc-4b03-b706-004420322813",
                 "scan_number": 5,
                 "scan_motors": ["samx", "samy"],
                 "readout_priority": {
@@ -417,15 +422,14 @@
                 "num_points": 143,
             },
         ),
         messages.ScanStatusMessage(
             scan_id="6ff7a89a-79e5-43ad-828b-c1e1aeed5803",
             status="open",
             info={
-                "readout_priority": "monitored",
                 "DIID": 4,
                 "RID": "a53538b4-79f3-4132-91b5-d044e438f460",
                 "scan_id": "3ea07f69-b0ee-44fa-8451-b85824a37397",
                 "queue_id": "84e5bc19-e2fc-4b03-b706-004420322813",
                 "scan_number": 5,
                 "scan_motors": ["samx", "samy", "eyex", "bpm3a"],
                 "readout_priority": {
@@ -472,39 +476,39 @@
 
 
 @pytest.mark.parametrize(
     "scan_msg, point_id, primary",
     [
         [
             messages.DeviceMessage(
-                signals={"samx": {"samx": 0.51, "setpoint": 0.5, "motor_is_moving": 0}},
+                signals={"samx": {"value": 0.51, "timestamp": 1234.56}},
                 metadata={
                     "scan_id": "adlk-jalskdja",
                     "readout_priority": "monitored",
                     "point_id": 23,
                 },
             ),
             23,
             True,
         ],
         [
             messages.DeviceMessage(
-                signals={"samx": {"samx": 0.51, "setpoint": 0.5, "motor_is_moving": 0}},
+                signals={"samx": {"value": 0.51, "timestamp": 1234.56}},
                 metadata={
                     "scan_id": "adlk-jalskdjb",
                     "readout_priority": "monitored",
                     "point_id": 23,
                 },
             ),
             23,
             False,
         ],
         [
             messages.DeviceMessage(
-                signals={"samx": {"samx": 0.51, "setpoint": 0.5, "motor_is_moving": 0}},
+                signals={"samx": {"value": 0.51, "timestamp": 1234.56}},
                 metadata={"scan_id": "adlk-jalskdjc", "readout_priority": "monitored"},
             ),
             23,
             False,
         ],
     ],
 )
@@ -648,15 +652,19 @@
         sb._update_monitor_signals(scan_id, point_id)
         assert sb.sync_storage[scan_id][point_id]["bpm3a"] == {"value": 400}
 
 
 def test_get_last_device_readback(scan_bundler_mock):
     sb = scan_bundler_mock
     dev_msg = messages.DeviceMessage(
-        signals={"samx": {"samx": 0.51, "setpoint": 0.5, "motor_is_moving": 0}},
+        signals={
+            "samx": {"value": 0.51},
+            "setpoint": {"value": 0.5},
+            "motor_is_moving": {"value": 0},
+        },
         metadata={"scan_id": "laksjd", "readout_priority": "monitored"},
     )
     with mock.patch.object(sb, "connector") as connector_mock:
         connector_mock.execute_pipeline.return_value = [dev_msg]
         ret = sb._get_last_device_readback([sb.device_manager.devices.samx])
         assert connector_mock.get.mock_calls == [
             mock.call(MessageEndpoints.device_readback("samx"), connector_mock.pipeline())
```

### Comparing `bec_server-2.9.3/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py` & `bec_server-2.9.4/tests/tests_scan_bundler/test_scan_bundler_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scan_server/test_path_optimization.py` & `bec_server-2.9.4/tests/tests_scan_server/test_path_optimization.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scan_server/test_scan_guard.py` & `bec_server-2.9.4/tests/tests_scan_server/test_scan_guard.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scan_server/test_scan_server_cli_launch.py` & `bec_server-2.9.4/tests/tests_scan_server/test_scan_server_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scan_server/test_scan_server_queue.py` & `bec_server-2.9.4/tests/tests_scan_server/test_scan_server_queue.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scan_server/test_scan_stubs.py` & `bec_server-2.9.4/tests/tests_scan_server/test_scan_stubs.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scan_server/test_scan_worker.py` & `bec_server-2.9.4/tests/tests_scan_server/test_scan_worker.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scan_server/test_scans.py` & `bec_server-2.9.4/tests/tests_scan_server/test_scans.py`

 * *Files 0% similar despite different names*

```diff
@@ -1949,15 +1949,15 @@
                         action="set",
                         parameter={"value": 5, "wait_group": "scan_motor"},
                         metadata={"readout_priority": "monitored", "DIID": 10, "response": True},
                     ),
                     messages.DeviceInstructionMessage(
                         device="samx",
                         action="publish_data_as_read",
-                        parameter={"data": {"samx": {"rb1": {"value": 1}}}},
+                        parameter={"data": {"rb1": {"value": 1}}},
                         metadata={"readout_priority": "monitored", "DIID": 11, "point_id": 0},
                     ),
                     messages.DeviceInstructionMessage(
                         device="samx",
                         action="set",
                         parameter={"value": 0, "wait_group": "scan_motor"},
                         metadata={"readout_priority": "monitored", "DIID": 12},
```

### Comparing `bec_server-2.9.3/tests/tests_scihub/test_repeated_timer.py` & `bec_server-2.9.4/tests/tests_scihub/test_repeated_timer.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scihub/test_scibec_config_handler.py` & `bec_server-2.9.4/tests/tests_scihub/test_scibec_config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scihub/test_scibec_connector.py` & `bec_server-2.9.4/tests/tests_scihub/test_scibec_connector.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scihub/test_scibec_metadata_handler.py` & `bec_server-2.9.4/tests/tests_scihub/test_scibec_metadata_handler.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scihub/test_scihub_cli_launch.py` & `bec_server-2.9.4/tests/tests_scihub/test_scihub_cli_launch.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/tests/tests_scihub/test_scilog_connector.py` & `bec_server-2.9.4/tests/tests_scihub/test_scilog_connector.py`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/.gitignore` & `bec_server-2.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bec_server-2.9.3/pyproject.toml` & `bec_server-2.9.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bec-server"
-version = "2.9.3"
+version = "2.9.4"
 description = "BEC server"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
@@ -56,7 +56,14 @@
 
 [tool.hatch.build.targets.wheel]
 include = ["*"]
 
 [tool.black]
 line-length = 100
 skip-magic-trailing-comma = true
+
+[tool.isort]
+profile = "black"
+line_length = 100
+multi_line_output = 3
+include_trailing_comma = true
+known_first_party = ["bec_lib", "bec_server", "bec_ipython_client"]
```

### Comparing `bec_server-2.9.3/PKG-INFO` & `bec_server-2.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bec-server
-Version: 2.9.3
+Version: 2.9.4
 Summary: BEC server
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Project-URL: Homepage, https://gitlab.psi.ch/bec/bec
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
```

