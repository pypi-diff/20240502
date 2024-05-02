# Comparing `tmp/b_lambda_layer_common-4.4.0.tar.gz` & `tmp/b_lambda_layer_common-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b_lambda_layer_common-4.4.0.tar", last modified: Thu Dec 22 08:17:01 2022, max compression
+gzip compressed data, was "b_lambda_layer_common-4.5.0.tar", last modified: Thu May  2 12:44:32 2024, max compression
```

## Comparing `b_lambda_layer_common-4.4.0.tar` & `b_lambda_layer_common-4.5.0.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.969753 b_lambda_layer_common-4.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12902 2022-12-22 08:17:01.969753 b_lambda_layer_common-4.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.953753 b_lambda_layer_common-4.4.0/b_lambda_layer_common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.953753 b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/cognito_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/exception_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/neighbour_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/remove_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/response_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.953753 b_lambda_layer_common-4.4.0/b_lambda_layer_common/cache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/cache/in_memory_data_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.953753 b_lambda_layer_common-4.4.0/b_lambda_layer_common/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/events/event_bridge_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.957753 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/b_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.957753 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/already_exists_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/bad_request_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/conflict_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/database_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/dependency_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/failed_rollback_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/forbidden_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/internal_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/malformed_permission_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/malformed_value_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/misconfigured_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/not_found_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/not_reached_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/unauthorized_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/exception_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/http_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.957753 b_lambda_layer_common-4.4.0/b_lambda_layer_common/ssm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/ssm/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/ssm/refreshable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/ssm/ssm_parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.961753 b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/decimal_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/do_not_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/field_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/http_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/http_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/list_bytes_batcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/os_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/sfn_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/skip_invocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/xml_to_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.961753 b_lambda_layer_common-4.4.0/b_lambda_layer_common/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/validation/legacy_field_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/validation/value_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/validation/value_validator_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.961753 b_lambda_layer_common-4.4.0/b_lambda_layer_common/ws_api_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/ws_api_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common/ws_api_gateway/ws_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.953753 b_lambda_layer_common-4.4.0/b_lambda_layer_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12902 2022-12-22 08:17:01.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2022-12-22 08:17:01.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-22 08:17:01.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2022-12-22 08:17:01.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.949753 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.961753 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.965753 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_cognito_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_exception_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_neighbour_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_remove_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_response_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.965753 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/cache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/cache/test_in_memory_data_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.965753 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/events/test_event_bridge_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.965753 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/exceptions/test_b_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/exceptions/test_exception_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/exceptions/test_http_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.965753 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/ssm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/ssm/dummy_ssm_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/ssm/test_refreshable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/ssm/test_ssm_parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.969753 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_decimal_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_do_not_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_field_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_http_call.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_http_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_list_bytes_batcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_os_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_skip_invocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_xml_to_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.969753 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/validation/test_legacy_field_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/validation/test_value_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/validation/test_value_validator_presets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-22 08:17:01.969753 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/ws_api_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/ws_api_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/ws_api_gateway/test_ws_message.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-22 08:17:01.969753 b_lambda_layer_common-4.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2022-12-22 08:16:02.000000 b_lambda_layer_common-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.447920 b_lambda_layer_common-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13080 2024-05-02 12:44:32.447920 b_lambda_layer_common-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.435920 b_lambda_layer_common-4.5.0/b_lambda_layer_common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.435920 b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/cognito_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/exception_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/neighbour_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/remove_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/response_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.435920 b_lambda_layer_common-4.5.0/b_lambda_layer_common/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/cache/in_memory_data_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.435920 b_lambda_layer_common-4.5.0/b_lambda_layer_common/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/events/event_bridge_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.439920 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/b_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.439920 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/already_exists_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/bad_request_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/conflict_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/database_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/dependency_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/failed_rollback_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/forbidden_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/internal_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/malformed_permission_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/malformed_value_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/misconfigured_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/not_found_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/not_reached_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/unauthorized_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/exception_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/http_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.439920 b_lambda_layer_common-4.5.0/b_lambda_layer_common/ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/ssm/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/ssm/refreshable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/ssm/ssm_parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.443920 b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/decimal_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/do_not_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/field_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/http_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/http_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/list_bytes_batcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/os_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/sfn_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/skip_invocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/xml_to_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.443920 b_lambda_layer_common-4.5.0/b_lambda_layer_common/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/validation/legacy_field_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/validation/value_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/validation/value_validator_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.443920 b_lambda_layer_common-4.5.0/b_lambda_layer_common/ws_api_gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/ws_api_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common/ws_api_gateway/ws_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.435920 b_lambda_layer_common-4.5.0/b_lambda_layer_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13080 2024-05-02 12:44:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-05-02 12:44:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:44:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-02 12:44:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.431920 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.443920 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.443920 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_cognito_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_exception_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_neighbour_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_remove_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_response_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.443920 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/cache/test_in_memory_data_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.443920 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/events/test_event_bridge_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.443920 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/exceptions/test_b_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/exceptions/test_exception_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/exceptions/test_http_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.443920 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/ssm/dummy_ssm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/ssm/test_refreshable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/ssm/test_ssm_parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.447920 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_decimal_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_do_not_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_field_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_http_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_http_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_list_bytes_batcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_os_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_skip_invocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_xml_to_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.447920 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/validation/test_legacy_field_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13232 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/validation/test_value_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/validation/test_value_validator_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:44:32.447920 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/ws_api_gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/ws_api_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/ws_api_gateway/test_ws_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 12:44:32.447920 b_lambda_layer_common-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-02 12:43:32.000000 b_lambda_layer_common-4.5.0/setup.py
```

### Comparing `b_lambda_layer_common-4.4.0/HISTORY.md` & `b_lambda_layer_common-4.5.0/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Release history
 
+### 4.5.0
+* Update of the `CognitoAccessToken` class to parse authentication token either from the request headers or 
+from the request context.
+
 ### 4.4.0
 * Add decorator `remove_header` removing desired headers from API Gateway integration lambda event.
 
 ### 4.3.0
 * Improve `ValueValidator` by adding `not_contains_whitespace` method.
 * Make `ValueValidatorPresets` more flexible.
```

### Comparing `b_lambda_layer_common-4.4.0/LICENSE` & `b_lambda_layer_common-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/PKG-INFO` & `b_lambda_layer_common-4.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b_lambda_layer_common
-Version: 4.4.0
+Version: 4.5.0
 Summary: Common opinionated utilities for every day development.
 Home-page: https://github.com/biomapas/B.LambdaLayerCommon.git
 License: Apache License 2.0
 Description: # B.LambdaLayerCommon
         
         ![Pipeline](https://github.com/Biomapas/B.LambdaLayerCommon/workflows/Pipeline/badge.svg?branch=master)
         
@@ -112,14 +112,18 @@
         Contributions of any kind are gladly welcome. 
         You may contact us directly, create a pull-request or an issue in github platform. 
         Lets modernize the world together.
         
         
         # Release history
         
+        ### 4.5.0
+        * Update of the `CognitoAccessToken` class to parse authentication token either from the request headers or 
+        from the request context.
+        
         ### 4.4.0
         * Add decorator `remove_header` removing desired headers from API Gateway integration lambda event.
         
         ### 4.3.0
         * Improve `ValueValidator` by adding `not_contains_whitespace` method.
         * Make `ValueValidatorPresets` more flexible.
```

### Comparing `b_lambda_layer_common-4.4.0/README.md` & `b_lambda_layer_common-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/api_key.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/api_key.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/body.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/body.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/cognito_access_token.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/cognito_access_token.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,19 +11,22 @@
     def __init__(self, event: Dict[str, Any]) -> None:
         """
         Constructor.
 
         :param event: Lambda event.
         """
         try:
-            self.__auth_token = event['headers']['authorization']
+            request_context = event.get('requestContext', {})
+
+            # The authentication token can be located either in the request headers or in the context.
+            self.__auth_token = event.get('headers', {}).get('authorization') or request_context['authorizer']['auth_token']
 
             # If JWT claims are not located in event.requestContext.authorizer.claims
             # they could be found in event.requestContext.authorizer instead.
-            self.__claims = event['requestContext']['authorizer']['claims'] or event['requestContext']['authorizer']
+            self.__claims = request_context.get('authorizer', {}).get('claims') or request_context['authorizer']
 
             assert self.token_use == 'access'
         except (KeyError, AssertionError) as ex:
             raise UnauthorizedError('Missing access token.')
 
     @property
     def auth_token(self):
```

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/exception_middleware.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/exception_middleware.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/neighbour_endpoint.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/neighbour_endpoint.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/remove_header.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/remove_header.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/response.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/response.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/response_headers.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/response_headers.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/api_gateway/url.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/api_gateway/url.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/cache/in_memory_data_cache.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/cache/in_memory_data_cache.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/events/event_bridge_factory.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/events/event_bridge_factory.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/b_exception.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/b_exception.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/already_exists_error.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/already_exists_error.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/bad_request_error.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/bad_request_error.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/conflict_error.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/conflict_error.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/database_error.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/database_error.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/dependency_error.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/dependency_error.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/failed_rollback_error.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/failed_rollback_error.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/forbidden_error.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/forbidden_error.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/internal_error.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/internal_error.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/malformed_permission_error.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/malformed_permission_error.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/malformed_value_error.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/malformed_value_error.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/misconfigured_error.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/misconfigured_error.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/not_found_error.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/not_found_error.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/not_reached_error.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/not_reached_error.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/container/unauthorized_error.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/container/unauthorized_error.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/exception_mapper.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/exception_mapper.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/exceptions/http_exception.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/exceptions/http_exception.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/ssm/fetcher.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/ssm/fetcher.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/ssm/refreshable.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/ssm/refreshable.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/ssm/ssm_parameter.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/ssm/ssm_parameter.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/do_not_update.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/do_not_update.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/http_call.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/http_call.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/http_endpoint.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/http_endpoint.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/list_bytes_batcher.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/list_bytes_batcher.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/logging.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/logging.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/sfn_call.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/sfn_call.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/skip_invocation.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/skip_invocation.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/util/xml_to_dict.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/util/xml_to_dict.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/validation/legacy_field_validator.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/validation/legacy_field_validator.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/validation/value_validator.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/validation/value_validator.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/validation/value_validator_presets.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/validation/value_validator_presets.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common/ws_api_gateway/ws_message.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common/ws_api_gateway/ws_message.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common.egg-info/PKG-INFO` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b-lambda-layer-common
-Version: 4.4.0
+Version: 4.5.0
 Summary: Common opinionated utilities for every day development.
 Home-page: https://github.com/biomapas/B.LambdaLayerCommon.git
 License: Apache License 2.0
 Description: # B.LambdaLayerCommon
         
         ![Pipeline](https://github.com/Biomapas/B.LambdaLayerCommon/workflows/Pipeline/badge.svg?branch=master)
         
@@ -112,14 +112,18 @@
         Contributions of any kind are gladly welcome. 
         You may contact us directly, create a pull-request or an issue in github platform. 
         Lets modernize the world together.
         
         
         # Release history
         
+        ### 4.5.0
+        * Update of the `CognitoAccessToken` class to parse authentication token either from the request headers or 
+        from the request context.
+        
         ### 4.4.0
         * Add decorator `remove_header` removing desired headers from API Gateway integration lambda event.
         
         ### 4.3.0
         * Improve `ValueValidator` by adding `not_contains_whitespace` method.
         * Make `ValueValidatorPresets` more flexible.
```

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common.egg-info/SOURCES.txt` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_api_key.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_api_key.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_body.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_body.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_exception_middleware.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_exception_middleware.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_neighbour_endpoint.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_neighbour_endpoint.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_remove_header.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_remove_header.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_response.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_response.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/api_gateway/test_response_headers.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/api_gateway/test_response_headers.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/exceptions/test_b_exception.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/exceptions/test_b_exception.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/exceptions/test_exception_mapper.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/exceptions/test_exception_mapper.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/exceptions/test_http_exception.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/exceptions/test_http_exception.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/ssm/dummy_ssm_client.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/ssm/dummy_ssm_client.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/ssm/test_refreshable.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/ssm/test_refreshable.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/ssm/test_ssm_parameter.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/ssm/test_ssm_parameter.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_http_call.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_http_call.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_http_endpoint.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_http_endpoint.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_list_bytes_batcher.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_list_bytes_batcher.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_skip_invocation.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_skip_invocation.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/util/test_xml_to_dict.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/util/test_xml_to_dict.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/validation/test_legacy_field_validator.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/validation/test_legacy_field_validator.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/validation/test_value_validator.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/validation/test_value_validator.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/validation/test_value_validator_presets.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/validation/test_value_validator_presets.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/b_lambda_layer_common_test/unit/ws_api_gateway/test_ws_message.py` & `b_lambda_layer_common-4.5.0/b_lambda_layer_common_test/unit/ws_api_gateway/test_ws_message.py`

 * *Files identical despite different names*

### Comparing `b_lambda_layer_common-4.4.0/setup.py` & `b_lambda_layer_common-4.5.0/setup.py`

 * *Files identical despite different names*

