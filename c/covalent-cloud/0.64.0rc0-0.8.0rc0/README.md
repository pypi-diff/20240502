# Comparing `tmp/covalent-cloud-0.64.0rc0.tar.gz` & `tmp/covalent-cloud-0.8.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-cloud-0.64.0rc0.tar", last modified: Thu May  2 14:26:59 2024, max compression
+gzip compressed data, was "covalent-cloud-0.8.0rc0.tar", last modified: Sat Apr 29 00:10:27 2023, max compression
```

## Comparing `covalent-cloud-0.64.0rc0.tar` & `covalent-cloud-0.8.0rc0.tar`

### file list

```diff
@@ -1,101 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.972017 covalent-cloud-0.64.0rc0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-02 14:26:59.972017 covalent-cloud-0.64.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.960017 covalent-cloud-0.64.0rc0/covalent_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.964017 covalent-cloud-0.64.0rc0/covalent_cloud/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/analytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.964017 covalent-cloud-0.64.0rc0/covalent_cloud/cloud_executor/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/cloud_executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/cloud_executor/cloud_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.964017 covalent-cloud-0.64.0rc0/covalent_cloud/cloud_executor/models/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/cloud_executor/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/cloud_executor/models/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/cloud_executor/models/sw_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.964017 covalent-cloud-0.64.0rc0/covalent_cloud/dispatch_management/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/dispatch_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15397 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/dispatch_management/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11287 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/dispatch_management/interface_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17058 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/dispatch_management/results_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.964017 covalent-cloud-0.64.0rc0/covalent_cloud/function_serve/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/function_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4462 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/function_serve/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/function_serve/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/function_serve/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/function_serve/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/function_serve/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/function_serve/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13575 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/function_serve/service_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.964017 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.964017 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/executors/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/executors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.968016 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/middleware/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.968016 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/middleware/qclients/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/middleware/qclients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/middleware/qclients/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/middleware/qclients/remote_qclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.968016 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/qelectron_sdk/schemas/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.968016 covalent-cloud-0.64.0rc0/covalent_cloud/service_account_interface/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/service_account_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/service_account_interface/auth_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/service_account_interface/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.968016 covalent-cloud-0.64.0rc0/covalent_cloud/shared/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/shared/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.968016 covalent-cloud-0.64.0rc0/covalent_cloud/shared/classes/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/shared/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/shared/classes/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/shared/classes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/shared/classes/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/shared/classes/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.968016 covalent-cloud-0.64.0rc0/covalent_cloud/shared/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/shared/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/shared/schemas/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.968016 covalent-cloud-0.64.0rc0/covalent_cloud/software_environment/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/software_environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.968016 covalent-cloud-0.64.0rc0/covalent_cloud/swe_management/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/swe_management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.968016 covalent-cloud-0.64.0rc0/covalent_cloud/swe_management/models/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/swe_management/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/swe_management/models/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/swe_management/secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/swe_management/swe_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.968016 covalent-cloud-0.64.0rc0/covalent_cloud/volume/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/covalent_cloud/volume/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.964017 covalent-cloud-0.64.0rc0/covalent_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-02 14:26:59.000000 covalent-cloud-0.64.0rc0/covalent_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-02 14:26:59.000000 covalent-cloud-0.64.0rc0/covalent_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:26:59.000000 covalent-cloud-0.64.0rc0/covalent_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 14:26:59.000000 covalent-cloud-0.64.0rc0/covalent_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 14:26:59.000000 covalent-cloud-0.64.0rc0/covalent_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 14:26:59.972017 covalent-cloud-0.64.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.960017 covalent-cloud-0.64.0rc0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.972017 covalent-cloud-0.64.0rc0/tests/dispatch_management_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/tests/dispatch_management_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/tests/dispatch_management_tests/future_classes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/tests/dispatch_management_tests/helpers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/tests/dispatch_management_tests/interface_functions_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.972017 covalent-cloud-0.64.0rc0/tests/function_serve_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/tests/function_serve_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/tests/function_serve_tests/deployment_info_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.972017 covalent-cloud-0.64.0rc0/tests/shared/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/tests/shared/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.972017 covalent-cloud-0.64.0rc0/tests/shared/classes/
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/tests/shared/classes/APIClient_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/tests/shared/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/tests/shared/classes/helpers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:26:59.972017 covalent-cloud-0.64.0rc0/tests/swe_management_tests/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/tests/swe_management_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-05-02 14:26:47.000000 covalent-cloud-0.64.0rc0/tests/swe_management_tests/swe_manager_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.444949 covalent-cloud-0.8.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-29 00:10:27.444949 covalent-cloud-0.8.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/electron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/transport_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/analytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/cloud_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/sw_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/interface_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/results_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/auth_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/electron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/transport_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/software_environment/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/software_environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/swe_management/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/swe_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/swe_management/swe_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-29 00:10:27.444949 covalent-cloud-0.8.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/future_classes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/helpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/interface_functions_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/shared/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/shared/classes/APIClient_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/shared/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/swe_management_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/swe_management_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/swe_management_tests/swe_manager_test.py
```

### Comparing `covalent-cloud-0.64.0rc0/LICENSE` & `covalent-cloud-0.8.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.64.0rc0/PKG-INFO` & `covalent-cloud-0.8.0rc0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: covalent-cloud
-Version: 0.64.0rc0
+Version: 0.8.0rc0
 Summary: Covalent Cloud SDK
 Home-page: https://github.com/AgnostiqHQ/covalent-cloud-sdk
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
-Download-URL: https://github.com/AgnostiqHQ/covalent-cloud-sdk/archive/v0.64.0.tar.gz
-Description: 
+Download-URL: https://github.com/AgnostiqHQ/covalent-cloud-sdk/archive/v0.8.0.tar.gz
+Description: &nbsp;
+        
+        <div align="center">
+        
+        [![covalent](https://img.shields.io/badge/covalent-0.208.0rc0-purple)](https://github.com/AgnostiqHQ/covalent)
+        [![agpl](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0.en.html)
+        
+        </div>
+        
         ## Covalent Cloud SDK
         
-        [Covalent](https://github.com/AgnostiqHQ/covalent) is a python based workflow orchestration tool used to execute HPC and quantum tasks in heterogeneous environments.
+        [Covalent](https://github.com/AgnostiqHQ/covalent) is a python based workflow orchestration tool used to execute HPC and quantum tasks in heterogenous environments.
         
         Installing Covalent Cloud SDK gives users access to the enterprise version of Covalent.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
```

### Comparing `covalent-cloud-0.64.0rc0/covalent_cloud/dispatch_management/helpers.py` & `covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/results_manager.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,488 +1,525 @@
 # Copyright 2023 Agnostiq Inc.
 
 
-"""Module for Covalent Cloud dispatching and related functionalities."""
+"""Helpers for result fetching."""
 
-import json
+
+from __future__ import annotations
+
+import enum
 import os
-import sys
-import tempfile
-from concurrent.futures import ThreadPoolExecutor, wait
-from copy import deepcopy
-from functools import wraps
 from pathlib import Path
-from typing import Callable, List, Optional, Union
+from typing import Any, Optional
 
-import covalent as ct
 import requests
 from covalent._results_manager.result import Result
-from covalent._serialize.result import merge_response_manifest, serialize_result, strip_local_uris
+from covalent._results_manager.wait import EXTREME
 from covalent._shared_files import logger
-from covalent._shared_files.defaults import parameter_prefix
-from covalent._shared_files.schemas.asset import AssetSchema
-from covalent._shared_files.schemas.result import ResultSchema
-from covalent._workflow.lattice import Lattice
+from covalent._shared_files.exceptions import MissingLatticeRecordError
+from covalent._workflow.transport import TransportableObject
 from requests.adapters import HTTPAdapter
-from rich.progress import BarColumn, MofNCompleteColumn, Progress, TaskID
-from urllib3.util.retry import Retry
-
-from covalent_cloud.shared.schemas.volume import Volume
+from urllib3.util import Retry
 
-from ..shared.classes.api import APIClient
-from ..shared.classes.exceptions import (
-    CovalentAPIKeyError,
-    CovalentGenericAPIError,
-    CovalentSDKError,
-)
+from .._serialize.common import load_asset
+from .._serialize.electron import ASSET_FILENAME_MAP as ELECTRON_ASSET_FILENAMES
+from .._serialize.electron import ASSET_TYPES as ELECTRON_ASSET_TYPES
+from .._serialize.lattice import ASSET_FILENAME_MAP as LATTICE_ASSET_FILENAMES
+from .._serialize.lattice import ASSET_TYPES as LATTICE_ASSET_TYPES
+from .._serialize.result import ASSET_FILENAME_MAP as RESULT_ASSET_FILENAMES
+from .._serialize.result import ASSET_TYPES as RESULT_ASSET_TYPES
+from .._serialize.result import deserialize_result
+from ..shared.classes.api import AuthConfigManager
 from ..shared.classes.settings import Settings, settings
-
-_dispatch_executor = ThreadPoolExecutor()
-
-_VALID_EXECUTORS = {"cloud"}
-
-dispatch_cache_dir = Path(settings.dispatch_cache_dir)
-dispatch_cache_dir.mkdir(parents=True, exist_ok=True)
+from ..shared.schemas.asset import AssetSchema
+from ..shared.schemas.result import ResultSchema
 
 app_log = logger.app_log
+log_stack_info = logger.log_stack_info
 
 
-class AssetUploadThreadFailure(CovalentSDKError):
-    message: str = "One or more asset upload threads did not finish execution."
-    code: str = "dispatch/asset-upload-thread/fail"
-
-    def __init__(self) -> None:
-        super().__init__(self.message, self.code)
-
-
-class AssetUploadException(CovalentSDKError):
-    message: str = "One or more asset upload raised exceptions."
-    code: str = "dispatch/asset-upload/exception"
-
-    def __init__(self, msg: str = ""):
-        super().__init__(message=msg, code=self.code)
-
-
-def validate_executors(lat: Lattice) -> bool:
-    # Check lattice default executor and workflow_executor
-
-    valid_lattice_executors = True
-    valid_electron_executors = True
-
-    if lat.metadata["executor"] not in _VALID_EXECUTORS:
-        app_log.debug(f"Found illegal lattice executor: {lat.metadata['executor']}")
-        valid_lattice_executors = False
-    if lat.metadata["workflow_executor"] not in _VALID_EXECUTORS:
-        app_log.debug(
-            f"Found illegal lattice workflow executor: {lat.metadata['workflow_executor']}"
-        )
-        valid_lattice_executors = False
-
-    tg = lat.transport_graph
-
-    for i in tg._graph.nodes:
-        name = tg.get_node_value(i, "name")
-
-        if name.startswith(parameter_prefix):
-            continue
-
-        metadata = tg.get_node_value(i, "metadata")
-        if metadata["executor"] not in _VALID_EXECUTORS:
-            app_log.debug(f"Found illegal electron executor: {metadata['executor']} in node {i}")
-            valid_electron_executors = False
-            break
-
-    return valid_lattice_executors and valid_electron_executors
-
+SDK_NODE_META_KEYS = {
+    "executor",
+    "executor_data",
+    "deps",
+    "call_before",
+    "call_after",
+}
+
+SDK_LAT_META_KEYS = {
+    "executor",
+    "executor_data",
+    "workflow_executor",
+    "workflow_executor_data",
+    "deps",
+    "call_before",
+    "call_after",
+}
+
+DEFERRED_KEYS = {
+    "output",
+    "value",
+    "result",
+}
+
+
+# Multi-part
+
+
+class AssetScope(enum.Enum):
+    RESULT = "result"
+    LATTICE = "lattice"
+    NODE = "node"
+
+
+# Utility function to decode TransportableObjects
+def _decode(value: Any):
+    if isinstance(value, TransportableObject):
+        return value.get_deserialized()
+    else:
+        return value
 
-def associate_volume_to_executors(lat: Lattice, volume: Volume) -> bool:
 
-    lat.metadata["executor_data"]["attributes"]["volume_id"] = volume.id
-    lat.metadata["workflow_executor_data"]["attributes"]["volume_id"] = volume.id
+class FutureVar:
+    """A class that represents a variable that is not yet available.
 
-    tg = lat.transport_graph
+    List of private attributes: _dispatch_id, _task_id, _name
+    List of public and immutable attributes: value
+    """
 
-    for i in tg._graph.nodes:
-        name = tg.get_node_value(i, "name")
+    def __init__(
+        self,
+        result_manager: ResultManager,
+        scope: AssetScope,
+        name: str,
+        dispatch_id: str,
+        task_id: Optional[int],
+    ):
+        self._scope = scope
+        self._dispatch_id = dispatch_id
+        self._task_id = task_id
+        self._name = name
+        self._value = None
+        self._result_manager = result_manager
+        self._downloaded = False
+
+        if self._scope == AssetScope.RESULT:
+            size = self._result_manager._manifest["assets"][name]["size"]
+
+        if self._scope == AssetScope.LATTICE:
+            size = self._result_manager._manifest["lattice"]["assets"][name]["size"]
+
+        if self._scope == AssetScope.NODE:
+            node = self._result_manager._manifest["lattice"]["transport_graph"]["nodes"][task_id]
+            size = node["assets"][name]["size"]
+
+        self._size = size
+
+    @property
+    def value(self):
+        return self._value
+
+    @property
+    def size(self):
+        return self._size
+
+    # TODO - save artifacts to local storage first instead of loading
+    # them entirely in memory.
+    def load(self) -> None:
+        """Query Covalent Cloud to retrieve and populate 'value' attribute.'"""
+
+        if self._scope == AssetScope.RESULT:
+            if not self._downloaded:
+                self._result_manager.download_result_asset(self._name)
+                self._downloaded = True
+            self._value = _decode(self._result_manager.load_result_asset(self._name))
+
+        if self._scope == AssetScope.LATTICE:
+            if not self._downloaded:
+                self._result_manager.download_lattice_asset(self._name)
+                self._downloaded = True
+            self._value = _decode(self._result_manager.load_lattice_asset(self._name))
+
+        if self._scope == AssetScope.NODE:
+            if not self._downloaded:
+                self._result_manager.download_node_asset(self._task_id, self._name)
+                self._downloaded = True
+            self._value = _decode(self._result_manager.load_node_asset(self._task_id, self._name))
+
+    def __str__(self) -> str:
+        if self._downloaded:
+            return str(self.value)
+        else:
+            return "<FutureVar>"
 
-        if name.startswith(parameter_prefix):
-            continue
+    # infinite recursion
+    def __deepcopy__(self, memo):
+        """Make a deep copy.
 
-        metadata = tg.get_node_value(i, "metadata")
-        metadata["executor_data"]["attributes"]["volume_id"] = volume.id
+        Detaches the result_manager attribute to avoid infinite
+        recursion.
 
+        """
+        cls = type(self)
+        fv = cls.__new__(cls)
+        fv.__init__(None, self._scope, self._name, self._dispatch_id, self._task_id)
+        return fv
 
-def inject_parameter_outputs(lat: Lattice):
-    # Hack to pre-compute the output of parameter nodes. This will be
-    # no longer needed once OS develop does the same during
-    # `build_graph`.
 
-    tg = lat.transport_graph
-    if not tg._graph.nodes:
-        return
+class FutureResult(Result):
+    """A class that represents a dispatch result that is not yet available.
 
-    for node_id in tg._graph.nodes:
-        name = tg.get_node_value(node_id, "name")
-        if name.startswith(parameter_prefix):
-            value = tg.get_node_value(node_id, "value")
-            tg.set_node_value(node_id, "output", value)
+    List of private attributes: _dispatch_id, _root_dispatch_id
+    List of public and immutable attributes: dispatch_name, start_time, end_time, status, lattice, result, inputs, error
+    """
 
+    @property
+    def result(self) -> Any:
+        return self._result
+
+    @property
+    def inputs(self) -> Any:
+        return self._inputs
+
+    @property
+    def error(self) -> str:
+        return self._error
+
+    @staticmethod
+    def _from_result_object(res: Result):
+        fr = FutureResult(res.lattice)
+        fr.__dict__ = res.__dict__
+        return fr
+
+    def __str__(self):
+        """String representation of the result object"""
+
+        show_result_str = f"""
+Lattice Result
+==============
+status: {self._status}
+result: {self.result}
+inputs: {self.inputs}
+error: {self.error}
+
+start_time: {self.start_time}
+end_time: {self.end_time}
+
+dispatch_id: {self.dispatch_id}
+
+Node Outputs
+------------
+"""
+        node_outputs = self.get_all_node_outputs()
+        for k, v in node_outputs.items():
+            show_result_str += f"{k}: {v}\n"
 
-# For multistage dispatches
+        return show_result_str
 
 
-def register(
-    orig_lattice: Lattice,
-    volume: Union[Volume, None] = None,
+def _get_result_export_from_dispatcher(
+    dispatch_id: str,
+    wait: bool = False,
+    status_only: bool = False,
     settings: Settings = settings,
-) -> Callable:
+) -> ResultSchema:
     """
-    Wrapping the dispatching functionality to allow input passing
-    and server address specification.
-
-    Afterwards, send the lattice to the dispatcher server and return
-    the assigned dispatch id.
+    Internal function to get the results of a dispatch from the server without checking if it is ready to read.
 
     Args:
-        orig_lattice: The lattice/workflow to send to the dispatcher server.
-        volume: [optional] Volume instance
-        dispatcher_addr: The address of the dispatcher server.  If None then then defaults to the address set in Covalent's config.
+        dispatch_id: The dispatch id of the result.
+        wait: Controls how long the method waits for the server to return a result. If False, the method will not wait and will return the current status of the workflow. If True, the method will wait for the result to finish and keep retrying for sys.maxsize.
+        status_only: If true, only returns result status, not the full result object, default is False.
+        dispatcher_addr: Dispatcher server address, defaults to the address set in covalent.config.
 
     Returns:
-        Wrapper function which takes the inputs of the workflow as arguments
+        The result object from the server.
+
+    Raises:
+        MissingLatticeRecordError: If the result is not found.
     """
 
     dispatcher_addr = settings.dispatcher_uri
 
-    @wraps(orig_lattice)
-    def wrapper(*args, **kwargs) -> str:
-        """
-        Send the lattice to the dispatcher server and return
-        the assigned dispatch id.
+    retries = int(EXTREME) if wait else 5
 
-        Args:
-            *args: The inputs of the workflow.
-            **kwargs: The keyword arguments of the workflow.
-
-        Returns:
-            The dispatch id of the workflow.
-        """
-
-        try:
-
-            lattice = deepcopy(orig_lattice)
-
-            # Enabling task_packing for the build_graph call as it isn't
-            # supported yet by OS covalent.
-            old_task_packing = ct.get_config("sdk.task_packing")
-            ct.set_config("sdk.task_packing", "true")
-            lattice.build_graph(*args, **kwargs)
-            ct.set_config("sdk.task_packing", old_task_packing)
-
-            if volume:
-                associate_volume_to_executors(lattice, volume)
-
-            # Temporary workaround until OS develop also
-            # does this during `build_graph.
-            inject_parameter_outputs(lattice)
-
-            with tempfile.TemporaryDirectory() as tmp_dir:
-                if settings.redispatch.is_redispatch:
-                    redispatch_id = settings.redispatch.id
-                else:
-                    redispatch_id = ""
-                manifest = prepare_manifest(lattice, tmp_dir, redispatch_id)
-                return_manifest = register_manifest(manifest, settings)
-                new_dispatch_id = return_manifest.metadata.dispatch_id
-
-                path = dispatch_cache_dir / f"{new_dispatch_id}"
-
-                with open(path, "w") as f:
-                    f.write(manifest.json())
+    adapter = HTTPAdapter(max_retries=Retry(total=retries, backoff_factor=1))
+    http = requests.Session()
+    http.mount("http://", adapter)
+    http.mount("https://", adapter)
+    url = dispatcher_addr + "/api/v1/export/" + dispatch_id
+
+    api_key = AuthConfigManager.get_api_key(settings)
+    headers = {"x-api-key": api_key}
+
+    response = http.get(
+        url,
+        params={"wait": bool(int(wait)), "status_only": status_only},
+        headers=headers,
+    )
+    if response.status_code == 404:
+        raise MissingLatticeRecordError
+    response.raise_for_status()
+    export = response.json()
+    return export
 
-                upload_assets(manifest)
 
-                return new_dispatch_id
+# Functions for computing local URIs
+def get_node_asset_path(results_dir: str, node_id: int, key: str):
+    filename = ELECTRON_ASSET_FILENAMES[key]
+    return results_dir + f"/node_{node_id}/{filename}"
 
-        except Exception as e:
-            raise e
 
-    return wrapper
+def get_lattice_asset_path(results_dir: str, key: str):
+    filename = LATTICE_ASSET_FILENAMES[key]
+    return results_dir + f"/{filename}"
 
 
-def start(
-    dispatch_id: str,
-    settings: Settings = settings,
-) -> Callable:
-    """
-    Wrapping the dispatching functionality to allow input passing
-    and server address specification.
+def get_result_asset_path(results_dir: str, key: str):
+    filename = RESULT_ASSET_FILENAMES[key]
+    return results_dir + f"/{filename}"
 
-    Afterwards, send the lattice to the dispatcher server and return
-    the assigned dispatch id.
 
-    Args:
-        orig_lattice: The lattice/workflow to send to the dispatcher server.
-        dispatcher_addr: The address of the dispatcher server.  If None then then defaults to the address set in Covalent's config.
+# Asset transfers
 
-    Returns:
-        Wrapper function which takes the inputs of the workflow as arguments
-    """
 
-    dispatcher_addr = settings.dispatcher_uri
-    dispatcher_port = settings.dispatcher_port
+def download_asset(remote_uri: str, local_path: str, chunk_size: int = 1024 * 1024):
+    api_key = AuthConfigManager.get_api_key(settings)
+    headers = {"x-api-key": api_key}
+    r = requests.get(remote_uri, stream=True, headers=headers)
+    r.raise_for_status()
+    with open(local_path, "wb") as f:
+        for chunk in r.iter_content(chunk_size=chunk_size):
+            f.write(chunk)
 
-    client = APIClient(host_uri=dispatcher_addr, settings=settings, port=dispatcher_port)
-    endpoint = f"/api/v1/dispatchv2/start/{dispatch_id}"
 
-    try:
-        r = client.put(endpoint)
-    except requests.exceptions.HTTPError as e:
-        print(e.response.text, file=sys.stderr)
-        raise e
-    return r.content.decode("utf-8").strip().replace('"', "")
+def _get_result_asset_uri(manifest: dict, key: str) -> str:
+    return manifest["assets"][key]["remote_uri"]
 
 
-def prepare_manifest(lattice, storage_path, dispatch_id: str = "") -> ResultSchema:
-    """Prepare a built-out lattice for submission"""
+def _download_result_asset(manifest: dict, results_dir: str, key: str):
+    remote_uri = manifest["assets"][key]["remote_uri"]
+    local_path = get_result_asset_path(results_dir, key)
+    download_asset(remote_uri, local_path)
+    manifest["assets"][key]["uri"] = "file://" + local_path
 
-    result_object = Result(lattice, dispatch_id=dispatch_id)
-    return serialize_result(result_object, storage_path)
 
+def _get_lattice_asset_uri(manifest: dict, key: str) -> str:
+    lattice_assets = manifest["lattice"]["assets"]
+    return lattice_assets[key]["remote_uri"]
 
-def register_manifest(
-    manifest: ResultSchema,
-    settings: Settings = settings,
-    parent_dispatch_id: Optional[str] = None,
-    push_assets: bool = True,
-) -> ResultSchema:
-    """Submits a manifest for registration.
 
-    Returns:
-        Dictionary representation of manifest with asset remote_uris filled in
+def _download_lattice_asset(manifest: dict, results_dir: str, key: str):
+    lattice_assets = manifest["lattice"]["assets"]
+    remote_uri = lattice_assets[key]["remote_uri"]
+    local_path = get_lattice_asset_path(results_dir, key)
+    download_asset(remote_uri, local_path)
+    lattice_assets[key]["uri"] = "file://" + local_path
 
-    Side effect:
-        If push_assets is False, the server will
-        automatically pull the task assets from the submitted asset URIs.
 
-    Raises:
-        CovalentAPIKeyError: If the API key is invalid.
+def _get_node_asset_uri(manifest: dict, node_id: int, key: str):
+    node = manifest["lattice"]["transport_graph"]["nodes"][node_id]
+    node_assets = node["assets"]
+    return node_assets[key]["remote_uri"]
 
-    """
-    dispatcher_addr = settings.dispatcher_uri
-    dispatcher_port = settings.dispatcher_port
 
-    stripped = strip_local_uris(manifest) if push_assets else manifest
-    client = APIClient(
-        host_uri=dispatcher_addr,
-        settings=settings,
-        port=dispatcher_port,
-        headers={"Content-Type": "application/json"},
-    )
-    endpoint = "/api/v2/lattices"
+def _download_node_asset(manifest: dict, results_dir: str, node_id: int, key: str):
+    node = manifest["lattice"]["transport_graph"]["nodes"][node_id]
+    node_assets = node["assets"]
+    remote_uri = node_assets[key]["remote_uri"]
+    local_path = get_node_asset_path(results_dir, node_id, key)
+    download_asset(remote_uri, local_path)
+    node_assets[key]["uri"] = "file://" + local_path
 
-    if parent_dispatch_id:
-        endpoint = f"{endpoint}/{parent_dispatch_id}"
 
-    try:
-        r = client.post(endpoint, request_options={"data": stripped.json()})
-    except requests.exceptions.HTTPError as e:
-        if e.response.status_code == 401 and e.response.json()["code"] == "auth/unauthorized":
-            raise CovalentAPIKeyError(
-                message="A valid API key is required to register a dispatch.",
-                code=e.response.json()["code"],
-            ) from e
-        else:
-            raise CovalentGenericAPIError(error=e)
+def _load_result_asset(manifest: dict, key: str):
+    asset_meta = AssetSchema(**manifest["assets"][key])
+    return load_asset(asset_meta, RESULT_ASSET_TYPES[key])
 
-    parsed_resp = ResultSchema.parse_obj(r.json())
 
-    return merge_response_manifest(manifest, parsed_resp)
+def _load_lattice_asset(manifest: dict, key: str):
+    asset_meta = AssetSchema(**manifest["lattice"]["assets"][key])
+    return load_asset(asset_meta, LATTICE_ASSET_TYPES[key])
 
 
-def upload_assets(manifest: ResultSchema):
-    assets = _extract_assets(manifest)
-    _upload(assets)
+def _load_node_asset(manifest: dict, node_id: int, key: str):
+    node = manifest["lattice"]["transport_graph"]["nodes"][node_id]
+    asset_meta = AssetSchema(**node["assets"][key])
+    return load_asset(asset_meta, ELECTRON_ASSET_TYPES[key])
 
 
-def _extract_assets(manifest: ResultSchema) -> List[AssetSchema]:
-    # workflow-level assets
-    dispatch_assets = manifest.assets
-    assets = [asset for key, asset in dispatch_assets]
-    lattice = manifest.lattice
-    lattice_assets = lattice.assets
-    assets.extend(asset for key, asset in lattice_assets)
-    # Node assets
-    tg = lattice.transport_graph
-    nodes = tg.nodes
-    for node in nodes:
-        node_assets = node.assets
-        assets.extend(asset for key, asset in node_assets)
-    return assets
+class ResultManager:
+    def __init__(self, manifest: ResultSchema, results_dir: str):
+        self.result_object = deserialize_result(manifest)
+        self._manifest = manifest.dict()
+        self._results_dir = results_dir
 
+    def save(self, path: Optional[str] = None):
+        if not path:
+            path = os.path.join(self._results_dir, "manifest.json")
+        with open(path, "w") as f:
+            f.write(ResultSchema.parse_obj(self._manifest).json())
 
-def _upload(assets: List[AssetSchema]) -> None:
-    """Upload assets to remote storage.
+    @staticmethod
+    def load(path: str, results_dir: str) -> "ResultManager":
+        with open(path, "r") as f:
+            manifest_json = f.read()
 
-    Args:
-        assets: List of AssetSchema objects to upload.
+        return ResultManager(ResultSchema.parse_raw(manifest_json), results_dir)
 
-    Raises:
-        RuntimeError: If any of the assets fail to upload.
+    def _populate_result_object(self):
+        dispatch_id = self._manifest["metadata"]["dispatch_id"]
 
-    """
-    total_assets = len(assets)
-    _upload_futures = []
+        # result assets
+        for key in RESULT_ASSET_TYPES:
+            remote_uri = _get_result_asset_uri(self._manifest, key)
+            fv = FutureVar(self, AssetScope.RESULT, key, dispatch_id, None)
+            self.result_object.__dict__[f"_{key}"] = fv
 
-    with Progress(
-        "[progress.description]{task.description}",
-        BarColumn(),
-        "[progress.percentage]{task.percentage:>4.1f}%",
-        MofNCompleteColumn(),
-        disable=(os.environ.get("COVALENT_CLOUD_DISABLE_RICH") == 1),
-    ) as progress:
-        task = progress.add_task("[green]Uploading assets...", total=total_assets)
-
-        for asset in assets:
-
-            if asset.size == 0:
-                progress.advance(task, advance=1)
-                progress.refresh()
-                total_assets -= 1
-                continue
-
-            # Unset attributes won't be saved to the staging dir during
-            # prepare_manifest.
-            if not asset.uri:
-                continue
-            fut = _dispatch_executor.submit(
-                _upload_asset, asset.uri, asset.remote_uri, task, progress
-            )
-            _upload_futures.append(fut)
+        # lattice assets
+        for key in LATTICE_ASSET_TYPES:
+            remote_uri = _get_lattice_asset_uri(self._manifest, key)
+            fv = FutureVar(self, AssetScope.LATTICE, key, dispatch_id, None)
+            if key in SDK_LAT_META_KEYS:
+                self.result_object.lattice.metadata[key] = fv
+            else:
+                self.result_object.lattice.__dict__[key] = fv
 
-        done, _ = wait(_upload_futures)
+        # transport graph node assets
+        tg = self.result_object.lattice.transport_graph
+        for node_id in tg._graph.nodes:
+            for key in ELECTRON_ASSET_TYPES:
+                remote_uri = _get_node_asset_uri(self._manifest, node_id, key)
+                fv = FutureVar(self, AssetScope.NODE, key, dispatch_id, node_id)
+                if key in SDK_NODE_META_KEYS:
+                    node_meta = tg.get_node_value(node_id, "metadata")
+                    node_meta[key] = fv
+                else:
+                    tg.set_node_value(node_id, key, fv)
 
-        if len(done) < total_assets:
-            raise AssetUploadThreadFailure
+    def download_result_asset(self, key: str):
+        _download_result_asset(self._manifest, self._results_dir, key)
 
-        _exceptions = []
-        for fut in done:
-            if ex := fut.exception(timeout=0.1):
-                _exceptions.append(ex)
+    def download_lattice_asset(self, key: str):
+        _download_lattice_asset(self._manifest, self._results_dir, key)
 
-        if _exceptions:
-            msg = f"Attempted and failed to upload {len(_exceptions)} out of {total_assets} due to raised exceptions."
-            print(msg, file=sys.stderr)
-            app_log.debug(_exceptions)
-            raise AssetUploadException(msg)
+    def download_node_asset(self, node_id: int, key: str):
+        _download_node_asset(self._manifest, self._results_dir, node_id, key)
+
+    def load_result_asset(self, key: str) -> Any:
+        return _load_result_asset(self._manifest, key)
+
+    def load_lattice_asset(self, key: str) -> Any:
+        return _load_lattice_asset(self._manifest, key)
+
+    def load_node_asset(self, node_id: int, key: str) -> Any:
+        return _load_node_asset(self._manifest, node_id, key)
+
+    @staticmethod
+    def from_dispatch_id(
+        dispatch_id: str,
+        results_dir: str,
+        wait: bool = False,
+        settings: Settings = settings,
+    ) -> "ResultManager":
+        export = _get_result_export_from_dispatcher(
+            dispatch_id,
+            wait,
+            status_only=False,
+            settings=settings,
+        )
 
+        manifest = ResultSchema.parse_obj(export["result_export"])
 
-def _upload_asset(local_uri: str, remote_uri: str, task: TaskID, progress: Progress) -> None:
-    """Upload a single asset to remote storage with automatic retries.
+        # sort the nodes
+        manifest.lattice.transport_graph.nodes.sort(key=lambda x: x.id)
 
-    Args:
-        local_uri: Local URI of the asset to upload.
-        remote_uri: Remote URI to upload the asset to.
-        task: Task ID of the progress bar task.
-        progress: Progress bar object.
+        rm = ResultManager(manifest, results_dir)
+        result_object = rm.result_object
+        result_object._results_dir = results_dir
+        Path(results_dir).mkdir(parents=True, exist_ok=True)
 
-    Raises:
-        requests.exceptions.HTTPError: If the upload fails.
+        # Create node subdirectories
+        for node_id in result_object.lattice.transport_graph._graph.nodes:
+            node_dir = results_dir + f"/node_{node_id}"
+            Path(node_dir).mkdir(exist_ok=True)
 
-    """
-    scheme_prefix = "file://"
-    if local_uri.startswith(scheme_prefix):
-        local_path = local_uri[len(scheme_prefix) :]
-    else:
-        local_path = local_uri
+        return rm
 
-    retry_strategy = Retry(
-        total=5,
-        backoff_factor=0.1,
-        allowed_methods={"PUT"},
-    )
-    session = requests.Session()
-    session.mount("https://", HTTPAdapter(max_retries=retry_strategy))
 
-    try:
-        if os.path.getsize(local_path) == 0:
-            r = session.put(remote_uri, headers={"Content-Length": "0"}, data="")
-        else:
-            with open(local_path, "rb") as f:
-                r = session.put(remote_uri, data=f)
-                r.raise_for_status()
-    except Exception:
-        raise
-
-    if r.status_code == requests.codes.ok:
-        progress.advance(task, advance=1)
-        progress.refresh()
+def get_result_manager(dispatch_id, results_dir=None, wait=False, settings=settings):
+    if not results_dir:
+        results_dir = settings.results_dir + f"/{dispatch_id}"
+    return ResultManager.from_dispatch_id(dispatch_id, results_dir, wait, settings)
 
 
-def fast_redispatch(
+def _get_result_multistage(
     dispatch_id: str,
-    input_args: list,
-    input_kwargs: dict,
+    wait: bool = False,
     settings: Settings = settings,
-) -> Callable:
+    status_only: bool = False,
+) -> Result:
     """
-    Redispatches a Covalent workflow to the Covalent Cloud and returns the assigned dispatch ID.
+    Get the results of a dispatch from a file.
 
     Args:
-        dispatch_id: The dispatch ID of the workflow to re-dispatch.
-        input_args: The positional arguments of the workflow.
-        input_kwargs: The keyword arguments of the workflow.
-        settings: The settings object to use. If None, the default settings will be used.
+        dispatch_id: The dispatch id of the result.
+        wait: Controls how long the method waits for the server to return a result. If False, the method will not wait and will return the current status of the workflow. If True, the method will wait for the result to finish and keep retrying for sys.maxsize.
 
     Returns:
-        The dispatch ID of the re-dispatched workflow.
+        The result from the file.
 
     """
 
-    dispatcher_addr = settings.dispatcher_uri
-    dispatcher_port = settings.dispatcher_port
+    try:
+        if status_only:
+            return _get_result_export_from_dispatcher(
+                dispatch_id=dispatch_id,
+                wait=wait,
+                status_only=status_only,
+                settings=settings,
+            )
+        else:
+            rm = get_result_manager(dispatch_id, None, wait, settings)
+            rm._populate_result_object()
 
-    client = APIClient(host_uri=dispatcher_addr, settings=settings, port=dispatcher_port)
-    endpoint = f"/api/v2/dispatch/{dispatch_id}/redispatch"
-    payload = {
-        "api_key": settings.auth.api_key,  # TODO: remove this from payload after cloud-server is updated
-        "dispatch_id": dispatch_id,
-        "input_args": input_args,
-        "input_kwargs": input_kwargs,
-    }
+    except MissingLatticeRecordError as ex:
+        app_log.warning(
+            f"Dispatch ID {dispatch_id} was not found in the database. Incorrect dispatch id."
+        )
 
-    try:
-        r = client.post(endpoint, request_options={"data": json.dumps(payload)})
-    except requests.exceptions.HTTPError as e:
-        print(e.response.text, file=sys.stderr)
-        raise e
-    return r.json()["dispatch_id"]
+        raise ex
 
+    return rm.result_object
 
-def track_redispatch(
+
+def get_result(
     dispatch_id: str,
-    original_dispatch_id: str,
+    wait: bool = False,
     settings: Settings = settings,
-) -> Callable:
+    status_only: bool = False,
+) -> Result:
 
-    dispatcher_addr = settings.dispatcher_uri
-    dispatcher_port = settings.dispatcher_port
+    if not dispatch_id:
+        return None
 
-    client = APIClient(host_uri=dispatcher_addr, settings=settings, port=dispatcher_port)
-    endpoint = f"/api/v2/lattices/{dispatch_id}"
+    res = _get_result_multistage(
+        dispatch_id=dispatch_id,
+        wait=wait,
+        settings=settings,
+        status_only=status_only,
+    )
+    if status_only:
+        return res
+    else:
+        result_object = res
 
-    payload = {
-        "original_dispatch_id": original_dispatch_id,
-    }
+    # Populate sublattice results
+    tg = result_object.lattice.transport_graph
+    for node_id in tg._graph.nodes:
+        sub_dispatch_id = tg.get_node_value(node_id, "sub_dispatch_id")
+        sub_result_object = get_result(sub_dispatch_id, wait, settings, status_only)
+        tg.set_node_value(node_id, "sublattice_result", sub_result_object)
 
-    try:
-        r = client.put(endpoint, request_options={"data": json.dumps(payload)})
-        r_json = r.json()
-        update_response = {
-            "dispatch_id": r_json["dispatch_id"],
-            "original_dispatch_id": r_json["original_dispatch_id"],
-        }
-    except requests.exceptions.HTTPError as e:
-        print(e.response.text, file=sys.stderr)
-        raise e
+    fr = FutureResult._from_result_object(result_object)
 
-    return update_response
+    return fr
```

### Comparing `covalent-cloud-0.64.0rc0/covalent_cloud.egg-info/PKG-INFO` & `covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: covalent-cloud
-Version: 0.64.0rc0
+Version: 0.8.0rc0
 Summary: Covalent Cloud SDK
 Home-page: https://github.com/AgnostiqHQ/covalent-cloud-sdk
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
-Download-URL: https://github.com/AgnostiqHQ/covalent-cloud-sdk/archive/v0.64.0.tar.gz
-Description: 
+Download-URL: https://github.com/AgnostiqHQ/covalent-cloud-sdk/archive/v0.8.0.tar.gz
+Description: &nbsp;
+        
+        <div align="center">
+        
+        [![covalent](https://img.shields.io/badge/covalent-0.208.0rc0-purple)](https://github.com/AgnostiqHQ/covalent)
+        [![agpl](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0.en.html)
+        
+        </div>
+        
         ## Covalent Cloud SDK
         
-        [Covalent](https://github.com/AgnostiqHQ/covalent) is a python based workflow orchestration tool used to execute HPC and quantum tasks in heterogeneous environments.
+        [Covalent](https://github.com/AgnostiqHQ/covalent) is a python based workflow orchestration tool used to execute HPC and quantum tasks in heterogenous environments.
         
         Installing Covalent Cloud SDK gives users access to the enterprise version of Covalent.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
```

### Comparing `covalent-cloud-0.64.0rc0/covalent_cloud.egg-info/SOURCES.txt` & `covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,66 +7,49 @@
 setup.py
 covalent_cloud/__init__.py
 covalent_cloud.egg-info/PKG-INFO
 covalent_cloud.egg-info/SOURCES.txt
 covalent_cloud.egg-info/dependency_links.txt
 covalent_cloud.egg-info/requires.txt
 covalent_cloud.egg-info/top_level.txt
+covalent_cloud/_serialize/__init__.py
+covalent_cloud/_serialize/common.py
+covalent_cloud/_serialize/electron.py
+covalent_cloud/_serialize/lattice.py
+covalent_cloud/_serialize/result.py
+covalent_cloud/_serialize/transport_graph.py
 covalent_cloud/analytics/__init__.py
 covalent_cloud/cloud_executor/__init__.py
 covalent_cloud/cloud_executor/cloud_executor.py
 covalent_cloud/cloud_executor/models/__init__.py
 covalent_cloud/cloud_executor/models/gpu.py
 covalent_cloud/cloud_executor/models/sw_environment.py
 covalent_cloud/dispatch_management/__init__.py
 covalent_cloud/dispatch_management/helpers.py
 covalent_cloud/dispatch_management/interface_functions.py
 covalent_cloud/dispatch_management/results_manager.py
-covalent_cloud/function_serve/__init__.py
-covalent_cloud/function_serve/assets.py
-covalent_cloud/function_serve/client.py
-covalent_cloud/function_serve/common.py
-covalent_cloud/function_serve/decorators.py
-covalent_cloud/function_serve/deployment.py
-covalent_cloud/function_serve/models.py
-covalent_cloud/function_serve/service_class.py
-covalent_cloud/qelectron_sdk/__init__.py
-covalent_cloud/qelectron_sdk/executors/__init__.py
-covalent_cloud/qelectron_sdk/executors/base.py
-covalent_cloud/qelectron_sdk/middleware/__init__.py
-covalent_cloud/qelectron_sdk/middleware/core.py
-covalent_cloud/qelectron_sdk/middleware/qclients/__init__.py
-covalent_cloud/qelectron_sdk/middleware/qclients/base_client.py
-covalent_cloud/qelectron_sdk/middleware/qclients/remote_qclient.py
-covalent_cloud/qelectron_sdk/schemas/__init__.py
-covalent_cloud/qelectron_sdk/schemas/schemas.py
 covalent_cloud/service_account_interface/__init__.py
 covalent_cloud/service_account_interface/auth_config_manager.py
 covalent_cloud/service_account_interface/client.py
 covalent_cloud/shared/__init__.py
 covalent_cloud/shared/classes/__init__.py
 covalent_cloud/shared/classes/api.py
-covalent_cloud/shared/classes/exceptions.py
-covalent_cloud/shared/classes/helpers.py
 covalent_cloud/shared/classes/settings.py
 covalent_cloud/shared/schemas/__init__.py
-covalent_cloud/shared/schemas/volume.py
+covalent_cloud/shared/schemas/asset.py
+covalent_cloud/shared/schemas/edge.py
+covalent_cloud/shared/schemas/electron.py
+covalent_cloud/shared/schemas/lattice.py
+covalent_cloud/shared/schemas/result.py
+covalent_cloud/shared/schemas/transport_graph.py
 covalent_cloud/software_environment/__init__.py
 covalent_cloud/swe_management/__init__.py
-covalent_cloud/swe_management/secrets_manager.py
 covalent_cloud/swe_management/swe_manager.py
-covalent_cloud/swe_management/models/__init__.py
-covalent_cloud/swe_management/models/environment.py
-covalent_cloud/volume/__init__.py
-covalent_cloud/volume/volume.py
 tests/dispatch_management_tests/__init__.py
 tests/dispatch_management_tests/future_classes_test.py
 tests/dispatch_management_tests/helpers_test.py
 tests/dispatch_management_tests/interface_functions_test.py
-tests/function_serve_tests/__init__.py
-tests/function_serve_tests/deployment_info_test.py
 tests/shared/__init__.py
 tests/shared/classes/APIClient_test.py
 tests/shared/classes/__init__.py
-tests/shared/classes/helpers_test.py
 tests/swe_management_tests/__init__.py
 tests/swe_management_tests/swe_manager_test.py
```

### Comparing `covalent-cloud-0.64.0rc0/pyproject.toml` & `covalent-cloud-0.8.0rc0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # you (or the person or organization that you represent) and Agnostiq Inc. Your rights to
 # access and use this file is subject to the terms and conditions of such agreement.
 # Please ensure you carefully review such agreements and, if you have any questions
 # please reach out to Agnostiq at: [support@agnostiq.com].
 
 
 # Copyright 2021-2022 Agnostiq Inc.
-# Note: This file is subject to a proprietary license agreement entered into between you
-# (or the person or organization that you represent) and Agnostiq Inc.
+# Note: This file is subject to a proprietary license agreement entered into between you 
+# (or the person or organization that you represent) and Agnostiq Inc. 
 # Your rights to access and use this file is subject to the terms and conditions of such agreement.
-# Please ensure you carefully review such agreements and, if you have any questions or concerns,
+# Please ensure you carefully review such agreements and, if you have any questions or concerns, 
 # please reach out to Agnostiq at: [support@agnostiq.com].
 
 
 [tool.black]
 target_version = ['py38']
 line-length = 99
 include = '\.pyi?$'
```

### Comparing `covalent-cloud-0.64.0rc0/setup.py` & `covalent-cloud-0.8.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.64.0rc0/tests/dispatch_management_tests/future_classes_test.py` & `covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/future_classes_test.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.64.0rc0/tests/dispatch_management_tests/helpers_test.py` & `covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/helpers_test.py`

 * *Files identical despite different names*

### Comparing `covalent-cloud-0.64.0rc0/tests/shared/classes/APIClient_test.py` & `covalent-cloud-0.8.0rc0/tests/shared/classes/APIClient_test.py`

 * *Files identical despite different names*

