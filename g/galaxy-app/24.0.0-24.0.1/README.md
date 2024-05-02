# Comparing `tmp/galaxy-app-24.0.0.tar.gz` & `tmp/galaxy_app-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-app-24.0.0.tar", last modified: Wed Apr  3 02:46:37 2024, max compression
+gzip compressed data, was "galaxy_app-24.0.1.tar", last modified: Thu May  2 13:49:42 2024, max compression
```

## Comparing `galaxy-app-24.0.0.tar` & `galaxy_app-24.0.1.tar`

### file list

```diff
@@ -1,707 +1,707 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    58057 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    60604 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.432251 galaxy-app-24.0.0/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.432251 galaxy-app-24.0.0/galaxy/actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17523 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/actions/library.py
--rw-r--r--   0 runner    (1001) docker     (127)    38970 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.432251 galaxy-app-24.0.0/galaxy/app_unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/app_unittest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/app_unittest_utils/galaxy_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/app_unittest_utils/toolbox_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/app_unittest_utils/tools_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.436251 galaxy-app-24.0.0/galaxy/authnz/
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/authnz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29236 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/authnz/custos_authnz.py
--rw-r--r--   0 runner    (1001) docker     (127)    27994 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/authnz/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22343 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/authnz/psa_authnz.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/authnz/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.436251 galaxy-app-24.0.0/galaxy/carbon_emissions/
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/carbon_emissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.436251 galaxy-app-24.0.0/galaxy/celery/
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/celery/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/celery/base_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    17119 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/celery/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/config_watchers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.436251 galaxy-app-24.0.0/galaxy/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/conditional-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/lint-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/pinned-lint-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16149 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/pinned-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/pinned-typecheck-requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3373 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/update.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      721 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/dependencies/update_lint_requirements.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/di.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.436251 galaxy-app-24.0.0/galaxy/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12593 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/forms/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.440251 galaxy-app-24.0.0/galaxy/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)   121947 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15794 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/command_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    73578 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/dynamic_tool_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    59027 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/rule_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.440251 galaxy-app-24.0.0/galaxy/jobs/rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.444251 galaxy-app-24.0.0/galaxy/jobs/runners/
--rw-r--r--   0 runner    (1001) docker     (127)    40111 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22955 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    11145 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/chronos.py
--rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/condor.py
--rw-r--r--   0 runner    (1001) docker     (127)    20985 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/drmaa.py
--rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/godocker.py
--rw-r--r--   0 runner    (1001) docker     (127)    56110 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    23554 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)    55187 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/pulsar.py
--rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/state_handler_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.444251 galaxy-app-24.0.0/galaxy/jobs/runners/state_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/state_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/state_handlers/_safe_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/state_handlers/resubmit.py
--rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    31764 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/univa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.444251 galaxy-app-24.0.0/galaxy/jobs/runners/util/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.444251 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.444251 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/slurm_torque.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/torque.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.448252 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/shell/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/shell/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/shell/rsh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.448252 galaxy-app-24.0.0/galaxy/jobs/runners/util/condor/
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/condor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/external.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/fork_safe_write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.448252 galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/CLUSTER_SLOTS_STATEMENT.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/DEFAULT_JOB_FILE_TEMPLATE.sh
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/MEMORY_STATEMENT_TEMPLATE.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/kill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/process_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/pykube_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/runners/util/sudo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.448252 galaxy-app-24.0.0/galaxy/jobs/splitters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/splitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/splitters/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/splitters/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/jobs/stock_rules.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9033 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/main_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.460252 galaxy-app-24.0.0/galaxy/managers/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/annotatable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    53644 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/citations.py
--rw-r--r--   0 runner    (1001) docker     (127)    18890 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/cloudauthzs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38419 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    12540 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/collections_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11780 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    40089 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8025 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/dbkeys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/deletable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/display_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/export_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/genomes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/group_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/group_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    28314 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/hdas.py
--rw-r--r--   0 runner    (1001) docker     (127)    11507 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/hdcas.py
--rw-r--r--   0 runner    (1001) docker     (127)    42387 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/histories.py
--rw-r--r--   0 runner    (1001) docker     (127)    28357 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/history_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/interactivetool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/item_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/job_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    45695 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/lddas.py
--rw-r--r--   0 runner    (1001) docker     (127)    16788 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/library_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)   185469 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/markdown_export_base.css
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/markdown_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    41485 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/markdown_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/model_stores.py
--rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    24542 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/quotas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/ratable.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/rbac_secured.py
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/remote_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/secured.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    22209 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/sharable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/taggable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/tool_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    38938 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/visualizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    98587 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/managers/workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/queue_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/queues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.460252 galaxy-app-24.0.0/galaxy/short_term_storage/
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/short_term_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/structured_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.460252 galaxy-app-24.0.0/galaxy/tool_shed/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.460252 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    46846 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/install_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    51730 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/installed_repository_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.460252 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/metadata/installed_repository_metadata_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.460252 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/repository_dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/repository_dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36468 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/repository_dependencies/repository_dependency_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.460252 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/tools/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    27537 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/tools/tool_panel_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/update_repository_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.464252 galaxy-app-24.0.0/galaxy/tool_shed/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55922 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/metadata/metadata_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/repository_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.464252 galaxy-app-24.0.0/galaxy/tool_shed/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/tools/data_table_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/tools/tool_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.464252 galaxy-app-24.0.0/galaxy/tool_shed/unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/unittest_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.464252 galaxy-app-24.0.0/galaxy/tool_shed/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/basic_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/container_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    17636 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/dependency_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/hg_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/metadata_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    35443 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/repository_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/shed_util_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/tool_dependency_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/tool_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    38555 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tool_shed/util/utility_container_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.472252 galaxy-app-24.0.0/galaxy/tools/
--rw-r--r--   0 runner    (1001) docker     (127)   173796 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.472252 galaxy-app-24.0.0/galaxy/tools/actions/
--rw-r--r--   0 runner    (1001) docker     (127)    61141 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/history_imp_exp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/model_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    19134 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/actions/upload_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/apply_rules.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/biotools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/build_list.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/build_list_1.2.0.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.472252 galaxy-app-24.0.0/galaxy/tools/bundled/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.472252 galaxy-app-24.0.0/galaxy/tools/bundled/data_export/
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_export/export_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_export/export_remote.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_export/send.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_export/send.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.480252 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/access_libraries.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/biomart.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/biomart_test.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/cbi_rice_mart.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ebi_sra.xml
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/eupathdb.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/fly_modencode.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/flymine.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/flymine_test.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/genbank.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/genbank.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/gramene_mart.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/hapmapmart.xml
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/hbvar.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/import.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/intermine.xml
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/metabolicmine.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/microbial_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/microbial_import.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/microbial_import_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/modmine.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/mousemine.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ncbi_datasets.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ratmine.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/sra.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser_archaea.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser_test.xml
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/upload.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/worm_modencode.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/wormbase.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/wormbase_test.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/yeastmine.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/data_source/zebrafishmine.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.480252 galaxy-app-24.0.0/galaxy/tools/bundled/expression_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/expression_tools/expression_macros.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/expression_tools/parse_values_from_file.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16734 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/expression_tools/pick_value.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.480252 galaxy-app-24.0.0/galaxy/tools/bundled/extract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/extract/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12747 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/extract/extract_genomic_dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/extract/extract_genomic_dna.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/extract/liftOver_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/extract/liftOver_wrapper.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.496252 galaxy-app-24.0.0/galaxy/tools/bundled/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/CreateInterval.pl
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/CreateInterval.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_concat_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_concat_fasta.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_fasta.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_lav.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_lav.xml
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_lav_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/bed2gff.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/bed_to_bigbed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/bed_to_gff_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/catWrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/catWrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/changeCase.pl
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/changeCase.xml
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/commWrapper.pl
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/commWrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/compare.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/condense_characters.pl
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/condense_characters.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/convert_characters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/convert_characters.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/cutWrapper.pl
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/cutWrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/fileGrep.xml
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/fixedValueColumn.pl
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/fixedValueColumn.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.496252 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/extract_GFF_Features.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/extract_GFF_Features.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff2bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff_to_bed_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/grep.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/grep.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/grep_1.0.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gtf2bedgraph.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/gtf_to_bedgraph_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/headWrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15920 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/join.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/joinWrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/joiner.xml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/joiner2.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/lav_to_bed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/lav_to_bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/lav_to_bed_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/mergeCols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/mergeCols.xml
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/pasteWrapper.pl
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/pasteWrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/random_lines_two_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/randomlines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/randomlines.xml
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/remove_beginning.pl
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/remove_beginning.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/secure_hash_message_digest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/secure_hash_message_digest.xml
--rw-r--r--   0 runner    (1001) docker     (127)    46787 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/sff_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/sff_extractor.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/sorter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/sorter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/tailWrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/trimmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/trimmer.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     5433 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2707 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     4410 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/uniq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/uniq.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/wc_gnu.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/wig_to_bigwig.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)      919 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/wiggle_to_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/filters/wiggle_to_simple.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.504252 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/default_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_askomics.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_bam_iobio.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_cellxgene_0.16.2.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_cellxgene_1.1.1.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_climate_notebook.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_ethercalc.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_geoexplorer.xml
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_guacamole_desktop.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_hicbrowser.xml
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_higlass.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_isee.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook.xml
--rw-r--r--   0 runner    (1001) docker     (127)    16488 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook_1.0.0.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_metashark.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_mgnify_notebook.xml
--rw-r--r--   0 runner    (1001) docker     (127)    15412 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_ml_jupyter_notebook.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_neo4j.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_openrefine.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_pangeo_notebook.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_panoply.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_paraview.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_pavian.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_phinch.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_pyiron.xml
--rw-r--r--   0 runner    (1001) docker     (127)    19354 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_qiskit_jupyter_notebook.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_radiant.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_rstudio.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_simtext_app.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_vcf_iobio.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_vrm_editor.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_wallace.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_wilson.xml
--rw-r--r--   0 runner    (1001) docker     (127)    28382 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/interactive/simtext_app.R
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.512252 galaxy-app-24.0.0/galaxy/tools/bundled/maf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/genebed_maf_to_fasta.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     6278 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval2maf.py
--rw-r--r--   0 runner    (1001) docker     (127)    19538 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval2maf.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval2maf_pairwise.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8936 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.xml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/macros.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_by_block_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_by_block_number.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_filter.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_size.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_to_species.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_to_species.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_reverse_complement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_reverse_complement.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_split_by_species.py
--rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_split_by_species.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_stats.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_thread_for_species.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_thread_for_species.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_bed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_bed_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_fasta.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2018 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_fasta_concat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2116 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_fasta_multiple_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_interval.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.512252 galaxy-app-24.0.0/galaxy/tools/bundled/meme/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/meme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/meme/fimo.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/meme/fimo_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    16909 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/meme/meme.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.512252 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/blat_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/blat_wrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)    28145 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_wrapper.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.516252 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2627 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/bwa_solid2fastq_modified.pl
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid2fastq.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid2fastq.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.516252 galaxy-app-24.0.0/galaxy/tools/bundled/ngs_simulation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/ngs_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/ngs_simulation/ngs_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/ngs_simulation/ngs_simulation.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.520253 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1331 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/BEAM2_wrapper.sh
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/beam.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2033 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/gpass.pl
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/gpass.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/ldtools.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1000 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/ldtools_wrapper.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1533 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToDavid.pl
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToDavid.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     2713 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToGProfile.pl
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToGProfile.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     3346 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/lped_to_geno.pl
--rw-r--r--   0 runner    (1001) docker     (127)    15041 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/lps.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1142 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/lps_tool_wrapper.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     7394 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2gd_snp.pl
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2gd_snp.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     4319 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2pg.pl
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2pg.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1389 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/mergeSnps.pl
--rwxr-xr-x   0 runner    (1001) docker     (127)     9287 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/pagetag.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/pass.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/pass_wrapper.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     7131 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/senatag.py
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/sift.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     5328 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/sift_variants_wrapper.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.520253 galaxy-app-24.0.0/galaxy/tools/bundled/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/plotting/bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/plotting/bar_chart.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/plotting/boxplot.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.520253 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13460 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.xml
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/maq_cs_wrapper_code.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3011 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/qualsolid_boxplot_graph.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/solid_qual_boxplot.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/solid_qual_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/solid_qual_stats.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.524253 galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17496 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velvetg.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velvetg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velveth.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velveth_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.524253 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)    19821 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/PerM.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19924 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/bfast_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    20856 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/bfast_wrapper.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     4977 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/fastq_statistics.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/mosaik.xml
--rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/srma_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/srma_wrapper.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.528253 galaxy-app-24.0.0/galaxy/tools/bundled/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/aggregate_binned_scores_in_intervals.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     8793 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/aggregate_scores_in_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/filtering.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/filtering_1_1_0.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/grouping.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     5492 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/gsummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/gsummary.xml
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/bundled/stats/r_wrapper.sh
--rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.528253 galaxy-app-24.0.0/galaxy/tools/data/
--rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24682 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/data_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/data_fetch.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.528253 galaxy-app-24.0.0/galaxy/tools/data_manager/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/data_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11221 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/data_manager/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/duplicate_file_to_collection.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.528253 galaxy-app-24.0.0/galaxy/tools/error_reports/
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.528253 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/base_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/github.py
--rw-r--r--   0 runner    (1001) docker     (127)    14012 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/sentry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    38958 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/exception_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)    27977 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/execute.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.528253 galaxy-app-24.0.0/galaxy/tools/expressions/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/expressions/cwlNodeEngine.js
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/expressions/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/expressions/script.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/expressions/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/extract_dataset.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/filter_empty_collection.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/filter_failed_collection.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/filter_from_file.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.528253 galaxy-app-24.0.0/galaxy/tools/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/flatten_collection.xml
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/harmonize_two_collections_list.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.532253 galaxy-app-24.0.0/galaxy/tools/imp_exp/
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/imp_exp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/imp_exp/exp_history_to_archive.xml
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/imp_exp/exp_history_to_uri.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/imp_exp/export_history.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/imp_exp/imp_history_from_archive.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/imp_exp/unpack_tar_gz_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/keep_success_collection.xml
--rw-r--r--   0 runner    (1001) docker     (127)    14158 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/merge_collection.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.532253 galaxy-app-24.0.0/galaxy/tools/parameters/
--rw-r--r--   0 runner    (1001) docker     (127)    26963 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   119986 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/cancelable_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/dataset_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    38238 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/dynamic_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    35745 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/history_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/input_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (127)    24117 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/workflow_building_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/wrapped.py
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/parameters/wrapped_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    16840 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/recommendations.py
--rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/relabel_from_file.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/remote_tool_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/repositories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.532253 galaxy-app-24.0.0/galaxy/tools/search/
--rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/sort_collection_list.xml
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/special_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/tag_collection_from_file.xml
--rw-r--r--   0 runner    (1001) docker     (127)    17886 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/unzip_collection.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.532253 galaxy-app-24.0.0/galaxy/tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.532253 galaxy-app-24.0.0/galaxy/tools/util/galaxyops/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/util/galaxyops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30671 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/util/maf_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    30444 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/tools/zip_collection.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/visualization/data_providers/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/cigar.py
--rw-r--r--   0 runner    (1001) docker     (127)    62285 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/genome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/baseparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/newickparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/nexusparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/phyloxmlparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/data_providers/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/visualization/genome/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/genome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14883 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/genomes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/visualization/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21848 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/plugins/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11707 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/plugins/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/plugins/resource_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/plugins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/visualization/tracks/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/visualization/tracks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/webhooks/
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/webhooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.536253 galaxy-app-24.0.0/galaxy/work/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/work/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/work/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.540253 galaxy-app-24.0.0/galaxy/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18797 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)   114980 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.540253 galaxy-app-24.0.0/galaxy/workflow/refactor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/refactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28870 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/refactor/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/refactor/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.540253 galaxy-app-24.0.0/galaxy/workflow/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.540253 galaxy-app-24.0.0/galaxy/workflow/reports/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/reports/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/reports/generators/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.540253 galaxy-app-24.0.0/galaxy/workflow/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/resources/example.py.sample
--rw-r--r--   0 runner    (1001) docker     (127)    31810 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    30630 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/run_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.540253 galaxy-app-24.0.0/galaxy/workflow/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/schedulers/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    17008 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/scheduling_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy/workflow/trs_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/galaxy_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    60604 2024-04-03 02:46:37.000000 galaxy-app-24.0.0/galaxy_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26467 2024-04-03 02:46:37.000000 galaxy-app-24.0.0/galaxy_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:46:37.000000 galaxy-app-24.0.0/galaxy_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 02:46:37.000000 galaxy-app-24.0.0/galaxy_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-03 02:46:37.000000 galaxy-app-24.0.0/galaxy_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 02:46:37.000000 galaxy-app-24.0.0/galaxy_app.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/galaxy_ext/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/galaxy_ext/container_monitor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/container_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/container_monitor/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/galaxy_ext/expressions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/expressions/handle_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/galaxy_ext/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/metadata/set_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/galaxy_ext/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-03 02:46:37.548253 galaxy-app-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/tool_shed_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/tool_shed_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/tool_shed_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:37.544253 galaxy-app-24.0.0/tool_shed_client/schema/
--rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/tool_shed_client/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/tool_shed_client/schema/trs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/tool_shed_client/schema/trs_service_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-03 02:43:42.000000 galaxy-app-24.0.0/tool_shed_client/trs_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.550216 galaxy_app-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    62224 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    64771 2024-05-02 13:49:42.550216 galaxy_app-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.438216 galaxy_app-24.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.438216 galaxy_app-24.0.1/galaxy/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17523 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/actions/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38970 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.438216 galaxy_app-24.0.1/galaxy/app_unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/app_unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/app_unittest_utils/galaxy_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/app_unittest_utils/toolbox_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/app_unittest_utils/tools_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.442216 galaxy_app-24.0.1/galaxy/authnz/
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/authnz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29236 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/authnz/custos_authnz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27965 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/authnz/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22343 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/authnz/psa_authnz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/authnz/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.442216 galaxy_app-24.0.1/galaxy/carbon_emissions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/carbon_emissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.442216 galaxy_app-24.0.1/galaxy/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/celery/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/celery/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17119 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/celery/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/config_watchers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.442216 galaxy_app-24.0.1/galaxy/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/dependencies/conditional-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/dependencies/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/dependencies/lint-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/dependencies/pinned-lint-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16149 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/dependencies/pinned-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/dependencies/pinned-typecheck-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3373 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/dependencies/update.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      721 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/dependencies/update_lint_requirements.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/di.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.442216 galaxy_app-24.0.1/galaxy/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12593 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/forms/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.446215 galaxy_app-24.0.1/galaxy/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)   121947 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15794 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/command_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    73578 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/dynamic_tool_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59015 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8854 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/rule_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.446215 galaxy_app-24.0.1/galaxy/jobs/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.450215 galaxy_app-24.0.1/galaxy/jobs/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)    40111 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22955 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11145 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/chronos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13833 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/condor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20985 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/drmaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/godocker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56110 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23554 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55187 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/pulsar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/state_handler_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.450215 galaxy_app-24.0.1/galaxy/jobs/runners/state_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/state_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/state_handlers/_safe_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/state_handlers/resubmit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11622 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31764 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/univa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.450215 galaxy_app-24.0.1/galaxy/jobs/runners/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.450215 galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.450215 galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/job/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/job/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/job/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/job/slurm_torque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/job/torque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.454216 galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/shell/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/shell/rsh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.454216 galaxy_app-24.0.1/galaxy/jobs/runners/util/condor/
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/condor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/fork_safe_write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.454216 galaxy_app-24.0.1/galaxy/jobs/runners/util/job_script/
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/job_script/CLUSTER_SLOTS_STATEMENT.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/job_script/DEFAULT_JOB_FILE_TEMPLATE.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/job_script/MEMORY_STATEMENT_TEMPLATE.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/job_script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/kill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/process_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/pykube_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/runners/util/sudo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.454216 galaxy_app-24.0.1/galaxy/jobs/splitters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/splitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/splitters/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/splitters/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/jobs/stock_rules.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9033 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/main_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.466216 galaxy_app-24.0.1/galaxy/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/annotatable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53644 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/citations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18890 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/cloudauthzs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38429 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12756 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/collections_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11780 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40089 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8025 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/dbkeys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/deletable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/display_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/export_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/genomes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28302 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/hdas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11507 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/hdcas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42387 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/histories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28359 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/history_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/interactivetool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/item_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/job_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45695 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/lddas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16788 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/library_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)   185469 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/licenses.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/markdown_export_base.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/markdown_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41485 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/markdown_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/model_stores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24542 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/quotas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/ratable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/rbac_secured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/remote_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/secured.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22209 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/sharable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/taggable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/tool_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38938 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7272 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98745 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/managers/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/queue_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/queues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.466216 galaxy_app-24.0.1/galaxy/short_term_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/short_term_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/structured_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.466216 galaxy_app-24.0.1/galaxy/tool_shed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.466216 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46846 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/install_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51730 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/installed_repository_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.466216 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/metadata/installed_repository_metadata_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.466216 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/repository_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/repository_dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36468 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/repository_dependencies/repository_dependency_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.466216 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/tools/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27537 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/tools/tool_panel_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/update_repository_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.470216 galaxy_app-24.0.1/galaxy/tool_shed/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55922 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/metadata/metadata_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/repository_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.470216 galaxy_app-24.0.1/galaxy/tool_shed/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/tools/data_table_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/tools/tool_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.470216 galaxy_app-24.0.1/galaxy/tool_shed/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/unittest_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.470216 galaxy_app-24.0.1/galaxy/tool_shed/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/util/basic_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/util/container_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17636 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/util/dependency_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/util/hg_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/util/metadata_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35540 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/util/repository_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/util/shed_util_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/util/tool_dependency_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/util/tool_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38555 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tool_shed/util/utility_container_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.478216 galaxy_app-24.0.1/galaxy/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)   174122 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.478216 galaxy_app-24.0.1/galaxy/tools/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)    61557 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/actions/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/actions/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7074 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/actions/history_imp_exp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/actions/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/actions/model_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/actions/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19051 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/actions/upload_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/apply_rules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/biotools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/build_list.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/build_list_1.2.0.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.482216 galaxy_app-24.0.1/galaxy/tools/bundled/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.482216 galaxy_app-24.0.1/galaxy/tools/bundled/data_export/
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_export/export_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_export/export_remote.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_export/send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_export/send.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.486216 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/access_libraries.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/biomart.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/biomart_test.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/cbi_rice_mart.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/ebi_sra.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/eupathdb.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/fly_modencode.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/flymine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/flymine_test.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/genbank.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/genbank.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/gramene_mart.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/hapmapmart.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/hbvar.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/import.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/intermine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/metabolicmine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/microbial_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/microbial_import.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/microbial_import_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/modmine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/mousemine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/ncbi_datasets.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/ratmine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/sra.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser_archaea.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser_test.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/upload.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/worm_modencode.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/wormbase.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/wormbase_test.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/yeastmine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/data_source/zebrafishmine.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.486216 galaxy_app-24.0.1/galaxy/tools/bundled/expression_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/expression_tools/expression_macros.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/expression_tools/parse_values_from_file.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16734 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/expression_tools/pick_value.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.490216 galaxy_app-24.0.1/galaxy/tools/bundled/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/extract/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12747 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/extract/extract_genomic_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/extract/extract_genomic_dna.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/extract/liftOver_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/extract/liftOver_wrapper.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.502216 galaxy_app-24.0.1/galaxy/tools/bundled/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/CreateInterval.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/CreateInterval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/axt_to_concat_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/axt_to_concat_fasta.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/axt_to_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/axt_to_fasta.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/axt_to_lav.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/axt_to_lav.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/axt_to_lav_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/bed2gff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/bed_to_bigbed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/bed_to_gff_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/catWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/catWrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/changeCase.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/changeCase.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/commWrapper.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/commWrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/compare.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/condense_characters.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/condense_characters.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/convert_characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/convert_characters.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/cutWrapper.pl
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/cutWrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/fileGrep.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/fixedValueColumn.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/fixedValueColumn.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.502216 galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/extract_GFF_Features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/extract_GFF_Features.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff2bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff_to_bed_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/grep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/grep.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/grep_1.0.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/gtf2bedgraph.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/gtf_to_bedgraph_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/headWrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15920 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/joinWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/joiner.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/joiner2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/lav_to_bed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/lav_to_bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/lav_to_bed_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/mergeCols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/mergeCols.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/pasteWrapper.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/pasteWrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/random_lines_two_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/randomlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/randomlines.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/remove_beginning.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/remove_beginning.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/secure_hash_message_digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/secure_hash_message_digest.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    46787 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/sff_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/sff_extractor.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/sorter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/sorter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/tailWrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/trimmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/trimmer.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5433 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2707 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4410 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/uniq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/uniq.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/wc_gnu.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/wig_to_bigwig.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      919 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/wiggle_to_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/filters/wiggle_to_simple.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.510216 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/default_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_askomics.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_bam_iobio.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_cellxgene_0.16.2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_cellxgene_1.1.1.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_climate_notebook.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_ethercalc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_geoexplorer.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_guacamole_desktop.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_hicbrowser.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_higlass.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_isee.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    16488 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook_1.0.0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_metashark.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_mgnify_notebook.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    15412 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_ml_jupyter_notebook.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_neo4j.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_openrefine.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_pangeo_notebook.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_panoply.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_paraview.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_pavian.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_phinch.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_pyiron.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    19354 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_qiskit_jupyter_notebook.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_radiant.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_rstudio.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_simtext_app.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_vcf_iobio.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_vrm_editor.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_wallace.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_wilson.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    28382 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/interactive/simtext_app.R
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.514216 galaxy_app-24.0.1/galaxy/tools/bundled/maf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/genebed_maf_to_fasta.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6278 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/interval2maf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19538 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/interval2maf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/interval2maf_pairwise.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8936 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/macros.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_by_block_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_by_block_number.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11781 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_filter.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_limit_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_limit_size.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_limit_to_species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_limit_to_species.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_reverse_complement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_reverse_complement.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_split_by_species.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_split_by_species.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_stats.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_thread_for_species.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_thread_for_species.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_bed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_bed_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_fasta.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2018 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_fasta_concat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2116 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_fasta_multiple_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_interval.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.518216 galaxy_app-24.0.1/galaxy/tools/bundled/meme/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/meme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/meme/fimo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/meme/fimo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16909 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/meme/meme.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.518216 galaxy_app-24.0.1/galaxy/tools/bundled/metag_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/metag_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/metag_tools/blat_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/metag_tools/blat_wrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    28145 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/metag_tools/shrimp_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/metag_tools/shrimp_wrapper.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.518216 galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2627 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/bwa_solid2fastq_modified.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/solid2fastq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/solid2fastq.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.518216 galaxy_app-24.0.1/galaxy/tools/bundled/ngs_simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/ngs_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/ngs_simulation/ngs_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/ngs_simulation/ngs_simulation.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.526216 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1331 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/BEAM2_wrapper.sh
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/beam.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2033 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/gpass.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/gpass.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/ldtools.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1000 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/ldtools_wrapper.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1533 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/linkToDavid.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/linkToDavid.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2713 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/linkToGProfile.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/linkToGProfile.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3346 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/lped_to_geno.pl
+-rw-r--r--   0 runner    (1001) docker     (127)    15041 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/lps.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1142 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/lps_tool_wrapper.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7394 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/master2gd_snp.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/master2gd_snp.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4319 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/master2pg.pl
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/master2pg.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1389 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/mergeSnps.pl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9287 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/pagetag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/pass.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/pass_wrapper.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7131 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/senatag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/sift.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5328 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/sift_variants_wrapper.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.526216 galaxy_app-24.0.1/galaxy/tools/bundled/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/plotting/bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/plotting/bar_chart.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/plotting/boxplot.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.526216 galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13460 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/maq_cs_wrapper_code.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3011 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/qualsolid_boxplot_graph.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/solid_qual_boxplot.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/solid_qual_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/solid_qual_stats.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.526216 galaxy_app-24.0.1/galaxy/tools/bundled/sr_assembly/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/sr_assembly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17496 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/sr_assembly/velvetg.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/sr_assembly/velvetg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/sr_assembly/velveth.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/sr_assembly/velveth_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.530216 galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)    19821 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/PerM.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19924 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/bfast_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20856 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/bfast_wrapper.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4977 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/fastq_statistics.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/mosaik.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    10175 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/srma_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11238 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/srma_wrapper.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.530216 galaxy_app-24.0.1/galaxy/tools/bundled/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/stats/aggregate_binned_scores_in_intervals.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8793 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/stats/aggregate_scores_in_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/stats/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/stats/filtering.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/stats/filtering_1_1_0.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/stats/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/stats/grouping.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5492 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/stats/gsummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/stats/gsummary.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/bundled/stats/r_wrapper.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.530216 galaxy_app-24.0.1/galaxy/tools/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24682 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/data_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/data_fetch.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.530216 galaxy_app-24.0.1/galaxy/tools/data_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/data_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11221 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/data_manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/duplicate_file_to_collection.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.530216 galaxy_app-24.0.1/galaxy/tools/error_reports/
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/error_reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.534216 galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/base_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14012 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39014 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/exception_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27986 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/execute.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.534216 galaxy_app-24.0.1/galaxy/tools/expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/expressions/cwlNodeEngine.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/expressions/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/expressions/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/expressions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/extract_dataset.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/filter_empty_collection.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/filter_failed_collection.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/filter_from_file.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.534216 galaxy_app-24.0.1/galaxy/tools/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/flatten_collection.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/harmonize_two_collections_list.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.534216 galaxy_app-24.0.1/galaxy/tools/imp_exp/
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/imp_exp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/imp_exp/exp_history_to_archive.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/imp_exp/exp_history_to_uri.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/imp_exp/export_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/imp_exp/imp_history_from_archive.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/imp_exp/unpack_tar_gz_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/keep_success_collection.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    14158 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/merge_collection.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.538216 galaxy_app-24.0.1/galaxy/tools/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)    27147 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119181 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/parameters/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/parameters/cancelable_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/parameters/dataset_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38533 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/parameters/dynamic_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35766 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/parameters/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/parameters/history_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/parameters/input_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/parameters/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/parameters/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24209 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/parameters/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/parameters/workflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/parameters/wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/parameters/wrapped_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16831 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/recommendations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/relabel_from_file.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/remote_tool_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.538216 galaxy_app-24.0.1/galaxy/tools/search/
+-rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/sort_collection_list.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/special_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/tag_collection_from_file.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    17886 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/unzip_collection.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.538216 galaxy_app-24.0.1/galaxy/tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.538216 galaxy_app-24.0.1/galaxy/tools/util/galaxyops/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/util/galaxyops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30671 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/util/maf_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30444 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/tools/zip_collection.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.538216 galaxy_app-24.0.1/galaxy/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.538216 galaxy_app-24.0.1/galaxy/visualization/data_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/data_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7424 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/data_providers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/data_providers/cigar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62285 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/data_providers/genome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.542216 galaxy_app-24.0.1/galaxy/visualization/data_providers/phyloviz/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/data_providers/phyloviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/data_providers/phyloviz/baseparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/data_providers/phyloviz/newickparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/data_providers/phyloviz/nexusparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/data_providers/phyloviz/phyloxmlparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/data_providers/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.542216 galaxy_app-24.0.1/galaxy/visualization/genome/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/genome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14883 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/genomes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.542216 galaxy_app-24.0.1/galaxy/visualization/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21848 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/plugins/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11707 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12802 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/plugins/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/plugins/resource_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/plugins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.542216 galaxy_app-24.0.1/galaxy/visualization/tracks/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/visualization/tracks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.542216 galaxy_app-24.0.1/galaxy/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/webhooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.542216 galaxy_app-24.0.1/galaxy/work/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/work/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/work/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.546216 galaxy_app-24.0.1/galaxy/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18797 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114184 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.546216 galaxy_app-24.0.1/galaxy/workflow/refactor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/refactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28916 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/refactor/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/refactor/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.546216 galaxy_app-24.0.1/galaxy/workflow/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.546216 galaxy_app-24.0.1/galaxy/workflow/reports/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/reports/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/reports/generators/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.546216 galaxy_app-24.0.1/galaxy/workflow/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/resources/example.py.sample
+-rw-r--r--   0 runner    (1001) docker     (127)    31810 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30630 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/run_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.546216 galaxy_app-24.0.1/galaxy/workflow/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/schedulers/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17008 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/scheduling_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy/workflow/trs_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.550216 galaxy_app-24.0.1/galaxy_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    64771 2024-05-02 13:49:42.000000 galaxy_app-24.0.1/galaxy_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26458 2024-05-02 13:49:42.000000 galaxy_app-24.0.1/galaxy_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:49:42.000000 galaxy_app-24.0.1/galaxy_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 13:49:42.000000 galaxy_app-24.0.1/galaxy_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-02 13:49:42.000000 galaxy_app-24.0.1/galaxy_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 13:49:42.000000 galaxy_app-24.0.1/galaxy_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.546216 galaxy_app-24.0.1/galaxy_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy_ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.546216 galaxy_app-24.0.1/galaxy_ext/container_monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy_ext/container_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy_ext/container_monitor/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.550216 galaxy_app-24.0.1/galaxy_ext/expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy_ext/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy_ext/expressions/handle_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.550216 galaxy_app-24.0.1/galaxy_ext/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy_ext/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy_ext/metadata/set_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/galaxy_ext/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-02 13:49:42.550216 galaxy_app-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.550216 galaxy_app-24.0.1/tool_shed_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/tool_shed_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/tool_shed_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:42.550216 galaxy_app-24.0.1/tool_shed_client/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/tool_shed_client/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/tool_shed_client/schema/trs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/tool_shed_client/schema/trs_service_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-02 13:46:45.000000 galaxy_app-24.0.1/tool_shed_client/trs_util.py
```

### Comparing `galaxy-app-24.0.0/HISTORY.rst` & `galaxy_app-24.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,142 @@
+Metadata-Version: 2.1
+Name: galaxy-app
+Version: 24.0.1
+Summary: Galaxy application (backend)
+Home-page: https://github.com/galaxyproject/galaxy
+Author: Galaxy Project and Community
+Author-email: galaxy-committers@lists.galaxyproject.org
+License: AFL
+Keywords: Galaxy
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Academic Free License (AFL)
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: galaxy-auth
+Requires-Dist: galaxy-config
+Requires-Dist: galaxy-data
+Requires-Dist: galaxy-files
+Requires-Dist: galaxy-job-execution
+Requires-Dist: galaxy-job-metrics
+Requires-Dist: galaxy-objectstore
+Requires-Dist: galaxy-tool-util[cwl,edam]
+Requires-Dist: galaxy-tours
+Requires-Dist: galaxy-util
+Requires-Dist: galaxy-web-framework
+Requires-Dist: galaxy-web-stack
+Requires-Dist: Beaker
+Requires-Dist: boltons
+Requires-Dist: bx-python
+Requires-Dist: celery
+Requires-Dist: cloudauthz==0.6.0
+Requires-Dist: dparse
+Requires-Dist: gxformat2
+Requires-Dist: kombu>=5.3
+Requires-Dist: lagom
+Requires-Dist: lxml!=4.2.2
+Requires-Dist: Mako
+Requires-Dist: Markdown
+Requires-Dist: MarkupSafe
+Requires-Dist: packaging
+Requires-Dist: paramiko!=2.9.0,!=2.9.1
+Requires-Dist: pebble
+Requires-Dist: pulsar-galaxy-lib>=0.15.0.dev0
+Requires-Dist: pydantic!=2.6.0,!=2.6.1,>=2
+Requires-Dist: pysam>=0.21
+Requires-Dist: PyJWT
+Requires-Dist: PyYAML
+Requires-Dist: refgenconf>=0.12.0
+Requires-Dist: regex
+Requires-Dist: requests
+Requires-Dist: SQLAlchemy<2,>=1.4.25
+Requires-Dist: sqlitedict
+Requires-Dist: starlette
+Requires-Dist: svgwrite
+Requires-Dist: typing-extensions
+Requires-Dist: WebOb
+Requires-Dist: Whoosh
+
+
+.. image:: https://badge.fury.io/py/galaxy-app.svg
+   :target: https://pypi.org/project/galaxy-app/
+
+
+Overview
+--------
+
+The Galaxy_ application logic (backend).
+
+* Code: https://github.com/galaxyproject/galaxy
+
+.. _Galaxy: http://galaxyproject.org/
+
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix tool version switch in editor by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17858 <https://github.com/galaxyproject/galaxy/pull/17858>`_
+* Fix workflow run form failing on certain histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17869 <https://github.com/galaxyproject/galaxy/pull/17869>`_
+* Always serialize element_count and populated when listing contents by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17890 <https://github.com/galaxyproject/galaxy/pull/17890>`_
+* Fix saving workflows with freehand_comments only by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17901 <https://github.com/galaxyproject/galaxy/pull/17901>`_
+* Always discard session after __handle_waiting_jobs is done by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17913 <https://github.com/galaxyproject/galaxy/pull/17913>`_
+* Fix workflow run form for workflows with null rename PJA by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17929 <https://github.com/galaxyproject/galaxy/pull/17929>`_
+* Revert unnecessary error change by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17948 <https://github.com/galaxyproject/galaxy/pull/17948>`_
+* Fix missing implicit conversion for mapped over jobs by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17952 <https://github.com/galaxyproject/galaxy/pull/17952>`_
+* Fix get_content_as_text for compressed text datatypes by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17976 <https://github.com/galaxyproject/galaxy/pull/17976>`_
+* Backport: Fix bug: call unique() on result, not select stmt by `@jdavcs <https://github.com/jdavcs>`_ in `#17981 <https://github.com/galaxyproject/galaxy/pull/17981>`_
+* Fix `LengthValidator` if no value passed by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17983 <https://github.com/galaxyproject/galaxy/pull/17983>`_
+* Raise ``RequestParameterInvalidException`` if collection element has unknown extension by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17985 <https://github.com/galaxyproject/galaxy/pull/17985>`_
+* Don't attempt to commit in dry_run mode by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17987 <https://github.com/galaxyproject/galaxy/pull/17987>`_
+* Don't fail if reporting invalid parameter values by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18002 <https://github.com/galaxyproject/galaxy/pull/18002>`_
+* Include exception info when something goes wrong while refreshing tokens by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18008 <https://github.com/galaxyproject/galaxy/pull/18008>`_
+* Avoid exception when opening apply rules tool and no collection in history by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18011 <https://github.com/galaxyproject/galaxy/pull/18011>`_
+* Don't commit without having set a hid by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18014 <https://github.com/galaxyproject/galaxy/pull/18014>`_
+* Raise appropriate exception if user forces a collection that is not populated with elements as input by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18023 <https://github.com/galaxyproject/galaxy/pull/18023>`_
+* Fix tag regex pattern by `@jdavcs <https://github.com/jdavcs>`_ in `#18025 <https://github.com/galaxyproject/galaxy/pull/18025>`_
+* Fix History Dataset Association creation so that hid is always set by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18036 <https://github.com/galaxyproject/galaxy/pull/18036>`_
+* Change wrong quota_source value from KeyError to ValueError by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18040 <https://github.com/galaxyproject/galaxy/pull/18040>`_
+* Check database connection to issue a rollback if no connection by `@jdavcs <https://github.com/jdavcs>`_ in `#18070 <https://github.com/galaxyproject/galaxy/pull/18070>`_
+
+============
+Enhancements
+============
+
+* Fix remote files sources error handling by `@davelopez <https://github.com/davelopez>`_ in `#18027 <https://github.com/galaxyproject/galaxy/pull/18027>`_
+
+=============
+Other changes
+=============
+
+* Drop left-over debug statement by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17939 <https://github.com/galaxyproject/galaxy/pull/17939>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
@@ -42,15 +171,15 @@
 * Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
 * Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
 * Toward declarative help for Galaxy markdown directives. by `@jmchilton <https://github.com/jmchilton>`_ in `#16979 <https://github.com/galaxyproject/galaxy/pull/16979>`_
 * Extend regex groups in stdio regex matches by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17016 <https://github.com/galaxyproject/galaxy/pull/17016>`_
 * Vueify Admin User Grid by `@guerler <https://github.com/guerler>`_ in `#17030 <https://github.com/galaxyproject/galaxy/pull/17030>`_
 * Remove web framework dependency from tools by `@davelopez <https://github.com/davelopez>`_ in `#17058 <https://github.com/galaxyproject/galaxy/pull/17058>`_
 * Add select parameter with options from remote resources by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17087 <https://github.com/galaxyproject/galaxy/pull/17087>`_
-*  Expose more tool information / navigability in UI. by `@jmchilton <https://github.com/jmchilton>`_ in `#17105 <https://github.com/galaxyproject/galaxy/pull/17105>`_
+* Expose more tool information / navigability in UI. by `@jmchilton <https://github.com/jmchilton>`_ in `#17105 <https://github.com/galaxyproject/galaxy/pull/17105>`_
 * Vueify Admin Roles Grid by `@guerler <https://github.com/guerler>`_ in `#17118 <https://github.com/galaxyproject/galaxy/pull/17118>`_
 * SA2.0 updates: handling "object is being merged into a Session along the backref cascade path" by `@jdavcs <https://github.com/jdavcs>`_ in `#17122 <https://github.com/galaxyproject/galaxy/pull/17122>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17123 <https://github.com/galaxyproject/galaxy/pull/17123>`_
 * Vueify Admin Groups Grid by `@guerler <https://github.com/guerler>`_ in `#17126 <https://github.com/galaxyproject/galaxy/pull/17126>`_
 * Towards SQLAlchemy 2.0: fix last cases of RemovedIn20Warning by `@jdavcs <https://github.com/jdavcs>`_ in `#17132 <https://github.com/galaxyproject/galaxy/pull/17132>`_
 * Vueify Admin Forms and Quota grids by `@guerler <https://github.com/guerler>`_ in `#17141 <https://github.com/galaxyproject/galaxy/pull/17141>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17157 <https://github.com/galaxyproject/galaxy/pull/17157>`_
```

### Comparing `galaxy-app-24.0.0/LICENSE` & `galaxy_app-24.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/PKG-INFO` & `galaxy_app-24.0.1/galaxy_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-app
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy application (backend)
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -85,14 +85,58 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix tool version switch in editor by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17858 <https://github.com/galaxyproject/galaxy/pull/17858>`_
+* Fix workflow run form failing on certain histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17869 <https://github.com/galaxyproject/galaxy/pull/17869>`_
+* Always serialize element_count and populated when listing contents by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17890 <https://github.com/galaxyproject/galaxy/pull/17890>`_
+* Fix saving workflows with freehand_comments only by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17901 <https://github.com/galaxyproject/galaxy/pull/17901>`_
+* Always discard session after __handle_waiting_jobs is done by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17913 <https://github.com/galaxyproject/galaxy/pull/17913>`_
+* Fix workflow run form for workflows with null rename PJA by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17929 <https://github.com/galaxyproject/galaxy/pull/17929>`_
+* Revert unnecessary error change by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17948 <https://github.com/galaxyproject/galaxy/pull/17948>`_
+* Fix missing implicit conversion for mapped over jobs by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17952 <https://github.com/galaxyproject/galaxy/pull/17952>`_
+* Fix get_content_as_text for compressed text datatypes by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17976 <https://github.com/galaxyproject/galaxy/pull/17976>`_
+* Backport: Fix bug: call unique() on result, not select stmt by `@jdavcs <https://github.com/jdavcs>`_ in `#17981 <https://github.com/galaxyproject/galaxy/pull/17981>`_
+* Fix `LengthValidator` if no value passed by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17983 <https://github.com/galaxyproject/galaxy/pull/17983>`_
+* Raise ``RequestParameterInvalidException`` if collection element has unknown extension by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17985 <https://github.com/galaxyproject/galaxy/pull/17985>`_
+* Don't attempt to commit in dry_run mode by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17987 <https://github.com/galaxyproject/galaxy/pull/17987>`_
+* Don't fail if reporting invalid parameter values by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18002 <https://github.com/galaxyproject/galaxy/pull/18002>`_
+* Include exception info when something goes wrong while refreshing tokens by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18008 <https://github.com/galaxyproject/galaxy/pull/18008>`_
+* Avoid exception when opening apply rules tool and no collection in history by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18011 <https://github.com/galaxyproject/galaxy/pull/18011>`_
+* Don't commit without having set a hid by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18014 <https://github.com/galaxyproject/galaxy/pull/18014>`_
+* Raise appropriate exception if user forces a collection that is not populated with elements as input by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18023 <https://github.com/galaxyproject/galaxy/pull/18023>`_
+* Fix tag regex pattern by `@jdavcs <https://github.com/jdavcs>`_ in `#18025 <https://github.com/galaxyproject/galaxy/pull/18025>`_
+* Fix History Dataset Association creation so that hid is always set by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18036 <https://github.com/galaxyproject/galaxy/pull/18036>`_
+* Change wrong quota_source value from KeyError to ValueError by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18040 <https://github.com/galaxyproject/galaxy/pull/18040>`_
+* Check database connection to issue a rollback if no connection by `@jdavcs <https://github.com/jdavcs>`_ in `#18070 <https://github.com/galaxyproject/galaxy/pull/18070>`_
+
+============
+Enhancements
+============
+
+* Fix remote files sources error handling by `@davelopez <https://github.com/davelopez>`_ in `#18027 <https://github.com/galaxyproject/galaxy/pull/18027>`_
+
+=============
+Other changes
+=============
+
+* Drop left-over debug statement by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17939 <https://github.com/galaxyproject/galaxy/pull/17939>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
@@ -127,15 +171,15 @@
 * Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
 * Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
 * Toward declarative help for Galaxy markdown directives. by `@jmchilton <https://github.com/jmchilton>`_ in `#16979 <https://github.com/galaxyproject/galaxy/pull/16979>`_
 * Extend regex groups in stdio regex matches by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17016 <https://github.com/galaxyproject/galaxy/pull/17016>`_
 * Vueify Admin User Grid by `@guerler <https://github.com/guerler>`_ in `#17030 <https://github.com/galaxyproject/galaxy/pull/17030>`_
 * Remove web framework dependency from tools by `@davelopez <https://github.com/davelopez>`_ in `#17058 <https://github.com/galaxyproject/galaxy/pull/17058>`_
 * Add select parameter with options from remote resources by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17087 <https://github.com/galaxyproject/galaxy/pull/17087>`_
-*  Expose more tool information / navigability in UI. by `@jmchilton <https://github.com/jmchilton>`_ in `#17105 <https://github.com/galaxyproject/galaxy/pull/17105>`_
+* Expose more tool information / navigability in UI. by `@jmchilton <https://github.com/jmchilton>`_ in `#17105 <https://github.com/galaxyproject/galaxy/pull/17105>`_
 * Vueify Admin Roles Grid by `@guerler <https://github.com/guerler>`_ in `#17118 <https://github.com/galaxyproject/galaxy/pull/17118>`_
 * SA2.0 updates: handling "object is being merged into a Session along the backref cascade path" by `@jdavcs <https://github.com/jdavcs>`_ in `#17122 <https://github.com/galaxyproject/galaxy/pull/17122>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17123 <https://github.com/galaxyproject/galaxy/pull/17123>`_
 * Vueify Admin Groups Grid by `@guerler <https://github.com/guerler>`_ in `#17126 <https://github.com/galaxyproject/galaxy/pull/17126>`_
 * Towards SQLAlchemy 2.0: fix last cases of RemovedIn20Warning by `@jdavcs <https://github.com/jdavcs>`_ in `#17132 <https://github.com/galaxyproject/galaxy/pull/17132>`_
 * Vueify Admin Forms and Quota grids by `@guerler <https://github.com/guerler>`_ in `#17141 <https://github.com/galaxyproject/galaxy/pull/17141>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17157 <https://github.com/galaxyproject/galaxy/pull/17157>`_
```

### Comparing `galaxy-app-24.0.0/galaxy/actions/library.py` & `galaxy_app-24.0.1/galaxy/actions/library.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/app.py` & `galaxy_app-24.0.1/galaxy/app.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/app_unittest_utils/galaxy_mock.py` & `galaxy_app-24.0.1/galaxy/app_unittest_utils/galaxy_mock.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/app_unittest_utils/toolbox_support.py` & `galaxy_app-24.0.1/galaxy/app_unittest_utils/toolbox_support.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/app_unittest_utils/tools_support.py` & `galaxy_app-24.0.1/galaxy/app_unittest_utils/tools_support.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/authnz/__init__.py` & `galaxy_app-24.0.1/galaxy/authnz/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/authnz/custos_authnz.py` & `galaxy_app-24.0.1/galaxy/authnz/custos_authnz.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/authnz/managers.py` & `galaxy_app-24.0.1/galaxy/authnz/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,17 +336,16 @@
                 msg = f"An error occurred when refreshing user token on `{auth.provider}` identity provider: {message}"
                 log.error(msg)
                 return False
             refreshed = backend.refresh(trans, auth)
             if refreshed:
                 log.debug(f"Refreshed user token via `{auth.provider}` identity provider")
             return True
-        except Exception as e:
-            msg = f"An error occurred when refreshing user token: {e}"
-            log.error(msg)
+        except Exception:
+            log.exception("An error occurred when refreshing user token")
             return False
 
     def refresh_expiring_oidc_tokens(self, trans, user=None):
         user = trans.user or user
         if not isinstance(user, model.User):
             return
         for auth in user.custos_auth or []:
```

### Comparing `galaxy-app-24.0.0/galaxy/authnz/psa_authnz.py` & `galaxy_app-24.0.1/galaxy/authnz/psa_authnz.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/carbon_emissions/__init__.py` & `galaxy_app-24.0.1/galaxy/carbon_emissions/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/celery/__init__.py` & `galaxy_app-24.0.1/galaxy/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/celery/_serialization.py` & `galaxy_app-24.0.1/galaxy/celery/_serialization.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/celery/base_task.py` & `galaxy_app-24.0.1/galaxy/celery/base_task.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/celery/tasks.py` & `galaxy_app-24.0.1/galaxy/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/config_watchers.py` & `galaxy_app-24.0.1/galaxy/config_watchers.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/dependencies/__init__.py` & `galaxy_app-24.0.1/galaxy/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/dependencies/conditional-requirements.txt` & `galaxy_app-24.0.1/galaxy/dependencies/conditional-requirements.txt`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/dependencies/dev-requirements.txt` & `galaxy_app-24.0.1/galaxy/dependencies/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/dependencies/pinned-requirements.txt` & `galaxy_app-24.0.1/galaxy/dependencies/pinned-requirements.txt`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/dependencies/pinned-typecheck-requirements.txt` & `galaxy_app-24.0.1/galaxy/dependencies/pinned-typecheck-requirements.txt`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/dependencies/update.sh` & `galaxy_app-24.0.1/galaxy/dependencies/update.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/dependencies/update_lint_requirements.sh` & `galaxy_app-24.0.1/galaxy/dependencies/update_lint_requirements.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/di.py` & `galaxy_app-24.0.1/galaxy/di.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/forms/forms.py` & `galaxy_app-24.0.1/galaxy/forms/forms.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/__init__.py` & `galaxy_app-24.0.1/galaxy/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/command_factory.py` & `galaxy_app-24.0.1/galaxy/jobs/command_factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/dynamic_tool_destination.py` & `galaxy_app-24.0.1/galaxy/jobs/dynamic_tool_destination.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/handler.py` & `galaxy_app-24.0.1/galaxy/jobs/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,14 +391,16 @@
         )
         if self.job_grabber is not None:
             self.job_grabber.grab_unhandled_items()
         try:
             self.__handle_waiting_jobs()
         except StopSignalException:
             pass
+        finally:
+            self.sa_session.remove()
         log.trace(monitor_step_timer.to_str())
 
     def __handle_waiting_jobs(self):
         """
         Gets any new jobs (either from the database or from its own queue), then iterates over all new and waiting jobs
         to check the state of the jobs each depends on. If the job has dependencies that have not finished, it goes to
         the waiting queue. If the job has dependencies with errors, it is marked as having errors and removed from the
@@ -579,17 +581,14 @@
         # Remove cached wrappers for any jobs that are no longer being tracked
         for id in set(self.job_wrappers.keys()) - set(new_waiting_jobs):
             del self.job_wrappers[id]
         # Commit updated state
         with transaction(self.sa_session):
             self.sa_session.commit()
 
-        # Done with the session
-        self.sa_session.remove()
-
     def __filter_jobs_with_invalid_input_states(self, jobs):
         """
         Takes  list of jobs and filters out jobs whose input datasets are in invalid state and
         set these jobs and their dependent jobs to paused.
         """
         job_ids_to_check = [j.id for j in jobs]
         queries = []
```

### Comparing `galaxy-app-24.0.0/galaxy/jobs/manager.py` & `galaxy_app-24.0.1/galaxy/jobs/manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/mapper.py` & `galaxy_app-24.0.1/galaxy/jobs/mapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/rule_helper.py` & `galaxy_app-24.0.1/galaxy/jobs/rule_helper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/__init__.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/aws.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/aws.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/chronos.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/chronos.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/cli.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/cli.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/condor.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/condor.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/drmaa.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/drmaa.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/godocker.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/godocker.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/kubernetes.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/kubernetes.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/local.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/local.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/pbs.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/pbs.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/pulsar.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/pulsar.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/slurm.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/slurm.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/state_handler_factory.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/state_handler_factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/state_handlers/_safe_eval.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/state_handlers/_safe_eval.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/state_handlers/resubmit.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/state_handlers/resubmit.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/tasks.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/tasks.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/univa.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/univa.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/__init__.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/__init__.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/__init__.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/job/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/lsf.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/job/lsf.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/pbs.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/job/pbs.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/slurm.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/job/slurm.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/slurm_torque.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/job/slurm_torque.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/job/torque.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/job/torque.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/shell/local.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/shell/local.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/cli/shell/rsh.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/cli/shell/rsh.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/condor/__init__.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/condor/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/env.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/env.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/external.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/external.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/fork_safe_write.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/fork_safe_write.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/CLUSTER_SLOTS_STATEMENT.sh` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/job_script/CLUSTER_SLOTS_STATEMENT.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/DEFAULT_JOB_FILE_TEMPLATE.sh` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/job_script/DEFAULT_JOB_FILE_TEMPLATE.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/MEMORY_STATEMENT_TEMPLATE.sh` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/job_script/MEMORY_STATEMENT_TEMPLATE.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/job_script/__init__.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/job_script/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/kill.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/kill.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/process_groups.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/process_groups.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/pykube_util.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/pykube_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/runners/util/sudo.py` & `galaxy_app-24.0.1/galaxy/jobs/runners/util/sudo.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/splitters/basic.py` & `galaxy_app-24.0.1/galaxy/jobs/splitters/basic.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/splitters/multi.py` & `galaxy_app-24.0.1/galaxy/jobs/splitters/multi.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/jobs/stock_rules.py` & `galaxy_app-24.0.1/galaxy/jobs/stock_rules.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/main.py` & `galaxy_app-24.0.1/galaxy/main.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/main_config.py` & `galaxy_app-24.0.1/galaxy/main_config.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/__init__.py` & `galaxy_app-24.0.1/galaxy/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/annotatable.py` & `galaxy_app-24.0.1/galaxy/managers/annotatable.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/api_keys.py` & `galaxy_app-24.0.1/galaxy/managers/api_keys.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/base.py` & `galaxy_app-24.0.1/galaxy/managers/base.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/citations.py` & `galaxy_app-24.0.1/galaxy/managers/citations.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/cloud.py` & `galaxy_app-24.0.1/galaxy/managers/cloud.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/cloudauthzs.py` & `galaxy_app-24.0.1/galaxy/managers/cloudauthzs.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/collections.py` & `galaxy_app-24.0.1/galaxy/managers/collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         implicit_output_name=None,
         tags=None,
         completed_collection=None,
     ):
         # TODO: prebuild all required HIDs and send them in so no need to flush in between.
         dataset_collection = self.precreate_dataset_collection(
             structure,
-            allow_unitialized_element=implicit_output_name is not None,
+            allow_uninitialized_element=implicit_output_name is not None,
             completed_collection=completed_collection,
             implicit_output_name=implicit_output_name,
         )
         instance = self._create_instance_for_collection(
             trans,
             parent,
             name,
@@ -108,18 +108,18 @@
             implicit_output_name=implicit_output_name,
             flush=False,
             tags=tags,
         )
         return instance
 
     def precreate_dataset_collection(
-        self, structure, allow_unitialized_element=True, completed_collection=None, implicit_output_name=None
+        self, structure, allow_uninitialized_element=True, completed_collection=None, implicit_output_name=None
     ):
         has_structure = not structure.is_leaf and structure.children_known
-        if not has_structure and allow_unitialized_element:
+        if not has_structure and allow_uninitialized_element:
             dataset_collection = model.DatasetCollectionElement.UNINITIALIZED_ELEMENT
         elif not has_structure:
             collection_type_description = structure.collection_type_description
             dataset_collection = model.DatasetCollection(populated=False)
             dataset_collection.collection_type = collection_type_description.collection_type
         else:
             collection_type_description = structure.collection_type_description
@@ -139,15 +139,15 @@
                         )
                         element = next(it, None)
                 if element is None:
                     if substructure.is_leaf:
                         element = model.DatasetCollectionElement.UNINITIALIZED_ELEMENT
                     else:
                         element = self.precreate_dataset_collection(
-                            substructure, allow_unitialized_element=allow_unitialized_element
+                            substructure, allow_uninitialized_element=allow_uninitialized_element
                         )
 
                 element = model.DatasetCollectionElement(
                     collection=dataset_collection,
                     element=element,
                     element_identifier=identifier,
                     element_index=index,
```

### Comparing `galaxy-app-24.0.0/galaxy/managers/collections_util.py` & `galaxy_app-24.0.1/galaxy/managers/collections_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import logging
 import math
+from typing import (
+    Any,
+    Dict,
+)
 
 from galaxy import (
     exceptions,
     model,
 )
 from galaxy.util import string_as_bool
 
@@ -149,43 +153,46 @@
             dict_value["implicit_collection_jobs_id"] = icj.id
         else:
             dict_value["implicit_collection_jobs_id"] = None
 
     return dict_value
 
 
-def dictify_element_reference(element, rank_fuzzy_counts=None, recursive=True, security=None):
+def dictify_element_reference(
+    element: model.DatasetCollectionElement, rank_fuzzy_counts=None, recursive=True, security=None
+):
     """Load minimal details of elements required to show outline of contents in history panel.
 
     History panel can use this reference to expand to full details if individual dataset elements
     are clicked.
     """
     dictified = element.to_dict(view="element")
     if (element_object := element.element_object) is not None:
-        object_details = dict(
+        object_details: Dict[str, Any] = dict(
             id=element_object.id,
             model_class=element_object.__class__.__name__,
         )
-        if element.child_collection:
+        if isinstance(element_object, model.DatasetCollection):
             object_details["collection_type"] = element_object.collection_type
+            object_details["element_count"] = element_object.element_count
+            object_details["populated"] = element_object.populated_optimized
 
             # Recursively yield elements for each nested collection...
             if recursive:
-                child_collection = element.child_collection
-                elements, rest_fuzzy_counts = get_fuzzy_count_elements(child_collection, rank_fuzzy_counts)
+                elements, rest_fuzzy_counts = get_fuzzy_count_elements(element_object, rank_fuzzy_counts)
                 object_details["elements"] = [
                     dictify_element_reference(_, rank_fuzzy_counts=rest_fuzzy_counts, recursive=recursive)
                     for _ in elements
                 ]
-                object_details["element_count"] = child_collection.element_count
         else:
             object_details["state"] = element_object.state
             object_details["hda_ldda"] = "hda"
-            object_details["history_id"] = element_object.history_id
-            object_details["tags"] = element_object.make_tag_string_list()
+            if isinstance(element_object, model.HistoryDatasetAssociation):
+                object_details["history_id"] = element_object.history_id
+                object_details["tags"] = element_object.make_tag_string_list()
 
         dictified["object"] = object_details
     else:
         dictified["object"] = None
     return dictified
```

### Comparing `galaxy-app-24.0.0/galaxy/managers/configuration.py` & `galaxy_app-24.0.1/galaxy/managers/configuration.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/context.py` & `galaxy_app-24.0.1/galaxy/managers/context.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/datasets.py` & `galaxy_app-24.0.1/galaxy/managers/datasets.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/datatypes.py` & `galaxy_app-24.0.1/galaxy/managers/datatypes.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/dbkeys.py` & `galaxy_app-24.0.1/galaxy/managers/dbkeys.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/deletable.py` & `galaxy_app-24.0.1/galaxy/managers/deletable.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/display_applications.py` & `galaxy_app-24.0.1/galaxy/managers/display_applications.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/executables.py` & `galaxy_app-24.0.1/galaxy/managers/executables.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/export_tracker.py` & `galaxy_app-24.0.1/galaxy/managers/export_tracker.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/folders.py` & `galaxy_app-24.0.1/galaxy/managers/folders.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/forms.py` & `galaxy_app-24.0.1/galaxy/managers/forms.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/genomes.py` & `galaxy_app-24.0.1/galaxy/managers/genomes.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/group_roles.py` & `galaxy_app-24.0.1/galaxy/managers/group_roles.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/group_users.py` & `galaxy_app-24.0.1/galaxy/managers/group_users.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/groups.py` & `galaxy_app-24.0.1/galaxy/managers/groups.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/hdas.py` & `galaxy_app-24.0.1/galaxy/managers/hdas.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     PurgeDatasetsTaskRequest,
     RequestUser,
 )
 from galaxy.structured_app import (
     MinimalManagerApp,
     StructuredApp,
 )
+from galaxy.util.compression_utils import get_fileobj
 
 log = logging.getLogger(__name__)
 
 
 class HistoryDatasetAssociationNoHistoryException(Exception):
     pass
 
@@ -197,15 +198,15 @@
     ) -> model.HistoryDatasetAssociation:
         """
         Copy hda, including annotation and tags, add to history and return the given HDA.
         """
         if not isinstance(item, model.HistoryDatasetAssociation):
             raise TypeError()
         hda = item
-        copy = hda.copy(parent_id=kwargs.get("parent_id"), copy_hid=False, copy_tags=hda.tags, flush=flush)
+        copy = hda.copy(parent_id=kwargs.get("parent_id"), copy_hid=False, copy_tags=hda.tags, flush=False)
         if hide_copy:
             copy.visible = False
         if history:
             history.stage_addition(copy)
 
         copy.set_size()
 
@@ -216,20 +217,14 @@
                 history.add_pending_items()
             session = object_session(copy)
             with transaction(session):
                 session.commit()
 
         return copy
 
-    def copy_ldda(self, history, ldda, **kwargs):
-        """
-        Copy this HDA as a LDDA and return.
-        """
-        return ldda.to_history_dataset_association(history, add_to_history=True)
-
     # .... deletion and purging
     def purge(self, hda, flush=True, **kwargs):
         if self.app.config.enable_celery_tasks:
             from galaxy.celery.tasks import purge_hda
 
             user = kwargs.get("user")
             return purge_hda.delay(hda_id=hda.id, task_user_id=getattr(user, "id", None))
@@ -299,19 +294,21 @@
         MAX_PEEK_SIZE = 1000000
 
         truncated = False
         hda_data = None
         # For now, cannot get data from non-text datasets.
         if not isinstance(hda.datatype, datatypes.data.Text):
             return truncated, hda_data
-        if not os.path.exists(hda.get_file_name()):
+        file_path = hda.get_file_name()
+        if not os.path.exists(file_path):
             return truncated, hda_data
 
-        truncated = preview and os.stat(hda.get_file_name()).st_size > MAX_PEEK_SIZE
-        hda_data = open(hda.get_file_name()).read(MAX_PEEK_SIZE)
+        truncated = preview and os.stat(file_path).st_size > MAX_PEEK_SIZE
+        with get_fileobj(file_path) as fh:
+            hda_data = fh.read(MAX_PEEK_SIZE)
         return truncated, hda_data
 
     # .... annotatable
     def annotation(self, hda):
         # override to scope to history owner
         return self._user_annotation(hda, hda.user)
 
@@ -554,14 +551,15 @@
 
     def add_serializers(self):
         super().add_serializers()
         taggable.TaggableSerializerMixin.add_serializers(self)
         annotatable.AnnotatableSerializerMixin.add_serializers(self)
 
         serializers: Dict[str, base.Serializer] = {
+            "hid": lambda item, key, **context: item.hid if item.hid is not None else -1,
             "model_class": lambda item, key, **context: "HistoryDatasetAssociation",
             "history_content_type": lambda item, key, **context: "dataset",
             "hda_ldda": lambda item, key, **context: "hda",
             "type_id": self.serialize_type_id,
             "copied_from_ldda_id": self.serialize_copied_from_ldda_id,
             "history_id": self.serialize_id,
             # remapped
```

### Comparing `galaxy-app-24.0.0/galaxy/managers/hdcas.py` & `galaxy_app-24.0.1/galaxy/managers/hdcas.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/histories.py` & `galaxy_app-24.0.1/galaxy/managers/histories.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/history_contents.py` & `galaxy_app-24.0.1/galaxy/managers/history_contents.py`

 * *Files 0% similar despite different names*

```diff
@@ -588,15 +588,15 @@
                 if op == "eq":
                     ids = self.app.object_store.get_quota_source_map().ids_per_quota_source(
                         include_default_quota_source=True
                     )
                     if val == "__null__":
                         val = None
                     if val not in ids:
-                        raise KeyError(f"Could not find key {val} in object store keys {list(ids.keys())}")
+                        raise ValueError(f"Could not find key {val} in object store keys {list(ids.keys())}")
                     object_store_ids = ids[val]
                     return sql.column("object_store_id").in_(object_store_ids)
 
                 raise_filter_err(attr, op, val, "bad op in filter")
 
         if (column_filter := get_filter(attr, op, val)) is not None:
             return self.parsed_filter(filter_type="orm", filter=column_filter)
```

### Comparing `galaxy-app-24.0.0/galaxy/managers/interactivetool.py` & `galaxy_app-24.0.1/galaxy/managers/interactivetool.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/item_tags.py` & `galaxy_app-24.0.1/galaxy/managers/item_tags.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/job_connections.py` & `galaxy_app-24.0.1/galaxy/managers/job_connections.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/jobs.py` & `galaxy_app-24.0.1/galaxy/managers/jobs.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/lddas.py` & `galaxy_app-24.0.1/galaxy/managers/lddas.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/libraries.py` & `galaxy_app-24.0.1/galaxy/managers/libraries.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/library_datasets.py` & `galaxy_app-24.0.1/galaxy/managers/library_datasets.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/licenses.json` & `galaxy_app-24.0.1/galaxy/managers/licenses.json`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/licenses.py` & `galaxy_app-24.0.1/galaxy/managers/licenses.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/markdown_parse.py` & `galaxy_app-24.0.1/galaxy/managers/markdown_parse.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/markdown_util.py` & `galaxy_app-24.0.1/galaxy/managers/markdown_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/metrics.py` & `galaxy_app-24.0.1/galaxy/managers/metrics.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/model_stores.py` & `galaxy_app-24.0.1/galaxy/managers/model_stores.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/notification.py` & `galaxy_app-24.0.1/galaxy/managers/notification.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/pages.py` & `galaxy_app-24.0.1/galaxy/managers/pages.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/quotas.py` & `galaxy_app-24.0.1/galaxy/managers/quotas.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/ratable.py` & `galaxy_app-24.0.1/galaxy/managers/ratable.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/rbac_secured.py` & `galaxy_app-24.0.1/galaxy/managers/rbac_secured.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/remote_files.py` & `galaxy_app-24.0.1/galaxy/managers/remote_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Optional,
     Set,
 )
 
 from galaxy import exceptions
 from galaxy.files import (
     ConfiguredFileSources,
+    FileSourcePath,
     ProvidesUserFileSourcesUserContext,
 )
 from galaxy.files.sources import (
     FilesSourceOptions,
     PluginKind,
 )
 from galaxy.managers.context import ProvidesUserContext
@@ -90,18 +91,18 @@
             index = file_source.list(
                 file_source_path.path,
                 recursive=recursive,
                 user_context=user_file_source_context,
                 opts=opts,
             )
         except exceptions.MessageException:
-            log.warning(f"Problem listing file source path {file_source_path}", exc_info=True)
+            log.warning(self._get_error_message(file_source_path), exc_info=True)
             raise
         except Exception:
-            message = f"Problem listing file source path {file_source_path}"
+            message = self._get_error_message(file_source_path)
             log.warning(message, exc_info=True)
             raise exceptions.InternalServerError(message)
         if format == RemoteFilesFormat.flat:
             # rip out directories, ensure sorted by path
             index = [i for i in index if i["class"] == "File"]
             index = sorted(index, key=itemgetter("path"))
         elif format == RemoteFilesFormat.jstree:
@@ -127,14 +128,17 @@
                     )
                 )
             userdir_jstree = jstree.JSTree(jstree_paths)
             index = userdir_jstree.jsonData()
 
         return index
 
+    def _get_error_message(self, file_source_path: FileSourcePath) -> str:
+        return f"Problem listing file source path {file_source_path.file_source.get_uri_root()}{file_source_path.path}"
+
     def get_files_source_plugins(
         self,
         user_context: ProvidesUserContext,
         browsable_only: Optional[bool] = True,
         include_kind: Optional[Set[PluginKind]] = None,
         exclude_kind: Optional[Set[PluginKind]] = None,
     ):
@@ -158,14 +162,17 @@
         target = entry_data.target
         user_file_source_context = ProvidesUserFileSourcesUserContext(user_ctx)
         self._file_sources.validate_uri_root(target, user_context=user_file_source_context)
         file_source_path = self._file_sources.get_file_source_path(target)
         file_source = file_source_path.file_source
         try:
             result = file_source.create_entry(entry_data.dict(), user_context=user_file_source_context)
+        except exceptions.MessageException:
+            log.warning(f"Problem creating entry {entry_data.name} in file source {entry_data.target}", exc_info=True)
+            raise
         except Exception:
             message = f"Problem creating entry {entry_data.name} in file source {entry_data.target}"
             log.warning(message, exc_info=True)
             raise exceptions.InternalServerError(message)
         return CreatedEntryResponse(
             name=result["name"],
             uri=result["uri"],
```

### Comparing `galaxy-app-24.0.0/galaxy/managers/roles.py` & `galaxy_app-24.0.1/galaxy/managers/roles.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/secured.py` & `galaxy_app-24.0.1/galaxy/managers/secured.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/session.py` & `galaxy_app-24.0.1/galaxy/managers/session.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/sharable.py` & `galaxy_app-24.0.1/galaxy/managers/sharable.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/taggable.py` & `galaxy_app-24.0.1/galaxy/managers/taggable.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/tags.py` & `galaxy_app-24.0.1/galaxy/managers/tags.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/tasks.py` & `galaxy_app-24.0.1/galaxy/managers/tasks.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/tool_data.py` & `galaxy_app-24.0.1/galaxy/managers/tool_data.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/tools.py` & `galaxy_app-24.0.1/galaxy/managers/tools.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/users.py` & `galaxy_app-24.0.1/galaxy/managers/users.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/visualizations.py` & `galaxy_app-24.0.1/galaxy/managers/visualizations.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/managers/workflows.py` & `galaxy_app-24.0.1/galaxy/managers/workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,20 +86,22 @@
 from galaxy.schema.schema import WorkflowIndexQueryPayload
 from galaxy.structured_app import MinimalManagerApp
 from galaxy.tools.parameters import (
     params_to_incoming,
     visit_input_values,
 )
 from galaxy.tools.parameters.basic import (
-    ConnectedValue,
     DataCollectionToolParameter,
     DataToolParameter,
+)
+from galaxy.tools.parameters.workflow_utils import (
+    ConnectedValue,
     RuntimeValue,
+    workflow_building_modes,
 )
-from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
 from galaxy.util.hash_util import md5_hash_str
 from galaxy.util.json import (
     safe_dumps,
     safe_loads,
 )
 from galaxy.util.sanitize_html import sanitize_html
 from galaxy.util.search import (
@@ -722,15 +724,16 @@
         data = raw_workflow_description.as_dict
         if isinstance(data, str):
             data = json.loads(data)
         if "tags" in data:
             trans.tag_handler.set_tags_from_list(
                 trans.user,
                 stored_workflow,
-                data.get("tags", []),
+                data["tags"],
+                flush=False,
             )
 
         if workflow_update_options.update_stored_workflow_attributes:
             update_dict = raw_workflow_description.as_dict
             if "name" in update_dict:
                 sanitized_name = sanitize_html(update_dict["name"])
                 if not sanitized_name:
@@ -1455,16 +1458,21 @@
             if not module:
                 raise exceptions.MessageException(f"Unrecognized step type: {step.type}")
             # Get user annotation if it exists, otherwise get owner annotation.
             annotation_str = self.get_item_annotation_str(trans.sa_session, trans.user, step) or ""
             if not annotation_str and annotation_owner:
                 annotation_str = self.get_item_annotation_str(trans.sa_session, annotation_owner, step) or ""
             content_id = module.get_content_id() if allow_upgrade else step.content_id
-            # Export differences for backward compatibility
-            tool_state = module.get_export_state()
+            try:
+                tool_state = module.get_export_state()
+            except ValueError:
+                # Fix state if necessary
+                module.check_and_update_state()
+                tool_state = module.get_export_state()
+
             # Step info
             step_dict = {
                 "id": step.order_index,
                 "type": module.type,
                 "content_id": content_id,
                 "tool_id": None,
                 "tool_version": module.get_version() if allow_upgrade else step.tool_version,
```

### Comparing `galaxy-app-24.0.0/galaxy/queue_worker.py` & `galaxy_app-24.0.1/galaxy/queue_worker.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/queues.py` & `galaxy_app-24.0.1/galaxy/queues.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/short_term_storage/__init__.py` & `galaxy_app-24.0.1/galaxy/short_term_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/structured_app.py` & `galaxy_app-24.0.1/galaxy/structured_app.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/cache.py` & `galaxy_app-24.0.1/galaxy/tool_shed/cache.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/client.py` & `galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/client.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/install_manager.py` & `galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/install_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/installed_repository_manager.py` & `galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/installed_repository_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/metadata/installed_repository_metadata_manager.py` & `galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/metadata/installed_repository_metadata_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/repository_dependencies/repository_dependency_manager.py` & `galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/repository_dependencies/repository_dependency_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/tools/data_manager.py` & `galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/tools/data_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/tools/tool_panel_manager.py` & `galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/tools/tool_panel_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/galaxy_install/update_repository_manager.py` & `galaxy_app-24.0.1/galaxy/tool_shed/galaxy_install/update_repository_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/metadata/metadata_generator.py` & `galaxy_app-24.0.1/galaxy/tool_shed/metadata/metadata_generator.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/repository_type.py` & `galaxy_app-24.0.1/galaxy/tool_shed/repository_type.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/tools/data_table_manager.py` & `galaxy_app-24.0.1/galaxy/tool_shed/tools/data_table_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/tools/tool_validator.py` & `galaxy_app-24.0.1/galaxy/tool_shed/tools/tool_validator.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/unittest_utils/__init__.py` & `galaxy_app-24.0.1/galaxy/tool_shed/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/util/basic_util.py` & `galaxy_app-24.0.1/galaxy/tool_shed/util/basic_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/util/container_util.py` & `galaxy_app-24.0.1/galaxy/tool_shed/util/container_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/util/dependency_display.py` & `galaxy_app-24.0.1/galaxy/tool_shed/util/dependency_display.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/util/hg_util.py` & `galaxy_app-24.0.1/galaxy/tool_shed/util/hg_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/util/metadata_util.py` & `galaxy_app-24.0.1/galaxy/tool_shed/util/metadata_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/util/repository_util.py` & `galaxy_app-24.0.1/galaxy/tool_shed/util/repository_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,18 @@
     and_,
     false,
     or_,
 )
 from sqlalchemy.orm import joinedload
 
 from galaxy import util
-from galaxy.model.base import transaction
+from galaxy.model.base import (
+    check_database_connection,
+    transaction,
+)
 from galaxy.model.scoped_session import install_model_scoped_session
 from galaxy.model.tool_shed_install import ToolShedRepository
 from galaxy.tool_shed.util import basic_util
 from galaxy.util.tool_shed import (
     common_util,
     encoding_util,
 )
@@ -279,14 +282,15 @@
     repository_id=None,
     from_cache=False,
 ):
     """
     Return a tool shed repository database record defined by the combination of a toolshed, repository name,
     repository owner and either current or originally installed changeset_revision.
     """
+    check_database_connection(app.install_model.context)
     # We store the port, if one exists, in the database.
     tool_shed = common_util.remove_protocol_from_tool_shed_url(tool_shed)
     if from_cache:
         tsr_cache = getattr(app, "tool_shed_repository_cache", None)
         if tsr_cache:
             return app.tool_shed_repository_cache.get_installed_repository(
                 tool_shed=tool_shed,
```

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/util/shed_util_common.py` & `galaxy_app-24.0.1/galaxy/tool_shed/util/shed_util_common.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/util/tool_dependency_util.py` & `galaxy_app-24.0.1/galaxy/tool_shed/util/tool_dependency_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/util/tool_util.py` & `galaxy_app-24.0.1/galaxy/tool_shed/util/tool_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tool_shed/util/utility_container_manager.py` & `galaxy_app-24.0.1/galaxy/tool_shed/util/utility_container_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/__init__.py` & `galaxy_app-24.0.1/galaxy/tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     Group,
     Repeat,
     Section,
     UploadDataset,
 )
 from galaxy.tools.parameters.input_translation import ToolInputTranslator
 from galaxy.tools.parameters.meta import expand_meta_parameters
-from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
+from galaxy.tools.parameters.workflow_utils import workflow_building_modes
 from galaxy.tools.parameters.wrapped_json import json_wrap
 from galaxy.tools.test import parse_tests
 from galaxy.util import (
     in_directory,
     listify,
     Params,
     parse_xml_string,
@@ -3457,15 +3457,17 @@
             else:
                 copied_value = dce.element_object.copy(flush=False)
             new_elements[element_identifier] = copied_value
         return new_elements
 
     @staticmethod
     def element_is_valid(element: model.DatasetCollectionElement):
-        return element.element_object.is_ok
+        element_object = element.element_object
+        assert isinstance(element_object, model.DatasetInstance)
+        return element_object.is_ok
 
     def produce_outputs(self, trans, out_data, output_collections, incoming, history, **kwds):
         collection = incoming["input"]
 
         if hasattr(collection, "element_object"):
             # A list
             elements = collection.element_object.elements
@@ -3499,43 +3501,48 @@
 
 class FilterFailedDatasetsTool(FilterDatasetsTool):
     tool_type = "filter_failed_datasets_collection"
     require_dataset_ok = False
 
     @staticmethod
     def element_is_valid(element: model.DatasetCollectionElement):
-        return element.element_object.is_ok
+        element_object = element.element_object
+        assert isinstance(element_object, model.DatasetInstance)
+        return element_object.is_ok
 
 
 class KeepSuccessDatasetsTool(FilterDatasetsTool):
     tool_type = "keep_success_datasets_collection"
     require_terminal_states = False
     require_dataset_ok = False
     require_terminal_or_paused_states = True
 
     @staticmethod
     def element_is_valid(element: model.DatasetCollectionElement):
+        element_object = element.element_object
+        assert isinstance(element_object, model.DatasetInstance)
         if (
-            element.element_object.state != model.Dataset.states.PAUSED
-            and element.element_object.state in model.Dataset.non_ready_states
+            element_object.state != model.Dataset.states.PAUSED
+            and element_object.state in model.Dataset.non_ready_states
         ):
             raise ToolInputsNotReadyException("An input dataset is pending.")
-        return element.element_object.is_ok
+        return element_object.is_ok
 
 
 class FilterEmptyDatasetsTool(FilterDatasetsTool):
     tool_type = "filter_empty_datasets_collection"
     require_dataset_ok = False
 
     @staticmethod
     def element_is_valid(element: model.DatasetCollectionElement):
-        dataset_instance: model.DatasetInstance = element.element_object
-        if dataset_instance.has_data():
+        element_object = element.element_object
+        assert isinstance(element_object, model.DatasetInstance)
+        if element_object.has_data():
             # We have data, but it might just be a compressed archive of nothing
-            file_name = dataset_instance.get_file_name()
+            file_name = element_object.get_file_name()
             _, fh = get_fileobj_raw(file_name, mode="rb")
             if len(fh.read(1)):
                 return True
         return False
 
 
 class FlattenTool(DatabaseOperationTool):
```

### Comparing `galaxy-app-24.0.0/galaxy/tools/actions/__init__.py` & `galaxy_app-24.0.1/galaxy/tools/actions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,33 +13,37 @@
     TYPE_CHECKING,
     Union,
 )
 
 from packaging.version import Version
 
 from galaxy import model
-from galaxy.exceptions import ItemAccessibilityException
+from galaxy.exceptions import (
+    ItemAccessibilityException,
+    RequestParameterInvalidException,
+)
 from galaxy.job_execution.actions.post import ActionBox
+from galaxy.managers.context import ProvidesHistoryContext
 from galaxy.model import (
     HistoryDatasetAssociation,
     Job,
     LibraryDatasetDatasetAssociation,
     WorkflowRequestInputParameter,
 )
 from galaxy.model.base import transaction
 from galaxy.model.dataset_collections.builder import CollectionBuilder
 from galaxy.model.none_like import NoneDataset
 from galaxy.objectstore import ObjectStorePopulator
 from galaxy.tools.parameters import update_dataset_ids
 from galaxy.tools.parameters.basic import (
     DataCollectionToolParameter,
     DataToolParameter,
-    RuntimeValue,
     SelectToolParameter,
 )
+from galaxy.tools.parameters.workflow_utils import RuntimeValue
 from galaxy.tools.parameters.wrapped import (
     LegacyUnprefixedDict,
     WrappedParameters,
 )
 from galaxy.util import ExecutionTimer
 from galaxy.util.template import fill_template
 
@@ -94,15 +98,15 @@
 
     produces_real_jobs = True
 
     def _collect_input_datasets(
         self,
         tool,
         param_values,
-        trans,
+        trans: ProvidesHistoryContext,
         history,
         current_user_roles=None,
         dataset_collection_elements=None,
         collection_info=None,
     ):
         """
         Collect any dataset inputs from incoming. Returns a mapping from
@@ -252,14 +256,18 @@
                     record_permission(action, role_id)
 
                 _, extensions = collection.dataset_states_and_extensions_summary
                 conversion_required = False
                 for ext in extensions:
                     if ext:
                         datatype = trans.app.datatypes_registry.get_datatype_by_extension(ext)
+                        if not datatype:
+                            raise RequestParameterInvalidException(
+                                f"Extension '{ext}' unknown, cannot use dataset collection as input"
+                            )
                         if not datatype.matches_any(input.formats):
                             conversion_required = True
                             break
                 processed_dataset_dict = {}
                 for i, v in enumerate(collection.dataset_instances):
                     processed_dataset = None
                     if conversion_required:
```

### Comparing `galaxy-app-24.0.0/galaxy/tools/actions/data_manager.py` & `galaxy_app-24.0.1/galaxy/tools/actions/data_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/actions/data_source.py` & `galaxy_app-24.0.1/galaxy/tools/actions/data_source.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/actions/history_imp_exp.py` & `galaxy_app-24.0.1/galaxy/tools/actions/history_imp_exp.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/actions/metadata.py` & `galaxy_app-24.0.1/galaxy/tools/actions/metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/actions/model_operations.py` & `galaxy_app-24.0.1/galaxy/tools/actions/model_operations.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/actions/upload.py` & `galaxy_app-24.0.1/galaxy/tools/actions/upload.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/actions/upload_common.py` & `galaxy_app-24.0.1/galaxy/tools/actions/upload_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,16 +136,14 @@
         sa_session=trans.sa_session,
     )
     trans.sa_session.add(hda)
     if state:
         hda.state = state
     else:
         hda.state = hda.states.QUEUED
-    with transaction(trans.sa_session):
-        trans.sa_session.commit()
     history.add_dataset(hda, genome_build=uploaded_dataset.dbkey, quota=False)
     permissions = trans.app.security_agent.history_get_default_permissions(history)
     trans.app.security_agent.set_all_dataset_permissions(hda.dataset, permissions, new=True, flush=False)
     with transaction(trans.sa_session):
         trans.sa_session.commit()
     return hda
 
@@ -437,11 +435,10 @@
     # Stolen from galaxy.web.controllers.library_common (importing from which causes a circular issues).
     # Much faster way of retrieving all active sub-folders within a given folder than the
     # performance of the mapper.  This query also eagerloads the permissions on each folder.
     stmt = (
         select(LibraryFolder)
         .filter_by(parent=folder, deleted=False)
         .options(joinedload(LibraryFolder.actions))
-        .unique()
         .order_by(LibraryFolder.name)
     )
-    return trans.sa_session.scalars(stmt).all()
+    return trans.sa_session.scalars(stmt).unique().all()
```

### Comparing `galaxy-app-24.0.0/galaxy/tools/apply_rules.xml` & `galaxy_app-24.0.1/galaxy/tools/apply_rules.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/biotools.py` & `galaxy_app-24.0.1/galaxy/tools/biotools.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/build_list.xml` & `galaxy_app-24.0.1/galaxy/tools/build_list.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/build_list_1.2.0.xml` & `galaxy_app-24.0.1/galaxy/tools/build_list_1.2.0.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_export/export_remote.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_export/export_remote.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_export/export_remote.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_export/export_remote.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_export/send.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_export/send.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_export/send.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_export/send.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/biomart.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/biomart.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/biomart_test.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/biomart_test.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/cbi_rice_mart.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/cbi_rice_mart.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/data_source.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/data_source.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ebi_sra.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/ebi_sra.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/eupathdb.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/eupathdb.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/fly_modencode.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/fly_modencode.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/flymine.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/flymine.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/flymine_test.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/flymine_test.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/genbank.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/genbank.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/genbank.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/genbank.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/gramene_mart.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/gramene_mart.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/hapmapmart.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/hapmapmart.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/hbvar.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/hbvar.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/import.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/import.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/import.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/import.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/intermine.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/intermine.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/metabolicmine.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/metabolicmine.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/microbial_import.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/microbial_import.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/microbial_import.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/microbial_import.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/microbial_import_code.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/microbial_import_code.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/modmine.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/modmine.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/mousemine.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/mousemine.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ncbi_datasets.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/ncbi_datasets.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ratmine.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/ratmine.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/sra.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/sra.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser_archaea.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser_archaea.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/ucsc_tablebrowser_test.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/ucsc_tablebrowser_test.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/upload.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/upload.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/upload.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/upload.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/worm_modencode.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/worm_modencode.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/wormbase.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/wormbase.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/wormbase_test.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/wormbase_test.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/yeastmine.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/yeastmine.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/data_source/zebrafishmine.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/data_source/zebrafishmine.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/expression_tools/expression_macros.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/expression_tools/expression_macros.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/expression_tools/parse_values_from_file.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/expression_tools/parse_values_from_file.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/expression_tools/pick_value.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/expression_tools/pick_value.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/extract/extract_genomic_dna.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/extract/extract_genomic_dna.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/extract/extract_genomic_dna.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/extract/extract_genomic_dna.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/extract/liftOver_wrapper.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/extract/liftOver_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/extract/liftOver_wrapper.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/extract/liftOver_wrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/CreateInterval.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/CreateInterval.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_concat_fasta.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/axt_to_concat_fasta.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_concat_fasta.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/axt_to_concat_fasta.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_fasta.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/axt_to_fasta.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_fasta.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/axt_to_fasta.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_lav.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/axt_to_lav.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/axt_to_lav.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/axt_to_lav.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/bed2gff.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/bed2gff.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/bed_to_bigbed.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/bed_to_bigbed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/bed_to_gff_converter.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/bed_to_gff_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/catWrapper.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/catWrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/catWrapper.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/catWrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/changeCase.pl` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/changeCase.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/changeCase.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/changeCase.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/commWrapper.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/commWrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/compare.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/compare.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/condense_characters.pl` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/condense_characters.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/condense_characters.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/condense_characters.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/convert_characters.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/convert_characters.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/convert_characters.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/convert_characters.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/cutWrapper.pl` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/cutWrapper.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/cutWrapper.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/cutWrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/fileGrep.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/fileGrep.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/fixedValueColumn.pl` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/fixedValueColumn.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/fixedValueColumn.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/fixedValueColumn.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/extract_GFF_Features.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/extract_GFF_Features.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/extract_GFF_Features.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/extract_GFF_Features.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/gff_filter_by_attribute.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/gff_filter_by_feature_count.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff/gtf_filter_by_attribute_values_list.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff2bed.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff2bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gff_to_bed_converter.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/gff_to_bed_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/grep.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/grep.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/grep.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/grep.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/grep_1.0.1.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/grep_1.0.1.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gtf2bedgraph.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/gtf2bedgraph.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/gtf_to_bedgraph_converter.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/gtf_to_bedgraph_converter.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/headWrapper.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/headWrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/join.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/join.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/joinWrapper.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/joinWrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/joiner.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/joiner.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/joiner2.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/joiner2.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/lav_to_bed.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/lav_to_bed.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/lav_to_bed.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/lav_to_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/lav_to_bed_code.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/lav_to_bed_code.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/mergeCols.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/mergeCols.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/mergeCols.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/mergeCols.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/pasteWrapper.pl` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/pasteWrapper.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/pasteWrapper.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/pasteWrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/random_lines_two_pass.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/random_lines_two_pass.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/randomlines.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/randomlines.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/randomlines.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/randomlines.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/remove_beginning.pl` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/remove_beginning.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/remove_beginning.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/remove_beginning.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/secure_hash_message_digest.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/secure_hash_message_digest.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/secure_hash_message_digest.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/secure_hash_message_digest.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/sff_extract.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/sff_extract.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/sff_extractor.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/sff_extractor.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/sorter.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/sorter.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/sorter.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/sorter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/tailWrapper.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/tailWrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/trimmer.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/trimmer.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/trimmer.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/trimmer.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_exon_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/ucsc_gene_bed_to_intron_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/ucsc_gene_table_to_intervals.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/uniq.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/uniq.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/uniq.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/uniq.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/wc_gnu.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/wc_gnu.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/wig_to_bigwig.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/wig_to_bigwig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/wiggle_to_simple.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/wiggle_to_simple.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/filters/wiggle_to_simple.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/filters/wiggle_to_simple.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/default_notebook.ipynb` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/default_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_askomics.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_askomics.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_bam_iobio.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_bam_iobio.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_cellxgene_0.16.2.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_cellxgene_0.16.2.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_cellxgene_1.1.1.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_cellxgene_1.1.1.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_climate_notebook.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_climate_notebook.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_ethercalc.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_ethercalc.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_geoexplorer.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_geoexplorer.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_guacamole_desktop.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_guacamole_desktop.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_hicbrowser.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_hicbrowser.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_higlass.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_higlass.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_isee.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_isee.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook_1.0.0.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_jupyter_notebook_1.0.0.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_metashark.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_metashark.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_mgnify_notebook.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_mgnify_notebook.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_ml_jupyter_notebook.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_ml_jupyter_notebook.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_neo4j.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_neo4j.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_openrefine.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_openrefine.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_pangeo_notebook.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_pangeo_notebook.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_panoply.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_panoply.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_paraview.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_paraview.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_pavian.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_pavian.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_phinch.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_phinch.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_pyiron.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_pyiron.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_qiskit_jupyter_notebook.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_qiskit_jupyter_notebook.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_radiant.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_radiant.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_rstudio.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_rstudio.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_simtext_app.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_simtext_app.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_vcf_iobio.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_vcf_iobio.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_vrm_editor.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_vrm_editor.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_wallace.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_wallace.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/interactivetool_wilson.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/interactivetool_wilson.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/interactive/simtext_app.R` & `galaxy_app-24.0.1/galaxy/tools/bundled/interactive/simtext_app.R`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/genebed_maf_to_fasta.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/genebed_maf_to_fasta.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval2maf.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/interval2maf.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval2maf.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/interval2maf.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval2maf_pairwise.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/interval2maf_pairwise.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/interval_maf_to_merged_fasta.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_by_block_number.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_by_block_number.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_by_block_number.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_by_block_number.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_filter.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_filter.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_filter.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_filter.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_size.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_limit_size.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_size.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_limit_size.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_to_species.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_limit_to_species.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_limit_to_species.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_limit_to_species.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_reverse_complement.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_reverse_complement.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_reverse_complement.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_reverse_complement.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_split_by_species.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_split_by_species.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_split_by_species.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_split_by_species.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_stats.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_stats.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_stats.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_stats.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_thread_for_species.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_thread_for_species.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_thread_for_species.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_thread_for_species.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_bed.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_bed.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_bed.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_bed_code.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_bed_code.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_fasta.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_fasta.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_fasta_concat.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_fasta_concat.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_fasta_multiple_sets.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_fasta_multiple_sets.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_interval.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_interval.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/maf_to_interval.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/maf_to_interval.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/maf/vcf_to_maf_customtrack.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/meme/fimo.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/meme/fimo.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/meme/fimo_wrapper.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/meme/fimo_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/meme/meme.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/meme/meme.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/blat_wrapper.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/metag_tools/blat_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/blat_wrapper.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/metag_tools/blat_wrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/metag_tools/shrimp_color_wrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_wrapper.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/metag_tools/shrimp_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/metag_tools/shrimp_wrapper.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/metag_tools/shrimp_wrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/bwa_solid2fastq_modified.pl` & `galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/bwa_solid2fastq_modified.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/fastq_conversions.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/fastq_gen_conv.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid2fastq.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/solid2fastq.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid2fastq.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/solid2fastq.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/next_gen_conversion/solid_to_fastq.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/ngs_simulation/ngs_simulation.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/ngs_simulation/ngs_simulation.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/ngs_simulation/ngs_simulation.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/ngs_simulation/ngs_simulation.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/BEAM2_wrapper.sh` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/BEAM2_wrapper.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/beam.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/beam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/gpass.pl` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/gpass.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/gpass.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/gpass.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/ldtools.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/ldtools.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/ldtools_wrapper.sh` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/ldtools_wrapper.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToDavid.pl` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/linkToDavid.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToDavid.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/linkToDavid.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToGProfile.pl` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/linkToGProfile.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/linkToGProfile.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/linkToGProfile.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/lped_to_geno.pl` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/lped_to_geno.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/lps.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/lps.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/lps_tool_wrapper.sh` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/lps_tool_wrapper.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2gd_snp.pl` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/master2gd_snp.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2gd_snp.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/master2gd_snp.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2pg.pl` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/master2pg.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/master2pg.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/master2pg.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/mergeSnps.pl` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/mergeSnps.pl`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/pagetag.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/pagetag.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/pass.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/pass.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/senatag.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/senatag.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/sift.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/sift.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/phenotype_association/sift_variants_wrapper.sh` & `galaxy_app-24.0.1/galaxy/tools/bundled/phenotype_association/sift_variants_wrapper.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/plotting/bar_chart.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/plotting/bar_chart.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/plotting/bar_chart.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/plotting/bar_chart.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/plotting/boxplot.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/plotting/boxplot.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/maq_cs_wrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/qualsolid_boxplot_graph.sh` & `galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/qualsolid_boxplot_graph.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/solid_qual_boxplot.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/solid_qual_boxplot.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/solid_qual_stats.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/solid_qual_stats.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/solid_tools/solid_qual_stats.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/solid_tools/solid_qual_stats.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velvetg.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/sr_assembly/velvetg.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velvetg_wrapper.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/sr_assembly/velvetg_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velveth.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/sr_assembly/velveth.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/sr_assembly/velveth_wrapper.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/sr_assembly/velveth_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/PerM.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/PerM.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/bfast_wrapper.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/bfast_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/bfast_wrapper.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/bfast_wrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/fastq_statistics.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/fastq_statistics.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/mosaik.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/mosaik.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/srma_wrapper.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/srma_wrapper.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/sr_mapping/srma_wrapper.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/sr_mapping/srma_wrapper.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/stats/aggregate_binned_scores_in_intervals.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/stats/aggregate_binned_scores_in_intervals.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/stats/aggregate_scores_in_intervals.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/stats/aggregate_scores_in_intervals.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/stats/filtering.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/stats/filtering.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/stats/filtering.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/stats/filtering.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/stats/filtering_1_1_0.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/stats/filtering_1_1_0.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/stats/grouping.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/stats/grouping.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/stats/grouping.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/stats/grouping.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/stats/gsummary.py` & `galaxy_app-24.0.1/galaxy/tools/bundled/stats/gsummary.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/stats/gsummary.xml` & `galaxy_app-24.0.1/galaxy/tools/bundled/stats/gsummary.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/bundled/stats/r_wrapper.sh` & `galaxy_app-24.0.1/galaxy/tools/bundled/stats/r_wrapper.sh`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/cache.py` & `galaxy_app-24.0.1/galaxy/tools/cache.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/data/__init__.py` & `galaxy_app-24.0.1/galaxy/tools/data/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/data_fetch.py` & `galaxy_app-24.0.1/galaxy/tools/data_fetch.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/data_fetch.xml` & `galaxy_app-24.0.1/galaxy/tools/data_fetch.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/data_manager/manager.py` & `galaxy_app-24.0.1/galaxy/tools/data_manager/manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/duplicate_file_to_collection.xml` & `galaxy_app-24.0.1/galaxy/tools/duplicate_file_to_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/error_reports/__init__.py` & `galaxy_app-24.0.1/galaxy/tools/error_reports/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/__init__.py` & `galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/base_git.py` & `galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/base_git.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/email.py` & `galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/email.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/github.py` & `galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/github.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/gitlab.py` & `galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/gitlab.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/influxdb.py` & `galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/influxdb.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/json.py` & `galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/json.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/sentry.py` & `galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/sentry.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/error_reports/plugins/slack.py` & `galaxy_app-24.0.1/galaxy/tools/error_reports/plugins/slack.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/errors.py` & `galaxy_app-24.0.1/galaxy/tools/errors.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/evaluation.py` & `galaxy_app-24.0.1/galaxy/tools/evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,14 +353,15 @@
                     tool=self.tool,
                     name=input.name,
                     compute_environment=self.compute_environment,
                 )
                 element_identifier = element_identifier_mapper.identifier(dataset, param_dict)
                 if element_identifier:
                     wrapper_kwds["identifier"] = element_identifier
+                wrapper_kwds["formats"] = input.formats
                 input_values[input.name] = DatasetFilenameWrapper(dataset, **wrapper_kwds)
             elif isinstance(input, DataCollectionToolParameter):
                 dataset_collection = value
                 wrapper_kwds = dict(
                     datatypes_registry=self.app.datatypes_registry,
                     compute_environment=self.compute_environment,
                     tool=self.tool,
```

### Comparing `galaxy-app-24.0.0/galaxy/tools/execute.py` & `galaxy_app-24.0.1/galaxy/tools/execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 )
 from galaxy.tool_util.parser import ToolOutputCollectionPart
 from galaxy.tools.actions import (
     filter_output,
     on_text_for_names,
     ToolExecutionCache,
 )
-from galaxy.tools.parameters.basic import is_runtime_value
+from galaxy.tools.parameters.workflow_utils import is_runtime_value
 
 if typing.TYPE_CHECKING:
     from galaxy.tools import Tool
 
 log = logging.getLogger(__name__)
 
 SINGLE_EXECUTION_SUCCESS_MESSAGE = "Tool ${tool_id} created job ${job_id}"
```

### Comparing `galaxy-app-24.0.0/galaxy/tools/expressions/cwlNodeEngine.js` & `galaxy_app-24.0.1/galaxy/tools/expressions/cwlNodeEngine.js`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/expressions/evaluation.py` & `galaxy_app-24.0.1/galaxy/tools/expressions/evaluation.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/extract_dataset.xml` & `galaxy_app-24.0.1/galaxy/tools/extract_dataset.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/filter_empty_collection.xml` & `galaxy_app-24.0.1/galaxy/tools/filter_empty_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/filter_failed_collection.xml` & `galaxy_app-24.0.1/galaxy/tools/filter_failed_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/filter_from_file.xml` & `galaxy_app-24.0.1/galaxy/tools/filter_from_file.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/flatten_collection.xml` & `galaxy_app-24.0.1/galaxy/tools/flatten_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/harmonize_two_collections_list.xml` & `galaxy_app-24.0.1/galaxy/tools/harmonize_two_collections_list.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/imp_exp/__init__.py` & `galaxy_app-24.0.1/galaxy/tools/imp_exp/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/imp_exp/exp_history_to_archive.xml` & `galaxy_app-24.0.1/galaxy/tools/imp_exp/exp_history_to_archive.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/imp_exp/exp_history_to_uri.xml` & `galaxy_app-24.0.1/galaxy/tools/imp_exp/exp_history_to_uri.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/imp_exp/export_history.py` & `galaxy_app-24.0.1/galaxy/tools/imp_exp/export_history.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/imp_exp/imp_history_from_archive.xml` & `galaxy_app-24.0.1/galaxy/tools/imp_exp/imp_history_from_archive.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/imp_exp/unpack_tar_gz_archive.py` & `galaxy_app-24.0.1/galaxy/tools/imp_exp/unpack_tar_gz_archive.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/keep_success_collection.xml` & `galaxy_app-24.0.1/galaxy/tools/keep_success_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/merge_collection.xml` & `galaxy_app-24.0.1/galaxy/tools/merge_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/parameters/__init__.py` & `galaxy_app-24.0.1/galaxy/tools/parameters/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,27 +12,30 @@
 
 from galaxy.util import unicodify
 from galaxy.util.expressions import ExpressionContext
 from galaxy.util.json import safe_loads
 from .basic import (
     DataCollectionToolParameter,
     DataToolParameter,
-    is_runtime_value,
     ParameterValueError,
-    runtime_to_json,
     SelectToolParameter,
     ToolParameter,
 )
 from .grouping import (
     Conditional,
     Group,
     Repeat,
     Section,
     UploadDataset,
 )
+from .workflow_utils import (
+    is_runtime_value,
+    runtime_to_json,
+)
+from .wrapped import flat_to_nested_state
 
 REPLACE_ON_TRUTHY = object()
 
 # Some tools use the code tag and access the code base, expecting certain tool parameters to be available here.
 __all__ = ("DataCollectionToolParameter", "DataToolParameter", "SelectToolParameter")
 
 
@@ -511,14 +514,16 @@
     else:
         raise Exception(f"Input format {input_format} not recognized; input_format must be either legacy or 21.01.")
 
 
 def _populate_state_legacy(
     request_context, inputs, incoming, state, errors, prefix="", context=None, check=True, simple_errors=True
 ):
+    if context is None:
+        context = flat_to_nested_state(incoming)
     context = ExpressionContext(state, context)
     for input in inputs.values():
         state[input.name] = input.get_initial_value(request_context, context)
         key = prefix + input.name
         group_state = state[input.name]
         group_prefix = f"{key}|"
         if input.type == "repeat":
@@ -596,16 +601,16 @@
             while len(group_state) > file_count:
                 del group_state[-1]
             while file_count > len(group_state):
                 new_state = {"__index__": len(group_state)}
                 for upload_item in input.inputs.values():
                     new_state[upload_item.name] = upload_item.get_initial_value(request_context, context)
                 group_state.append(new_state)
-            for rep_state in group_state:
-                rep_index = rep_state["__index__"]
+            for rep_index, rep_state in enumerate(group_state):
+                rep_index = rep_state.get("__index__", rep_index)
                 rep_prefix = "%s_%d|" % (key, rep_index)
                 _populate_state_legacy(
                     request_context,
                     input.inputs,
                     incoming,
                     rep_state,
                     errors,
```

### Comparing `galaxy-app-24.0.0/galaxy/tools/parameters/basic.py` & `galaxy_app-24.0.1/galaxy/tools/parameters/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     HistoryDatasetAssociation,
     HistoryDatasetCollectionAssociation,
     LibraryDatasetDatasetAssociation,
 )
 from galaxy.model.dataset_collections import builder
 from galaxy.schema.fetch_data import FilesPayload
 from galaxy.tool_util.parser import get_input_source as ensure_input_source
-from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
+from galaxy.tools.parameters.workflow_utils import workflow_building_modes
 from galaxy.util import (
     sanitize_param,
     string_as_bool,
     string_as_bool_or_none,
     unicodify,
     XML,
 )
@@ -57,14 +57,20 @@
 from . import (
     dynamic_options,
     history_query,
     validation,
 )
 from .dataset_matcher import get_dataset_matcher_factory
 from .sanitize import ToolParameterSanitizer
+from .workflow_utils import (
+    is_runtime_value,
+    runtime_to_json,
+    runtime_to_object,
+    RuntimeValue,
+)
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
     from galaxy.security.idencoding import IdEncodingHelper
 
 log = logging.getLogger(__name__)
@@ -83,20 +89,14 @@
     if search and WORKFLOW_PARAMETER_REGULAR_EXPRESSION.search(value):
         return True
     if not search and WORKFLOW_PARAMETER_REGULAR_EXPRESSION.match(value):
         return True
     return False
 
 
-def is_runtime_value(value):
-    return isinstance(value, RuntimeValue) or (
-        isinstance(value, MutableMapping) and value.get("__class__") in ["RuntimeValue", "ConnectedValue"]
-    )
-
-
 def is_runtime_context(trans, other_values):
     if trans.workflow_building_mode:
         return True
     for context_value in other_values.values():
         if is_runtime_value(context_value):
             return True
         for v in util.listify(context_value):
@@ -888,14 +888,19 @@
             return self.value
 
     def to_dict(self, trans, other_values=None):
         d = super().to_dict(trans)
         return d
 
 
+def iter_to_string(iterable: typing.Iterable[typing.Any]) -> typing.Generator[str, None, None]:
+    for item in iterable:
+        yield str(item)
+
+
 class SelectToolParameter(ToolParameter):
     """
     Parameter that takes on one (or many) or a specific set of values.
 
     >>> from galaxy.util.bunch import Bunch
     >>> trans = Bunch(app=None, history=Bunch(), workflow_building_mode=False)
     >>> p = SelectToolParameter(None, XML(
@@ -1037,16 +1042,17 @@
                     is_dynamic=self.is_dynamic,
                 )
             if set(value).issubset(legal_values):
                 return value
             elif set(value).issubset(set(fallback_values.keys())):
                 return [fallback_values[v] for v in value]
             else:
+                invalid_options = iter_to_string(set(value) - set(legal_values))
                 raise ParameterValueError(
-                    f"invalid options ({','.join(set(value) - set(legal_values))!r}) were selected (valid options: {','.join(legal_values)})",
+                    f"invalid options ({','.join(invalid_options)!r}) were selected (valid options: {','.join(iter_to_string(legal_values))})",
                     self.name,
                     is_dynamic=self.is_dynamic,
                 )
         else:
             value_is_none = value == "None" and "None" not in legal_values
             if value_is_none or not value:
                 if self.multiple:
@@ -1062,15 +1068,15 @@
                 return value
             elif value in fallback_values:
                 return fallback_values[value]
             elif not require_legal_value:
                 return value
             else:
                 raise ParameterValueError(
-                    f"an invalid option ({value!r}) was selected (valid options: {','.join(legal_values)})",
+                    f"an invalid option ({value!r}) was selected (valid options: {','.join(iter_to_string(legal_values))})",
                     self.name,
                     value,
                     is_dynamic=self.is_dynamic,
                 )
 
     def to_param_dict_string(self, value, other_values=None):
         if value in (None, []):
@@ -1490,15 +1496,14 @@
         if self.usecolnames:
             dataset = other_values.get(self.data_ref, None)
             if (
                 hasattr(dataset, "metadata")
                 and hasattr(dataset.metadata, "column_names")
                 and dataset.metadata.element_is_set("column_names")
             ):
-                log.error(f"column_names {dataset.metadata.column_names}")
                 column_list = [
                     ("%d" % (i + 1), "c%d: %s" % (i + 1, x)) for i, x in enumerate(dataset.metadata.column_names)
                 ]
             else:
                 try:
                     with open(dataset.get_file_name()) as f:
                         head = f.readline()
@@ -2637,16 +2642,15 @@
         input_source = ensure_input_source(input_source)
         super().__init__(tool, input_source)
         self.data_ref = input_source.get("data_ref", None)
 
     def to_dict(self, trans, other_values=None):
         other_values = other_values or {}
         d = ToolParameter.to_dict(self, trans)
-        if (target_name := self.data_ref) in other_values:
-            target = other_values[target_name]
+        if target := other_values.get(self.data_ref):
             if not is_runtime_value(target):
                 d["target"] = {
                     "src": "hdca" if hasattr(target, "collection") else "hda",
                     "id": trans.app.security.encode_id(target.id),
                 }
         return d
 
@@ -2773,44 +2777,14 @@
     data_collection=DataCollectionToolParameter,
     rules=RulesListToolParameter,
     directory_uri=DirectoryUriToolParameter,
     drill_down=DrillDownSelectToolParameter,
 )
 
 
-def runtime_to_json(runtime_value):
-    if isinstance(runtime_value, ConnectedValue) or (
-        isinstance(runtime_value, MutableMapping) and runtime_value["__class__"] == "ConnectedValue"
-    ):
-        return {"__class__": "ConnectedValue"}
-    else:
-        return {"__class__": "RuntimeValue"}
-
-
-def runtime_to_object(runtime_value):
-    if isinstance(runtime_value, ConnectedValue) or (
-        isinstance(runtime_value, MutableMapping) and runtime_value["__class__"] == "ConnectedValue"
-    ):
-        return ConnectedValue()
-    else:
-        return RuntimeValue()
-
-
-class RuntimeValue:
-    """
-    Wrapper to note a value that is not yet set, but will be required at runtime.
-    """
-
-
-class ConnectedValue(RuntimeValue):
-    """
-    Wrapper to note a value that is not yet set, but will be inferred from a connection.
-    """
-
-
 def history_item_dict_to_python(value, app, name):
     if isinstance(value, MutableMapping) and "src" in value:
         if value["src"] not in ("hda", "dce", "ldda", "hdca"):
             raise ParameterValueError(f"Invalid value {value}", name)
         return src_id_to_item(sa_session=app.model.context, security=app.security, value=value)
```

### Comparing `galaxy-app-24.0.0/galaxy/tools/parameters/cancelable_request.py` & `galaxy_app-24.0.1/galaxy/tools/parameters/cancelable_request.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/parameters/dataset_matcher.py` & `galaxy_app-24.0.1/galaxy/tools/parameters/dataset_matcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
     def hdca_match(self, history_dataset_collection_association):
         dataset_collection = history_dataset_collection_association.collection
         return self.dataset_collection_match(dataset_collection)
 
     def dataset_collection_match(self, dataset_collection):
         # If dataset collection not yet populated, cannot determine if it
         # would be a valid match for this parameter.
-        if not dataset_collection.populated:
+        if not dataset_collection.populated_optimized:
             return False
 
         valid = True
         uses_implicit_conversion = False
         for element in dataset_collection.elements:
             match_element = self.__valid_element(element)
             if not match_element:
```

### Comparing `galaxy-app-24.0.0/galaxy/tools/parameters/dynamic_options.py` & `galaxy_app-24.0.1/galaxy/tools/parameters/dynamic_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,18 @@
     DatasetCollectionElement,
     HistoryDatasetAssociation,
     HistoryDatasetCollectionAssociation,
     MetadataFile,
     User,
 )
 from galaxy.tools.expressions import do_eval
-from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
+from galaxy.tools.parameters.workflow_utils import (
+    is_runtime_value,
+    workflow_building_modes,
+)
 from galaxy.util import (
     Element,
     string_as_bool,
 )
 from galaxy.util.template import fill_template
 from . import validation
 from .cancelable_request import request
@@ -733,24 +736,28 @@
                         continue
                     if getattr(dataset, "purged", False) or getattr(dataset, "deleted", False):
                         log.warning(f"The metadata file inferred from key `{meta_file_key}` was deleted!")
                         continue
                 if not hasattr(dataset, "get_file_name"):
                     continue
                 # Ensure parsing dynamic options does not consume more than a megabyte worth memory.
-                path = dataset.get_file_name()
-                if os.path.getsize(path) < 1048576:
-                    with open(path) as fh:
-                        options += self.parse_file_fields(fh)
-                else:
-                    # Pass just the first megabyte to parse_file_fields.
-                    log.warning("Attempting to load options from large file, reading just first megabyte")
-                    with open(path) as fh:
-                        contents = fh.read(1048576)
-                    options += self.parse_file_fields(StringIO(contents))
+                try:
+                    path = dataset.get_file_name()
+                    if os.path.getsize(path) < 1048576:
+                        with open(path) as fh:
+                            options += self.parse_file_fields(fh)
+                    else:
+                        # Pass just the first megabyte to parse_file_fields.
+                        log.warning("Attempting to load options from large file, reading just first megabyte")
+                        with open(path) as fh:
+                            contents = fh.read(1048576)
+                        options += self.parse_file_fields(StringIO(contents))
+                except Exception as e:
+                    log.warning("Could not read contents from %s: %s", dataset, str(e))
+                    continue
         elif self.tool_data_table:
             options = self.tool_data_table.get_fields()
             if trans and trans.user and trans.workflow_building_mode != workflow_building_modes.ENABLED:
                 options += self.get_user_options(trans.user)
         elif self.file_fields:
             options = list(self.file_fields)
         else:
@@ -961,14 +968,16 @@
             HistoryDatasetAssociation,
             DatasetCollectionElement,
             DatasetListWrapper,
             HistoryDatasetCollectionAssociation,
             list,
         ),
     ):
+        if is_runtime_value(ref):
+            return []
         raise ValueError
     if isinstance(ref, DatasetCollectionElement) and ref.hda:
         ref = ref.hda
     if isinstance(ref, (DatasetFilenameWrapper, HistoryDatasetAssociation)):
         ref = [ref]
     elif isinstance(ref, HistoryDatasetCollectionAssociation):
         ref = ref.to_hda_representative(multiple=True)
```

### Comparing `galaxy-app-24.0.0/galaxy/tools/parameters/grouping.py` & `galaxy_app-24.0.1/galaxy/tools/parameters/grouping.py`

 * *Files 0% similar despite different names*

```diff
@@ -614,16 +614,16 @@
         dbkey = self.get_dbkey(context)
         tag_using_filenames = context.get("tag_using_filenames", False)
         tags = context.get("tags", False)
         force_composite = asbool(context.get("force_composite", "False"))
         writable_files = d_type.writable_files
         writable_files_offset = 0
         groups_incoming = [None for _ in range(file_count)]
-        for group_incoming in context.get(self.name, []):
-            i = int(group_incoming["__index__"])
+        for i, group_incoming in enumerate(context.get(self.name, [])):
+            i = int(group_incoming.get("__index__", i))
             groups_incoming[i] = group_incoming
         if d_type.composite_type is not None or force_composite:
             # handle uploading of composite datatypes
             # Only one Dataset can be created
             dataset = Dataset()
             dataset.type = "composite"
             dataset.file_type = file_type
```

### Comparing `galaxy-app-24.0.0/galaxy/tools/parameters/history_query.py` & `galaxy_app-24.0.1/galaxy/tools/parameters/history_query.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/parameters/input_translation.py` & `galaxy_app-24.0.1/galaxy/tools/parameters/input_translation.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/parameters/meta.py` & `galaxy_app-24.0.1/galaxy/tools/parameters/meta.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from galaxy.model import HistoryDatasetCollectionAssociation
 from galaxy.model.dataset_collections import (
     matching,
     subcollections,
 )
 from galaxy.util import permutations
 from . import visit_input_values
+from .wrapped import process_key
 
 log = logging.getLogger(__name__)
 
 WorkflowParameterExpansion = namedtuple(
     "WorkflowParameterExpansion", ["param_combinations", "param_keys", "input_combinations"]
 )
 
@@ -149,39 +150,14 @@
         params_keys.append(new_keys)
         param_combinations.append(new_params)
         input_combinations.append(new_inputs)
 
     return WorkflowParameterExpansion(param_combinations, params_keys, input_combinations)
 
 
-def process_key(incoming_key, incoming_value, d):
-    key_parts = incoming_key.split("|")
-    if len(key_parts) == 1:
-        # Regular parameter
-        if incoming_key in d and not incoming_value:
-            # In case we get an empty repeat after we already filled in a repeat element
-            return
-        d[incoming_key] = incoming_value
-    elif key_parts[0].rsplit("_", 1)[-1].isdigit():
-        # Repeat
-        input_name, index = key_parts[0].rsplit("_", 1)
-        index = int(index)
-        d.setdefault(input_name, [])
-        newlist = [{} for _ in range(index + 1)]
-        d[input_name].extend(newlist[len(d[input_name]) :])
-        subdict = d[input_name][index]
-        process_key("|".join(key_parts[1:]), incoming_value=incoming_value, d=subdict)
-    else:
-        # Section / Conditional
-        input_name = key_parts[0]
-        subdict = {}
-        d[input_name] = subdict
-        process_key("|".join(key_parts[1:]), incoming_value=incoming_value, d=subdict)
-
-
 ExpandedT = Tuple[List[Dict[str, Any]], Optional[matching.MatchingCollections]]
 
 
 def expand_meta_parameters(trans, tool, incoming) -> ExpandedT:
     """
     Take in a dictionary of raw incoming parameters and expand to a list
     of expanded incoming parameters (one set of parameters per tool
@@ -262,14 +238,16 @@
             encoded_hdc_id = incoming_val["id"]
             subcollection_type = incoming_val.get("map_over_type", None)
         except TypeError:
             encoded_hdc_id = incoming_val
             subcollection_type = None
     hdc_id = trans.app.security.decode_id(encoded_hdc_id)
     hdc = trans.sa_session.get(HistoryDatasetCollectionAssociation, hdc_id)
+    if not hdc.collection.populated_optimized:
+        raise exceptions.ToolInputsNotReadyException("An input collection is not populated.")
     collections_to_match.add(input_key, hdc, subcollection_type=subcollection_type, linked=linked)
     if subcollection_type is not None:
         subcollection_elements = subcollections.split_dataset_collection_instance(hdc, subcollection_type)
         return subcollection_elements
     else:
         hdas = []
         for element in hdc.collection.dataset_elements:
```

### Comparing `galaxy-app-24.0.0/galaxy/tools/parameters/sanitize.py` & `galaxy_app-24.0.1/galaxy/tools/parameters/sanitize.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/parameters/validation.py` & `galaxy_app-24.0.1/galaxy/tools/parameters/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,17 @@
 
     def __init__(self, message, length_min, length_max, negate):
         if message is None:
             message = f"Must {'not ' if negate == 'true' else ''}have length of at least {length_min} and at most {length_max}"
         super().__init__(message, range_min=length_min, range_max=length_max, negate=negate)
 
     def validate(self, value, trans=None):
-        super().validate(len(value), trans)
+        if value is None:
+            raise ValueError("No value provided")
+        super().validate(len(value) if value else 0, trans)
 
 
 class DatasetOkValidator(Validator):
     """
     Validator that checks if a dataset is in an 'ok' state
     """
```

### Comparing `galaxy-app-24.0.0/galaxy/tools/parameters/wrapped.py` & `galaxy_app-24.0.1/galaxy/tools/parameters/wrapped.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from collections import UserDict
-from typing import Dict
+from typing import (
+    Any,
+    Dict,
+    List,
+)
 
 from galaxy.tools.parameters.basic import (
     DataCollectionToolParameter,
     DataToolParameter,
     SelectToolParameter,
 )
 from galaxy.tools.parameters.grouping import (
@@ -154,8 +158,40 @@
         elif isinstance(value, list):
             new_list.append(make_list_copy(value))
         else:
             new_list.append(value)
     return new_list
 
 
-__all__ = ("LegacyUnprefixedDict", "WrappedParameters", "make_dict_copy")
+def process_key(incoming_key: str, incoming_value: Any, d: Dict[str, Any]):
+    key_parts = incoming_key.split("|")
+    if len(key_parts) == 1:
+        # Regular parameter
+        if incoming_key in d and not incoming_value:
+            # In case we get an empty repeat after we already filled in a repeat element
+            return
+        d[incoming_key] = incoming_value
+    elif key_parts[0].rsplit("_", 1)[-1].isdigit():
+        # Repeat
+        input_name, _index = key_parts[0].rsplit("_", 1)
+        index = int(_index)
+        d.setdefault(input_name, [])
+        newlist: List[Dict[Any, Any]] = [{} for _ in range(index + 1)]
+        d[input_name].extend(newlist[len(d[input_name]) :])
+        subdict = d[input_name][index]
+        process_key("|".join(key_parts[1:]), incoming_value=incoming_value, d=subdict)
+    else:
+        # Section / Conditional
+        input_name = key_parts[0]
+        subdict = d.get(input_name, {})
+        d[input_name] = subdict
+        process_key("|".join(key_parts[1:]), incoming_value=incoming_value, d=subdict)
+
+
+def flat_to_nested_state(incoming: Dict[str, Any]):
+    nested_state: Dict[str, Any] = {}
+    for key, value in incoming.items():
+        process_key(key, value, nested_state)
+    return nested_state
+
+
+__all__ = ("LegacyUnprefixedDict", "WrappedParameters", "make_dict_copy", "process_key", "flat_to_nested_state")
```

### Comparing `galaxy-app-24.0.0/galaxy/tools/parameters/wrapped_json.py` & `galaxy_app-24.0.1/galaxy/tools/parameters/wrapped_json.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/recommendations.py` & `galaxy_app-24.0.1/galaxy/tools/recommendations.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import h5py
 import numpy as np
 import requests
 import yaml
 
 from galaxy.tools.parameters import populate_state
-from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
+from galaxy.tools.parameters.workflow_utils import workflow_building_modes
 from galaxy.util import DEFAULT_SOCKET_TIMEOUT
 from galaxy.workflow.modules import module_factory
 
 log = logging.getLogger(__name__)
 
 
 class ToolRecommendations:
```

### Comparing `galaxy-app-24.0.0/galaxy/tools/relabel_from_file.xml` & `galaxy_app-24.0.1/galaxy/tools/relabel_from_file.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/remote_tool_eval.py` & `galaxy_app-24.0.1/galaxy/tools/remote_tool_eval.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/repositories.py` & `galaxy_app-24.0.1/galaxy/tools/repositories.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/search/__init__.py` & `galaxy_app-24.0.1/galaxy/tools/search/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/sort_collection_list.xml` & `galaxy_app-24.0.1/galaxy/tools/sort_collection_list.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/special_tools.py` & `galaxy_app-24.0.1/galaxy/tools/special_tools.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/tag_collection_from_file.xml` & `galaxy_app-24.0.1/galaxy/tools/tag_collection_from_file.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/test.py` & `galaxy_app-24.0.1/galaxy/tools/test.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/unzip_collection.xml` & `galaxy_app-24.0.1/galaxy/tools/unzip_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/util/galaxyops/__init__.py` & `galaxy_app-24.0.1/galaxy/tools/util/galaxyops/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/util/maf_utilities.py` & `galaxy_app-24.0.1/galaxy/tools/util/maf_utilities.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/wrappers.py` & `galaxy_app-24.0.1/galaxy/tools/wrappers.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/tools/zip_collection.xml` & `galaxy_app-24.0.1/galaxy/tools/zip_collection.xml`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/data_providers/basic.py` & `galaxy_app-24.0.1/galaxy/visualization/data_providers/basic.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/data_providers/cigar.py` & `galaxy_app-24.0.1/galaxy/visualization/data_providers/cigar.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/data_providers/genome.py` & `galaxy_app-24.0.1/galaxy/visualization/data_providers/genome.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/__init__.py` & `galaxy_app-24.0.1/galaxy/visualization/data_providers/phyloviz/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/baseparser.py` & `galaxy_app-24.0.1/galaxy/visualization/data_providers/phyloviz/baseparser.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/newickparser.py` & `galaxy_app-24.0.1/galaxy/visualization/data_providers/phyloviz/newickparser.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/nexusparser.py` & `galaxy_app-24.0.1/galaxy/visualization/data_providers/phyloviz/nexusparser.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/data_providers/phyloviz/phyloxmlparser.py` & `galaxy_app-24.0.1/galaxy/visualization/data_providers/phyloviz/phyloxmlparser.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/data_providers/registry.py` & `galaxy_app-24.0.1/galaxy/visualization/data_providers/registry.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/genomes.py` & `galaxy_app-24.0.1/galaxy/visualization/genomes.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/plugins/config_parser.py` & `galaxy_app-24.0.1/galaxy/visualization/plugins/config_parser.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/plugins/plugin.py` & `galaxy_app-24.0.1/galaxy/visualization/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/plugins/registry.py` & `galaxy_app-24.0.1/galaxy/visualization/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/plugins/resource_parser.py` & `galaxy_app-24.0.1/galaxy/visualization/plugins/resource_parser.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/visualization/plugins/utils.py` & `galaxy_app-24.0.1/galaxy/visualization/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/webhooks/__init__.py` & `galaxy_app-24.0.1/galaxy/webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/work/context.py` & `galaxy_app-24.0.1/galaxy/work/context.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/workflow/extract.py` & `galaxy_app-24.0.1/galaxy/workflow/extract.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/workflow/modules.py` & `galaxy_app-24.0.1/galaxy/workflow/modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,33 +64,35 @@
     params_to_incoming,
     visit_input_values,
 )
 from galaxy.tools.parameters.basic import (
     BaseDataToolParameter,
     BooleanToolParameter,
     ColorToolParameter,
-    ConnectedValue,
     DataCollectionToolParameter,
     DataToolParameter,
     FloatToolParameter,
     HiddenToolParameter,
     IntegerToolParameter,
-    is_runtime_value,
     parameter_types,
     raw_to_galaxy,
-    runtime_to_json,
     SelectToolParameter,
     TextToolParameter,
 )
 from galaxy.tools.parameters.grouping import (
     Conditional,
     ConditionalWhen,
 )
 from galaxy.tools.parameters.history_query import HistoryQuery
-from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
+from galaxy.tools.parameters.workflow_utils import (
+    ConnectedValue,
+    is_runtime_value,
+    runtime_to_json,
+    workflow_building_modes,
+)
 from galaxy.tools.parameters.wrapped import make_dict_copy
 from galaxy.util import (
     listify,
     unicodify,
 )
 from galaxy.util.bunch import Bunch
 from galaxy.util.json import safe_loads
@@ -1985,26 +1987,14 @@
                 if (
                     is_data
                     and connections is not None
                     and steps is not None
                     and self.trans.workflow_building_mode is workflow_building_modes.USE_HISTORY
                 ):
                     if prefixed_name in input_connections_by_name:
-                        connection = input_connections_by_name[prefixed_name]
-                        output_step = next(
-                            output_step for output_step in steps if connection.output_step_id == output_step.id
-                        )
-                        if output_step.type.startswith("data"):
-                            output_inputs = output_step.module.get_runtime_inputs(output_step, connections=connections)
-                            output_value = output_inputs["input"].get_initial_value(self.trans, context)
-                            if input_type == "data" and isinstance(
-                                output_value, self.trans.app.model.HistoryDatasetCollectionAssociation
-                            ):
-                                return output_value.to_hda_representative()
-                            return output_value
                         return ConnectedValue()
                     else:
                         return input.get_initial_value(self.trans, context)
                 elif (is_data and connections is None) or prefixed_name in input_connections_by_name:
                     return ConnectedValue()
 
             visit_input_values(self.tool.inputs, self.state.inputs, callback)
@@ -2387,21 +2377,22 @@
             output_name = None
         if "action_arguments" in value:
             action_arguments = value["action_arguments"]
         else:
             action_arguments = None
         return PostJobAction(value["action_type"], step, output_name, action_arguments)
 
-    def get_informal_replacement_parameters(self, step) -> List[str]:
+    def get_informal_replacement_parameters(self, step: WorkflowStep) -> List[str]:
         """Return a list of replacement parameters."""
         replacement_parameters = set()
         for pja in step.post_job_actions:
-            for argument in pja.action_arguments.values():
-                for match in re.findall(r"\$\{(.+?)\}", unicodify(argument)):
-                    replacement_parameters.add(match)
+            if action_arguments := pja.action_arguments:
+                for argument in action_arguments.values():
+                    for match in re.findall(r"\$\{(.+?)\}", unicodify(argument)):
+                        replacement_parameters.add(match)
 
         return list(replacement_parameters)
 
 
 class WorkflowModuleFactory:
     def __init__(self, module_types: Dict[str, Type[WorkflowModule]]):
         self.module_types = module_types
```

### Comparing `galaxy-app-24.0.0/galaxy/workflow/refactor/execute.py` & `galaxy_app-24.0.1/galaxy/workflow/refactor/execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from typing import (
     Any,
     Dict,
 )
 
 from galaxy.exceptions import RequestParameterInvalidException
 from galaxy.tools.parameters import visit_input_values
-from galaxy.tools.parameters.basic import (
+from galaxy.tools.parameters.basic import contains_workflow_parameter
+from galaxy.tools.parameters.workflow_utils import (
     ConnectedValue,
-    contains_workflow_parameter,
     runtime_to_json,
 )
 from .schema import (
     AddInputAction,
     AddStepAction,
     ConnectAction,
     DisconnectAction,
```

### Comparing `galaxy-app-24.0.0/galaxy/workflow/refactor/schema.py` & `galaxy_app-24.0.1/galaxy/workflow/refactor/schema.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/workflow/render.py` & `galaxy_app-24.0.1/galaxy/workflow/render.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/workflow/reports/__init__.py` & `galaxy_app-24.0.1/galaxy/workflow/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/workflow/reports/generators/__init__.py` & `galaxy_app-24.0.1/galaxy/workflow/reports/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/workflow/reports/generators/markdown.py` & `galaxy_app-24.0.1/galaxy/workflow/reports/generators/markdown.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/workflow/resources/__init__.py` & `galaxy_app-24.0.1/galaxy/workflow/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/workflow/resources/example.py.sample` & `galaxy_app-24.0.1/galaxy/workflow/resources/example.py.sample`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/workflow/run.py` & `galaxy_app-24.0.1/galaxy/workflow/run.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/workflow/run_request.py` & `galaxy_app-24.0.1/galaxy/workflow/run_request.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/workflow/schedulers/__init__.py` & `galaxy_app-24.0.1/galaxy/workflow/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/workflow/schedulers/core.py` & `galaxy_app-24.0.1/galaxy/workflow/schedulers/core.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/workflow/scheduling_manager.py` & `galaxy_app-24.0.1/galaxy/workflow/scheduling_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy/workflow/steps.py` & `galaxy_app-24.0.1/galaxy/workflow/steps.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ This module contains utility methods for reasoning about and ordering
 workflow steps.
 """
 
 import math
+from itertools import chain
 
 from galaxy.util.topsort import (
     CycleError,
     topsort,
     topsort_levels,
 )
 
@@ -54,24 +55,24 @@
 
             for comment in comments:
                 if comment.type == "freehand":
                     freehand_comments.append(comment)
                 else:
                     sortable_comments.append(comment)
 
-            # consider comments to find normalization position
-            min_left_comments = min(comment.position[0] for comment in sortable_comments)
-            min_top_comments = min(comment.position[1] for comment in sortable_comments)
-            min_left = min(min_left_comments, min_left)
-            min_top = min(min_top_comments, min_top)
+            if sortable_comments:
+                # consider comments to find normalization position
+                min_left_comments = min(comment.position[0] for comment in sortable_comments)
+                min_top_comments = min(comment.position[1] for comment in sortable_comments)
+                min_left = min(min_left_comments, min_left)
+                min_top = min(min_top_comments, min_top)
 
             # normalize comments by min_left and min_top
-            for comment_list in [sortable_comments, freehand_comments]:
-                for comment in comment_list:
-                    comment.position = [comment.position[0] - min_left, comment.position[1] - min_top]
+            for comment in chain(sortable_comments, freehand_comments):
+                comment.position = [comment.position[0] - min_left, comment.position[1] - min_top]
 
             # order by Euclidean distance to the origin
             sortable_comments.sort(key=lambda comment: math.sqrt(comment.position[0] ** 2 + comment.position[1] ** 2))
 
             # replace comments list with sorted comments
             ordered_comments = freehand_comments
             ordered_comments.extend(sortable_comments)
```

### Comparing `galaxy-app-24.0.0/galaxy/workflow/trs_proxy.py` & `galaxy_app-24.0.1/galaxy/workflow/trs_proxy.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy_app.egg-info/PKG-INFO` & `galaxy_app-24.0.1/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,96 +1,55 @@
-Metadata-Version: 2.1
-Name: galaxy-app
-Version: 24.0.0
-Summary: Galaxy application (backend)
-Home-page: https://github.com/galaxyproject/galaxy
-Author: Galaxy Project and Community
-Author-email: galaxy-committers@lists.galaxyproject.org
-License: AFL
-Keywords: Galaxy
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: galaxy-auth
-Requires-Dist: galaxy-config
-Requires-Dist: galaxy-data
-Requires-Dist: galaxy-files
-Requires-Dist: galaxy-job-execution
-Requires-Dist: galaxy-job-metrics
-Requires-Dist: galaxy-objectstore
-Requires-Dist: galaxy-tool-util[cwl,edam]
-Requires-Dist: galaxy-tours
-Requires-Dist: galaxy-util
-Requires-Dist: galaxy-web-framework
-Requires-Dist: galaxy-web-stack
-Requires-Dist: Beaker
-Requires-Dist: boltons
-Requires-Dist: bx-python
-Requires-Dist: celery
-Requires-Dist: cloudauthz==0.6.0
-Requires-Dist: dparse
-Requires-Dist: gxformat2
-Requires-Dist: kombu>=5.3
-Requires-Dist: lagom
-Requires-Dist: lxml!=4.2.2
-Requires-Dist: Mako
-Requires-Dist: Markdown
-Requires-Dist: MarkupSafe
-Requires-Dist: packaging
-Requires-Dist: paramiko!=2.9.0,!=2.9.1
-Requires-Dist: pebble
-Requires-Dist: pulsar-galaxy-lib>=0.15.0.dev0
-Requires-Dist: pydantic!=2.6.0,!=2.6.1,>=2
-Requires-Dist: pysam>=0.21
-Requires-Dist: PyJWT
-Requires-Dist: PyYAML
-Requires-Dist: refgenconf>=0.12.0
-Requires-Dist: regex
-Requires-Dist: requests
-Requires-Dist: SQLAlchemy<2,>=1.4.25
-Requires-Dist: sqlitedict
-Requires-Dist: starlette
-Requires-Dist: svgwrite
-Requires-Dist: typing-extensions
-Requires-Dist: WebOb
-Requires-Dist: Whoosh
-
-
-.. image:: https://badge.fury.io/py/galaxy-app.svg
-   :target: https://pypi.org/project/galaxy-app/
+History
+-------
+
+.. to_doc
 
+-------------------
+24.0.1 (2024-05-02)
+-------------------
 
-Overview
---------
 
-The Galaxy_ application logic (backend).
+=========
+Bug fixes
+=========
+
+* Fix tool version switch in editor by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17858 <https://github.com/galaxyproject/galaxy/pull/17858>`_
+* Fix workflow run form failing on certain histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17869 <https://github.com/galaxyproject/galaxy/pull/17869>`_
+* Always serialize element_count and populated when listing contents by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17890 <https://github.com/galaxyproject/galaxy/pull/17890>`_
+* Fix saving workflows with freehand_comments only by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17901 <https://github.com/galaxyproject/galaxy/pull/17901>`_
+* Always discard session after __handle_waiting_jobs is done by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17913 <https://github.com/galaxyproject/galaxy/pull/17913>`_
+* Fix workflow run form for workflows with null rename PJA by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17929 <https://github.com/galaxyproject/galaxy/pull/17929>`_
+* Revert unnecessary error change by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17948 <https://github.com/galaxyproject/galaxy/pull/17948>`_
+* Fix missing implicit conversion for mapped over jobs by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17952 <https://github.com/galaxyproject/galaxy/pull/17952>`_
+* Fix get_content_as_text for compressed text datatypes by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17976 <https://github.com/galaxyproject/galaxy/pull/17976>`_
+* Backport: Fix bug: call unique() on result, not select stmt by `@jdavcs <https://github.com/jdavcs>`_ in `#17981 <https://github.com/galaxyproject/galaxy/pull/17981>`_
+* Fix `LengthValidator` if no value passed by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17983 <https://github.com/galaxyproject/galaxy/pull/17983>`_
+* Raise ``RequestParameterInvalidException`` if collection element has unknown extension by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17985 <https://github.com/galaxyproject/galaxy/pull/17985>`_
+* Don't attempt to commit in dry_run mode by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17987 <https://github.com/galaxyproject/galaxy/pull/17987>`_
+* Don't fail if reporting invalid parameter values by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18002 <https://github.com/galaxyproject/galaxy/pull/18002>`_
+* Include exception info when something goes wrong while refreshing tokens by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18008 <https://github.com/galaxyproject/galaxy/pull/18008>`_
+* Avoid exception when opening apply rules tool and no collection in history by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18011 <https://github.com/galaxyproject/galaxy/pull/18011>`_
+* Don't commit without having set a hid by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18014 <https://github.com/galaxyproject/galaxy/pull/18014>`_
+* Raise appropriate exception if user forces a collection that is not populated with elements as input by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18023 <https://github.com/galaxyproject/galaxy/pull/18023>`_
+* Fix tag regex pattern by `@jdavcs <https://github.com/jdavcs>`_ in `#18025 <https://github.com/galaxyproject/galaxy/pull/18025>`_
+* Fix History Dataset Association creation so that hid is always set by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18036 <https://github.com/galaxyproject/galaxy/pull/18036>`_
+* Change wrong quota_source value from KeyError to ValueError by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18040 <https://github.com/galaxyproject/galaxy/pull/18040>`_
+* Check database connection to issue a rollback if no connection by `@jdavcs <https://github.com/jdavcs>`_ in `#18070 <https://github.com/galaxyproject/galaxy/pull/18070>`_
 
-* Code: https://github.com/galaxyproject/galaxy
+============
+Enhancements
+============
 
-.. _Galaxy: http://galaxyproject.org/
+* Fix remote files sources error handling by `@davelopez <https://github.com/davelopez>`_ in `#18027 <https://github.com/galaxyproject/galaxy/pull/18027>`_
 
-History
--------
+=============
+Other changes
+=============
 
-.. to_doc
+* Drop left-over debug statement by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17939 <https://github.com/galaxyproject/galaxy/pull/17939>`_
 
 -------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
@@ -127,15 +86,15 @@
 * Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
 * Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
 * Toward declarative help for Galaxy markdown directives. by `@jmchilton <https://github.com/jmchilton>`_ in `#16979 <https://github.com/galaxyproject/galaxy/pull/16979>`_
 * Extend regex groups in stdio regex matches by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17016 <https://github.com/galaxyproject/galaxy/pull/17016>`_
 * Vueify Admin User Grid by `@guerler <https://github.com/guerler>`_ in `#17030 <https://github.com/galaxyproject/galaxy/pull/17030>`_
 * Remove web framework dependency from tools by `@davelopez <https://github.com/davelopez>`_ in `#17058 <https://github.com/galaxyproject/galaxy/pull/17058>`_
 * Add select parameter with options from remote resources by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17087 <https://github.com/galaxyproject/galaxy/pull/17087>`_
-*  Expose more tool information / navigability in UI. by `@jmchilton <https://github.com/jmchilton>`_ in `#17105 <https://github.com/galaxyproject/galaxy/pull/17105>`_
+* Expose more tool information / navigability in UI. by `@jmchilton <https://github.com/jmchilton>`_ in `#17105 <https://github.com/galaxyproject/galaxy/pull/17105>`_
 * Vueify Admin Roles Grid by `@guerler <https://github.com/guerler>`_ in `#17118 <https://github.com/galaxyproject/galaxy/pull/17118>`_
 * SA2.0 updates: handling "object is being merged into a Session along the backref cascade path" by `@jdavcs <https://github.com/jdavcs>`_ in `#17122 <https://github.com/galaxyproject/galaxy/pull/17122>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17123 <https://github.com/galaxyproject/galaxy/pull/17123>`_
 * Vueify Admin Groups Grid by `@guerler <https://github.com/guerler>`_ in `#17126 <https://github.com/galaxyproject/galaxy/pull/17126>`_
 * Towards SQLAlchemy 2.0: fix last cases of RemovedIn20Warning by `@jdavcs <https://github.com/jdavcs>`_ in `#17132 <https://github.com/galaxyproject/galaxy/pull/17132>`_
 * Vueify Admin Forms and Quota grids by `@guerler <https://github.com/guerler>`_ in `#17141 <https://github.com/galaxyproject/galaxy/pull/17141>`_
 * Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17157 <https://github.com/galaxyproject/galaxy/pull/17157>`_
```

### Comparing `galaxy-app-24.0.0/galaxy_app.egg-info/SOURCES.txt` & `galaxy_app-24.0.1/galaxy_app.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -547,15 +547,15 @@
 galaxy/tools/parameters/dynamic_options.py
 galaxy/tools/parameters/grouping.py
 galaxy/tools/parameters/history_query.py
 galaxy/tools/parameters/input_translation.py
 galaxy/tools/parameters/meta.py
 galaxy/tools/parameters/sanitize.py
 galaxy/tools/parameters/validation.py
-galaxy/tools/parameters/workflow_building_modes.py
+galaxy/tools/parameters/workflow_utils.py
 galaxy/tools/parameters/wrapped.py
 galaxy/tools/parameters/wrapped_json.py
 galaxy/tools/search/__init__.py
 galaxy/tools/util/__init__.py
 galaxy/tools/util/maf_utilities.py
 galaxy/tools/util/galaxyops/__init__.py
 galaxy/visualization/__init__.py
```

### Comparing `galaxy-app-24.0.0/galaxy_app.egg-info/requires.txt` & `galaxy_app-24.0.1/galaxy_app.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy_ext/expressions/handle_job.py` & `galaxy_app-24.0.1/galaxy_ext/expressions/handle_job.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/galaxy_ext/metadata/set_metadata.py` & `galaxy_app-24.0.1/galaxy_ext/metadata/set_metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/setup.cfg` & `galaxy_app-24.0.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-app
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-auth
 	galaxy-config
 	galaxy-data
```

### Comparing `galaxy-app-24.0.0/tool_shed_client/schema/__init__.py` & `galaxy_app-24.0.1/tool_shed_client/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/tool_shed_client/schema/trs.py` & `galaxy_app-24.0.1/tool_shed_client/schema/trs.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/tool_shed_client/schema/trs_service_info.py` & `galaxy_app-24.0.1/tool_shed_client/schema/trs_service_info.py`

 * *Files identical despite different names*

### Comparing `galaxy-app-24.0.0/tool_shed_client/trs_util.py` & `galaxy_app-24.0.1/tool_shed_client/trs_util.py`

 * *Files identical despite different names*

