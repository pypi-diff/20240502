# Comparing `tmp/blissclient-0.2.0.tar.gz` & `tmp/blissclient-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blissclient-0.2.0.tar", last modified: Tue Jan 30 13:58:49 2024, max compression
+gzip compressed data, was "blissclient-0.2.1.tar", last modified: Thu May  2 14:25:43 2024, max compression
```

## Comparing `blissclient-0.2.0.tar` & `blissclient-0.2.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:58:49.467659 blissclient-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1768 2024-01-30 13:58:49.467659 blissclient-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1310 2024-01-19 13:28:14.000000 blissclient-0.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-01-19 13:28:14.000000 blissclient-0.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-01-30 13:58:49.471659 blissclient-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-01-19 13:28:14.000000 blissclient-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:58:49.463659 blissclient-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:58:49.463659 blissclient-0.2.0/src/blissclient/
--rw-rw-rw-   0 root         (0) root         (0)      255 2024-01-30 13:58:22.000000 blissclient-0.2.0/src/blissclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-01-29 15:44:50.000000 blissclient-0.2.0/src/blissclient/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2589 2024-01-30 13:58:22.000000 blissclient-0.2.0/src/blissclient/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:58:49.463659 blissclient-0.2.0/src/blissclient/high_level/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/high_level/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/high_level/base.py
--rw-rw-rw-   0 root         (0) root         (0)      280 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/high_level/config.py
--rw-rw-rw-   0 root         (0) root         (0)     6512 2024-01-30 13:35:16.000000 blissclient-0.2.0/src/blissclient/high_level/hardware.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2024-01-30 06:51:31.000000 blissclient-0.2.0/src/blissclient/high_level/scan.py
--rw-rw-rw-   0 root         (0) root         (0)     5565 2024-01-30 13:18:37.000000 blissclient-0.2.0/src/blissclient/high_level/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:58:49.463659 blissclient-0.2.0/src/blissclient/openapi/
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      865 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/api_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:58:49.467659 blissclient-0.2.0/src/blissclient/openapi/models/
--rw-rw-rw-   0 root         (0) root         (0)      331 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/ActiveMG.py
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/CallFunction.py
--rw-rw-rw-   0 root         (0) root         (0)      374 2024-01-22 10:31:59.000000 blissclient-0.2.0/src/blissclient/openapi/models/CallFunctionAsyncState.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2024-01-22 10:21:50.000000 blissclient-0.2.0/src/blissclient/openapi/models/CallFunctionResponse.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-01-22 10:21:50.000000 blissclient-0.2.0/src/blissclient/openapi/models/CallObjectFunction.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2024-01-22 10:21:50.000000 blissclient-0.2.0/src/blissclient/openapi/models/CallObjectFunctionResponse.py
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/CallScanSavingBody.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/ErrorResponse.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/HardwareObjectSchema.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/LayoutItem.py
--rw-rw-rw-   0 root         (0) root         (0)      377 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/LayoutRoot.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/MessageResponse.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/MonitorConfigSchema.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2024-01-22 08:51:22.000000 blissclient-0.2.0/src/blissclient/openapi/models/Paginated_HardwareObjectSchema_.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/PublicConfigSchema.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/RegisterHardwareSchema.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2024-01-22 10:21:50.000000 blissclient-0.2.0/src/blissclient/openapi/models/ScanSaving.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/SetObjectProperty.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/TerminalSizeBody.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/UpdateActiveMGBody.py
--rw-rw-rw-   0 root         (0) root         (0)      643 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/UpdateScanSavingBody.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/ValidationErrorModel.py
--rw-rw-rw-   0 root         (0) root         (0)      735 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:58:49.467659 blissclient-0.2.0/src/blissclient/openapi/services/
--rw-rw-rw-   0 root         (0) root         (0)     1330 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/services/Config_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/services/Console_service.py
--rw-rw-rw-   0 root         (0) root         (0)     6599 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/services/Hardware_service.py
--rw-rw-rw-   0 root         (0) root         (0)    10349 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/services/Session_service.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1367 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/services/async_Config_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1441 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/services/async_Console_service.py
--rw-rw-rw-   0 root         (0) root         (0)     6784 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/services/async_Hardware_service.py
--rw-rw-rw-   0 root         (0) root         (0)    10627 2024-01-19 13:28:14.000000 blissclient-0.2.0/src/blissclient/openapi/services/async_Session_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:58:49.463659 blissclient-0.2.0/src/blissclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1768 2024-01-30 13:58:49.000000 blissclient-0.2.0/src/blissclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2379 2024-01-30 13:58:49.000000 blissclient-0.2.0/src/blissclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 13:58:49.000000 blissclient-0.2.0/src/blissclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2024-01-30 13:58:49.000000 blissclient-0.2.0/src/blissclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-01-30 13:58:49.000000 blissclient-0.2.0/src/blissclient.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 13:58:49.467659 blissclient-0.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-01-22 10:39:11.000000 blissclient-0.2.0/tests/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)      817 2024-01-22 10:31:59.000000 blissclient-0.2.0/tests/test_client_hardware.py
--rw-rw-rw-   0 root         (0) root         (0)     1650 2024-01-19 13:28:14.000000 blissclient-0.2.0/tests/test_client_session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:25:43.303583 blissclient-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-05-02 14:25:43.303583 blissclient-0.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2024-05-02 14:23:37.000000 blissclient-0.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-02 14:23:37.000000 blissclient-0.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-05-02 14:25:43.303583 blissclient-0.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-05-02 14:23:37.000000 blissclient-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:25:43.299583 blissclient-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:25:43.299583 blissclient-0.2.1/src/blissclient/
+-rw-rw-rw-   0 root         (0) root         (0)      255 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2589 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:25:43.299583 blissclient-0.2.1/src/blissclient/high_level/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 14:25:41.000000 blissclient-0.2.1/src/blissclient/high_level/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/high_level/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      280 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/high_level/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6512 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/high_level/hardware.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/high_level/scan.py
+-rw-rw-rw-   0 root         (0) root         (0)     5630 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/high_level/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:25:43.299583 blissclient-0.2.1/src/blissclient/openapi/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      865 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/api_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:25:43.303583 blissclient-0.2.1/src/blissclient/openapi/models/
+-rw-rw-rw-   0 root         (0) root         (0)      331 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/ActiveMG.py
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/CallFunction.py
+-rw-rw-rw-   0 root         (0) root         (0)      374 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/CallFunctionAsyncState.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/CallFunctionResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/CallObjectFunction.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/CallObjectFunctionResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/CallScanSavingBody.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/ErrorResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/HardwareObjectSchema.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/LayoutItem.py
+-rw-rw-rw-   0 root         (0) root         (0)      377 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/LayoutRoot.py
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/MessageResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/MonitorConfigSchema.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/Paginated_HardwareObjectSchema_.py
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/PublicConfigSchema.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/RegisterHardwareSchema.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/ScanSaving.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/SetObjectProperty.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/TerminalSizeBody.py
+-rw-rw-rw-   0 root         (0) root         (0)      319 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/UpdateActiveMGBody.py
+-rw-rw-rw-   0 root         (0) root         (0)      643 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/UpdateScanSavingBody.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/ValidationErrorModel.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:25:43.303583 blissclient-0.2.1/src/blissclient/openapi/services/
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/services/Config_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/services/Console_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     6599 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/services/Hardware_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    10349 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/services/Session_service.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-02 14:25:41.000000 blissclient-0.2.1/src/blissclient/openapi/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/services/async_Config_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/services/async_Console_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     6784 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/services/async_Hardware_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    10627 2024-05-02 14:23:37.000000 blissclient-0.2.1/src/blissclient/openapi/services/async_Session_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:25:43.299583 blissclient-0.2.1/src/blissclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-05-02 14:25:43.000000 blissclient-0.2.1/src/blissclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2379 2024-05-02 14:25:43.000000 blissclient-0.2.1/src/blissclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 14:25:43.000000 blissclient-0.2.1/src/blissclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2024-05-02 14:25:43.000000 blissclient-0.2.1/src/blissclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-02 14:25:43.000000 blissclient-0.2.1/src/blissclient.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 14:25:43.303583 blissclient-0.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-02 14:23:37.000000 blissclient-0.2.1/tests/test_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      817 2024-05-02 14:23:37.000000 blissclient-0.2.1/tests/test_client_hardware.py
+-rw-rw-rw-   0 root         (0) root         (0)     1650 2024-05-02 14:23:37.000000 blissclient-0.2.1/tests/test_client_session.py
```

### Comparing `blissclient-0.2.0/PKG-INFO` & `blissclient-0.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: blissclient
-Version: 0.2.0
-Summary: Client for Bliss API
-Home-page: https://gitlab.esrf.fr/bliss/bliss-client
-Author: BCU (ESRF)
-License: MIT
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-
 # blissclient
 
 A python client for `blissterm`, the high-level client is fully typed ready for auto-completion in any modern IDE.
 
 
 ## Getting Started
```

### Comparing `blissclient-0.2.0/README.md` & `blissclient-0.2.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: blissclient
+Version: 0.2.1
+Summary: Client for Bliss API
+Home-page: https://gitlab.esrf.fr/bliss/bliss-client
+Author: BCU (ESRF)
+License: MIT
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: httpx
+Requires-Dist: pydantic>=2
+Requires-Dist: python-socketio[client]>=5.11
+Provides-Extra: test
+Requires-Dist: pytest>=7; extra == "test"
+Provides-Extra: dev
+Requires-Dist: pytest>=7; extra == "dev"
+Requires-Dist: black>=22; extra == "dev"
+Requires-Dist: flake8>=4; extra == "dev"
+
 # blissclient
 
 A python client for `blissterm`, the high-level client is fully typed ready for auto-completion in any modern IDE.
 
 
 ## Getting Started
```

### Comparing `blissclient-0.2.0/setup.cfg` & `blissclient-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/client.py` & `blissclient-0.2.1/src/blissclient/client.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/exceptions.py` & `blissclient-0.2.1/src/blissclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/high_level/hardware.py` & `blissclient-0.2.1/src/blissclient/high_level/hardware.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/high_level/scan.py` & `blissclient-0.2.1/src/blissclient/high_level/scan.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/high_level/session.py` & `blissclient-0.2.1/src/blissclient/high_level/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,16 +147,18 @@
         )
         return ScanSavingRepr(**scan_saving.dict())
 
     def update_scan_saving(self, **kwargs):
         """Update a `SCAN_SAVING property"""
         return ScanSavingResource_patch__session_name__scan_saving_patch(
             self._session_name,
-            data=UpdateScanSavingBody(kwargs),
+            data=UpdateScanSavingBody(**kwargs),
             api_config_override=self._api_config,
         )
 
     def call_scan_saving(self, function: str):
         """Call a `SCAN_SAVING` function"""
         return ScanSavingResource_post__session_name__scan_saving_post(
-            self._session_name, data=CallScanSavingBody(function=function)
+            self._session_name,
+            data=CallScanSavingBody(function=function),
+            api_config_override=self._api_config,
         )
```

### Comparing `blissclient-0.2.0/src/blissclient/openapi/api_config.py` & `blissclient-0.2.1/src/blissclient/openapi/api_config.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/openapi/models/CallFunction.py` & `blissclient-0.2.1/src/blissclient/openapi/models/CallFunction.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/openapi/models/HardwareObjectSchema.py` & `blissclient-0.2.1/src/blissclient/openapi/models/HardwareObjectSchema.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/openapi/models/PublicConfigSchema.py` & `blissclient-0.2.1/src/blissclient/openapi/models/PublicConfigSchema.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/openapi/models/ScanSaving.py` & `blissclient-0.2.1/src/blissclient/openapi/models/ScanSaving.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/openapi/models/UpdateScanSavingBody.py` & `blissclient-0.2.1/src/blissclient/openapi/models/UpdateScanSavingBody.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/openapi/models/__init__.py` & `blissclient-0.2.1/src/blissclient/openapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/openapi/services/Config_service.py` & `blissclient-0.2.1/src/blissclient/openapi/services/Config_service.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/openapi/services/Console_service.py` & `blissclient-0.2.1/src/blissclient/openapi/services/Console_service.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/openapi/services/Hardware_service.py` & `blissclient-0.2.1/src/blissclient/openapi/services/Hardware_service.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/openapi/services/Session_service.py` & `blissclient-0.2.1/src/blissclient/openapi/services/Session_service.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/openapi/services/async_Config_service.py` & `blissclient-0.2.1/src/blissclient/openapi/services/async_Config_service.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/openapi/services/async_Console_service.py` & `blissclient-0.2.1/src/blissclient/openapi/services/async_Console_service.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/openapi/services/async_Hardware_service.py` & `blissclient-0.2.1/src/blissclient/openapi/services/async_Hardware_service.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient/openapi/services/async_Session_service.py` & `blissclient-0.2.1/src/blissclient/openapi/services/async_Session_service.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/src/blissclient.egg-info/PKG-INFO` & `blissclient-0.2.1/src/blissclient.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 Metadata-Version: 2.1
 Name: blissclient
-Version: 0.2.0
+Version: 0.2.1
 Summary: Client for Bliss API
 Home-page: https://gitlab.esrf.fr/bliss/bliss-client
 Author: BCU (ESRF)
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: httpx
+Requires-Dist: pydantic>=2
+Requires-Dist: python-socketio[client]>=5.11
 Provides-Extra: test
+Requires-Dist: pytest>=7; extra == "test"
 Provides-Extra: dev
+Requires-Dist: pytest>=7; extra == "dev"
+Requires-Dist: black>=22; extra == "dev"
+Requires-Dist: flake8>=4; extra == "dev"
 
 # blissclient
 
 A python client for `blissterm`, the high-level client is fully typed ready for auto-completion in any modern IDE.
 
 
 ## Getting Started
```

### Comparing `blissclient-0.2.0/src/blissclient.egg-info/SOURCES.txt` & `blissclient-0.2.1/src/blissclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/tests/test_client_hardware.py` & `blissclient-0.2.1/tests/test_client_hardware.py`

 * *Files identical despite different names*

### Comparing `blissclient-0.2.0/tests/test_client_session.py` & `blissclient-0.2.1/tests/test_client_session.py`

 * *Files identical despite different names*

