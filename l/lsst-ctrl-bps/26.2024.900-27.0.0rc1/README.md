# Comparing `tmp/lsst-ctrl-bps-26.2024.900.tar.gz` & `tmp/lsst_ctrl_bps-27.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-ctrl-bps-26.2024.900.tar", last modified: Thu Feb 29 10:21:39 2024, max compression
+gzip compressed data, was "lsst_ctrl_bps-27.0.0rc1.tar", last modified: Wed May  1 21:16:44 2024, max compression
```

## Comparing `lsst-ctrl-bps-26.2024.900.tar` & `lsst_ctrl_bps-27.0.0rc1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.637210 lsst-ctrl-bps-26.2024.900/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-29 10:21:39.637210 lsst-ctrl-bps-26.2024.900/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.625210 lsst-ctrl-bps-26.2024.900/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.629210 lsst-ctrl-bps-26.2024.900/doc/lsst.ctrl.bps/
--rw-r--r--   0 runner    (1001) docker     (127)    17300 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/doc/lsst.ctrl.bps/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/doc/lsst.ctrl.bps/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    44773 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/doc/lsst.ctrl.bps/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.629210 lsst-ctrl-bps-26.2024.900/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.629210 lsst-ctrl-bps-26.2024.900/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.629210 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.633210 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_draw.py
--rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cancel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.633210 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/bps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.633210 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/cmd/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.633210 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/option_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/clustered_quantum_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    21140 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.633210 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/etc/bps_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/etc/bps_eb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    30486 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/generic_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/pre_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/quantum_clustering_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/submit.py
--rw-r--r--   0 runner    (1001) docker     (127)    42853 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/wms_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.637210 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:21:39.000000 lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-29 10:21:39.637210 lsst-ctrl-bps-26.2024.900/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:39.637210 lsst-ctrl-bps-26.2024.900/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_bps_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_bpsconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_cli_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_clustered_quantum_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_generic_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_pre_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_quantum_clustering_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-02-29 10:21:26.000000 lsst-ctrl-bps-26.2024.900/tests/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:44.951300 lsst_ctrl_bps-27.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-01 21:16:44.951300 lsst_ctrl_bps-27.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:44.939300 lsst_ctrl_bps-27.0.0rc1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:44.939300 lsst_ctrl_bps-27.0.0rc1/doc/lsst.ctrl.bps/
+-rw-r--r--   0 runner    (1001) docker     (127)    17300 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/doc/lsst.ctrl.bps/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/doc/lsst.ctrl.bps/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    44773 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/doc/lsst.ctrl.bps/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:44.939300 lsst_ctrl_bps-27.0.0rc1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:44.939300 lsst_ctrl_bps-27.0.0rc1/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:44.939300 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:44.943300 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/bps_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/bps_draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/bps_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/bps_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cancel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:44.943300 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/bps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:44.943300 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/cmd/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:44.947300 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/opt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/opt/option_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/opt/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/clustered_quantum_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22623 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:44.947300 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/etc/bps_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/etc/bps_eb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    30486 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/generic_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10914 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/pre_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/quantum_clustering_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/submit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42853 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:16:44.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12810 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/wms_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:44.947300 lsst_ctrl_bps-27.0.0rc1/python/lsst_ctrl_bps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-01 21:16:44.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst_ctrl_bps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-01 21:16:44.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst_ctrl_bps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:44.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst_ctrl_bps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 21:16:44.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst_ctrl_bps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-01 21:16:44.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst_ctrl_bps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 21:16:44.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst_ctrl_bps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:44.000000 lsst_ctrl_bps-27.0.0rc1/python/lsst_ctrl_bps.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-01 21:16:44.951300 lsst_ctrl_bps-27.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:44.947300 lsst_ctrl_bps-27.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/tests/test_bps_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/tests/test_bpsconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/tests/test_cli_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/tests/test_clustered_quantum_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/tests/test_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/tests/test_generic_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/tests/test_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/tests/test_pre_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/tests/test_quantum_clustering_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8203 2024-05-01 21:16:38.000000 lsst_ctrl_bps-27.0.0rc1/tests/test_transform.py
```

### Comparing `lsst-ctrl-bps-26.2024.900/PKG-INFO` & `lsst_ctrl_bps-27.0.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: Pluggable execution of workflow graphs from Rubin pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-bps-26.2024.900/README.md` & `lsst_ctrl_bps-27.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/bsd_license.txt` & `lsst_ctrl_bps-27.0.0rc1/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/doc/lsst.ctrl.bps/CHANGES.rst` & `lsst_ctrl_bps-27.0.0rc1/doc/lsst.ctrl.bps/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/doc/lsst.ctrl.bps/index.rst` & `lsst_ctrl_bps-27.0.0rc1/doc/lsst.ctrl.bps/index.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/doc/lsst.ctrl.bps/quickstart.rst` & `lsst_ctrl_bps-27.0.0rc1/doc/lsst.ctrl.bps/quickstart.rst`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/gpl-v3.0.txt` & `lsst_ctrl_bps-27.0.0rc1/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/pyproject.toml` & `lsst_ctrl_bps-27.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/__init__.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/__init__.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/__init__.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_config.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/bps_config.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_draw.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/bps_draw.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_reports.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/bps_reports.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/bps_utils.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/bps_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cancel.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cancel.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/bps.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/bps.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/cmd/__init__.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/cmd/commands.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/__init__.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/arguments.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/opt/arguments.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/option_groups.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/opt/option_groups.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/cli/opt/options.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/cli/opt/options.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/clustered_quantum_graph.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/clustered_quantum_graph.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/constants.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/constants.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/drivers.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/drivers.py`

 * *Files 2% similar despite different names*

```diff
@@ -402,37 +402,69 @@
     kwargs.setdefault("runWmsSubmissionChecks", True)
 
     _LOG.info(
         "DISCLAIMER: All values regarding memory consumption reported below are approximate and may "
         "not accurately reflect actual memory usage by the bps process."
     )
 
+    remote_build = {}
+    config = BpsConfig(config_file, BPS_SEARCH_ORDER)
+    _, remote_build = config.search("remoteBuild", opt={"default": {}})
+    if remote_build:
+        if config["wmsServiceClass"] == "lsst.ctrl.bps.panda.PanDAService":
+            if not remote_build.search("enabled", opt={"default": False})[1]:
+                remote_build = {}
+                _LOG.info("The workflow is sumitted to the local Data Facility.")
+            else:
+                _LOG.info("Remote submission is enabled. The workflow is sumitted to a remote Data Facility.")
+                _LOG.info("Initializing execution environment")
+                with time_this(
+                    log=_LOG,
+                    level=logging.INFO,
+                    prefix=None,
+                    msg="Initializing execution environment completed",
+                    mem_usage=True,
+                    mem_unit=DEFAULT_MEM_UNIT,
+                    mem_fmt=DEFAULT_MEM_FMT,
+                ):
+                    config = _init_submission_driver(config_file, **kwargs)
+                    kwargs["remote_build"] = remote_build
+                    kwargs["config_file"] = config_file
+                    wms_workflow = None
+    else:
+        _LOG.info("The workflow is sumitted to the local Data Facility.")
+
     _LOG.info("Starting submission process")
     with time_this(
         log=_LOG,
         level=logging.INFO,
         prefix=None,
         msg="Completed entire submission process",
         mem_usage=True,
         mem_unit=DEFAULT_MEM_UNIT,
         mem_fmt=DEFAULT_MEM_FMT,
     ):
-        wms_workflow_config, wms_workflow = prepare_driver(config_file, **kwargs)
+        if not remote_build:
+            wms_workflow_config, wms_workflow = prepare_driver(config_file, **kwargs)
+        else:
+            wms_workflow_config = config
 
         _LOG.info("Starting submit stage")
         with time_this(
             log=_LOG,
             level=logging.INFO,
             prefix=None,
             msg="Completed submit stage",
             mem_usage=True,
             mem_unit=DEFAULT_MEM_UNIT,
             mem_fmt=DEFAULT_MEM_FMT,
         ):
-            submit(wms_workflow_config, wms_workflow)
+            workflow = submit(wms_workflow_config, wms_workflow, **kwargs)
+            if not wms_workflow:
+                wms_workflow = workflow
             _LOG.info("Run '%s' submitted for execution with id '%s'", wms_workflow.name, wms_workflow.run_id)
     if _LOG.isEnabledFor(logging.INFO):
         _LOG.info(
             "Peak memory usage for bps process %s (main), %s (largest child process)",
             *tuple(f"{val.to(DEFAULT_MEM_UNIT):{DEFAULT_MEM_FMT}}" for val in get_peak_mem_usage()),
         )
```

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/etc/bps_defaults.yaml` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/etc/bps_defaults.yaml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/etc/bps_eb.yaml` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/etc/bps_eb.yaml`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/generic_workflow.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/generic_workflow.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/ping.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/ping.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/pre_transform.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/pre_transform.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/prepare.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/prepare.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/quantum_clustering_funcs.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/quantum_clustering_funcs.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/report.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/report.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/restart.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/restart.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/submit.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/submit.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,44 +34,52 @@
 from lsst.utils.logging import VERBOSE
 from lsst.utils.timer import time_this, timeMethod
 
 _LOG = logging.getLogger(__name__)
 
 
 @timeMethod(logger=_LOG, logLevel=VERBOSE)
-def submit(config, wms_workflow, wms_service=None):
+def submit(config, wms_workflow, wms_service=None, **kwargs):
     """Convert generic workflow to a workflow for a particular WMS.
 
     Parameters
     ----------
     config : `lsst.ctrl.bps.BpsConfig`
         Configuration values to be used by submission.
     wms_workflow : `lsst.ctrl.bps.BaseWmsWorkflow`
         The workflow to submit.
     wms_service : `lsst.ctrl.bps.BaseWmsService`, optional
         The workflow management service to which the workflow should be
         submitted.
+    **kwargs : `~typing.Any`
+        Additional modifiers to submit a workflow.
 
     Returns
     -------
     wms_workflow : `lsst.ctrl.bps.BaseWmsWorkflow`
         WMS-specific workflow.
     """
     if wms_service is None:
         wms_service_class = doImport(config["wmsServiceClass"])
         wms_service = wms_service_class(config)
 
-    _, when_create = config.search(".executionButler.whenCreate")
-    if when_create.upper() == "SUBMIT":
-        _, execution_butler_dir = config.search(".bps_defined.executionButlerDir")
-        _LOG.info("Creating execution butler in '%s'", execution_butler_dir)
-        with time_this(log=_LOG, level=logging.INFO, prefix=None, msg="Completed creating execution butler"):
-            _create_execution_butler(
-                config, config["runQgraphFile"], execution_butler_dir, config["submitPath"]
-            )
+    remote_build = kwargs["remote_build"] if "remote_build" in kwargs else None
+    kwargs["config"] = config
+
+    if not remote_build:
+        _, when_create = config.search(".executionButler.whenCreate")
+        if when_create.upper() == "SUBMIT":
+            _, execution_butler_dir = config.search(".bps_defined.executionButlerDir")
+            _LOG.info("Creating execution butler in '%s'", execution_butler_dir)
+            with time_this(
+                log=_LOG, level=logging.INFO, prefix=None, msg="Completed creating execution butler"
+            ):
+                _create_execution_butler(
+                    config, config["runQgraphFile"], execution_butler_dir, config["submitPath"]
+                )
 
     _LOG.info("Submitting run to a workflow management system for execution")
     with time_this(
         log=_LOG, level=logging.INFO, prefix=None, msg="Completed submitting to a workflow management system"
     ):
-        workflow = wms_service.submit(wms_workflow)
+        workflow = wms_service.submit(wms_workflow, **kwargs)
     return workflow
```

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/transform.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/transform.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst/ctrl/bps/wms_service.py` & `lsst_ctrl_bps-27.0.0rc1/python/lsst/ctrl/bps/wms_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,21 +188,23 @@
         Returns
         -------
         wms_workflow : `lsst.ctrl.bps.BaseWmsWorkflow`
             Prepared WMS Workflow to submit for execution.
         """
         raise NotImplementedError
 
-    def submit(self, workflow):
+    def submit(self, workflow, **kwargs):
         """Submit a single WMS workflow.
 
         Parameters
         ----------
         workflow : `lsst.ctrl.bps.BaseWmsWorkflow`
             Prepared WMS Workflow to submit for execution.
+        **kwargs : `~typing.Any`
+            Additional modifiers to the configuration.
         """
         raise NotImplementedError
 
     def restart(self, wms_workflow_id):
         """Restart a workflow from the point of failure.
 
         Parameters
```

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/PKG-INFO` & `lsst_ctrl_bps-27.0.0rc1/python/lsst_ctrl_bps.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-ctrl-bps
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: Pluggable execution of workflow graphs from Rubin pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/ctrl_bps
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-ctrl-bps-26.2024.900/python/lsst_ctrl_bps.egg-info/SOURCES.txt` & `lsst_ctrl_bps-27.0.0rc1/python/lsst_ctrl_bps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/tests/test_bps_utils.py` & `lsst_ctrl_bps-27.0.0rc1/tests/test_bps_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/tests/test_bpsconfig.py` & `lsst_ctrl_bps-27.0.0rc1/tests/test_bpsconfig.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/tests/test_cli_commands.py` & `lsst_ctrl_bps-27.0.0rc1/tests/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/tests/test_clustered_quantum_graph.py` & `lsst_ctrl_bps-27.0.0rc1/tests/test_clustered_quantum_graph.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/tests/test_drivers.py` & `lsst_ctrl_bps-27.0.0rc1/tests/test_drivers.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/tests/test_generic_workflow.py` & `lsst_ctrl_bps-27.0.0rc1/tests/test_generic_workflow.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/tests/test_ping.py` & `lsst_ctrl_bps-27.0.0rc1/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/tests/test_pre_transform.py` & `lsst_ctrl_bps-27.0.0rc1/tests/test_pre_transform.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/tests/test_quantum_clustering_funcs.py` & `lsst_ctrl_bps-27.0.0rc1/tests/test_quantum_clustering_funcs.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/tests/test_report.py` & `lsst_ctrl_bps-27.0.0rc1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `lsst-ctrl-bps-26.2024.900/tests/test_transform.py` & `lsst_ctrl_bps-27.0.0rc1/tests/test_transform.py`

 * *Files identical despite different names*

