# Comparing `tmp/celitech_sdk-1.1.54.tar.gz` & `tmp/celitech_sdk-1.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celitech_sdk-1.1.54.tar", last modified: Tue Apr 30 13:20:37 2024, max compression
+gzip compressed data, was "celitech_sdk-1.1.55.tar", last modified: Thu May  2 11:27:29 2024, max compression
```

## Comparing `celitech_sdk-1.1.54.tar` & `celitech_sdk-1.1.55.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.614398 celitech_sdk-1.1.54/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-04-30 13:20:37.614398 celitech_sdk-1.1.54/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 13:20:37.614398 celitech_sdk-1.1.54/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.602398 celitech_sdk-1.1.54/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.606397 celitech_sdk-1.1.54/src/celitech/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.606397 celitech_sdk-1.1.54/src/celitech/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.606397 celitech_sdk-1.1.54/src/celitech/models/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/create_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/create_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/edit_purchase_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/edit_purchase_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/get_esim_device_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/get_esim_history_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/get_esim_mac_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/get_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/get_purchase_consumption_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/list_destinations_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/list_packages_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/list_purchases_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/top_up_esim_ok_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/top_up_esim_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.610398 celitech_sdk-1.1.54/src/celitech/models/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/utils/cast_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/models/utils/json_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.610398 celitech_sdk-1.1.54/src/celitech/net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.610398 celitech_sdk-1.1.54/src/celitech/net/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/environment/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.610398 celitech_sdk-1.1.54/src/celitech/net/headers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/headers/base_header.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.610398 celitech_sdk-1.1.54/src/celitech/net/request_chain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/request_chain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.610398 celitech_sdk-1.1.54/src/celitech/net/request_chain/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/request_chain/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/request_chain/handlers/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/request_chain/handlers/hook_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/request_chain/handlers/http_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/request_chain/handlers/retry_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/request_chain/request_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.610398 celitech_sdk-1.1.54/src/celitech/net/transport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/transport/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/transport/request_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/transport/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/transport/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/net/transport/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.614398 celitech_sdk-1.1.54/src/celitech/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/services/destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/services/e_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/services/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/services/purchases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.614398 celitech_sdk-1.1.54/src/celitech/services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/services/utils/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/services/utils/default_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-30 13:20:25.000000 celitech_sdk-1.1.54/src/celitech/services/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 13:20:37.614398 celitech_sdk-1.1.54/src/celitech_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-04-30 13:20:37.000000 celitech_sdk-1.1.54/src/celitech_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-30 13:20:37.000000 celitech_sdk-1.1.54/src/celitech_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 13:20:37.000000 celitech_sdk-1.1.54/src/celitech_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 13:20:37.000000 celitech_sdk-1.1.54/src/celitech_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 13:20:37.000000 celitech_sdk-1.1.54/src/celitech_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.961631 celitech_sdk-1.1.55/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-05-02 11:27:29.961631 celitech_sdk-1.1.55/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 11:27:29.961631 celitech_sdk-1.1.55/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.945631 celitech_sdk-1.1.55/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.949631 celitech_sdk-1.1.55/src/celitech/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.949631 celitech_sdk-1.1.55/src/celitech/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.953631 celitech_sdk-1.1.55/src/celitech/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/create_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/create_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/edit_purchase_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/edit_purchase_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/get_esim_device_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/get_esim_history_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/get_esim_mac_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/get_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/get_purchase_consumption_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/list_destinations_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/list_packages_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/list_purchases_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/top_up_esim_ok_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/top_up_esim_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.953631 celitech_sdk-1.1.55/src/celitech/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/utils/cast_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/models/utils/json_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.953631 celitech_sdk-1.1.55/src/celitech/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.953631 celitech_sdk-1.1.55/src/celitech/net/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/environment/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.953631 celitech_sdk-1.1.55/src/celitech/net/headers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/headers/base_header.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.953631 celitech_sdk-1.1.55/src/celitech/net/request_chain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/request_chain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.957631 celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/hook_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/http_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/retry_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/request_chain/request_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.957631 celitech_sdk-1.1.55/src/celitech/net/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/transport/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/transport/request_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/transport/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/transport/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/net/transport/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.957631 celitech_sdk-1.1.55/src/celitech/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/e_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/purchases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.957631 celitech_sdk-1.1.55/src/celitech/services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/utils/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/utils/default_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-05-02 11:27:14.000000 celitech_sdk-1.1.55/src/celitech/services/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:27:29.957631 celitech_sdk-1.1.55/src/celitech_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-05-02 11:27:29.000000 celitech_sdk-1.1.55/src/celitech_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-02 11:27:29.000000 celitech_sdk-1.1.55/src/celitech_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 11:27:29.000000 celitech_sdk-1.1.55/src/celitech_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 11:27:29.000000 celitech_sdk-1.1.55/src/celitech_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 11:27:29.000000 celitech_sdk-1.1.55/src/celitech_sdk.egg-info/top_level.txt
```

### Comparing `celitech_sdk-1.1.54/LICENSE` & `celitech_sdk-1.1.55/LICENSE`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/PKG-INFO` & `celitech_sdk-1.1.55/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: celitech-sdk
-Version: 1.1.54
+Version: 1.1.55
 Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 
-# Celitech Python SDK 1.1.54
+# Celitech Python SDK 1.1.55
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.54
+- SDK version: 1.1.55
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -124,21 +124,15 @@
 ```py
 from celitech import Celitech, Environment
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.packages.list_packages(
-    destination="FRA",
-    start_date="2023-11-01",
-    end_date="2023-11-20",
-    after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
-    limit=20
-)
+result = sdk.packages.list_packages()
 
 print(result)
 ```
 
 ### PurchasesService
 
 A list of all methods in the `PurchasesService` service. Click on the method name to view detailed information about that method.
@@ -178,21 +172,15 @@
 ```py
 from celitech import Celitech, Environment
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.purchases.list_purchases(
-    iccid="1111222233334444555",
-    after_date="2023-11-01",
-    before_date="2023-11-20",
-    after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
-    limit=20
-)
+result = sdk.purchases.list_purchases()
 
 print(result)
 ```
 
 #### **create_purchase**
 
 This endpoint is used to purchase a new eSIM by providing the package details.
@@ -209,32 +197,20 @@
 
 `CreatePurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
-from celitech.models import CreatePurchaseRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreatePurchaseRequest(
-    destination="FRA",
-    data_limit_in_gb=1,
-    start_date="2023-11-01",
-    end_date="2023-11-20",
-    email="example@domain.com",
-    network_brand="CELITECH",
-    start_time=0.16,
-    end_time=0.96
-)
-
-result = sdk.purchases.create_purchase(request_body=request_body)
+result = sdk.purchases.create_purchase()
 
 print(result)
 ```
 
 #### **top_up_esim**
 
 This endpoint is used to top-up an eSIM with the previously associated destination by providing an existing ICCID and the package details. The top-up is not feasible for eSIMs in "DELETED" or "ERROR" state.
@@ -251,31 +227,20 @@
 
 `TopUpEsimOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
-from celitech.models import TopUpEsimRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TopUpEsimRequest(
-    iccid="1111222233334444555",
-    data_limit_in_gb=1,
-    start_date="2023-11-01",
-    end_date="2023-11-20",
-    email="example@domain.com",
-    start_time=2.14,
-    end_time=9.34
-)
-
-result = sdk.purchases.top_up_esim(request_body=request_body)
+result = sdk.purchases.top_up_esim()
 
 print(result)
 ```
 
 #### **edit_purchase**
 
 This endpoint allows you to modify the dates of an existing package with a future activation start time. Editing can only be performed for packages that have not been activated, and it cannot change the package size. The modification must not change the package duration category to ensure pricing consistency.
@@ -292,29 +257,20 @@
 
 `EditPurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
-from celitech.models import EditPurchaseRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-request_body = EditPurchaseRequest(
-    purchase_id="ae471106-c8b4-42cf-b83a-b061291f2922",
-    start_date="2023-11-01",
-    end_date="2023-11-20",
-    start_time=8.29,
-    end_time=0.24
-)
-
-result = sdk.purchases.edit_purchase(request_body=request_body)
+result = sdk.purchases.edit_purchase()
 
 print(result)
 ```
 
 #### **get_purchase_consumption**
 
 This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages.
```

### Comparing `celitech_sdk-1.1.54/README.md` & `celitech_sdk-1.1.55/src/celitech_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,23 @@
-# Celitech Python SDK 1.1.54
+Metadata-Version: 2.1
+Name: celitech-sdk
+Version: 1.1.55
+Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+
+# Celitech Python SDK 1.1.55
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.54
+- SDK version: 1.1.55
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -114,21 +124,15 @@
 ```py
 from celitech import Celitech, Environment
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.packages.list_packages(
-    destination="FRA",
-    start_date="2023-11-01",
-    end_date="2023-11-20",
-    after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
-    limit=20
-)
+result = sdk.packages.list_packages()
 
 print(result)
 ```
 
 ### PurchasesService
 
 A list of all methods in the `PurchasesService` service. Click on the method name to view detailed information about that method.
@@ -168,21 +172,15 @@
 ```py
 from celitech import Celitech, Environment
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.purchases.list_purchases(
-    iccid="1111222233334444555",
-    after_date="2023-11-01",
-    before_date="2023-11-20",
-    after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
-    limit=20
-)
+result = sdk.purchases.list_purchases()
 
 print(result)
 ```
 
 #### **create_purchase**
 
 This endpoint is used to purchase a new eSIM by providing the package details.
@@ -199,32 +197,20 @@
 
 `CreatePurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
-from celitech.models import CreatePurchaseRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreatePurchaseRequest(
-    destination="FRA",
-    data_limit_in_gb=1,
-    start_date="2023-11-01",
-    end_date="2023-11-20",
-    email="example@domain.com",
-    network_brand="CELITECH",
-    start_time=0.16,
-    end_time=0.96
-)
-
-result = sdk.purchases.create_purchase(request_body=request_body)
+result = sdk.purchases.create_purchase()
 
 print(result)
 ```
 
 #### **top_up_esim**
 
 This endpoint is used to top-up an eSIM with the previously associated destination by providing an existing ICCID and the package details. The top-up is not feasible for eSIMs in "DELETED" or "ERROR" state.
@@ -241,31 +227,20 @@
 
 `TopUpEsimOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
-from celitech.models import TopUpEsimRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TopUpEsimRequest(
-    iccid="1111222233334444555",
-    data_limit_in_gb=1,
-    start_date="2023-11-01",
-    end_date="2023-11-20",
-    email="example@domain.com",
-    start_time=2.14,
-    end_time=9.34
-)
-
-result = sdk.purchases.top_up_esim(request_body=request_body)
+result = sdk.purchases.top_up_esim()
 
 print(result)
 ```
 
 #### **edit_purchase**
 
 This endpoint allows you to modify the dates of an existing package with a future activation start time. Editing can only be performed for packages that have not been activated, and it cannot change the package size. The modification must not change the package duration category to ensure pricing consistency.
@@ -282,29 +257,20 @@
 
 `EditPurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
-from celitech.models import EditPurchaseRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-request_body = EditPurchaseRequest(
-    purchase_id="ae471106-c8b4-42cf-b83a-b061291f2922",
-    start_date="2023-11-01",
-    end_date="2023-11-20",
-    start_time=8.29,
-    end_time=0.24
-)
-
-result = sdk.purchases.edit_purchase(request_body=request_body)
+result = sdk.purchases.edit_purchase()
 
 print(result)
 ```
 
 #### **get_purchase_consumption**
 
 This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages.
```

### Comparing `celitech_sdk-1.1.54/src/celitech/hooks/hook.py` & `celitech_sdk-1.1.55/src/celitech/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/__init__.py` & `celitech_sdk-1.1.55/src/celitech/models/__init__.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/base.py` & `celitech_sdk-1.1.55/src/celitech/models/base.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/create_purchase_ok_response.py` & `celitech_sdk-1.1.55/src/celitech/models/create_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/create_purchase_request.py` & `celitech_sdk-1.1.55/src/celitech/models/create_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/edit_purchase_ok_response.py` & `celitech_sdk-1.1.55/src/celitech/models/edit_purchase_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/edit_purchase_request.py` & `celitech_sdk-1.1.55/src/celitech/models/edit_purchase_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/get_esim_device_ok_response.py` & `celitech_sdk-1.1.55/src/celitech/models/get_esim_device_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/get_esim_history_ok_response.py` & `celitech_sdk-1.1.55/src/celitech/models/get_esim_history_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/get_esim_mac_ok_response.py` & `celitech_sdk-1.1.55/src/celitech/models/get_esim_mac_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/get_esim_ok_response.py` & `celitech_sdk-1.1.55/src/celitech/models/get_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/get_purchase_consumption_ok_response.py` & `celitech_sdk-1.1.55/src/celitech/models/get_purchase_consumption_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/list_destinations_ok_response.py` & `celitech_sdk-1.1.55/src/celitech/models/list_destinations_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/list_packages_ok_response.py` & `celitech_sdk-1.1.55/src/celitech/models/list_packages_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/list_purchases_ok_response.py` & `celitech_sdk-1.1.55/src/celitech/models/list_purchases_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/top_up_esim_ok_response.py` & `celitech_sdk-1.1.55/src/celitech/models/top_up_esim_ok_response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/top_up_esim_request.py` & `celitech_sdk-1.1.55/src/celitech/models/top_up_esim_request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/utils/cast_models.py` & `celitech_sdk-1.1.55/src/celitech/models/utils/cast_models.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/models/utils/json_map.py` & `celitech_sdk-1.1.55/src/celitech/models/utils/json_map.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/net/request_chain/handlers/base_handler.py` & `celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/net/request_chain/handlers/hook_handler.py` & `celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/hook_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/net/request_chain/handlers/http_handler.py` & `celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/http_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/net/request_chain/handlers/retry_handler.py` & `celitech_sdk-1.1.55/src/celitech/net/request_chain/handlers/retry_handler.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/net/request_chain/request_chain.py` & `celitech_sdk-1.1.55/src/celitech/net/request_chain/request_chain.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/net/transport/request.py` & `celitech_sdk-1.1.55/src/celitech/net/transport/request.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/net/transport/request_error.py` & `celitech_sdk-1.1.55/src/celitech/net/transport/request_error.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/net/transport/response.py` & `celitech_sdk-1.1.55/src/celitech/net/transport/response.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/net/transport/serializer.py` & `celitech_sdk-1.1.55/src/celitech/net/transport/serializer.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/net/transport/utils.py` & `celitech_sdk-1.1.55/src/celitech/net/transport/utils.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/sdk.py` & `celitech_sdk-1.1.55/src/celitech/sdk.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/services/destinations.py` & `celitech_sdk-1.1.55/src/celitech/services/destinations.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/services/e_sim.py` & `celitech_sdk-1.1.55/src/celitech/services/e_sim.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/services/packages.py` & `celitech_sdk-1.1.55/src/celitech/services/packages.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/services/purchases.py` & `celitech_sdk-1.1.55/src/celitech/services/purchases.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/services/utils/base_service.py` & `celitech_sdk-1.1.55/src/celitech/services/utils/base_service.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/services/utils/default_headers.py` & `celitech_sdk-1.1.55/src/celitech/services/utils/default_headers.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech/services/utils/validator.py` & `celitech_sdk-1.1.55/src/celitech/services/utils/validator.py`

 * *Files identical despite different names*

### Comparing `celitech_sdk-1.1.54/src/celitech_sdk.egg-info/PKG-INFO` & `celitech_sdk-1.1.55/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,13 @@
-Metadata-Version: 2.1
-Name: celitech-sdk
-Version: 1.1.54
-Summary: Welcome to the CELITECH API documentation!  Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/) 
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-
-# Celitech Python SDK 1.1.54
+# Celitech Python SDK 1.1.55
 
 A Python SDK for Celitech.
 
 - API version: 1.1.0
-- SDK version: 1.1.54
+- SDK version: 1.1.55
 
 Welcome to the CELITECH API documentation! Useful links: [Homepage](https://www.celitech.com) | [Support email](mailto:support@celitech.com) | [Blog](https://www.celitech.com/blog/)
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Environment Variables](#environment-variables)
@@ -124,21 +114,15 @@
 ```py
 from celitech import Celitech, Environment
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.packages.list_packages(
-    destination="FRA",
-    start_date="2023-11-01",
-    end_date="2023-11-20",
-    after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
-    limit=20
-)
+result = sdk.packages.list_packages()
 
 print(result)
 ```
 
 ### PurchasesService
 
 A list of all methods in the `PurchasesService` service. Click on the method name to view detailed information about that method.
@@ -178,21 +162,15 @@
 ```py
 from celitech import Celitech, Environment
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-result = sdk.purchases.list_purchases(
-    iccid="1111222233334444555",
-    after_date="2023-11-01",
-    before_date="2023-11-20",
-    after_cursor="Y3JlYXRlZEF0OjE1OTk0OTMwOTgsZGVzdGluYXRpb246QVVTLG1pbkRheXM6MCxkYXRhTGltaXRJbkJ5dGVzOjUzNjg3MDkxMjA",
-    limit=20
-)
+result = sdk.purchases.list_purchases()
 
 print(result)
 ```
 
 #### **create_purchase**
 
 This endpoint is used to purchase a new eSIM by providing the package details.
@@ -209,32 +187,20 @@
 
 `CreatePurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
-from celitech.models import CreatePurchaseRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-request_body = CreatePurchaseRequest(
-    destination="FRA",
-    data_limit_in_gb=1,
-    start_date="2023-11-01",
-    end_date="2023-11-20",
-    email="example@domain.com",
-    network_brand="CELITECH",
-    start_time=0.16,
-    end_time=0.96
-)
-
-result = sdk.purchases.create_purchase(request_body=request_body)
+result = sdk.purchases.create_purchase()
 
 print(result)
 ```
 
 #### **top_up_esim**
 
 This endpoint is used to top-up an eSIM with the previously associated destination by providing an existing ICCID and the package details. The top-up is not feasible for eSIMs in "DELETED" or "ERROR" state.
@@ -251,31 +217,20 @@
 
 `TopUpEsimOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
-from celitech.models import TopUpEsimRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-request_body = TopUpEsimRequest(
-    iccid="1111222233334444555",
-    data_limit_in_gb=1,
-    start_date="2023-11-01",
-    end_date="2023-11-20",
-    email="example@domain.com",
-    start_time=2.14,
-    end_time=9.34
-)
-
-result = sdk.purchases.top_up_esim(request_body=request_body)
+result = sdk.purchases.top_up_esim()
 
 print(result)
 ```
 
 #### **edit_purchase**
 
 This endpoint allows you to modify the dates of an existing package with a future activation start time. Editing can only be performed for packages that have not been activated, and it cannot change the package size. The modification must not change the package duration category to ensure pricing consistency.
@@ -292,29 +247,20 @@
 
 `EditPurchaseOkResponse`
 
 **Example Usage Code Snippet**
 
 ```py
 from celitech import Celitech, Environment
-from celitech.models import EditPurchaseRequest
 
 sdk = Celitech(
     base_url=Environment.DEFAULT.value
 )
 
-request_body = EditPurchaseRequest(
-    purchase_id="ae471106-c8b4-42cf-b83a-b061291f2922",
-    start_date="2023-11-01",
-    end_date="2023-11-20",
-    start_time=8.29,
-    end_time=0.24
-)
-
-result = sdk.purchases.edit_purchase(request_body=request_body)
+result = sdk.purchases.edit_purchase()
 
 print(result)
 ```
 
 #### **get_purchase_consumption**
 
 This endpoint can be called for consumption notifications (e.g. every 1 hour or when the user clicks a button). It returns the data balance (consumption) of purchased packages.
```

### Comparing `celitech_sdk-1.1.54/src/celitech_sdk.egg-info/SOURCES.txt` & `celitech_sdk-1.1.55/src/celitech_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

