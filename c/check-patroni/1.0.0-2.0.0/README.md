# Comparing `tmp/check_patroni-1.0.0.tar.gz` & `tmp/check_patroni-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "check_patroni-1.0.0.tar", last modified: Mon Aug 28 10:12:55 2023, max compression
+gzip compressed data, was "check_patroni-2.0.0.tar", last modified: Thu May  2 07:58:27 2024, max compression
```

## Comparing `check_patroni-1.0.0.tar` & `check_patroni-2.0.0.tar`

### file list

```diff
@@ -1,83 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:12:55.761679 check_patroni-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (999)      197 2023-08-28 10:12:45.000000 check_patroni-1.0.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (999)     2000 2023-08-28 10:12:45.000000 check_patroni-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (999)     3273 2023-08-28 10:12:45.000000 check_patroni-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (999)      918 2023-08-28 10:12:45.000000 check_patroni-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      192 2023-08-28 10:12:45.000000 check_patroni-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)    13956 2023-08-28 10:12:55.761679 check_patroni-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    13360 2023-08-28 10:12:45.000000 check_patroni-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:12:55.757679 check_patroni-1.0.0/check_patroni/
--rw-r--r--   0 runner    (1001) docker     (999)       90 2023-08-28 10:12:45.000000 check_patroni-1.0.0/check_patroni/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)       61 2023-08-28 10:12:45.000000 check_patroni-1.0.0/check_patroni/__main__.py
--rw-r--r--   0 runner    (1001) docker     (999)    22364 2023-08-28 10:12:45.000000 check_patroni-1.0.0/check_patroni/cli.py
--rw-r--r--   0 runner    (1001) docker     (999)     8285 2023-08-28 10:12:45.000000 check_patroni-1.0.0/check_patroni/cluster.py
--rw-r--r--   0 runner    (1001) docker     (999)     1491 2023-08-28 10:12:45.000000 check_patroni-1.0.0/check_patroni/convert.py
--rw-r--r--   0 runner    (1001) docker     (999)     9246 2023-08-28 10:12:45.000000 check_patroni-1.0.0/check_patroni/node.py
--rw-r--r--   0 runner    (1001) docker     (999)     3131 2023-08-28 10:12:45.000000 check_patroni-1.0.0/check_patroni/types.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:12:55.757679 check_patroni-1.0.0/check_patroni.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)    13956 2023-08-28 10:12:55.000000 check_patroni-1.0.0/check_patroni.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2479 2023-08-28 10:12:55.000000 check_patroni-1.0.0/check_patroni.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 10:12:55.000000 check_patroni-1.0.0/check_patroni.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       57 2023-08-28 10:12:55.000000 check_patroni-1.0.0/check_patroni.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 10:12:55.000000 check_patroni-1.0.0/check_patroni.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)       86 2023-08-28 10:12:55.000000 check_patroni-1.0.0/check_patroni.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       14 2023-08-28 10:12:55.000000 check_patroni-1.0.0/check_patroni.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:12:55.757679 check_patroni-1.0.0/docs/
--rwxr-xr-x   0 runner    (1001) docker     (999)     3511 2023-08-28 10:12:45.000000 check_patroni-1.0.0/docs/make_readme.sh
--rw-r--r--   0 runner    (1001) docker     (999)      778 2023-08-28 10:12:45.000000 check_patroni-1.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (999)      132 2023-08-28 10:12:45.000000 check_patroni-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       37 2023-08-28 10:12:45.000000 check_patroni-1.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 10:12:55.761679 check_patroni-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1576 2023-08-28 10:12:45.000000 check_patroni-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:12:55.757679 check_patroni-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      415 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 10:12:55.761679 check_patroni-1.0.0/tests/json/
--rw-r--r--   0 runner    (1001) docker     (999)      389 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_config_has_changed.json
--rw-r--r--   0 runner    (1001) docker     (999)      681 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_has_leader_ko.json
--rw-r--r--   0 runner    (1001) docker     (999)      684 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_has_leader_ok.json
--rw-r--r--   0 runner    (1001) docker     (999)      692 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_has_leader_ok_standby_leader.json
--rw-r--r--   0 runner    (1001) docker     (999)      690 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_has_replica_ko.json
--rw-r--r--   0 runner    (1001) docker     (999)      698 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_has_replica_ko_lag.json
--rw-r--r--   0 runner    (1001) docker     (999)      689 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_has_replica_ok.json
--rw-r--r--   0 runner    (1001) docker     (999)      688 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_has_replica_ok_lag.json
--rw-r--r--   0 runner    (1001) docker     (999)      609 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_has_scheduled_action_ko_restart.json
--rw-r--r--   0 runner    (1001) docker     (999)      559 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_has_scheduled_action_ko_switchover.json
--rw-r--r--   0 runner    (1001) docker     (999)      689 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_has_scheduled_action_ok.json
--rw-r--r--   0 runner    (1001) docker     (999)      701 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_is_in_maintenance_ko.json
--rw-r--r--   0 runner    (1001) docker     (999)      702 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_is_in_maintenance_ko_pause_false.json
--rw-r--r--   0 runner    (1001) docker     (999)      684 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_is_in_maintenance_ok.json
--rw-r--r--   0 runner    (1001) docker     (999)      702 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_is_in_maintenance_ok_pause_false.json
--rw-r--r--   0 runner    (1001) docker     (999)      230 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_node_count_critical.json
--rw-r--r--   0 runner    (1001) docker     (999)      662 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_node_count_healthy_critical.json
--rw-r--r--   0 runner    (1001) docker     (999)      457 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_node_count_healthy_warning.json
--rw-r--r--   0 runner    (1001) docker     (999)      684 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_node_count_ok.json
--rw-r--r--   0 runner    (1001) docker     (999)      457 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/cluster_node_count_warning.json
--rw-r--r--   0 runner    (1001) docker     (999)      568 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/node_is_leader_ko.json
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/node_is_leader_ko_standby_leader.json
--rw-r--r--   0 runner    (1001) docker     (999)      568 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/node_is_leader_ok.json
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/node_is_leader_ok_standby_leader.json
--rw-r--r--   0 runner    (1001) docker     (999)      595 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/node_is_pending_restart_ko.json
--rw-r--r--   0 runner    (1001) docker     (999)      568 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/node_is_pending_restart_ok.json
--rw-r--r--   0 runner    (1001) docker     (999)      449 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/node_is_primary_ko.json
--rw-r--r--   0 runner    (1001) docker     (999)      568 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/node_is_primary_ok.json
--rw-r--r--   0 runner    (1001) docker     (999)      568 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/node_is_replica_ko.json
--rw-r--r--   0 runner    (1001) docker     (999)      449 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/node_is_replica_ok.json
--rw-r--r--   0 runner    (1001) docker     (999)      568 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/node_patroni_version.json
--rw-r--r--   0 runner    (1001) docker     (999)      568 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/json/node_tl_has_changed.json
--rw-r--r--   0 runner    (1001) docker     (999)      765 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (999)     5548 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/test_cluster_config_has_changed.py
--rw-r--r--   0 runner    (1001) docker     (999)     1510 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/test_cluster_has_leader.py
--rw-r--r--   0 runner    (1001) docker     (999)     5119 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/test_cluster_has_replica.py
--rw-r--r--   0 runner    (1001) docker     (999)     1818 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/test_cluster_has_scheduled_action.py
--rw-r--r--   0 runner    (1001) docker     (999)     1589 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/test_cluster_is_in_maintenance.py
--rw-r--r--   0 runner    (1001) docker     (999)     5382 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/test_cluster_node_count.py
--rw-r--r--   0 runner    (1001) docker     (999)      944 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/test_node_is_alive.py
--rw-r--r--   0 runner    (1001) docker     (999)     1699 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/test_node_is_leader.py
--rw-r--r--   0 runner    (1001) docker     (999)     1107 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/test_node_is_pending_restart.py
--rw-r--r--   0 runner    (1001) docker     (999)     1000 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/test_node_is_primary.py
--rw-r--r--   0 runner    (1001) docker     (999)     5687 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/test_node_is_replica.py
--rw-r--r--   0 runner    (1001) docker     (999)     1262 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/test_node_patroni_version.py
--rw-r--r--   0 runner    (1001) docker     (999)     4802 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/test_node_tl_has_changed.py
--rw-r--r--   0 runner    (1001) docker     (999)     1451 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tests/tools.py
--rw-r--r--   0 runner    (1001) docker     (999)     1164 2023-08-28 10:12:45.000000 check_patroni-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:58:27.410641 check_patroni-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 07:58:19.000000 check_patroni-2.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-02 07:58:19.000000 check_patroni-2.0.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-02 07:58:19.000000 check_patroni-2.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-02 07:58:19.000000 check_patroni-2.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-02 07:58:19.000000 check_patroni-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 07:58:19.000000 check_patroni-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17578 2024-05-02 07:58:27.410641 check_patroni-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16982 2024-05-02 07:58:19.000000 check_patroni-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-02 07:58:19.000000 check_patroni-2.0.0/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:58:27.402641 check_patroni-2.0.0/check_patroni/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 07:58:19.000000 check_patroni-2.0.0/check_patroni/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 07:58:19.000000 check_patroni-2.0.0/check_patroni/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25588 2024-05-02 07:58:19.000000 check_patroni-2.0.0/check_patroni/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-05-02 07:58:19.000000 check_patroni-2.0.0/check_patroni/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-02 07:58:19.000000 check_patroni-2.0.0/check_patroni/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-02 07:58:19.000000 check_patroni-2.0.0/check_patroni/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-02 07:58:19.000000 check_patroni-2.0.0/check_patroni/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:58:27.402641 check_patroni-2.0.0/check_patroni.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17578 2024-05-02 07:58:27.000000 check_patroni-2.0.0/check_patroni.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-02 07:58:27.000000 check_patroni-2.0.0/check_patroni.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 07:58:27.000000 check_patroni-2.0.0/check_patroni.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 07:58:27.000000 check_patroni-2.0.0/check_patroni.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 07:58:27.000000 check_patroni-2.0.0/check_patroni.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-02 07:58:27.000000 check_patroni-2.0.0/check_patroni.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-02 07:58:27.000000 check_patroni-2.0.0/check_patroni.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:58:27.402641 check_patroni-2.0.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4289 2024-05-02 07:58:19.000000 check_patroni-2.0.0/docs/make_readme.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-02 07:58:19.000000 check_patroni-2.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-02 07:58:19.000000 check_patroni-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 07:58:19.000000 check_patroni-2.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 07:58:27.410641 check_patroni-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-02 07:58:19.000000 check_patroni-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:58:27.406641 check_patroni-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:58:27.410641 check_patroni-2.0.0/tests/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_config_has_changed.json
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_leader_ko.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_leader_ko_standby_leader.json
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_leader_ko_standby_leader_archiving.json
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_leader_ok.json
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_leader_ok_standby_leader.json
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_replica_ko.json
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_replica_ko_all_replica.json
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_replica_ko_lag.json
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_replica_ko_wrong_tl.json
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_replica_ok.json
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_replica_ok_lag.json
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_replica_patroni_verion_3.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_replica_patroni_verion_3.1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_scheduled_action_ko_restart.json
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_scheduled_action_ko_switchover.json
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_has_scheduled_action_ok.json
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_is_in_maintenance_ko.json
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_is_in_maintenance_ko_pause_false.json
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_is_in_maintenance_ok.json
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_is_in_maintenance_ok_pause_false.json
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_node_count_critical.json
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_node_count_healthy_critical.json
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_node_count_healthy_warning.json
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_node_count_ko_in_archive_recovery.json
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_node_count_ok.json
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/cluster_node_count_warning.json
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/node_is_leader_ko.json
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/node_is_leader_ko_standby_leader.json
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/node_is_leader_ok.json
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/node_is_leader_ok_standby_leader.json
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/node_is_pending_restart_ko.json
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/node_is_pending_restart_ok.json
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/node_is_primary_ko.json
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/node_is_primary_ok.json
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/node_is_replica_ko.json
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/node_is_replica_ok.json
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/node_patroni_version.json
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/json/node_tl_has_changed.json
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/test_cluster_config_has_changed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/test_cluster_has_leader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/test_cluster_has_replica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/test_cluster_has_scheduled_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/test_cluster_is_in_maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9706 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/test_cluster_node_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/test_node_is_alive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/test_node_is_leader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/test_node_is_pending_restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/test_node_is_primary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/test_node_is_replica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/test_node_patroni_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tests/test_node_tl_has_changed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-02 07:58:19.000000 check_patroni-2.0.0/tox.ini
```

### Comparing `check_patroni-1.0.0/CHANGELOG.md` & `check_patroni-2.0.0/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,41 @@
 # Change log
 
-## Unreleased
+## check_patroni 2.0.0 - 2024-04-09
+
+### Changed
+
+* In `cluster_node_count`, a healthy standby, sync replica or standby leaders cannot be "in
+  archive recovery" because this service doesn't check for lag and timelines.
 
 ### Added
 
+* Add the timeline in the  `cluster_has_replica` perfstats. (#50)
+* Add a mention about shell completion support and shell versions in the doc. (#53)
+* Add the leader type and whether it's archiving to the `cluster_has_leader` perfstats. (#58)
+
 ### Fixed
 
+* Add compatibility with [requests](https://requests.readthedocs.io)
+  version 2.25 and higher.
+* Fix what `cluster_has_replica` deems a healthy replica. (#50, reported by @mbanck)
+* Fix `cluster_has_replica` to display perfstats for replicas whenever it's possible (healthy or not). (#50)
+* Fix `cluster_has_leader` to correctly check for standby leaders. (#58, reported by @mbanck)
+* Fix `cluster_node_count` to correctly manage replication states. (#50, reported by @mbanck)
+
 ### Misc
 
+* Improve the documentation for `node_is_replica`.
+* Improve test coverage by running an HTTP server to fake the Patroni API (#55
+  by @dlax).
+* Work around old pytest versions in type annotations in the test suite.
+* Declare compatibility with click version 7.1 (or higher).
+* In tests, work around nagiosplugin 1.3.2 not properly handling stdout
+  redirection.
+
 ## check_patroni 1.0.0 - 2023-08-28
 
 Check patroni is now tagged as Production/Stable.
 
 ### Added
 
 * Add `sync_standby` as a valid replica type for `cluster_has_replica`. (contributed by @mattpoel)
```

### Comparing `check_patroni-1.0.0/CONTRIBUTING.md` & `check_patroni-2.0.0/CONTRIBUTING.md`

 * *Files 10% similar despite different names*

```diff
@@ -39,77 +39,56 @@
 install check_patroni. You can then add a server to the supervision and
 watch the graphs in grafana. It's in the `vagrant` directory.
 
 A vagrant file can be found in [this
 repository](https://github.com/ioguix/vagrant-patroni) to generate a patroni/etcd
 setup.
 
-The `README.md` can be geneated with `./docs/make_readme.sh`.
+The `README.md` can be generated with `./docs/make_readme.sh`.
 
 ## Executing Tests
 
 Crafting repeatable tests using a live Patroni cluster can be intricate. To
-simplify the development process, interactions with Patroni's API are
-substituted with a mock function that yields an HTTP return code and a JSON
-object outlining the cluster's status. The JSON files containing this
-information are housed in the `./tests/json` directory.
+simplify the development process, a fake HTTP server is set up as a test
+fixture and serves static files (either from `tests/json` directory or from
+in-memory data).
 
 An important consideration is that there is a potential drawback: if the JSON
 data is incorrect or if modifications have been made to Patroni without
 corresponding updates to the tests documented here, the tests might still pass
 erroneously.
 
 The tests are executed automatically for each PR using the ci (see
 `.github/workflow/lint.yml` and `.github/workflow/tests.yml`).
 
-Running the tests manually:
+Running the tests,
 
-* Using patroni's nominal replica state of `streaming` (since v3.0.4):
+* manually:
 
   ```bash
-  pytest ./tests
+  pytest --cov tests
   ```
 
-* Using patroni's nominal replica state of `running` (before v3.0.4):
-
-  ```bash
-  pytest --use-old-replica-state ./tests
-  ```
-
-* Using tox:
+* or using tox:
 
   ```bash
   tox -e lint    # mypy + flake8 + black + isort ° codespell
   tox            # pytests and "lint" tests for all supported version of python
   tox -e py      # pytests and "lint" tests for the default version of python
   ```
 
-Please note that when dealing with any service that checks the state of a node
-in patroni's `cluster` endpoint, the corresponding JSON test file must be added
-in `./tests/tools.py`.
+Please note that when dealing with any service that checks the state of a node,
+the related tests must use the `old_replica_state` fixture to test with both
+old (pre 3.0.4) and new replica states.
 
 A bash script, `check_patroni.sh`, is provided to facilitate testing all
 services on a Patroni endpoint (`./vagrant/check_patroni.sh`). It requires one
 parameter: the endpoint URL that will be used as the argument for the
 `-e/--endpoints` option of `check_patroni`. This script essentially compiles a
 list of service calls and executes them sequentially in a bash script. It
 creates a state file in the directory from which you run the script.
 
 Here's an example usage:
 
 ```bash
 ./vagrant/check_patroni.sh http://10.20.30.51:8008
 ```
-
-## Release
-
-Update the Changelog.
-
-The package is generated and uploaded to pypi when a `v*` tag is created (see
-`.github/workflow/publish.yml`).
-
-Alternatively, the release can be done manually with:
-
-```
-tox -e build
-tox -e upload
-```
```

### Comparing `check_patroni-1.0.0/LICENSE` & `check_patroni-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/PKG-INFO` & `check_patroni-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check_patroni
-Version: 1.0.0
+Version: 2.0.0
 Summary: Nagios plugin to check on patroni
 Home-page: https://github.com/dalibo/check_patroni
 Author: Dalibo
 Author-email: contact@dalibo.com
 License: PostgreSQL
 Keywords: patroni nagios check
 Classifier: Development Status :: 5 - Production/Stable
@@ -60,30 +60,30 @@
   cluster_has_scheduled_action  Check if the cluster has a scheduled...
   cluster_is_in_maintenance     Check if the cluster is in maintenance...
   cluster_node_count            Count the number of nodes in the cluster.
   node_is_alive                 Check if the node is alive ie patroni is...
   node_is_leader                Check if the node is a leader node.
   node_is_pending_restart       Check if the node is in pending restart...
   node_is_primary               Check if the node is the primary with the...
-  node_is_replica               Check if the node is a running replica...
+  node_is_replica               Check if the node is a replica with no...
   node_patroni_version          Check if the version is equal to the input
   node_tl_has_changed           Check if the timeline has changed.
 ```
 
 ## Install
 
 check_patroni is licensed under PostgreSQL license.
 
 ```
 $ pip install git+https://github.com/dalibo/check_patroni.git
 ```
 
 check_patroni works on python 3.6, we keep it that way because patroni also
 supports it and there are still lots of RH 7 variants around. That being said
-python 3.6 has been EOL for age and there is no support for it in the github
+python 3.6 has been EOL for ages and there is no support for it in the github
 CI.
 
 ## Support
 
 If you hit a bug or need help, open a [GitHub
 issue](https://github.com/dalibo/check_patroni/issues/new). Dalibo has no
 commitment on response time for public free support. Thanks for you
@@ -113,16 +113,16 @@
 * If `end` is omitted, infinity is assumed
 * To invert the match condition, prefix the range expression with `@`.
 
 A match is found when: `start <= VALUE <= end`.
 
 For example, the following command will raise:
 
-* a warning if there is less than 1 nodes, wich can be translated to outside of range [2;+INF[
-* a critical if there are no nodes, wich can be translated to outside of range [1;+INF[
+* a warning if there is less than 1 nodes, which can be translated to outside of range [2;+INF[
+* a critical if there are no nodes, which can be translated to outside of range [1;+INF[
 
 ```
 check_patroni -e https://10.20.199.3:8008 cluster_has_replica --warning 2: --critical 1:
 ```
 
 ## SSL
 
@@ -130,14 +130,38 @@
 
 * the server's CA certificate is not available or trusted by the client system:
   * `--ca_cert`: your certification chain `cat CA-certificate server-certificate > cabundle`
 * you have a client certificate for authenticating with Patroni's REST API:
   * `--cert_file`: your certificate or the concatenation of your certificate and private key
   * `--key_file`: your private key (optional)
 
+## Shell completion
+
+We use the [click] library which supports shell completion natively.
+
+Shell completion can be added by typing the following command or adding it to
+a file spécific to your shell of choice.
+
+* for Bash (add to `~/.bashrc`):
+  ```
+  eval "$(_CHECK_PATRONI_COMPLETE=bash_source check_patroni)"
+  ```
+* for Zsh  (add to `~/.zshrc`):
+  ```
+  eval "$(_CHECK_PATRONI_COMPLETE=zsh_source check_patroni)"
+  ```
+* for Fish (add to `~/.config/fish/completions/check_patroni.fish`):
+  ```
+  eval "$(_CHECK_PATRONI_COMPLETE=fish_source check_patroni)"
+  ```
+
+Please note that shell completion is not supported far all shell versions, for
+example only Bash versions older than 4.4 are supported.
+
+[click]: https://click.palletsprojects.com/en/8.1.x/shell-completion/
 
 ## Cluster services
 
 ### cluster_config_has_changed
 
 ```
 Usage: check_patroni cluster_config_has_changed [OPTIONS]
@@ -167,46 +191,80 @@
 ```
 Usage: check_patroni cluster_has_leader [OPTIONS]
 
   Check if the cluster has a leader.
 
   This check applies to any kind of leaders including standby leaders.
 
+  A leader is a node with the "leader" role and a "running" state.
+
+  A standby leader is a node with a "standby_leader" role and a "streaming" or
+  "in archive recovery" state. Please note that log shipping could be stuck
+  because the WAL are not available or applicable. Patroni doesn't provide
+  information about the origin cluster (timeline or lag), so we cannot check
+  if there is a problem in that particular case. That's why we issue a warning
+  when the node is "in archive recovery". We suggest using other supervision
+  tools to do this (eg. check_pgactivity).
+
   Check:
   * `OK`: if there is a leader node.
-  * `CRITICAL`: otherwise
+  * 'WARNING': if there is a stanby leader in archive mode.
+  * `CRITICAL`: otherwise.
 
-  Perfdata: `has_leader` is 1 if there is a leader node, 0 otherwise
+  Perfdata:
+  * `has_leader` is 1 if there is any kind of leader node, 0 otherwise
+  * `is_standby_leader_in_arc_rec` is 1 if the standby leader node is "in
+     archive recovery", 0 otherwise
+  * `is_standby_leader` is 1 if there is a standby leader node, 0 otherwise
+  * `is_leader` is 1 if there is a "classical" leader node, 0 otherwise
 
 Options:
   --help  Show this message and exit.
 ```
 
 ### cluster_has_replica
 
 ```
 Usage: check_patroni cluster_has_replica [OPTIONS]
 
   Check if the cluster has healthy replicas and/or if some are sync standbies
 
+  For patroni (and this check):
+  * a replica is `streaming` if the `pg_stat_wal_receiver` say's so.
+  * a replica is `in archive recovery`, if it's not `streaming` and has a `restore_command`.
+
   A healthy replica:
-  * is in running or streaming state (V3.0.4)
-  * has a replica or sync_standby role
-  * has a lag lower or equal to max_lag
+  * has a `replica` or `sync_standby` role
+  * has the same timeline as the leader and
+    * is in `running` state (patroni < V3.0.4)
+    * is in `streaming` or `in archive recovery` state (patroni >= V3.0.4)
+  * has a lag lower or equal to `max_lag`
+
+  Please note that replica `in archive recovery` could be stuck because the
+  WAL are not available or applicable (the server's timeline has diverged for
+  the leader's). We already detect the latter but we will miss the former.
+  Therefore, it's preferable to check for the lag in addition to the healthy
+  state if you rely on log shipping to help lagging standbies to catch up.
+
+  Since we require a healthy replica to have the same timeline as the leader,
+  it's possible that we raise alerts when the cluster is performing a
+  switchover or failover and the standbies are in the process of catching up
+  with the new leader. The alert shouldn't last long.
 
   Check:
   * `OK`: if the healthy_replica count and their lag are compatible with the replica count threshold.
           and if the sync_replica count is compatible with the sync replica count threshold.
   * `WARNING` / `CRITICAL`: otherwise
 
   Perfdata:
   * healthy_replica & unhealthy_replica count
   * the number of sync_replica, they are included in the previous count
-  * the lag of each replica labelled with  "member name"_lag
-  * a boolean to tell if the node is a sync stanbdy labelled with  "member name"_sync
+  * the lag of each replica labelled with "member name"_lag
+  * the timeline of each replica labelled with "member name"_timeline
+  * a boolean to tell if the node is a sync stanbdy labelled with "member name"_sync
 
 Options:
   -w, --warning TEXT    Warning threshold for the number of healthy replica
                         nodes.
   -c, --critical TEXT   Critical threshold for the number of healthy replica
                         nodes.
   --sync-warning TEXT   Warning threshold for the number of sync replica.
@@ -256,34 +314,45 @@
 ### cluster_node_count
 
 ```
 Usage: check_patroni cluster_node_count [OPTIONS]
 
   Count the number of nodes in the cluster.
 
+  The role refers to the role of the server in the cluster. Possible values
+  are:
+  * master or leader
+  * replica
+  * standby_leader
+  * sync_standby
+  * demoted
+  * promoted
+  * uninitialized
+
   The state refers to the state of PostgreSQL. Possible values are:
   * initializing new cluster, initdb failed
   * running custom bootstrap script, custom bootstrap failed
   * starting, start failed
   * restarting, restart failed
-  * running, streaming (for a replica V3.0.4)
+  * running, streaming, in archive recovery
   * stopping, stopped, stop failed
   * creating replica
   * crashed
 
-  The role refers to the role of the server in the cluster. Possible values
-  are:
-  * master or leader (V3.0.0+)
-  * replica
-  * demoted
-  * promoted
-  * uninitialized
+  The "healthy" checks only ensures that:
+  * a leader has the running state
+  * a standby_leader has the running or streaming (V3.0.4) state
+  * a replica or sync-standby has the running or streaming (V3.0.4) state
+
+  Since we dont check the lag or timeline, "in archive recovery" is not
+  considered a valid state for this service. See cluster_has_leader and
+  cluster_has_replica for specialized checks.
 
   Check:
-  * Compares the number of nodes against the normal and healthy (running + streaming) nodes warning and critical thresholds.
+  * Compares the number of nodes against the normal and healthy nodes warning and critical thresholds.
   * `OK`:  If they are not provided.
 
   Perfdata:
   * `members`: the member count.
   * `healthy_members`: the running and streaming member count.
   * all the roles of the nodes in the cluster with their count (start with "role_").
   * all the statuses of the nodes in the cluster with their count (start with "state_").
@@ -322,15 +391,15 @@
 ### node_is_pending_restart
 
 ```
 Usage: check_patroni node_is_pending_restart [OPTIONS]
 
   Check if the node is in pending restart state.
 
-  This situation can arise if the configuration has been modified but requiers
+  This situation can arise if the configuration has been modified but requires
   a restart of PostgreSQL to take effect.
 
   Check:
   * `OK`: if the node has no pending restart tag.
   * `CRITICAL`: otherwise
 
   Perfdata: `is_pending_restart` is 1 if the node has pending restart tag, 0
@@ -383,20 +452,29 @@
 ```
 
 ### node_is_replica
 
 ```
 Usage: check_patroni node_is_replica [OPTIONS]
 
-  Check if the node is a running replica with no noloadbalance tag.
+  Check if the node is a replica with no noloadbalance tag.
 
   It is possible to check if the node is synchronous or asynchronous. If
-  nothing is specified any kind of replica is accepted. When checking for a
+  nothing is specified any kind of replica is accepted.  When checking for a
   synchronous replica, it's not possible to specify a lag.
 
+  This service is using the following Patroni endpoints: replica, asynchronous
+  and synchronous. The first two implement the `lag` tag. For these endpoints
+  the state of a replica node doesn't reflect the replication state
+  (`streaming` or `in archive recovery`), we only know if it's `running`. The
+  timeline is also not checked.
+
+  Therefore, if a cluster is using asynchronous replication, it is recommended
+  to check for the lag to detect a divegence as soon as possible.
+
   Check:
   * `OK`: if the node is a running replica with noloadbalance tag and the lag is under the maximum threshold.
   * `CRITICAL`:  otherwise
 
   Perfdata: `is_replica` is 1 if the node is a running replica with
   noloadbalance tag and the lag is under the maximum threshold, 0 otherwise.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `check_patroni-1.0.0/README.md` & `check_patroni-2.0.0/check_patroni.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: check-patroni
+Version: 2.0.0
+Summary: Nagios plugin to check on patroni
+Home-page: https://github.com/dalibo/check_patroni
+Author: Dalibo
+Author-email: contact@dalibo.com
+License: PostgreSQL
+Keywords: patroni nagios check
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: PostgreSQL License
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: System :: Monitoring
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # check_patroni
 
 A nagios plugin for patroni.
 
 ## Features
 
 - Check presence of leader, replicas, node counts.
@@ -41,30 +60,30 @@
   cluster_has_scheduled_action  Check if the cluster has a scheduled...
   cluster_is_in_maintenance     Check if the cluster is in maintenance...
   cluster_node_count            Count the number of nodes in the cluster.
   node_is_alive                 Check if the node is alive ie patroni is...
   node_is_leader                Check if the node is a leader node.
   node_is_pending_restart       Check if the node is in pending restart...
   node_is_primary               Check if the node is the primary with the...
-  node_is_replica               Check if the node is a running replica...
+  node_is_replica               Check if the node is a replica with no...
   node_patroni_version          Check if the version is equal to the input
   node_tl_has_changed           Check if the timeline has changed.
 ```
 
 ## Install
 
 check_patroni is licensed under PostgreSQL license.
 
 ```
 $ pip install git+https://github.com/dalibo/check_patroni.git
 ```
 
 check_patroni works on python 3.6, we keep it that way because patroni also
 supports it and there are still lots of RH 7 variants around. That being said
-python 3.6 has been EOL for age and there is no support for it in the github
+python 3.6 has been EOL for ages and there is no support for it in the github
 CI.
 
 ## Support
 
 If you hit a bug or need help, open a [GitHub
 issue](https://github.com/dalibo/check_patroni/issues/new). Dalibo has no
 commitment on response time for public free support. Thanks for you
@@ -94,16 +113,16 @@
 * If `end` is omitted, infinity is assumed
 * To invert the match condition, prefix the range expression with `@`.
 
 A match is found when: `start <= VALUE <= end`.
 
 For example, the following command will raise:
 
-* a warning if there is less than 1 nodes, wich can be translated to outside of range [2;+INF[
-* a critical if there are no nodes, wich can be translated to outside of range [1;+INF[
+* a warning if there is less than 1 nodes, which can be translated to outside of range [2;+INF[
+* a critical if there are no nodes, which can be translated to outside of range [1;+INF[
 
 ```
 check_patroni -e https://10.20.199.3:8008 cluster_has_replica --warning 2: --critical 1:
 ```
 
 ## SSL
 
@@ -111,14 +130,38 @@
 
 * the server's CA certificate is not available or trusted by the client system:
   * `--ca_cert`: your certification chain `cat CA-certificate server-certificate > cabundle`
 * you have a client certificate for authenticating with Patroni's REST API:
   * `--cert_file`: your certificate or the concatenation of your certificate and private key
   * `--key_file`: your private key (optional)
 
+## Shell completion
+
+We use the [click] library which supports shell completion natively.
+
+Shell completion can be added by typing the following command or adding it to
+a file spécific to your shell of choice.
+
+* for Bash (add to `~/.bashrc`):
+  ```
+  eval "$(_CHECK_PATRONI_COMPLETE=bash_source check_patroni)"
+  ```
+* for Zsh  (add to `~/.zshrc`):
+  ```
+  eval "$(_CHECK_PATRONI_COMPLETE=zsh_source check_patroni)"
+  ```
+* for Fish (add to `~/.config/fish/completions/check_patroni.fish`):
+  ```
+  eval "$(_CHECK_PATRONI_COMPLETE=fish_source check_patroni)"
+  ```
+
+Please note that shell completion is not supported far all shell versions, for
+example only Bash versions older than 4.4 are supported.
+
+[click]: https://click.palletsprojects.com/en/8.1.x/shell-completion/
 
 ## Cluster services
 
 ### cluster_config_has_changed
 
 ```
 Usage: check_patroni cluster_config_has_changed [OPTIONS]
@@ -148,46 +191,80 @@
 ```
 Usage: check_patroni cluster_has_leader [OPTIONS]
 
   Check if the cluster has a leader.
 
   This check applies to any kind of leaders including standby leaders.
 
+  A leader is a node with the "leader" role and a "running" state.
+
+  A standby leader is a node with a "standby_leader" role and a "streaming" or
+  "in archive recovery" state. Please note that log shipping could be stuck
+  because the WAL are not available or applicable. Patroni doesn't provide
+  information about the origin cluster (timeline or lag), so we cannot check
+  if there is a problem in that particular case. That's why we issue a warning
+  when the node is "in archive recovery". We suggest using other supervision
+  tools to do this (eg. check_pgactivity).
+
   Check:
   * `OK`: if there is a leader node.
-  * `CRITICAL`: otherwise
+  * 'WARNING': if there is a stanby leader in archive mode.
+  * `CRITICAL`: otherwise.
 
-  Perfdata: `has_leader` is 1 if there is a leader node, 0 otherwise
+  Perfdata:
+  * `has_leader` is 1 if there is any kind of leader node, 0 otherwise
+  * `is_standby_leader_in_arc_rec` is 1 if the standby leader node is "in
+     archive recovery", 0 otherwise
+  * `is_standby_leader` is 1 if there is a standby leader node, 0 otherwise
+  * `is_leader` is 1 if there is a "classical" leader node, 0 otherwise
 
 Options:
   --help  Show this message and exit.
 ```
 
 ### cluster_has_replica
 
 ```
 Usage: check_patroni cluster_has_replica [OPTIONS]
 
   Check if the cluster has healthy replicas and/or if some are sync standbies
 
+  For patroni (and this check):
+  * a replica is `streaming` if the `pg_stat_wal_receiver` say's so.
+  * a replica is `in archive recovery`, if it's not `streaming` and has a `restore_command`.
+
   A healthy replica:
-  * is in running or streaming state (V3.0.4)
-  * has a replica or sync_standby role
-  * has a lag lower or equal to max_lag
+  * has a `replica` or `sync_standby` role
+  * has the same timeline as the leader and
+    * is in `running` state (patroni < V3.0.4)
+    * is in `streaming` or `in archive recovery` state (patroni >= V3.0.4)
+  * has a lag lower or equal to `max_lag`
+
+  Please note that replica `in archive recovery` could be stuck because the
+  WAL are not available or applicable (the server's timeline has diverged for
+  the leader's). We already detect the latter but we will miss the former.
+  Therefore, it's preferable to check for the lag in addition to the healthy
+  state if you rely on log shipping to help lagging standbies to catch up.
+
+  Since we require a healthy replica to have the same timeline as the leader,
+  it's possible that we raise alerts when the cluster is performing a
+  switchover or failover and the standbies are in the process of catching up
+  with the new leader. The alert shouldn't last long.
 
   Check:
   * `OK`: if the healthy_replica count and their lag are compatible with the replica count threshold.
           and if the sync_replica count is compatible with the sync replica count threshold.
   * `WARNING` / `CRITICAL`: otherwise
 
   Perfdata:
   * healthy_replica & unhealthy_replica count
   * the number of sync_replica, they are included in the previous count
-  * the lag of each replica labelled with  "member name"_lag
-  * a boolean to tell if the node is a sync stanbdy labelled with  "member name"_sync
+  * the lag of each replica labelled with "member name"_lag
+  * the timeline of each replica labelled with "member name"_timeline
+  * a boolean to tell if the node is a sync stanbdy labelled with "member name"_sync
 
 Options:
   -w, --warning TEXT    Warning threshold for the number of healthy replica
                         nodes.
   -c, --critical TEXT   Critical threshold for the number of healthy replica
                         nodes.
   --sync-warning TEXT   Warning threshold for the number of sync replica.
@@ -237,34 +314,45 @@
 ### cluster_node_count
 
 ```
 Usage: check_patroni cluster_node_count [OPTIONS]
 
   Count the number of nodes in the cluster.
 
+  The role refers to the role of the server in the cluster. Possible values
+  are:
+  * master or leader
+  * replica
+  * standby_leader
+  * sync_standby
+  * demoted
+  * promoted
+  * uninitialized
+
   The state refers to the state of PostgreSQL. Possible values are:
   * initializing new cluster, initdb failed
   * running custom bootstrap script, custom bootstrap failed
   * starting, start failed
   * restarting, restart failed
-  * running, streaming (for a replica V3.0.4)
+  * running, streaming, in archive recovery
   * stopping, stopped, stop failed
   * creating replica
   * crashed
 
-  The role refers to the role of the server in the cluster. Possible values
-  are:
-  * master or leader (V3.0.0+)
-  * replica
-  * demoted
-  * promoted
-  * uninitialized
+  The "healthy" checks only ensures that:
+  * a leader has the running state
+  * a standby_leader has the running or streaming (V3.0.4) state
+  * a replica or sync-standby has the running or streaming (V3.0.4) state
+
+  Since we dont check the lag or timeline, "in archive recovery" is not
+  considered a valid state for this service. See cluster_has_leader and
+  cluster_has_replica for specialized checks.
 
   Check:
-  * Compares the number of nodes against the normal and healthy (running + streaming) nodes warning and critical thresholds.
+  * Compares the number of nodes against the normal and healthy nodes warning and critical thresholds.
   * `OK`:  If they are not provided.
 
   Perfdata:
   * `members`: the member count.
   * `healthy_members`: the running and streaming member count.
   * all the roles of the nodes in the cluster with their count (start with "role_").
   * all the statuses of the nodes in the cluster with their count (start with "state_").
@@ -303,15 +391,15 @@
 ### node_is_pending_restart
 
 ```
 Usage: check_patroni node_is_pending_restart [OPTIONS]
 
   Check if the node is in pending restart state.
 
-  This situation can arise if the configuration has been modified but requiers
+  This situation can arise if the configuration has been modified but requires
   a restart of PostgreSQL to take effect.
 
   Check:
   * `OK`: if the node has no pending restart tag.
   * `CRITICAL`: otherwise
 
   Perfdata: `is_pending_restart` is 1 if the node has pending restart tag, 0
@@ -364,20 +452,29 @@
 ```
 
 ### node_is_replica
 
 ```
 Usage: check_patroni node_is_replica [OPTIONS]
 
-  Check if the node is a running replica with no noloadbalance tag.
+  Check if the node is a replica with no noloadbalance tag.
 
   It is possible to check if the node is synchronous or asynchronous. If
-  nothing is specified any kind of replica is accepted. When checking for a
+  nothing is specified any kind of replica is accepted.  When checking for a
   synchronous replica, it's not possible to specify a lag.
 
+  This service is using the following Patroni endpoints: replica, asynchronous
+  and synchronous. The first two implement the `lag` tag. For these endpoints
+  the state of a replica node doesn't reflect the replication state
+  (`streaming` or `in archive recovery`), we only know if it's `running`. The
+  timeline is also not checked.
+
+  Therefore, if a cluster is using asynchronous replication, it is recommended
+  to check for the lag to detect a divegence as soon as possible.
+
   Check:
   * `OK`: if the node is a running replica with noloadbalance tag and the lag is under the maximum threshold.
   * `CRITICAL`:  otherwise
 
   Perfdata: `is_replica` is 1 if the node is a running replica with
   noloadbalance tag and the lag is under the maximum threshold, 0 otherwise.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `check_patroni-1.0.0/check_patroni/cli.py` & `check_patroni-2.0.0/check_patroni/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -223,36 +223,47 @@
     critical: str,
     healthy_warning: str,
     healthy_critical: str,
 ) -> None:
     """Count the number of nodes in the cluster.
 
     \b
+    The role refers to the role of the server in the cluster. Possible values
+    are:
+    * master or leader
+    * replica
+    * standby_leader
+    * sync_standby
+    * demoted
+    * promoted
+    * uninitialized
+
+    \b
     The state refers to the state of PostgreSQL. Possible values are:
     * initializing new cluster, initdb failed
     * running custom bootstrap script, custom bootstrap failed
     * starting, start failed
     * restarting, restart failed
-    * running, streaming (for a replica V3.0.4)
+    * running, streaming, in archive recovery
     * stopping, stopped, stop failed
     * creating replica
     * crashed
 
     \b
-    The role refers to the role of the server in the cluster. Possible values
-    are:
-    * master or leader (V3.0.0+)
-    * replica
-    * demoted
-    * promoted
-    * uninitialized
+    The "healthy" checks only ensures that:
+    * a leader has the running state
+    * a standby_leader has the running or streaming (V3.0.4) state
+    * a replica or sync-standby has the running or streaming (V3.0.4) state
+
+    Since we dont check the lag or timeline, "in archive recovery" is not considered a valid state
+    for this service. See cluster_has_leader and cluster_has_replica for specialized checks.
 
     \b
     Check:
-    * Compares the number of nodes against the normal and healthy (running + streaming) nodes warning and critical thresholds.
+    * Compares the number of nodes against the normal and healthy nodes warning and critical thresholds.
     * `OK`:  If they are not provided.
 
     \b
     Perfdata:
     * `members`: the member count.
     * `healthy_members`: the running and streaming member count.
     * all the roles of the nodes in the cluster with their count (start with "role_").
@@ -281,25 +292,46 @@
 @click.pass_context
 @nagiosplugin.guarded
 def cluster_has_leader(ctx: click.Context) -> None:
     """Check if the cluster has a leader.
 
     This check applies to any kind of leaders including standby leaders.
 
+    A leader is a node with the "leader" role and a "running" state.
+
+    A standby leader is a node with a "standby_leader" role and a "streaming"
+    or "in archive recovery" state. Please note that log shipping could be
+    stuck because the WAL are not available or applicable. Patroni doesn't
+    provide information about the origin cluster (timeline or lag), so we
+    cannot check if there is a problem in that particular case. That's why we
+    issue a warning when the node is "in archive recovery". We suggest using
+    other supervision tools to do this (eg. check_pgactivity).
+
     \b
     Check:
     * `OK`: if there is a leader node.
-    * `CRITICAL`: otherwise
+    * 'WARNING': if there is a stanby leader in archive mode.
+    * `CRITICAL`: otherwise.
+
+    \b
+    Perfdata:
+    * `has_leader` is 1 if there is any kind of leader node, 0 otherwise
+    * `is_standby_leader_in_arc_rec` is 1 if the standby leader node is "in
+       archive recovery", 0 otherwise
+    * `is_standby_leader` is 1 if there is a standby leader node, 0 otherwise
+    * `is_leader` is 1 if there is a "classical" leader node, 0 otherwise
 
-    Perfdata: `has_leader` is 1 if there is a leader node, 0 otherwise
     """
     check = nagiosplugin.Check()
     check.add(
         ClusterHasLeader(ctx.obj.connection_info),
         nagiosplugin.ScalarContext("has_leader", None, "@0:0"),
+        nagiosplugin.ScalarContext("is_standby_leader_in_arc_rec", "@1:1", None),
+        nagiosplugin.ScalarContext("is_leader", None, None),
+        nagiosplugin.ScalarContext("is_standby_leader", None, None),
         ClusterHasLeaderSummary(),
     )
     check.main(verbose=ctx.obj.verbose, timeout=ctx.obj.timeout)
 
 
 @main.command(name="cluster_has_replica")
 @click.option(
@@ -338,31 +370,50 @@
     sync_warning: str,
     sync_critical: str,
     max_lag: str,
 ) -> None:
     """Check if the cluster has healthy replicas and/or if some are sync standbies
 
     \b
+    For patroni (and this check):
+    * a replica is `streaming` if the `pg_stat_wal_receiver` say's so.
+    * a replica is `in archive recovery`, if it's not `streaming` and has a `restore_command`.
+
+    \b
     A healthy replica:
-    * is in running or streaming state (V3.0.4)
-    * has a replica or sync_standby role
-    * has a lag lower or equal to max_lag
+    * has a `replica` or `sync_standby` role
+    * has the same timeline as the leader and
+      * is in `running` state (patroni < V3.0.4)
+      * is in `streaming` or `in archive recovery` state (patroni >= V3.0.4)
+    * has a lag lower or equal to `max_lag`
+
+    Please note that replica `in archive recovery` could be stuck because the WAL
+    are not available or applicable (the server's timeline has diverged for the
+    leader's). We already detect the latter but we will miss the former.
+    Therefore, it's preferable to check for the lag in addition to the healthy
+    state if you rely on log shipping to help lagging standbies to catch up.
+
+    Since we require a healthy replica to have the same timeline as the
+    leader, it's possible that we raise alerts when the cluster is performing a
+    switchover or failover and the standbies are in the process of catching up with
+    the new leader. The alert shouldn't last long.
 
     \b
     Check:
     * `OK`: if the healthy_replica count and their lag are compatible with the replica count threshold.
             and if the sync_replica count is compatible with the sync replica count threshold.
     * `WARNING` / `CRITICAL`: otherwise
 
     \b
     Perfdata:
     * healthy_replica & unhealthy_replica count
     * the number of sync_replica, they are included in the previous count
-    * the lag of each replica labelled with  "member name"_lag
-    * a boolean to tell if the node is a sync stanbdy labelled with  "member name"_sync
+    * the lag of each replica labelled with "member name"_lag
+    * the timeline of each replica labelled with "member name"_timeline
+    * a boolean to tell if the node is a sync stanbdy labelled with "member name"_sync
     """
 
     tmax_lag = size_to_byte(max_lag) if max_lag is not None else None
     check = nagiosplugin.Check()
     check.add(
         ClusterHasReplica(ctx.obj.connection_info, tmax_lag),
         nagiosplugin.ScalarContext(
@@ -373,14 +424,15 @@
         nagiosplugin.ScalarContext(
             "sync_replica",
             sync_warning,
             sync_critical,
         ),
         nagiosplugin.ScalarContext("unhealthy_replica"),
         nagiosplugin.ScalarContext("replica_lag"),
+        nagiosplugin.ScalarContext("replica_timeline"),
         nagiosplugin.ScalarContext("replica_sync"),
     )
     check.main(verbose=ctx.obj.verbose, timeout=ctx.obj.timeout)
 
 
 @main.command(name="cluster_config_has_changed")
 @click.option("--hash", "config_hash", type=str, help="A hash to compare with.")
@@ -565,18 +617,28 @@
     help="check if the replica is asynchronous",
 )
 @click.pass_context
 @nagiosplugin.guarded
 def node_is_replica(
     ctx: click.Context, max_lag: str, check_is_sync: bool, check_is_async: bool
 ) -> None:
-    """Check if the node is a running replica with no noloadbalance tag.
+    """Check if the node is a replica with no noloadbalance tag.
+
+    It is possible to check if the node is synchronous or asynchronous. If
+    nothing is specified any kind of replica is accepted.  When checking for a
+    synchronous replica, it's not possible to specify a lag.
+
+    This service is using the following Patroni endpoints: replica, asynchronous
+    and synchronous. The first two implement the `lag` tag. For these endpoints
+    the state of a replica node doesn't reflect the replication state
+    (`streaming` or `in archive recovery`), we only know if it's `running`. The
+    timeline is also not checked.
 
-    It is possible to check if the node is synchronous or asynchronous. If nothing is specified any kind of replica is accepted.
-    When checking for a synchronous replica, it's not possible to specify a lag.
+    Therefore, if a cluster is using asynchronous replication, it is
+    recommended to check for the lag to detect a divegence as soon as possible.
 
     \b
     Check:
     * `OK`: if the node is a running replica with noloadbalance tag and the lag is under the maximum threshold.
     * `CRITICAL`:  otherwise
 
     Perfdata: `is_replica` is 1 if the node is a running replica with noloadbalance tag and the lag is under the maximum threshold, 0 otherwise.
@@ -606,15 +668,15 @@
 @main.command(name="node_is_pending_restart")
 @click.pass_context
 @nagiosplugin.guarded
 def node_is_pending_restart(ctx: click.Context) -> None:
     """Check if the node is in pending restart state.
 
     This situation can arise if the configuration has been modified but
-    requiers a restart of PostgreSQL to take effect.
+    requires a restart of PostgreSQL to take effect.
 
     \b
     Check:
     * `OK`: if the node has no pending restart tag.
     * `CRITICAL`: otherwise
 
     Perfdata: `is_pending_restart` is 1 if the node has pending restart tag, 0 otherwise.
```

### Comparing `check_patroni-1.0.0/check_patroni/cluster.py` & `check_patroni-2.0.0/check_patroni/cluster.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,69 @@
 import hashlib
 import json
 from collections import Counter
-from typing import Iterable, Union
+from typing import Any, Iterable, Union
 
 import nagiosplugin
 
 from . import _log
 from .types import ConnectionInfo, PatroniResource, handle_unknown
 
 
 def replace_chars(text: str) -> str:
     return text.replace("'", "").replace(" ", "_")
 
 
 class ClusterNodeCount(PatroniResource):
-    def probe(self: "ClusterNodeCount") -> Iterable[nagiosplugin.Metric]:
+    def probe(self) -> Iterable[nagiosplugin.Metric]:
+        def debug_member(member: Any, health: str) -> None:
+            _log.debug(
+                "Node %(node_name)s is %(health)s: role %(role)s state %(state)s.",
+                {
+                    "node_name": member["name"],
+                    "health": health,
+                    "role": member["role"],
+                    "state": member["state"],
+                },
+            )
+
+        # get the cluster info
         item_dict = self.rest_api("cluster")
+
         role_counters: Counter[str] = Counter()
         roles = []
         status_counters: Counter[str] = Counter()
         statuses = []
+        healthy_member = 0
 
         for member in item_dict["members"]:
-            roles.append(replace_chars(member["role"]))
-            statuses.append(replace_chars(member["state"]))
+            state, role = member["state"], member["role"]
+            roles.append(replace_chars(role))
+            statuses.append(replace_chars(state))
+
+            if role == "leader" and state == "running":
+                healthy_member += 1
+                debug_member(member, "healthy")
+                continue
+
+            if role in ["standby_leader", "replica", "sync_standby"] and (
+                (self.has_detailed_states() and state == "streaming")
+                or (not self.has_detailed_states() and state == "running")
+            ):
+                healthy_member += 1
+                debug_member(member, "healthy")
+                continue
+
+            debug_member(member, "unhealthy")
         role_counters.update(roles)
         status_counters.update(statuses)
 
         # The actual check: members, healthy_members
         yield nagiosplugin.Metric("members", len(item_dict["members"]))
-        yield nagiosplugin.Metric(
-            "healthy_members",
-            status_counters["running"] + status_counters.get("streaming", 0),
-        )
+        yield nagiosplugin.Metric("healthy_members", healthy_member)
 
         # The performance data : role
         for role in role_counters:
             yield nagiosplugin.Metric(
                 f"role_{role}", role_counters[role], context="member_roles"
             )
 
@@ -44,118 +71,198 @@
         for state in status_counters:
             yield nagiosplugin.Metric(
                 f"state_{state}", status_counters[state], context="member_statuses"
             )
 
 
 class ClusterHasLeader(PatroniResource):
-    def probe(self: "ClusterHasLeader") -> Iterable[nagiosplugin.Metric]:
+    def probe(self) -> Iterable[nagiosplugin.Metric]:
         item_dict = self.rest_api("cluster")
 
         is_leader_found = False
+        is_standby_leader_found = False
+        is_standby_leader_in_arc_rec = False
         for member in item_dict["members"]:
-            if (
-                member["role"] in ("leader", "standby_leader")
-                and member["state"] == "running"
-            ):
+            if member["role"] == "leader" and member["state"] == "running":
                 is_leader_found = True
                 break
 
+            if member["role"] == "standby_leader":
+                if member["state"] not in ["streaming", "in archive recovery"]:
+                    # for patroni >= 3.0.4 any state would be wrong
+                    # for patroni <  3.0.4 a state different from running would be wrong
+                    if self.has_detailed_states() or member["state"] != "running":
+                        continue
+
+                if member["state"] in ["in archive recovery"]:
+                    is_standby_leader_in_arc_rec = True
+
+                is_standby_leader_found = True
+                break
         return [
             nagiosplugin.Metric(
                 "has_leader",
+                1 if is_leader_found or is_standby_leader_found else 0,
+            ),
+            nagiosplugin.Metric(
+                "is_standby_leader_in_arc_rec",
+                1 if is_standby_leader_in_arc_rec else 0,
+            ),
+            nagiosplugin.Metric(
+                "is_standby_leader",
+                1 if is_standby_leader_found else 0,
+            ),
+            nagiosplugin.Metric(
+                "is_leader",
                 1 if is_leader_found else 0,
-            )
+            ),
         ]
 
 
 class ClusterHasLeaderSummary(nagiosplugin.Summary):
-    def ok(self: "ClusterHasLeaderSummary", results: nagiosplugin.Result) -> str:
+    def ok(self, results: nagiosplugin.Result) -> str:
         return "The cluster has a running leader."
 
     @handle_unknown
-    def problem(self: "ClusterHasLeaderSummary", results: nagiosplugin.Result) -> str:
-        return "The cluster has no running leader."
+    def problem(self, results: nagiosplugin.Result) -> str:
+        return "The cluster has no running leader or the standby leader is in archive recovery."
 
 
 class ClusterHasReplica(PatroniResource):
-    def __init__(
-        self: "ClusterHasReplica",
-        connection_info: ConnectionInfo,
-        max_lag: Union[int, None],
-    ):
+    def __init__(self, connection_info: ConnectionInfo, max_lag: Union[int, None]):
         super().__init__(connection_info)
         self.max_lag = max_lag
 
-    def probe(self: "ClusterHasReplica") -> Iterable[nagiosplugin.Metric]:
-        item_dict = self.rest_api("cluster")
+    def probe(self) -> Iterable[nagiosplugin.Metric]:
+        def debug_member(member: Any, health: str) -> None:
+            _log.debug(
+                "Node %(node_name)s is %(health)s: lag %(lag)s, state %(state)s, tl %(tl)s.",
+                {
+                    "node_name": member["name"],
+                    "health": health,
+                    "lag": member["lag"],
+                    "state": member["state"],
+                    "tl": member["timeline"],
+                },
+            )
+
+        # get the cluster info
+        cluster_item_dict = self.rest_api("cluster")
 
         replicas = []
         healthy_replica = 0
         unhealthy_replica = 0
         sync_replica = 0
-        for member in item_dict["members"]:
-            # FIXME are there other acceptable states
+        leader_tl = None
+
+        # Look for replicas
+        for member in cluster_item_dict["members"]:
             if member["role"] in ["replica", "sync_standby"]:
-                # patroni 3.0.4 changed the standby state from running to streaming
-                if (
-                    member["state"] in ["running", "streaming"]
-                    and member["lag"] != "unknown"
-                ):
+                if member["lag"] == "unknown":
+                    # This could happen if the node is stopped
+                    # nagiosplugin doesn't handle strings in perfstats
+                    # so we have to ditch all the stats in that case
+                    debug_member(member, "unhealthy")
+                    unhealthy_replica += 1
+                    continue
+                else:
                     replicas.append(
                         {
                             "name": member["name"],
                             "lag": member["lag"],
+                            "timeline": member["timeline"],
                             "sync": 1 if member["role"] == "sync_standby" else 0,
                         }
                     )
 
-                    if member["role"] == "sync_standby":
-                        sync_replica += 1
+                # Get the leader tl if we haven't already
+                if leader_tl is None:
+                    # If there are no leaders, we will loop here for all
+                    # members because leader_tl will remain None. it's not
+                    # a big deal since having no leader is rare.
+                    for tmember in cluster_item_dict["members"]:
+                        if tmember["role"] == "leader":
+                            leader_tl = int(tmember["timeline"])
+                            break
 
-                    if self.max_lag is None or self.max_lag >= int(member["lag"]):
-                        healthy_replica += 1
-                        continue
-                unhealthy_replica += 1
+                    _log.debug(
+                        "Patroni's leader_timeline is %(leader_tl)s",
+                        {
+                            "leader_tl": leader_tl,
+                        },
+                    )
+
+                # Test for an unhealthy replica
+                if (
+                    self.has_detailed_states()
+                    and not (
+                        member["state"] in ["streaming", "in archive recovery"]
+                        and int(member["timeline"]) == leader_tl
+                    )
+                ) or (
+                    not self.has_detailed_states()
+                    and not (
+                        member["state"] == "running"
+                        and int(member["timeline"]) == leader_tl
+                    )
+                ):
+                    debug_member(member, "unhealthy")
+                    unhealthy_replica += 1
+                    continue
+
+                if member["role"] == "sync_standby":
+                    sync_replica += 1
+
+                if self.max_lag is None or self.max_lag >= int(member["lag"]):
+                    debug_member(member, "healthy")
+                    healthy_replica += 1
+                else:
+                    debug_member(member, "unhealthy")
+                    unhealthy_replica += 1
 
         # The actual check
         yield nagiosplugin.Metric("healthy_replica", healthy_replica)
         yield nagiosplugin.Metric("sync_replica", sync_replica)
 
         # The performance data : unhealthy replica count, replicas lag
         yield nagiosplugin.Metric("unhealthy_replica", unhealthy_replica)
         for replica in replicas:
             yield nagiosplugin.Metric(
                 f"{replica['name']}_lag", replica["lag"], context="replica_lag"
             )
             yield nagiosplugin.Metric(
+                f"{replica['name']}_timeline",
+                replica["timeline"],
+                context="replica_timeline",
+            )
+            yield nagiosplugin.Metric(
                 f"{replica['name']}_sync", replica["sync"], context="replica_sync"
             )
 
 
 # FIXME is this needed ??
 # class ClusterHasReplicaSummary(nagiosplugin.Summary):
 #     def ok(self, results):
 #     def problem(self, results):
 
 
 class ClusterConfigHasChanged(PatroniResource):
     def __init__(
-        self: "ClusterConfigHasChanged",
+        self,
         connection_info: ConnectionInfo,
         config_hash: str,  # Always contains the old hash
         state_file: str,  # Only used to update the hash in the state_file (when needed)
         save: bool = False,  # Save the configuration
     ):
         super().__init__(connection_info)
         self.state_file = state_file
         self.config_hash = config_hash
         self.save = save
 
-    def probe(self: "ClusterConfigHasChanged") -> Iterable[nagiosplugin.Metric]:
+    def probe(self) -> Iterable[nagiosplugin.Metric]:
         item_dict = self.rest_api("config")
 
         new_hash = hashlib.md5(json.dumps(item_dict).encode()).hexdigest()
 
         _log.debug("save result: %(issave)s", {"issave": self.save})
         old_hash = self.config_hash
         if self.state_file is not None and self.save:
@@ -179,44 +286,42 @@
                 "is_configuration_changed",
                 1 if new_hash != old_hash else 0,
             )
         ]
 
 
 class ClusterConfigHasChangedSummary(nagiosplugin.Summary):
-    def __init__(self: "ClusterConfigHasChangedSummary", config_hash: str) -> None:
+    def __init__(self, config_hash: str) -> None:
         self.old_config_hash = config_hash
 
     # Note: It would be helpful to display the old / new hash here. Unfortunately, it's not a metric.
     # So we only have the old / expected one.
-    def ok(self: "ClusterConfigHasChangedSummary", results: nagiosplugin.Result) -> str:
+    def ok(self, results: nagiosplugin.Result) -> str:
         return f"The hash of patroni's dynamic configuration has not changed ({self.old_config_hash})."
 
     @handle_unknown
-    def problem(
-        self: "ClusterConfigHasChangedSummary", results: nagiosplugin.Result
-    ) -> str:
+    def problem(self, results: nagiosplugin.Result) -> str:
         return f"The hash of patroni's dynamic configuration has changed. The old hash was {self.old_config_hash}."
 
 
 class ClusterIsInMaintenance(PatroniResource):
-    def probe(self: "ClusterIsInMaintenance") -> Iterable[nagiosplugin.Metric]:
+    def probe(self) -> Iterable[nagiosplugin.Metric]:
         item_dict = self.rest_api("cluster")
 
         # The actual check
         return [
             nagiosplugin.Metric(
                 "is_in_maintenance",
                 1 if "pause" in item_dict and item_dict["pause"] else 0,
             )
         ]
 
 
 class ClusterHasScheduledAction(PatroniResource):
-    def probe(self: "ClusterIsInMaintenance") -> Iterable[nagiosplugin.Metric]:
+    def probe(self) -> Iterable[nagiosplugin.Metric]:
         item_dict = self.rest_api("cluster")
 
         scheduled_switchover = 0
         scheduled_restart = 0
         if "scheduled_switchover" in item_dict:
             scheduled_switchover = 1
```

### Comparing `check_patroni-1.0.0/check_patroni/convert.py` & `check_patroni-2.0.0/check_patroni/convert.py`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/check_patroni/node.py` & `check_patroni-2.0.0/check_patroni/node.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,84 +3,79 @@
 import nagiosplugin
 
 from . import _log
 from .types import APIError, ConnectionInfo, PatroniResource, handle_unknown
 
 
 class NodeIsPrimary(PatroniResource):
-    def probe(self: "NodeIsPrimary") -> Iterable[nagiosplugin.Metric]:
+    def probe(self) -> Iterable[nagiosplugin.Metric]:
         try:
             self.rest_api("primary")
         except APIError:
             return [nagiosplugin.Metric("is_primary", 0)]
         return [nagiosplugin.Metric("is_primary", 1)]
 
 
 class NodeIsPrimarySummary(nagiosplugin.Summary):
-    def ok(self: "NodeIsPrimarySummary", results: nagiosplugin.Result) -> str:
+    def ok(self, results: nagiosplugin.Result) -> str:
         return "This node is the primary with the leader lock."
 
     @handle_unknown
-    def problem(self: "NodeIsPrimarySummary", results: nagiosplugin.Result) -> str:
+    def problem(self, results: nagiosplugin.Result) -> str:
         return "This node is not the primary with the leader lock."
 
 
 class NodeIsLeader(PatroniResource):
     def __init__(
-        self: "NodeIsLeader",
-        connection_info: ConnectionInfo,
-        check_is_standby_leader: bool,
+        self, connection_info: ConnectionInfo, check_is_standby_leader: bool
     ) -> None:
         super().__init__(connection_info)
         self.check_is_standby_leader = check_is_standby_leader
 
-    def probe(self: "NodeIsLeader") -> Iterable[nagiosplugin.Metric]:
+    def probe(self) -> Iterable[nagiosplugin.Metric]:
         apiname = "leader"
         if self.check_is_standby_leader:
             apiname = "standby-leader"
 
         try:
             self.rest_api(apiname)
         except APIError:
             return [nagiosplugin.Metric("is_leader", 0)]
         return [nagiosplugin.Metric("is_leader", 1)]
 
 
 class NodeIsLeaderSummary(nagiosplugin.Summary):
-    def __init__(
-        self: "NodeIsLeaderSummary",
-        check_is_standby_leader: bool,
-    ) -> None:
+    def __init__(self, check_is_standby_leader: bool) -> None:
         if check_is_standby_leader:
             self.leader_kind = "standby leader"
         else:
             self.leader_kind = "leader"
 
-    def ok(self: "NodeIsLeaderSummary", results: nagiosplugin.Result) -> str:
+    def ok(self, results: nagiosplugin.Result) -> str:
         return f"This node is a {self.leader_kind} node."
 
     @handle_unknown
-    def problem(self: "NodeIsLeaderSummary", results: nagiosplugin.Result) -> str:
+    def problem(self, results: nagiosplugin.Result) -> str:
         return f"This node is not a {self.leader_kind} node."
 
 
 class NodeIsReplica(PatroniResource):
     def __init__(
-        self: "NodeIsReplica",
+        self,
         connection_info: ConnectionInfo,
         max_lag: str,
         check_is_sync: bool,
         check_is_async: bool,
     ) -> None:
         super().__init__(connection_info)
         self.max_lag = max_lag
         self.check_is_sync = check_is_sync
         self.check_is_async = check_is_async
 
-    def probe(self: "NodeIsReplica") -> Iterable[nagiosplugin.Metric]:
+    def probe(self) -> Iterable[nagiosplugin.Metric]:
         try:
             if self.check_is_sync:
                 api_name = "synchronous"
             elif self.check_is_async:
                 api_name = "asynchronous"
             else:
                 api_name = "replica"
@@ -91,80 +86,73 @@
                 self.rest_api(f"{api_name}?lag={self.max_lag}")
         except APIError:
             return [nagiosplugin.Metric("is_replica", 0)]
         return [nagiosplugin.Metric("is_replica", 1)]
 
 
 class NodeIsReplicaSummary(nagiosplugin.Summary):
-    def __init__(
-        self: "NodeIsReplicaSummary",
-        lag: str,
-        check_is_sync: bool,
-        check_is_async: bool,
-    ) -> None:
+    def __init__(self, lag: str, check_is_sync: bool, check_is_async: bool) -> None:
         self.lag = lag
         if check_is_sync:
             self.replica_kind = "synchronous replica"
         elif check_is_async:
             self.replica_kind = "asynchronous replica"
         else:
             self.replica_kind = "replica"
 
-    def ok(self: "NodeIsReplicaSummary", results: nagiosplugin.Result) -> str:
+    def ok(self, results: nagiosplugin.Result) -> str:
         if self.lag is None:
             return (
                 f"This node is a running {self.replica_kind} with no noloadbalance tag."
             )
         return f"This node is a running {self.replica_kind} with no noloadbalance tag and the lag is under {self.lag}."
 
     @handle_unknown
-    def problem(self: "NodeIsReplicaSummary", results: nagiosplugin.Result) -> str:
+    def problem(self, results: nagiosplugin.Result) -> str:
         if self.lag is None:
             return f"This node is not a running {self.replica_kind} with no noloadbalance tag."
         return f"This node is not a running {self.replica_kind} with no noloadbalance tag and a lag under {self.lag}."
 
 
 class NodeIsPendingRestart(PatroniResource):
-    def probe(self: "NodeIsPendingRestart") -> Iterable[nagiosplugin.Metric]:
+    def probe(self) -> Iterable[nagiosplugin.Metric]:
         item_dict = self.rest_api("patroni")
 
         is_pending_restart = item_dict.get("pending_restart", False)
         return [
             nagiosplugin.Metric(
                 "is_pending_restart",
                 1 if is_pending_restart else 0,
             )
         ]
 
 
 class NodeIsPendingRestartSummary(nagiosplugin.Summary):
-    def ok(self: "NodeIsPendingRestartSummary", results: nagiosplugin.Result) -> str:
+    def ok(self, results: nagiosplugin.Result) -> str:
         return "This node doesn't have the pending restart flag."
 
     @handle_unknown
-    def problem(
-        self: "NodeIsPendingRestartSummary", results: nagiosplugin.Result
-    ) -> str:
+    def problem(self, results: nagiosplugin.Result) -> str:
         return "This node has the pending restart flag."
 
 
 class NodeTLHasChanged(PatroniResource):
     def __init__(
-        self: "NodeTLHasChanged",
+        self,
         connection_info: ConnectionInfo,
         timeline: str,  # Always contains the old timeline
         state_file: str,  # Only used to update the timeline in the state_file (when needed)
         save: bool,  # save timeline in state file
     ) -> None:
         super().__init__(connection_info)
         self.state_file = state_file
         self.timeline = timeline
         self.save = save
 
-    def probe(self: "NodeTLHasChanged") -> Iterable[nagiosplugin.Metric]:
+    def probe(self) -> Iterable[nagiosplugin.Metric]:
         item_dict = self.rest_api("patroni")
         new_tl = item_dict["timeline"]
 
         _log.debug("save result: %(issave)s", {"issave": self.save})
         old_tl = self.timeline
         if self.state_file is not None and self.save:
             _log.debug(
@@ -189,35 +177,31 @@
         )
 
         # The performance data : the timeline number
         yield nagiosplugin.Metric("timeline", new_tl)
 
 
 class NodeTLHasChangedSummary(nagiosplugin.Summary):
-    def __init__(self: "NodeTLHasChangedSummary", timeline: str) -> None:
+    def __init__(self, timeline: str) -> None:
         self.timeline = timeline
 
-    def ok(self: "NodeTLHasChangedSummary", results: nagiosplugin.Result) -> str:
+    def ok(self, results: nagiosplugin.Result) -> str:
         return f"The timeline is still {self.timeline}."
 
     @handle_unknown
-    def problem(self: "NodeTLHasChangedSummary", results: nagiosplugin.Result) -> str:
+    def problem(self, results: nagiosplugin.Result) -> str:
         return f"The expected timeline was {self.timeline} got {results['timeline'].metric}."
 
 
 class NodePatroniVersion(PatroniResource):
-    def __init__(
-        self: "NodePatroniVersion",
-        connection_info: ConnectionInfo,
-        patroni_version: str,
-    ) -> None:
+    def __init__(self, connection_info: ConnectionInfo, patroni_version: str) -> None:
         super().__init__(connection_info)
         self.patroni_version = patroni_version
 
-    def probe(self: "NodePatroniVersion") -> Iterable[nagiosplugin.Metric]:
+    def probe(self) -> Iterable[nagiosplugin.Metric]:
         item_dict = self.rest_api("patroni")
 
         version = item_dict["patroni"]["version"]
         _log.debug(
             "Version data: patroni version  %(version)s input version %(patroni_version)s",
             {"version": version, "patroni_version": self.patroni_version},
         )
@@ -228,36 +212,36 @@
                 "is_version_ok",
                 1 if version == self.patroni_version else 0,
             )
         ]
 
 
 class NodePatroniVersionSummary(nagiosplugin.Summary):
-    def __init__(self: "NodePatroniVersionSummary", patroni_version: str) -> None:
+    def __init__(self, patroni_version: str) -> None:
         self.patroni_version = patroni_version
 
-    def ok(self: "NodePatroniVersionSummary", results: nagiosplugin.Result) -> str:
+    def ok(self, results: nagiosplugin.Result) -> str:
         return f"Patroni's version is {self.patroni_version}."
 
     @handle_unknown
-    def problem(self: "NodePatroniVersionSummary", results: nagiosplugin.Result) -> str:
+    def problem(self, results: nagiosplugin.Result) -> str:
         # FIXME find a way to make the following work, check is perf data can be strings
         # return f"The expected patroni version was {self.patroni_version} got {results['patroni_version'].metric}."
         return f"Patroni's version is not {self.patroni_version}."
 
 
 class NodeIsAlive(PatroniResource):
-    def probe(self: "NodeIsAlive") -> Iterable[nagiosplugin.Metric]:
+    def probe(self) -> Iterable[nagiosplugin.Metric]:
         try:
             self.rest_api("liveness")
         except APIError:
             return [nagiosplugin.Metric("is_alive", 0)]
         return [nagiosplugin.Metric("is_alive", 1)]
 
 
 class NodeIsAliveSummary(nagiosplugin.Summary):
-    def ok(self: "NodeIsAliveSummary", results: nagiosplugin.Result) -> str:
+    def ok(self, results: nagiosplugin.Result) -> str:
         return "This node is alive (patroni is running)."
 
     @handle_unknown
-    def problem(self: "NodeIsAliveSummary", results: nagiosplugin.Result) -> str:
+    def problem(self, results: nagiosplugin.Result) -> str:
         return "This node is not alive (patroni is not running)."
```

### Comparing `check_patroni-1.0.0/check_patroni/types.py` & `check_patroni-2.0.0/check_patroni/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+from functools import lru_cache
 from typing import Any, Callable, List, Optional, Tuple, Union
 from urllib.parse import urlparse
 
 import attr
 import nagiosplugin
 import requests
 
@@ -24,19 +26,19 @@
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class Parameters:
     connection_info: ConnectionInfo
     timeout: int
     verbose: int
 
 
-@attr.s(auto_attribs=True, slots=True)
+@attr.s(auto_attribs=True, eq=False, slots=True)
 class PatroniResource(nagiosplugin.Resource):
     conn_info: ConnectionInfo
 
-    def rest_api(self: "PatroniResource", service: str) -> Any:
+    def rest_api(self, service: str) -> Any:
         """Try to connect to all the provided endpoints for the requested service"""
         for endpoint in self.conn_info.endpoints:
             cert: Optional[Union[Tuple[str, str], str]] = None
             verify: Optional[Union[str, bool]] = None
             if urlparse(endpoint).scheme == "https":
                 if self.conn_info.cert is not None:
                     # we can have: a key + a cert or a single file with key and cert.
@@ -67,18 +69,39 @@
             if r.status_code != 200:
                 raise APIError(
                     f"Failed to connect to {endpoint}/{service} status code {r.status_code}"
                 )
 
             try:
                 return r.json()
-            except requests.exceptions.JSONDecodeError:
+            except (json.JSONDecodeError, ValueError):
                 return None
         raise nagiosplugin.CheckError("Connection failed for all provided endpoints")
 
+    @lru_cache(maxsize=None)
+    def has_detailed_states(self) -> bool:
+        # get patroni's version to find out if the "streaming" and "in archive recovery" states are available
+        patroni_item_dict = self.rest_api("patroni")
+
+        if tuple(
+            int(v) for v in patroni_item_dict["patroni"]["version"].split(".", 2)
+        ) >= (3, 0, 4):
+            _log.debug(
+                "Patroni's version is %(version)s, more detailed states can be used to check for the health of replicas.",
+                {"version": patroni_item_dict["patroni"]["version"]},
+            )
+
+            return True
+
+        _log.debug(
+            "Patroni's version is %(version)s, the running state and the timelines must be used to check for the health of replicas.",
+            {"version": patroni_item_dict["patroni"]["version"]},
+        )
+        return False
+
 
 HandleUnknown = Callable[[nagiosplugin.Summary, nagiosplugin.Results], Any]
 
 
 def handle_unknown(func: HandleUnknown) -> HandleUnknown:
     """decorator to handle the unknown state in Summary.problem"""
```

### Comparing `check_patroni-1.0.0/check_patroni.egg-info/PKG-INFO` & `check_patroni-2.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: check-patroni
-Version: 1.0.0
-Summary: Nagios plugin to check on patroni
-Home-page: https://github.com/dalibo/check_patroni
-Author: Dalibo
-Author-email: contact@dalibo.com
-License: PostgreSQL
-Keywords: patroni nagios check
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: PostgreSQL License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: System :: Monitoring
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # check_patroni
 
 A nagios plugin for patroni.
 
 ## Features
 
 - Check presence of leader, replicas, node counts.
@@ -60,30 +41,30 @@
   cluster_has_scheduled_action  Check if the cluster has a scheduled...
   cluster_is_in_maintenance     Check if the cluster is in maintenance...
   cluster_node_count            Count the number of nodes in the cluster.
   node_is_alive                 Check if the node is alive ie patroni is...
   node_is_leader                Check if the node is a leader node.
   node_is_pending_restart       Check if the node is in pending restart...
   node_is_primary               Check if the node is the primary with the...
-  node_is_replica               Check if the node is a running replica...
+  node_is_replica               Check if the node is a replica with no...
   node_patroni_version          Check if the version is equal to the input
   node_tl_has_changed           Check if the timeline has changed.
 ```
 
 ## Install
 
 check_patroni is licensed under PostgreSQL license.
 
 ```
 $ pip install git+https://github.com/dalibo/check_patroni.git
 ```
 
 check_patroni works on python 3.6, we keep it that way because patroni also
 supports it and there are still lots of RH 7 variants around. That being said
-python 3.6 has been EOL for age and there is no support for it in the github
+python 3.6 has been EOL for ages and there is no support for it in the github
 CI.
 
 ## Support
 
 If you hit a bug or need help, open a [GitHub
 issue](https://github.com/dalibo/check_patroni/issues/new). Dalibo has no
 commitment on response time for public free support. Thanks for you
@@ -113,16 +94,16 @@
 * If `end` is omitted, infinity is assumed
 * To invert the match condition, prefix the range expression with `@`.
 
 A match is found when: `start <= VALUE <= end`.
 
 For example, the following command will raise:
 
-* a warning if there is less than 1 nodes, wich can be translated to outside of range [2;+INF[
-* a critical if there are no nodes, wich can be translated to outside of range [1;+INF[
+* a warning if there is less than 1 nodes, which can be translated to outside of range [2;+INF[
+* a critical if there are no nodes, which can be translated to outside of range [1;+INF[
 
 ```
 check_patroni -e https://10.20.199.3:8008 cluster_has_replica --warning 2: --critical 1:
 ```
 
 ## SSL
 
@@ -130,14 +111,38 @@
 
 * the server's CA certificate is not available or trusted by the client system:
   * `--ca_cert`: your certification chain `cat CA-certificate server-certificate > cabundle`
 * you have a client certificate for authenticating with Patroni's REST API:
   * `--cert_file`: your certificate or the concatenation of your certificate and private key
   * `--key_file`: your private key (optional)
 
+## Shell completion
+
+We use the [click] library which supports shell completion natively.
+
+Shell completion can be added by typing the following command or adding it to
+a file spécific to your shell of choice.
+
+* for Bash (add to `~/.bashrc`):
+  ```
+  eval "$(_CHECK_PATRONI_COMPLETE=bash_source check_patroni)"
+  ```
+* for Zsh  (add to `~/.zshrc`):
+  ```
+  eval "$(_CHECK_PATRONI_COMPLETE=zsh_source check_patroni)"
+  ```
+* for Fish (add to `~/.config/fish/completions/check_patroni.fish`):
+  ```
+  eval "$(_CHECK_PATRONI_COMPLETE=fish_source check_patroni)"
+  ```
+
+Please note that shell completion is not supported far all shell versions, for
+example only Bash versions older than 4.4 are supported.
+
+[click]: https://click.palletsprojects.com/en/8.1.x/shell-completion/
 
 ## Cluster services
 
 ### cluster_config_has_changed
 
 ```
 Usage: check_patroni cluster_config_has_changed [OPTIONS]
@@ -167,46 +172,80 @@
 ```
 Usage: check_patroni cluster_has_leader [OPTIONS]
 
   Check if the cluster has a leader.
 
   This check applies to any kind of leaders including standby leaders.
 
+  A leader is a node with the "leader" role and a "running" state.
+
+  A standby leader is a node with a "standby_leader" role and a "streaming" or
+  "in archive recovery" state. Please note that log shipping could be stuck
+  because the WAL are not available or applicable. Patroni doesn't provide
+  information about the origin cluster (timeline or lag), so we cannot check
+  if there is a problem in that particular case. That's why we issue a warning
+  when the node is "in archive recovery". We suggest using other supervision
+  tools to do this (eg. check_pgactivity).
+
   Check:
   * `OK`: if there is a leader node.
-  * `CRITICAL`: otherwise
+  * 'WARNING': if there is a stanby leader in archive mode.
+  * `CRITICAL`: otherwise.
 
-  Perfdata: `has_leader` is 1 if there is a leader node, 0 otherwise
+  Perfdata:
+  * `has_leader` is 1 if there is any kind of leader node, 0 otherwise
+  * `is_standby_leader_in_arc_rec` is 1 if the standby leader node is "in
+     archive recovery", 0 otherwise
+  * `is_standby_leader` is 1 if there is a standby leader node, 0 otherwise
+  * `is_leader` is 1 if there is a "classical" leader node, 0 otherwise
 
 Options:
   --help  Show this message and exit.
 ```
 
 ### cluster_has_replica
 
 ```
 Usage: check_patroni cluster_has_replica [OPTIONS]
 
   Check if the cluster has healthy replicas and/or if some are sync standbies
 
+  For patroni (and this check):
+  * a replica is `streaming` if the `pg_stat_wal_receiver` say's so.
+  * a replica is `in archive recovery`, if it's not `streaming` and has a `restore_command`.
+
   A healthy replica:
-  * is in running or streaming state (V3.0.4)
-  * has a replica or sync_standby role
-  * has a lag lower or equal to max_lag
+  * has a `replica` or `sync_standby` role
+  * has the same timeline as the leader and
+    * is in `running` state (patroni < V3.0.4)
+    * is in `streaming` or `in archive recovery` state (patroni >= V3.0.4)
+  * has a lag lower or equal to `max_lag`
+
+  Please note that replica `in archive recovery` could be stuck because the
+  WAL are not available or applicable (the server's timeline has diverged for
+  the leader's). We already detect the latter but we will miss the former.
+  Therefore, it's preferable to check for the lag in addition to the healthy
+  state if you rely on log shipping to help lagging standbies to catch up.
+
+  Since we require a healthy replica to have the same timeline as the leader,
+  it's possible that we raise alerts when the cluster is performing a
+  switchover or failover and the standbies are in the process of catching up
+  with the new leader. The alert shouldn't last long.
 
   Check:
   * `OK`: if the healthy_replica count and their lag are compatible with the replica count threshold.
           and if the sync_replica count is compatible with the sync replica count threshold.
   * `WARNING` / `CRITICAL`: otherwise
 
   Perfdata:
   * healthy_replica & unhealthy_replica count
   * the number of sync_replica, they are included in the previous count
-  * the lag of each replica labelled with  "member name"_lag
-  * a boolean to tell if the node is a sync stanbdy labelled with  "member name"_sync
+  * the lag of each replica labelled with "member name"_lag
+  * the timeline of each replica labelled with "member name"_timeline
+  * a boolean to tell if the node is a sync stanbdy labelled with "member name"_sync
 
 Options:
   -w, --warning TEXT    Warning threshold for the number of healthy replica
                         nodes.
   -c, --critical TEXT   Critical threshold for the number of healthy replica
                         nodes.
   --sync-warning TEXT   Warning threshold for the number of sync replica.
@@ -256,34 +295,45 @@
 ### cluster_node_count
 
 ```
 Usage: check_patroni cluster_node_count [OPTIONS]
 
   Count the number of nodes in the cluster.
 
+  The role refers to the role of the server in the cluster. Possible values
+  are:
+  * master or leader
+  * replica
+  * standby_leader
+  * sync_standby
+  * demoted
+  * promoted
+  * uninitialized
+
   The state refers to the state of PostgreSQL. Possible values are:
   * initializing new cluster, initdb failed
   * running custom bootstrap script, custom bootstrap failed
   * starting, start failed
   * restarting, restart failed
-  * running, streaming (for a replica V3.0.4)
+  * running, streaming, in archive recovery
   * stopping, stopped, stop failed
   * creating replica
   * crashed
 
-  The role refers to the role of the server in the cluster. Possible values
-  are:
-  * master or leader (V3.0.0+)
-  * replica
-  * demoted
-  * promoted
-  * uninitialized
+  The "healthy" checks only ensures that:
+  * a leader has the running state
+  * a standby_leader has the running or streaming (V3.0.4) state
+  * a replica or sync-standby has the running or streaming (V3.0.4) state
+
+  Since we dont check the lag or timeline, "in archive recovery" is not
+  considered a valid state for this service. See cluster_has_leader and
+  cluster_has_replica for specialized checks.
 
   Check:
-  * Compares the number of nodes against the normal and healthy (running + streaming) nodes warning and critical thresholds.
+  * Compares the number of nodes against the normal and healthy nodes warning and critical thresholds.
   * `OK`:  If they are not provided.
 
   Perfdata:
   * `members`: the member count.
   * `healthy_members`: the running and streaming member count.
   * all the roles of the nodes in the cluster with their count (start with "role_").
   * all the statuses of the nodes in the cluster with their count (start with "state_").
@@ -322,15 +372,15 @@
 ### node_is_pending_restart
 
 ```
 Usage: check_patroni node_is_pending_restart [OPTIONS]
 
   Check if the node is in pending restart state.
 
-  This situation can arise if the configuration has been modified but requiers
+  This situation can arise if the configuration has been modified but requires
   a restart of PostgreSQL to take effect.
 
   Check:
   * `OK`: if the node has no pending restart tag.
   * `CRITICAL`: otherwise
 
   Perfdata: `is_pending_restart` is 1 if the node has pending restart tag, 0
@@ -383,20 +433,29 @@
 ```
 
 ### node_is_replica
 
 ```
 Usage: check_patroni node_is_replica [OPTIONS]
 
-  Check if the node is a running replica with no noloadbalance tag.
+  Check if the node is a replica with no noloadbalance tag.
 
   It is possible to check if the node is synchronous or asynchronous. If
-  nothing is specified any kind of replica is accepted. When checking for a
+  nothing is specified any kind of replica is accepted.  When checking for a
   synchronous replica, it's not possible to specify a lag.
 
+  This service is using the following Patroni endpoints: replica, asynchronous
+  and synchronous. The first two implement the `lag` tag. For these endpoints
+  the state of a replica node doesn't reflect the replication state
+  (`streaming` or `in archive recovery`), we only know if it's `running`. The
+  timeline is also not checked.
+
+  Therefore, if a cluster is using asynchronous replication, it is recommended
+  to check for the lag to detect a divegence as soon as possible.
+
   Check:
   * `OK`: if the node is a running replica with noloadbalance tag and the lag is under the maximum threshold.
   * `CRITICAL`:  otherwise
 
   Perfdata: `is_replica` is 1 if the node is a running replica with
   noloadbalance tag and the lag is under the maximum threshold, 0 otherwise.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `check_patroni-1.0.0/check_patroni.egg-info/SOURCES.txt` & `check_patroni-2.0.0/check_patroni.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+.coveragerc
 .flake8
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
+RELEASE.md
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.py
 tox.ini
 check_patroni/__init__.py
 check_patroni/__main__.py
@@ -36,33 +38,39 @@
 tests/test_node_is_alive.py
 tests/test_node_is_leader.py
 tests/test_node_is_pending_restart.py
 tests/test_node_is_primary.py
 tests/test_node_is_replica.py
 tests/test_node_patroni_version.py
 tests/test_node_tl_has_changed.py
-tests/tools.py
 tests/json/cluster_config_has_changed.json
 tests/json/cluster_has_leader_ko.json
+tests/json/cluster_has_leader_ko_standby_leader.json
+tests/json/cluster_has_leader_ko_standby_leader_archiving.json
 tests/json/cluster_has_leader_ok.json
 tests/json/cluster_has_leader_ok_standby_leader.json
 tests/json/cluster_has_replica_ko.json
+tests/json/cluster_has_replica_ko_all_replica.json
 tests/json/cluster_has_replica_ko_lag.json
+tests/json/cluster_has_replica_ko_wrong_tl.json
 tests/json/cluster_has_replica_ok.json
 tests/json/cluster_has_replica_ok_lag.json
+tests/json/cluster_has_replica_patroni_verion_3.0.0.json
+tests/json/cluster_has_replica_patroni_verion_3.1.0.json
 tests/json/cluster_has_scheduled_action_ko_restart.json
 tests/json/cluster_has_scheduled_action_ko_switchover.json
 tests/json/cluster_has_scheduled_action_ok.json
 tests/json/cluster_is_in_maintenance_ko.json
 tests/json/cluster_is_in_maintenance_ko_pause_false.json
 tests/json/cluster_is_in_maintenance_ok.json
 tests/json/cluster_is_in_maintenance_ok_pause_false.json
 tests/json/cluster_node_count_critical.json
 tests/json/cluster_node_count_healthy_critical.json
 tests/json/cluster_node_count_healthy_warning.json
+tests/json/cluster_node_count_ko_in_archive_recovery.json
 tests/json/cluster_node_count_ok.json
 tests/json/cluster_node_count_warning.json
 tests/json/node_is_leader_ko.json
 tests/json/node_is_leader_ko_standby_leader.json
 tests/json/node_is_leader_ok.json
 tests/json/node_is_leader_ok_standby_leader.json
 tests/json/node_is_pending_restart_ko.json
```

### Comparing `check_patroni-1.0.0/docs/make_readme.sh` & `check_patroni-2.0.0/docs/make_readme.sh`

 * *Files 26% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 ```
 $ pip install git+https://github.com/dalibo/check_patroni.git
 ```
 
 check_patroni works on python 3.6, we keep it that way because patroni also
 supports it and there are still lots of RH 7 variants around. That being said
-python 3.6 has been EOL for age and there is no support for it in the github
+python 3.6 has been EOL for ages and there is no support for it in the github
 CI.
 
 ## Support
 
 If you hit a bug or need help, open a [GitHub
 issue](https://github.com/dalibo/check_patroni/issues/new). Dalibo has no
 commitment on response time for public free support. Thanks for you
@@ -76,16 +76,16 @@
 * If `end` is omitted, infinity is assumed
 * To invert the match condition, prefix the range expression with `@`.
 
 A match is found when: `start <= VALUE <= end`.
 
 For example, the following command will raise:
 
-* a warning if there is less than 1 nodes, wich can be translated to outside of range [2;+INF[
-* a critical if there are no nodes, wich can be translated to outside of range [1;+INF[
+* a warning if there is less than 1 nodes, which can be translated to outside of range [2;+INF[
+* a critical if there are no nodes, which can be translated to outside of range [1;+INF[
 
 ```
 check_patroni -e https://10.20.199.3:8008 cluster_has_replica --warning 2: --critical 1:
 ```
 
 ## SSL
 
@@ -93,14 +93,38 @@
 
 * the server's CA certificate is not available or trusted by the client system:
   * `--ca_cert`: your certification chain `cat CA-certificate server-certificate > cabundle`
 * you have a client certificate for authenticating with Patroni's REST API:
   * `--cert_file`: your certificate or the concatenation of your certificate and private key
   * `--key_file`: your private key (optional)
 
+## Shell completion
+
+We use the [click] library which supports shell completion natively.
+
+Shell completion can be added by typing the following command or adding it to
+a file spécific to your shell of choice.
+
+* for Bash (add to `~/.bashrc`):
+  ```
+  eval "$(_CHECK_PATRONI_COMPLETE=bash_source check_patroni)"
+  ```
+* for Zsh  (add to `~/.zshrc`):
+  ```
+  eval "$(_CHECK_PATRONI_COMPLETE=zsh_source check_patroni)"
+  ```
+* for Fish (add to `~/.config/fish/completions/check_patroni.fish`):
+  ```
+  eval "$(_CHECK_PATRONI_COMPLETE=fish_source check_patroni)"
+  ```
+
+Please note that shell completion is not supported far all shell versions, for
+example only Bash versions older than 4.4 are supported.
+
+[click]: https://click.palletsprojects.com/en/8.1.x/shell-completion/
 _EOF_
 readme
 readme "## Cluster services"
 readme
 readme "### cluster_config_has_changed"
 helpme cluster_config_has_changed
 readme "### cluster_has_leader"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `check_patroni-1.0.0/mypy.ini` & `check_patroni-2.0.0/mypy.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 [mypy]
+files = .
 show_error_codes = true
 strict = true
 exclude = build/
 
 [mypy-setup]
 ignore_errors = True
```

### Comparing `check_patroni-1.0.0/setup.py` & `check_patroni-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,23 +37,22 @@
     ],
     keywords="patroni nagios check",
     python_requires=">=3.6",
     install_requires=[
         "attrs >= 17, !=21.1",
         "requests",
         "nagiosplugin >= 1.3.2",
-        "click >= 8.0.1",
+        "click >= 7.1",
     ],
     extras_require={
         "test": [
-            "pytest",
-            "pytest-mock",
+            "importlib_metadata; python_version < '3.8'",
+            "pytest >= 6.0.2",
         ],
     },
     entry_points={
         "console_scripts": [
             "check_patroni=check_patroni.cli:main",
         ],
     },
     zip_safe=False,
 )
-
```

### Comparing `check_patroni-1.0.0/tests/json/cluster_has_leader_ko.json` & `check_patroni-2.0.0/tests/json/cluster_has_leader_ko.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/cluster_has_leader_ok.json` & `check_patroni-2.0.0/tests/json/cluster_has_leader_ok.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/cluster_has_leader_ok_standby_leader.json` & `check_patroni-2.0.0/tests/json/cluster_is_in_maintenance_ok.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9880952380952381%*

 * *Differences: {"'members'": "{0: {'role': 'leader'}}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "members": [
         {
             "api_url": "https://10.20.199.3:8008/patroni",
             "host": "10.20.199.3",
             "name": "srv1",
             "port": 5432,
-            "role": "standby_leader",
+            "role": "leader",
             "state": "running",
             "timeline": 51
         },
         {
             "api_url": "https://10.20.199.4:8008/patroni",
             "host": "10.20.199.4",
             "lag": 0,
```

### Comparing `check_patroni-1.0.0/tests/json/cluster_has_replica_ko.json` & `check_patroni-2.0.0/tests/json/cluster_has_replica_ko.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/cluster_has_replica_ko_lag.json` & `check_patroni-2.0.0/tests/json/cluster_has_replica_ko_lag.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/cluster_has_replica_ok.json` & `check_patroni-2.0.0/tests/json/cluster_has_scheduled_action_ok.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/cluster_has_replica_ok_lag.json` & `check_patroni-2.0.0/tests/json/cluster_has_replica_ok_lag.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/cluster_has_scheduled_action_ko_restart.json` & `check_patroni-2.0.0/tests/json/cluster_has_scheduled_action_ko_restart.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/cluster_has_scheduled_action_ko_switchover.json` & `check_patroni-2.0.0/tests/json/cluster_has_scheduled_action_ko_switchover.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/cluster_has_scheduled_action_ok.json` & `check_patroni-2.0.0/tests/json/cluster_has_replica_ok.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333333%*

 * *Differences: {"'members'": "{1: {'state': 'in archive recovery'}}"}*

```diff
@@ -12,15 +12,15 @@
         {
             "api_url": "https://10.20.199.4:8008/patroni",
             "host": "10.20.199.4",
             "lag": 0,
             "name": "srv2",
             "port": 5432,
             "role": "replica",
-            "state": "streaming",
+            "state": "in archive recovery",
             "timeline": 51
         },
         {
             "api_url": "https://10.20.199.5:8008/patroni",
             "host": "10.20.199.5",
             "lag": 0,
             "name": "srv3",
```

### Comparing `check_patroni-1.0.0/tests/json/cluster_is_in_maintenance_ko.json` & `check_patroni-2.0.0/tests/json/cluster_is_in_maintenance_ko.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/cluster_is_in_maintenance_ko_pause_false.json` & `check_patroni-2.0.0/tests/json/cluster_is_in_maintenance_ko_pause_false.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/cluster_is_in_maintenance_ok.json` & `check_patroni-2.0.0/tests/json/cluster_node_count_ok.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/cluster_is_in_maintenance_ok_pause_false.json` & `check_patroni-2.0.0/tests/json/cluster_is_in_maintenance_ok_pause_false.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/cluster_node_count_healthy_critical.json` & `check_patroni-2.0.0/tests/json/cluster_node_count_healthy_critical.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/cluster_node_count_ok.json` & `check_patroni-2.0.0/tests/json/cluster_has_leader_ko_standby_leader.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904763%*

 * *Differences: {"'members'": "{0: {'role': 'standby_leader', 'state': 'stopped'}}"}*

```diff
@@ -1,16 +1,16 @@
 {
     "members": [
         {
             "api_url": "https://10.20.199.3:8008/patroni",
             "host": "10.20.199.3",
             "name": "srv1",
             "port": 5432,
-            "role": "leader",
-            "state": "running",
+            "role": "standby_leader",
+            "state": "stopped",
             "timeline": 51
         },
         {
             "api_url": "https://10.20.199.4:8008/patroni",
             "host": "10.20.199.4",
             "lag": 0,
             "name": "srv2",
```

### Comparing `check_patroni-1.0.0/tests/json/node_is_leader_ko.json` & `check_patroni-2.0.0/tests/json/node_is_leader_ko.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/node_is_leader_ok.json` & `check_patroni-2.0.0/tests/json/node_is_leader_ok.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/node_is_pending_restart_ko.json` & `check_patroni-2.0.0/tests/json/node_is_pending_restart_ko.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/node_is_pending_restart_ok.json` & `check_patroni-2.0.0/tests/json/node_is_pending_restart_ok.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/node_is_primary_ok.json` & `check_patroni-2.0.0/tests/json/node_is_primary_ok.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/node_is_replica_ko.json` & `check_patroni-2.0.0/tests/json/node_is_replica_ko.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/node_patroni_version.json` & `check_patroni-2.0.0/tests/json/node_patroni_version.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/json/node_tl_has_changed.json` & `check_patroni-2.0.0/tests/json/node_tl_has_changed.json`

 * *Files identical despite different names*

### Comparing `check_patroni-1.0.0/tests/test_cluster_config_has_changed.py` & `check_patroni-2.0.0/tests/test_cluster_config_has_changed.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,165 +1,162 @@
+from pathlib import Path
+from typing import Iterator
+
 import nagiosplugin
+import pytest
 from click.testing import CliRunner
-from pytest_mock import MockerFixture
 
 from check_patroni.cli import main
 
-from .tools import here, my_mock
+from . import PatroniAPI
+
+
+@pytest.fixture(scope="module", autouse=True)
+def cluster_config_has_changed(patroni_api: PatroniAPI) -> Iterator[None]:
+    with patroni_api.routes({"config": "cluster_config_has_changed.json"}):
+        yield None
 
 
 def test_cluster_config_has_changed_ok_with_hash(
-    mocker: MockerFixture, use_old_replica_state: bool
+    runner: CliRunner, patroni_api: PatroniAPI
 ) -> None:
-    runner = CliRunner()
-
-    my_mock(mocker, "cluster_config_has_changed", 200)
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "cluster_config_has_changed",
             "--hash",
             "96b12d82571473d13e890b893734e731",
         ],
     )
     assert result.exit_code == 0
     assert (
         result.stdout
         == "CLUSTERCONFIGHASCHANGED OK - The hash of patroni's dynamic configuration has not changed (96b12d82571473d13e890b893734e731). | is_configuration_changed=0;;@1:1\n"
     )
 
 
 def test_cluster_config_has_changed_ok_with_state_file(
-    mocker: MockerFixture, use_old_replica_state: bool
+    runner: CliRunner, patroni_api: PatroniAPI, tmp_path: Path
 ) -> None:
-    runner = CliRunner()
-
-    with open(here / "cluster_config_has_changed.state_file", "w") as f:
+    state_file = tmp_path / "cluster_config_has_changed.state_file"
+    with state_file.open("w") as f:
         f.write('{"hash": "96b12d82571473d13e890b893734e731"}')
 
-    my_mock(mocker, "cluster_config_has_changed", 200)
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "cluster_config_has_changed",
             "--state-file",
-            str(here / "cluster_config_has_changed.state_file"),
+            str(state_file),
         ],
     )
     assert result.exit_code == 0
     assert (
         result.stdout
         == "CLUSTERCONFIGHASCHANGED OK - The hash of patroni's dynamic configuration has not changed (96b12d82571473d13e890b893734e731). | is_configuration_changed=0;;@1:1\n"
     )
 
 
 def test_cluster_config_has_changed_ko_with_hash(
-    mocker: MockerFixture, use_old_replica_state: bool
+    runner: CliRunner, patroni_api: PatroniAPI
 ) -> None:
-    runner = CliRunner()
-
-    my_mock(mocker, "cluster_config_has_changed", 200)
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "cluster_config_has_changed",
             "--hash",
             "96b12d82571473d13e890b8937ffffff",
         ],
     )
     assert result.exit_code == 2
     assert (
         result.stdout
         == "CLUSTERCONFIGHASCHANGED CRITICAL - The hash of patroni's dynamic configuration has changed. The old hash was 96b12d82571473d13e890b8937ffffff. | is_configuration_changed=1;;@1:1\n"
     )
 
 
 def test_cluster_config_has_changed_ko_with_state_file_and_save(
-    mocker: MockerFixture,
-    use_old_replica_state: bool,
+    runner: CliRunner, patroni_api: PatroniAPI, tmp_path: Path
 ) -> None:
-    runner = CliRunner()
-
-    with open(here / "cluster_config_has_changed.state_file", "w") as f:
+    state_file = tmp_path / "cluster_config_has_changed.state_file"
+    with state_file.open("w") as f:
         f.write('{"hash": "96b12d82571473d13e890b8937ffffff"}')
 
-    my_mock(mocker, "cluster_config_has_changed", 200)
     # test without saving the new hash
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "cluster_config_has_changed",
             "--state-file",
-            str(here / "cluster_config_has_changed.state_file"),
+            str(state_file),
         ],
     )
     assert result.exit_code == 2
     assert (
         result.stdout
         == "CLUSTERCONFIGHASCHANGED CRITICAL - The hash of patroni's dynamic configuration has changed. The old hash was 96b12d82571473d13e890b8937ffffff. | is_configuration_changed=1;;@1:1\n"
     )
 
-    cookie = nagiosplugin.Cookie(here / "cluster_config_has_changed.state_file")
+    state_file = tmp_path / "cluster_config_has_changed.state_file"
+    cookie = nagiosplugin.Cookie(state_file)
     cookie.open()
     new_config_hash = cookie.get("hash")
     cookie.close()
 
     assert new_config_hash == "96b12d82571473d13e890b8937ffffff"
 
     # test when we save the hash
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "cluster_config_has_changed",
             "--state-file",
-            str(here / "cluster_config_has_changed.state_file"),
+            str(state_file),
             "--save",
         ],
     )
     assert result.exit_code == 2
     assert (
         result.stdout
         == "CLUSTERCONFIGHASCHANGED CRITICAL - The hash of patroni's dynamic configuration has changed. The old hash was 96b12d82571473d13e890b8937ffffff. | is_configuration_changed=1;;@1:1\n"
     )
 
-    cookie = nagiosplugin.Cookie(here / "cluster_config_has_changed.state_file")
+    cookie = nagiosplugin.Cookie(state_file)
     cookie.open()
     new_config_hash = cookie.get("hash")
     cookie.close()
 
     assert new_config_hash == "96b12d82571473d13e890b893734e731"
 
 
 def test_cluster_config_has_changed_params(
-    mocker: MockerFixture, use_old_replica_state: bool
+    runner: CliRunner, patroni_api: PatroniAPI, tmp_path: Path
 ) -> None:
     # This one is placed last because it seems like the exceptions are not flushed from stderr for the next tests.
-    runner = CliRunner()
-
-    my_mock(mocker, "cluster_config_has_changed", 200)
+    fake_state_file = tmp_path / "fake_file_name.state_file"
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "cluster_config_has_changed",
             "--hash",
             "640df9f0211c791723f18fc3ed9dbb95",
             "--state-file",
-            str(here / "fake_file_name.state_file"),
+            str(fake_state_file),
         ],
     )
     assert result.exit_code == 3
     assert (
         result.stdout
         == "CLUSTERCONFIGHASCHANGED UNKNOWN: click.exceptions.UsageError: Either --hash or --state-file should be provided for this service\n"
     )
```

### Comparing `check_patroni-1.0.0/tests/test_cluster_has_scheduled_action.py` & `check_patroni-2.0.0/tests/test_cluster_has_scheduled_action.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 from click.testing import CliRunner
-from pytest_mock import MockerFixture
 
 from check_patroni.cli import main
 
-from .tools import my_mock
+from . import PatroniAPI
 
 
 def test_cluster_has_scheduled_action_ok(
-    mocker: MockerFixture, use_old_replica_state: bool
+    runner: CliRunner, patroni_api: PatroniAPI
 ) -> None:
-    runner = CliRunner()
-
-    my_mock(mocker, "cluster_has_scheduled_action_ok", 200)
-    result = runner.invoke(
-        main, ["-e", "https://10.20.199.3:8008", "cluster_has_scheduled_action"]
-    )
+    with patroni_api.routes({"cluster": "cluster_has_scheduled_action_ok.json"}):
+        result = runner.invoke(
+            main, ["-e", patroni_api.endpoint, "cluster_has_scheduled_action"]
+        )
     assert result.exit_code == 0
     assert (
         result.stdout
         == "CLUSTERHASSCHEDULEDACTION OK - has_scheduled_actions is 0 | has_scheduled_actions=0;;0 scheduled_restart=0 scheduled_switchover=0\n"
     )
 
 
 def test_cluster_has_scheduled_action_ko_switchover(
-    mocker: MockerFixture, use_old_replica_state: bool
+    runner: CliRunner, patroni_api: PatroniAPI
 ) -> None:
-    runner = CliRunner()
-
-    my_mock(mocker, "cluster_has_scheduled_action_ko_switchover", 200)
-    result = runner.invoke(
-        main, ["-e", "https://10.20.199.3:8008", "cluster_has_scheduled_action"]
-    )
+    with patroni_api.routes(
+        {"cluster": "cluster_has_scheduled_action_ko_switchover.json"}
+    ):
+        result = runner.invoke(
+            main, ["-e", patroni_api.endpoint, "cluster_has_scheduled_action"]
+        )
     assert result.exit_code == 2
     assert (
         result.stdout
         == "CLUSTERHASSCHEDULEDACTION CRITICAL - has_scheduled_actions is 1 (outside range 0:0) | has_scheduled_actions=1;;0 scheduled_restart=0 scheduled_switchover=1\n"
     )
 
 
 def test_cluster_has_scheduled_action_ko_restart(
-    mocker: MockerFixture, use_old_replica_state: bool
+    runner: CliRunner, patroni_api: PatroniAPI
 ) -> None:
-    runner = CliRunner()
-
-    my_mock(mocker, "cluster_has_scheduled_action_ko_restart", 200)
-    result = runner.invoke(
-        main, ["-e", "https://10.20.199.3:8008", "cluster_has_scheduled_action"]
-    )
+    with patroni_api.routes(
+        {"cluster": "cluster_has_scheduled_action_ko_restart.json"}
+    ):
+        result = runner.invoke(
+            main, ["-e", patroni_api.endpoint, "cluster_has_scheduled_action"]
+        )
     assert result.exit_code == 2
     assert (
         result.stdout
         == "CLUSTERHASSCHEDULEDACTION CRITICAL - has_scheduled_actions is 1 (outside range 0:0) | has_scheduled_actions=1;;0 scheduled_restart=1 scheduled_switchover=0\n"
     )
```

### Comparing `check_patroni-1.0.0/tests/test_node_is_leader.py` & `check_patroni-2.0.0/tests/test_node_is_leader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,58 @@
+from typing import Iterator
+
+import pytest
 from click.testing import CliRunner
-from pytest_mock import MockerFixture
 
 from check_patroni.cli import main
 
-from .tools import my_mock
-
+from . import PatroniAPI
 
-def test_node_is_leader_ok(mocker: MockerFixture, use_old_replica_state: bool) -> None:
-    runner = CliRunner()
 
-    my_mock(mocker, "node_is_leader_ok", 200)
-    result = runner.invoke(main, ["-e", "https://10.20.199.3:8008", "node_is_leader"])
+@pytest.fixture
+def node_is_leader_ok(patroni_api: PatroniAPI) -> Iterator[None]:
+    with patroni_api.routes(
+        {
+            "leader": "node_is_leader_ok.json",
+            "standby-leader": "node_is_leader_ok_standby_leader.json",
+        }
+    ):
+        yield None
+
+
+@pytest.mark.usefixtures("node_is_leader_ok")
+def test_node_is_leader_ok(runner: CliRunner, patroni_api: PatroniAPI) -> None:
+    result = runner.invoke(main, ["-e", patroni_api.endpoint, "node_is_leader"])
     assert result.exit_code == 0
     assert (
         result.stdout
         == "NODEISLEADER OK - This node is a leader node. | is_leader=1;;@0\n"
     )
 
-    my_mock(mocker, "node_is_leader_ok_standby_leader", 200)
     result = runner.invoke(
         main,
-        ["-e", "https://10.20.199.3:8008", "node_is_leader", "--is-standby-leader"],
+        ["-e", patroni_api.endpoint, "node_is_leader", "--is-standby-leader"],
     )
-    print(result.stdout)
     assert result.exit_code == 0
     assert (
         result.stdout
         == "NODEISLEADER OK - This node is a standby leader node. | is_leader=1;;@0\n"
     )
 
 
-def test_node_is_leader_ko(mocker: MockerFixture, use_old_replica_state: bool) -> None:
-    runner = CliRunner()
-
-    my_mock(mocker, "node_is_leader_ko", 503)
-    result = runner.invoke(main, ["-e", "https://10.20.199.3:8008", "node_is_leader"])
+def test_node_is_leader_ko(runner: CliRunner, patroni_api: PatroniAPI) -> None:
+    result = runner.invoke(main, ["-e", patroni_api.endpoint, "node_is_leader"])
     assert result.exit_code == 2
     assert (
         result.stdout
         == "NODEISLEADER CRITICAL - This node is not a leader node. | is_leader=0;;@0\n"
     )
 
-    my_mock(mocker, "node_is_leader_ko_standby_leader", 503)
     result = runner.invoke(
         main,
-        ["-e", "https://10.20.199.3:8008", "node_is_leader", "--is-standby-leader"],
+        ["-e", patroni_api.endpoint, "node_is_leader", "--is-standby-leader"],
     )
     assert result.exit_code == 2
     assert (
         result.stdout
         == "NODEISLEADER CRITICAL - This node is not a standby leader node. | is_leader=0;;@0\n"
     )
```

### Comparing `check_patroni-1.0.0/tests/test_node_is_primary.py` & `check_patroni-2.0.0/tests/test_node_is_primary.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 from click.testing import CliRunner
-from pytest_mock import MockerFixture
 
 from check_patroni.cli import main
 
-from .tools import my_mock
+from . import PatroniAPI
 
 
-def test_node_is_primary_ok(mocker: MockerFixture, use_old_replica_state: bool) -> None:
-    runner = CliRunner()
-
-    my_mock(mocker, "node_is_primary_ok", 200)
-    result = runner.invoke(main, ["-e", "https://10.20.199.3:8008", "node_is_primary"])
+def test_node_is_primary_ok(runner: CliRunner, patroni_api: PatroniAPI) -> None:
+    with patroni_api.routes({"primary": "node_is_primary_ok.json"}):
+        result = runner.invoke(main, ["-e", patroni_api.endpoint, "node_is_primary"])
     assert result.exit_code == 0
     assert (
         result.stdout
         == "NODEISPRIMARY OK - This node is the primary with the leader lock. | is_primary=1;;@0\n"
     )
 
 
-def test_node_is_primary_ko(mocker: MockerFixture, use_old_replica_state: bool) -> None:
-    runner = CliRunner()
-
-    my_mock(mocker, "node_is_primary_ko", 503)
-    result = runner.invoke(main, ["-e", "https://10.20.199.3:8008", "node_is_primary"])
+def test_node_is_primary_ko(runner: CliRunner, patroni_api: PatroniAPI) -> None:
+    result = runner.invoke(main, ["-e", patroni_api.endpoint, "node_is_primary"])
     assert result.exit_code == 2
     assert (
         result.stdout
         == "NODEISPRIMARY CRITICAL - This node is not the primary with the leader lock. | is_primary=0;;@0\n"
     )
```

### Comparing `check_patroni-1.0.0/tests/test_node_is_replica.py` & `check_patroni-2.0.0/tests/test_node_is_replica.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,172 +1,151 @@
+from typing import Iterator
+
+import pytest
 from click.testing import CliRunner
-from pytest_mock import MockerFixture
 
 from check_patroni.cli import main
 
-from .tools import my_mock
-
+from . import PatroniAPI
 
-def test_node_is_replica_ok(mocker: MockerFixture, use_old_replica_state: bool) -> None:
-    runner = CliRunner()
 
-    my_mock(mocker, "node_is_replica_ok", 200)
-    result = runner.invoke(main, ["-e", "https://10.20.199.3:8008", "node_is_replica"])
+@pytest.fixture
+def node_is_replica_ok(patroni_api: PatroniAPI) -> Iterator[None]:
+    with patroni_api.routes(
+        {
+            k: "node_is_replica_ok.json"
+            for k in ("replica", "synchronous", "asynchronous")
+        }
+    ):
+        yield None
+
+
+@pytest.mark.usefixtures("node_is_replica_ok")
+def test_node_is_replica_ok(runner: CliRunner, patroni_api: PatroniAPI) -> None:
+    result = runner.invoke(main, ["-e", patroni_api.endpoint, "node_is_replica"])
     assert result.exit_code == 0
     assert (
         result.stdout
         == "NODEISREPLICA OK - This node is a running replica with no noloadbalance tag. | is_replica=1;;@0\n"
     )
 
 
-def test_node_is_replica_ko(mocker: MockerFixture, use_old_replica_state: bool) -> None:
-    runner = CliRunner()
-
-    my_mock(mocker, "node_is_replica_ko", 503)
-    result = runner.invoke(main, ["-e", "https://10.20.199.3:8008", "node_is_replica"])
+def test_node_is_replica_ko(runner: CliRunner, patroni_api: PatroniAPI) -> None:
+    result = runner.invoke(main, ["-e", patroni_api.endpoint, "node_is_replica"])
     assert result.exit_code == 2
     assert (
         result.stdout
         == "NODEISREPLICA CRITICAL - This node is not a running replica with no noloadbalance tag. | is_replica=0;;@0\n"
     )
 
 
-def test_node_is_replica_ko_lag(
-    mocker: MockerFixture, use_old_replica_state: bool
-) -> None:
-    runner = CliRunner()
-
+def test_node_is_replica_ko_lag(runner: CliRunner, patroni_api: PatroniAPI) -> None:
     # We don't do the check ourselves, patroni does it and changes the return code
-    my_mock(mocker, "node_is_replica_ok", 503)
     result = runner.invoke(
-        main, ["-e", "https://10.20.199.3:8008", "node_is_replica", "--max-lag", "100"]
+        main, ["-e", patroni_api.endpoint, "node_is_replica", "--max-lag", "100"]
     )
     assert result.exit_code == 2
     assert (
         result.stdout
         == "NODEISREPLICA CRITICAL - This node is not a running replica with no noloadbalance tag and a lag under 100. | is_replica=0;;@0\n"
     )
 
-    my_mock(mocker, "node_is_replica_ok", 503)
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "node_is_replica",
             "--is-async",
             "--max-lag",
             "100",
         ],
     )
     assert result.exit_code == 2
     assert (
         result.stdout
         == "NODEISREPLICA CRITICAL - This node is not a running asynchronous replica with no noloadbalance tag and a lag under 100. | is_replica=0;;@0\n"
     )
 
 
-def test_node_is_replica_sync_ok(
-    mocker: MockerFixture, use_old_replica_state: bool
-) -> None:
-    runner = CliRunner()
-
+@pytest.mark.usefixtures("node_is_replica_ok")
+def test_node_is_replica_sync_ok(runner: CliRunner, patroni_api: PatroniAPI) -> None:
     # We don't do the check ourselves, patroni does it and changes the return code
-    my_mock(mocker, "node_is_replica_ok", 200)
     result = runner.invoke(
-        main, ["-e", "https://10.20.199.3:8008", "node_is_replica", "--is-sync"]
+        main, ["-e", patroni_api.endpoint, "node_is_replica", "--is-sync"]
     )
     assert result.exit_code == 0
     assert (
         result.stdout
         == "NODEISREPLICA OK - This node is a running synchronous replica with no noloadbalance tag. | is_replica=1;;@0\n"
     )
 
 
-def test_node_is_replica_sync_ko(
-    mocker: MockerFixture, use_old_replica_state: bool
-) -> None:
-    runner = CliRunner()
-
+def test_node_is_replica_sync_ko(runner: CliRunner, patroni_api: PatroniAPI) -> None:
     # We don't do the check ourselves, patroni does it and changes the return code
-    my_mock(mocker, "node_is_replica_ok", 503)
     result = runner.invoke(
-        main, ["-e", "https://10.20.199.3:8008", "node_is_replica", "--is-sync"]
+        main, ["-e", patroni_api.endpoint, "node_is_replica", "--is-sync"]
     )
     assert result.exit_code == 2
     assert (
         result.stdout
         == "NODEISREPLICA CRITICAL - This node is not a running synchronous replica with no noloadbalance tag. | is_replica=0;;@0\n"
     )
 
 
-def test_node_is_replica_async_ok(
-    mocker: MockerFixture, use_old_replica_state: bool
-) -> None:
-    runner = CliRunner()
-
+@pytest.mark.usefixtures("node_is_replica_ok")
+def test_node_is_replica_async_ok(runner: CliRunner, patroni_api: PatroniAPI) -> None:
     # We don't do the check ourselves, patroni does it and changes the return code
-    my_mock(mocker, "node_is_replica_ok", 200)
     result = runner.invoke(
-        main, ["-e", "https://10.20.199.3:8008", "node_is_replica", "--is-async"]
+        main, ["-e", patroni_api.endpoint, "node_is_replica", "--is-async"]
     )
     assert result.exit_code == 0
     assert (
         result.stdout
         == "NODEISREPLICA OK - This node is a running asynchronous replica with no noloadbalance tag. | is_replica=1;;@0\n"
     )
 
 
-def test_node_is_replica_async_ko(
-    mocker: MockerFixture, use_old_replica_state: bool
-) -> None:
-    runner = CliRunner()
-
+def test_node_is_replica_async_ko(runner: CliRunner, patroni_api: PatroniAPI) -> None:
     # We don't do the check ourselves, patroni does it and changes the return code
-    my_mock(mocker, "node_is_replica_ok", 503)
     result = runner.invoke(
-        main, ["-e", "https://10.20.199.3:8008", "node_is_replica", "--is-async"]
+        main, ["-e", patroni_api.endpoint, "node_is_replica", "--is-async"]
     )
     assert result.exit_code == 2
     assert (
         result.stdout
         == "NODEISREPLICA CRITICAL - This node is not a running asynchronous replica with no noloadbalance tag. | is_replica=0;;@0\n"
     )
 
 
-def test_node_is_replica_params(
-    mocker: MockerFixture, use_old_replica_state: bool
-) -> None:
-    runner = CliRunner()
-
+@pytest.mark.usefixtures("node_is_replica_ok")
+def test_node_is_replica_params(runner: CliRunner, patroni_api: PatroniAPI) -> None:
     # We don't do the check ourselves, patroni does it and changes the return code
-    my_mock(mocker, "node_is_replica_ok", 200)
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "node_is_replica",
             "--is-async",
             "--is-sync",
         ],
     )
     assert result.exit_code == 3
     assert (
         result.stdout
         == "NODEISREPLICA UNKNOWN: click.exceptions.UsageError: --is-sync and --is-async cannot be provided at the same time for this service\n"
     )
 
     # We don't do the check ourselves, patroni does it and changes the return code
-    my_mock(mocker, "node_is_replica_ok", 200)
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "node_is_replica",
             "--is-sync",
             "--max-lag",
             "1MB",
         ],
     )
     assert result.exit_code == 3
```

### Comparing `check_patroni-1.0.0/tests/test_node_tl_has_changed.py` & `check_patroni-2.0.0/tests/test_node_tl_has_changed.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,173 +1,173 @@
+from pathlib import Path
+from typing import Iterator
+
 import nagiosplugin
+import pytest
 from click.testing import CliRunner
-from pytest_mock import MockerFixture
 
 from check_patroni.cli import main
 
-from .tools import here, my_mock
+from . import PatroniAPI
+
+
+@pytest.fixture
+def node_tl_has_changed(patroni_api: PatroniAPI) -> Iterator[None]:
+    with patroni_api.routes({"patroni": "node_tl_has_changed.json"}):
+        yield None
 
 
+@pytest.mark.usefixtures("node_tl_has_changed")
 def test_node_tl_has_changed_ok_with_timeline(
-    mocker: MockerFixture, use_old_replica_state: bool
+    runner: CliRunner, patroni_api: PatroniAPI
 ) -> None:
-    runner = CliRunner()
-
-    my_mock(mocker, "node_tl_has_changed", 200)
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "node_tl_has_changed",
             "--timeline",
             "58",
         ],
     )
     assert result.exit_code == 0
     assert (
         result.stdout
         == "NODETLHASCHANGED OK - The timeline is still 58. | is_timeline_changed=0;;@1:1 timeline=58\n"
     )
 
 
+@pytest.mark.usefixtures("node_tl_has_changed")
 def test_node_tl_has_changed_ok_with_state_file(
-    mocker: MockerFixture, use_old_replica_state: bool
+    runner: CliRunner, patroni_api: PatroniAPI, tmp_path: Path
 ) -> None:
-    runner = CliRunner()
-
-    with open(here / "node_tl_has_changed.state_file", "w") as f:
+    state_file = tmp_path / "node_tl_has_changed.state_file"
+    with state_file.open("w") as f:
         f.write('{"timeline": 58}')
 
-    my_mock(mocker, "node_tl_has_changed", 200)
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "node_tl_has_changed",
             "--state-file",
-            str(here / "node_tl_has_changed.state_file"),
+            str(state_file),
         ],
     )
     assert result.exit_code == 0
     assert (
         result.stdout
         == "NODETLHASCHANGED OK - The timeline is still 58. | is_timeline_changed=0;;@1:1 timeline=58\n"
     )
 
 
+@pytest.mark.usefixtures("node_tl_has_changed")
 def test_node_tl_has_changed_ko_with_timeline(
-    mocker: MockerFixture, use_old_replica_state: bool
+    runner: CliRunner, patroni_api: PatroniAPI
 ) -> None:
-    runner = CliRunner()
-
-    my_mock(mocker, "node_tl_has_changed", 200)
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "node_tl_has_changed",
             "--timeline",
             "700",
         ],
     )
     assert result.exit_code == 2
     assert (
         result.stdout
         == "NODETLHASCHANGED CRITICAL - The expected timeline was 700 got 58. | is_timeline_changed=1;;@1:1 timeline=58\n"
     )
 
 
+@pytest.mark.usefixtures("node_tl_has_changed")
 def test_node_tl_has_changed_ko_with_state_file_and_save(
-    mocker: MockerFixture, use_old_replica_state: bool
+    runner: CliRunner, patroni_api: PatroniAPI, tmp_path: Path
 ) -> None:
-    runner = CliRunner()
-
-    with open(here / "node_tl_has_changed.state_file", "w") as f:
+    state_file = tmp_path / "node_tl_has_changed.state_file"
+    with state_file.open("w") as f:
         f.write('{"timeline": 700}')
 
-    my_mock(mocker, "node_tl_has_changed", 200)
     # test without saving the new tl
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "node_tl_has_changed",
             "--state-file",
-            str(here / "node_tl_has_changed.state_file"),
+            str(state_file),
         ],
     )
     assert result.exit_code == 2
     assert (
         result.stdout
         == "NODETLHASCHANGED CRITICAL - The expected timeline was 700 got 58. | is_timeline_changed=1;;@1:1 timeline=58\n"
     )
 
-    cookie = nagiosplugin.Cookie(here / "node_tl_has_changed.state_file")
+    cookie = nagiosplugin.Cookie(state_file)
     cookie.open()
     new_tl = cookie.get("timeline")
     cookie.close()
 
     assert new_tl == 700
 
     # test when we save the hash
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "node_tl_has_changed",
             "--state-file",
-            str(here / "node_tl_has_changed.state_file"),
+            str(state_file),
             "--save",
         ],
     )
     assert result.exit_code == 2
     assert (
         result.stdout
         == "NODETLHASCHANGED CRITICAL - The expected timeline was 700 got 58. | is_timeline_changed=1;;@1:1 timeline=58\n"
     )
 
-    cookie = nagiosplugin.Cookie(here / "node_tl_has_changed.state_file")
+    cookie = nagiosplugin.Cookie(state_file)
     cookie.open()
     new_tl = cookie.get("timeline")
     cookie.close()
 
     assert new_tl == 58
 
 
+@pytest.mark.usefixtures("node_tl_has_changed")
 def test_node_tl_has_changed_params(
-    mocker: MockerFixture, use_old_replica_state: bool
+    runner: CliRunner, patroni_api: PatroniAPI, tmp_path: Path
 ) -> None:
     # This one is placed last because it seems like the exceptions are not flushed from stderr for the next tests.
-    runner = CliRunner()
-
-    my_mock(mocker, "node_tl_has_changed", 200)
+    fake_state_file = tmp_path / "fake_file_name.state_file"
     result = runner.invoke(
         main,
         [
             "-e",
-            "https://10.20.199.3:8008",
+            patroni_api.endpoint,
             "node_tl_has_changed",
             "--timeline",
             "58",
             "--state-file",
-            str(here / "fake_file_name.state_file"),
+            str(fake_state_file),
         ],
     )
     assert result.exit_code == 3
     assert (
         result.stdout
         == "NODETLHASCHANGED UNKNOWN: click.exceptions.UsageError: Either --timeline or --state-file should be provided for this service\n"
     )
 
-    result = runner.invoke(
-        main, ["-e", "https://10.20.199.3:8008", "node_tl_has_changed"]
-    )
+    result = runner.invoke(main, ["-e", patroni_api.endpoint, "node_tl_has_changed"])
     assert result.exit_code == 3
     assert (
         result.stdout
         == "NODETLHASCHANGED UNKNOWN: click.exceptions.UsageError: Either --timeline or --state-file should be provided for this service\n"
     )
```

### Comparing `check_patroni-1.0.0/tox.ini` & `check_patroni-2.0.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 [tox]
 # the versions specified here are overridden by github workflow
 envlist = lint, mypy, py{37,38,39,310,311}
 skip_missing_interpreters = True
 
 [testenv]
-deps =
-    pytest
-    pytest-mock
+extras = test
 commands =
-    pytest {toxinidir}/check_patroni {toxinidir}/tests {posargs:-vv}
+    pytest {toxinidir}/check_patroni {toxinidir}/tests {posargs:-vv --log-level=debug}
 
 [testenv:lint]
 skip_install = True
 deps =
     codespell
     black
     flake8
     isort
 commands =
-    codespell {toxinidir}/check_patroni {toxinidir}/tests
+    codespell {toxinidir}/check_patroni {toxinidir}/tests {toxinidir}/docs/ {toxinidir}/RELEASE.md {toxinidir}/CONTRIBUTING.md
     black --check --diff {toxinidir}/check_patroni {toxinidir}/tests
     flake8 {toxinidir}/check_patroni {toxinidir}/tests
     isort --check --diff {toxinidir}/check_patroni {toxinidir}/tests
 
 [testenv:mypy]
 deps =
     mypy == 0.961
 commands =
     # we need to install types-requests
-    mypy --install-types --non-interactive {toxinidir}/check_patroni
+    mypy --install-types --non-interactive
 
 [testenv:build]
 deps =
     wheel
     setuptools
     twine
 allowlist_externals =
```

