# Comparing `tmp/assemblyline-core-4.5.1.dev98.tar.gz` & `tmp/assemblyline-core-4.5.1.dev99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyline-core-4.5.1.dev98.tar", last modified: Mon Apr 22 20:02:58 2024, max compression
+gzip compressed data, was "assemblyline-core-4.5.1.dev99.tar", last modified: Mon Apr 22 20:21:23 2024, max compression
```

## Comparing `assemblyline-core-4.5.1.dev98.tar` & `assemblyline-core-4.5.1.dev99.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.224266 assemblyline-core-4.5.1.dev98/
--rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/LICENCE.md
--rw-r--r--   0 vsts      (1001) docker     (127)     1814 2024-04-22 20:02:58.224266 assemblyline-core-4.5.1.dev98/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.192266 assemblyline-core-4.5.1.dev98/assemblyline_core/
--rw-r--r--   0 vsts      (1001) docker     (127)       12 2024-04-22 20:02:55.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/VERSION
--rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.200266 assemblyline-core-4.5.1.dev98/assemblyline_core/alerter/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/alerter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15813 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/alerter/processing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4964 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/alerter/run_alerter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.200266 assemblyline-core-4.5.1.dev98/assemblyline_core/archiver/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/archiver/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9179 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/archiver/run_archiver.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10237 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/badlist_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.208266 assemblyline-core-4.5.1.dev98/assemblyline_core/dispatching/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/dispatching/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      122 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/dispatching/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17216 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/dispatching/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    94587 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/dispatching/dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7403 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/dispatching/schedules.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/dispatching/timeout.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.208266 assemblyline-core-4.5.1.dev98/assemblyline_core/expiry/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/expiry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14062 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/expiry/run_expiry.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.208266 assemblyline-core-4.5.1.dev98/assemblyline_core/ingester/
--rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/ingester/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/ingester/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      190 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/ingester/constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39214 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/ingester/ingester.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.208266 assemblyline-core-4.5.1.dev98/assemblyline_core/metrics/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/metrics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30865 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/metrics/es_metrics.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16277 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/metrics/heartbeat_formatter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7559 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/metrics/helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20026 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/metrics/metrics_server.py
--rw-r--r--   0 vsts      (1001) docker     (127)      256 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/metrics/run_heartbeat_manager.py
--rw-r--r--   0 vsts      (1001) docker     (127)      250 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/metrics/run_metrics_aggregator.py
--rw-r--r--   0 vsts      (1001) docker     (127)      274 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/metrics/run_statistics_aggregator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.212266 assemblyline-core-4.5.1.dev98/assemblyline_core/plumber/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/plumber/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9534 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/plumber/run_plumber.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.212266 assemblyline-core-4.5.1.dev98/assemblyline_core/replay/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/replay/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18908 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/replay/client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.212266 assemblyline-core-4.5.1.dev98/assemblyline_core/replay/creator/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/replay/creator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2899 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/replay/creator/run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7790 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/replay/creator/run_worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.212266 assemblyline-core-4.5.1.dev98/assemblyline_core/replay/loader/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/replay/loader/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3564 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/replay/loader/run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3183 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/replay/loader/run_worker.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2577 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/replay/replay.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10914 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/safelist_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.212266 assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/collection.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.212266 assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/controllers/
--rw-r--r--   0 vsts      (1001) docker     (127)       90 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/controllers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24747 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/controllers/docker_ctl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2462 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/controllers/interface.py
--rw-r--r--   0 vsts      (1001) docker     (127)    65957 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/controllers/kubernetes_ctl.py
--rw-r--r--   0 vsts      (1001) docker     (127)      160 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/run_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49873 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/scaler_server.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12219 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/server_base.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10044 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/signature_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10982 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/submission_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23620 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/tasking_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.212266 assemblyline-core-4.5.1.dev98/assemblyline_core/updater/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/updater/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10044 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/updater/helper.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34206 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/updater/run_updater.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.220266 assemblyline-core-4.5.1.dev98/assemblyline_core/vacuum/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/vacuum/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5628 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/vacuum/crawler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/vacuum/department_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3478 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/vacuum/safelist.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/vacuum/stream_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29885 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/vacuum/worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.220266 assemblyline-core-4.5.1.dev98/assemblyline_core/workflow/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10391 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/assemblyline_core/workflow/run_workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.200266 assemblyline-core-4.5.1.dev98/assemblyline_core.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1814 2024-04-22 20:02:58.000000 assemblyline-core-4.5.1.dev98/assemblyline_core.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-04-22 20:02:58.000000 assemblyline-core-4.5.1.dev98/assemblyline_core.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-22 20:02:58.000000 assemblyline-core-4.5.1.dev98/assemblyline_core.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-04-22 20:02:58.000000 assemblyline-core-4.5.1.dev98/assemblyline_core.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-04-22 20:02:58.000000 assemblyline-core-4.5.1.dev98/assemblyline_core.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-22 20:02:58.224266 assemblyline-core-4.5.1.dev98/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     2020 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:02:58.224266 assemblyline-core-4.5.1.dev98/test/
--rw-r--r--   0 vsts      (1001) docker     (127)     5768 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/test/test_alerter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8754 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/test/test_badlist_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15228 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/test/test_dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2043 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/test/test_expiry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/test/test_plumber.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10842 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/test/test_replay.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9751 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/test/test_safelist_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2006 2024-04-22 20:02:43.000000 assemblyline-core-4.5.1.dev98/test/test_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5380 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/test/test_scheduler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3563 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/test/test_signature_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46102 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/test/test_simulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4419 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/test/test_vacuum.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6792 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/test/test_worker_ingest.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4780 2024-04-22 20:02:44.000000 assemblyline-core-4.5.1.dev98/test/test_worker_submit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.062404 assemblyline-core-4.5.1.dev99/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1396 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/LICENCE.md
+-rw-r--r--   0 vsts      (1001) docker     (127)     1814 2024-04-22 20:21:23.062404 assemblyline-core-4.5.1.dev99/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      860 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.022401 assemblyline-core-4.5.1.dev99/assemblyline_core/
+-rw-r--r--   0 vsts      (1001) docker     (127)       12 2024-04-22 20:21:16.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/VERSION
+-rw-r--r--   0 vsts      (1001) docker     (127)       49 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.022401 assemblyline-core-4.5.1.dev99/assemblyline_core/alerter/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/alerter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15813 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/alerter/processing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4964 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/alerter/run_alerter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.022401 assemblyline-core-4.5.1.dev99/assemblyline_core/archiver/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/archiver/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9179 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/archiver/run_archiver.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10237 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/badlist_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.022401 assemblyline-core-4.5.1.dev99/assemblyline_core/dispatching/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/dispatching/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      122 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/dispatching/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17216 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/dispatching/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    94587 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/dispatching/dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7403 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/dispatching/schedules.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2050 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/dispatching/timeout.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.034402 assemblyline-core-4.5.1.dev99/assemblyline_core/expiry/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/expiry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14062 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/expiry/run_expiry.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.038402 assemblyline-core-4.5.1.dev99/assemblyline_core/ingester/
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/ingester/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/ingester/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      190 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/ingester/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39214 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/ingester/ingester.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.042402 assemblyline-core-4.5.1.dev99/assemblyline_core/metrics/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/metrics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30865 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/metrics/es_metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16277 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/metrics/heartbeat_formatter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7559 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/metrics/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20026 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/metrics/metrics_server.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      256 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/metrics/run_heartbeat_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      250 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/metrics/run_metrics_aggregator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      274 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/metrics/run_statistics_aggregator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.042402 assemblyline-core-4.5.1.dev99/assemblyline_core/plumber/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/plumber/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9534 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/plumber/run_plumber.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.042402 assemblyline-core-4.5.1.dev99/assemblyline_core/replay/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/replay/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18908 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/replay/client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.046402 assemblyline-core-4.5.1.dev99/assemblyline_core/replay/creator/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/replay/creator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2899 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/replay/creator/run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7790 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/replay/creator/run_worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.046402 assemblyline-core-4.5.1.dev99/assemblyline_core/replay/loader/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/replay/loader/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3564 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/replay/loader/run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3183 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/replay/loader/run_worker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2577 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/replay/replay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10914 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/safelist_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.046402 assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1858 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/collection.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.050403 assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/controllers/
+-rw-r--r--   0 vsts      (1001) docker     (127)       90 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/controllers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24747 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/controllers/docker_ctl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2462 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/controllers/interface.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    65957 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/controllers/kubernetes_ctl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      160 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/run_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49873 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/scaler_server.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12219 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/server_base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10044 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/signature_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10982 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/submission_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23620 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/tasking_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.054403 assemblyline-core-4.5.1.dev99/assemblyline_core/updater/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/updater/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10044 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/updater/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34206 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/updater/run_updater.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.058403 assemblyline-core-4.5.1.dev99/assemblyline_core/vacuum/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/vacuum/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5628 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/vacuum/crawler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/vacuum/department_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3478 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/vacuum/safelist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/vacuum/stream_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29885 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/vacuum/worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.058403 assemblyline-core-4.5.1.dev99/assemblyline_core/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10391 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/assemblyline_core/workflow/run_workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.022401 assemblyline-core-4.5.1.dev99/assemblyline_core.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1814 2024-04-22 20:21:22.000000 assemblyline-core-4.5.1.dev99/assemblyline_core.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3136 2024-04-22 20:21:23.000000 assemblyline-core-4.5.1.dev99/assemblyline_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-22 20:21:22.000000 assemblyline-core-4.5.1.dev99/assemblyline_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-04-22 20:21:22.000000 assemblyline-core-4.5.1.dev99/assemblyline_core.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-04-22 20:21:22.000000 assemblyline-core-4.5.1.dev99/assemblyline_core.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-22 20:21:23.062404 assemblyline-core-4.5.1.dev99/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     2020 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-22 20:21:23.062404 assemblyline-core-4.5.1.dev99/test/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5768 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/test/test_alerter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8754 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/test/test_badlist_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15228 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/test/test_dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2043 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/test/test_expiry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/test/test_plumber.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10842 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/test/test_replay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9751 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/test/test_safelist_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2006 2024-04-22 20:20:59.000000 assemblyline-core-4.5.1.dev99/test/test_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5380 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/test/test_scheduler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3563 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/test/test_signature_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46102 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/test/test_simulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4419 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/test/test_vacuum.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6792 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/test/test_worker_ingest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4780 2024-04-22 20:21:00.000000 assemblyline-core-4.5.1.dev99/test/test_worker_submit.py
```

### Comparing `assemblyline-core-4.5.1.dev98/LICENCE.md` & `assemblyline-core-4.5.1.dev99/LICENCE.md`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/PKG-INFO` & `assemblyline-core-4.5.1.dev99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-core
-Version: 4.5.1.dev98
+Version: 4.5.1.dev99
 Summary: Assemblyline 4 - Core components
 Home-page: https://github.com/CybercentreCanada/assemblyline-core/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `assemblyline-core-4.5.1.dev98/README.md` & `assemblyline-core-4.5.1.dev99/README.md`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/alerter/processing.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/alerter/processing.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/alerter/run_alerter.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/alerter/run_alerter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/archiver/run_archiver.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/archiver/run_archiver.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/badlist_client.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/badlist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/dispatching/client.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/dispatching/client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/dispatching/dispatcher.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/dispatching/dispatcher.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/dispatching/schedules.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/dispatching/schedules.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/dispatching/timeout.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/dispatching/timeout.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/expiry/run_expiry.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/expiry/run_expiry.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/ingester/ingester.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/ingester/ingester.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/metrics/es_metrics.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/metrics/es_metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/metrics/heartbeat_formatter.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/metrics/heartbeat_formatter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/metrics/helper.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/metrics/helper.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/metrics/metrics_server.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/metrics/metrics_server.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/plumber/run_plumber.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/plumber/run_plumber.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/replay/client.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/replay/client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/replay/creator/run.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/replay/creator/run.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/replay/creator/run_worker.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/replay/creator/run_worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/replay/loader/run.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/replay/loader/run.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/replay/loader/run_worker.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/replay/loader/run_worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/replay/replay.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/replay/replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/safelist_client.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/safelist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/collection.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/collection.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/controllers/docker_ctl.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/controllers/docker_ctl.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/controllers/interface.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/controllers/interface.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/controllers/kubernetes_ctl.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/controllers/kubernetes_ctl.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/scaler/scaler_server.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/scaler/scaler_server.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/server_base.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/server_base.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/signature_client.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/signature_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/submission_client.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/submission_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/tasking_client.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/tasking_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/updater/helper.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/updater/helper.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/updater/run_updater.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/updater/run_updater.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/vacuum/crawler.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/vacuum/crawler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/vacuum/department_map.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/vacuum/department_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/vacuum/safelist.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/vacuum/safelist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/vacuum/stream_map.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/vacuum/stream_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/vacuum/worker.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/vacuum/worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core/workflow/run_workflow.py` & `assemblyline-core-4.5.1.dev99/assemblyline_core/workflow/run_workflow.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core.egg-info/PKG-INFO` & `assemblyline-core-4.5.1.dev99/assemblyline_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-core
-Version: 4.5.1.dev98
+Version: 4.5.1.dev99
 Summary: Assemblyline 4 - Core components
 Home-page: https://github.com/CybercentreCanada/assemblyline-core/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `assemblyline-core-4.5.1.dev98/assemblyline_core.egg-info/SOURCES.txt` & `assemblyline-core-4.5.1.dev99/assemblyline_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/setup.py` & `assemblyline-core-4.5.1.dev99/setup.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/test/test_alerter.py` & `assemblyline-core-4.5.1.dev99/test/test_alerter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/test/test_badlist_client.py` & `assemblyline-core-4.5.1.dev99/test/test_badlist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/test/test_dispatcher.py` & `assemblyline-core-4.5.1.dev99/test/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/test/test_expiry.py` & `assemblyline-core-4.5.1.dev99/test/test_expiry.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/test/test_plumber.py` & `assemblyline-core-4.5.1.dev99/test/test_plumber.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/test/test_replay.py` & `assemblyline-core-4.5.1.dev99/test/test_replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/test/test_safelist_client.py` & `assemblyline-core-4.5.1.dev99/test/test_safelist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/test/test_scaler.py` & `assemblyline-core-4.5.1.dev99/test/test_scaler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/test/test_scheduler.py` & `assemblyline-core-4.5.1.dev99/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/test/test_signature_client.py` & `assemblyline-core-4.5.1.dev99/test/test_signature_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/test/test_simulation.py` & `assemblyline-core-4.5.1.dev99/test/test_simulation.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/test/test_vacuum.py` & `assemblyline-core-4.5.1.dev99/test/test_vacuum.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/test/test_worker_ingest.py` & `assemblyline-core-4.5.1.dev99/test/test_worker_ingest.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.5.1.dev98/test/test_worker_submit.py` & `assemblyline-core-4.5.1.dev99/test/test_worker_submit.py`

 * *Files identical despite different names*

