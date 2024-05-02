# Comparing `tmp/e2b-0.9.6.tar.gz` & `tmp/e2b-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2b-0.9.6.tar", max compression
+gzip compressed data, was "e2b-0.9.7.tar", max compression
```

## Comparing `e2b-0.9.6.tar` & `e2b-0.9.7.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1493 2023-10-20 23:32:22.667117 e2b-0.9.6/README.md
--rw-r--r--   0        0        0      468 2023-10-20 23:32:22.667117 e2b-0.9.6/e2b/__init__.py
--rw-r--r--   0        0        0     1040 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/.openapi-generator-ignore
--rw-r--r--   0        0        0      711 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/__init__.py
--rw-r--r--   0        0        0        0 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/__init__.py
--rw-r--r--   0        0        0     1792 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/__init__.py
--rw-r--r--   0        0        0      214 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/api/__init__.py
--rw-r--r--   0        0        0     6231 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/api/default_api.py
--rw-r--r--   0        0        0    48260 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/api/envs_api.py
--rw-r--r--   0        0        0    26370 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/api/sessions_api.py
--rw-r--r--   0        0        0    28932 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/api_client.py
--rw-r--r--   0        0        0      805 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/api_response.py
--rw-r--r--   0        0        0    16716 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/configuration.py
--rw-r--r--   0        0        0     5000 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/exceptions.py
--rw-r--r--   0        0        0     1054 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/models/__init__.py
--rw-r--r--   0        0        0     2232 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/models/environment.py
--rw-r--r--   0        0        0      688 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/models/environment_state.py
--rw-r--r--   0        0        0     2138 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/models/environment_state_update.py
--rw-r--r--   0        0        0     2095 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/models/environment_title_update.py
--rw-r--r--   0        0        0     2340 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/models/envs_get200_response_inner.py
--rw-r--r--   0        0        0     2049 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/models/error.py
--rw-r--r--   0        0        0     2134 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/models/new_environment.py
--rw-r--r--   0        0        0     2574 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/models/new_session.py
--rw-r--r--   0        0        0     2769 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/models/session.py
--rw-r--r--   0        0        0     2949 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/models/sessions_get200_response_inner.py
--rw-r--r--   0        0        0      752 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/models/template.py
--rw-r--r--   0        0        0    13020 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client/rest.py
--rw-r--r--   0        0        0     4245 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v1/client_README.md
--rw-r--r--   0        0        0        0 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/__init__.py
--rw-r--r--   0        0        0     1599 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/__init__.py
--rw-r--r--   0        0        0      214 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/api/__init__.py
--rw-r--r--   0        0        0     6176 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/api/default_api.py
--rw-r--r--   0        0        0    47755 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/api/envs_api.py
--rw-r--r--   0        0        0    25966 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/api/sessions_api.py
--rw-r--r--   0        0        0    29311 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/api_client.py
--rw-r--r--   0        0        0      827 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/api_response.py
--rw-r--r--   0        0        0    16671 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/configuration.py
--rw-r--r--   0        0        0     5280 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/exceptions.py
--rw-r--r--   0        0        0      861 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/models/__init__.py
--rw-r--r--   0        0        0     2212 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/models/environment.py
--rw-r--r--   0        0        0      688 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/models/environment_state.py
--rw-r--r--   0        0        0     2118 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/models/environment_state_update.py
--rw-r--r--   0        0        0     2075 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/models/environment_title_update.py
--rw-r--r--   0        0        0     2051 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/models/error.py
--rw-r--r--   0        0        0     2114 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/models/new_environment.py
--rw-r--r--   0        0        0     2554 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/models/new_session.py
--rw-r--r--   0        0        0     2749 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/models/session.py
--rw-r--r--   0        0        0      752 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/models/template.py
--rw-r--r--   0        0        0    13141 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client/rest.py
--rw-r--r--   0        0        0     4070 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/api/v2/client_README.md
--rw-r--r--   0        0        0      178 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/constants.py
--rw-r--r--   0        0        0      594 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/session/__init__.py
--rw-r--r--   0        0        0     1720 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/session/code_snippet.py
--rw-r--r--   0        0        0       50 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/session/env_vars.py
--rw-r--r--   0        0        0      955 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/session/exception.py
--rw-r--r--   0        0        0     6840 2023-10-20 23:32:22.671117 e2b-0.9.6/e2b/session/filesystem.py
--rw-r--r--   0        0        0     3326 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/session/filesystem_watcher.py
--rw-r--r--   0        0        0     7434 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/session/main.py
--rw-r--r--   0        0        0      404 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/session/out.py
--rw-r--r--   0        0        0    11353 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/session/process.py
--rw-r--r--   0        0        0     2118 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/session/run_code.py
--rw-r--r--   0        0        0    11904 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/session/session_connection.py
--rw-r--r--   0        0        0     6194 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/session/session_rpc.py
--rw-r--r--   0        0        0     8580 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/session/terminal.py
--rw-r--r--   0        0        0     3224 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/session/websocket_client.py
--rw-r--r--   0        0        0       40 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/templates/__init__.py
--rw-r--r--   0        0        0     4070 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/templates/data_analysis.py
--rw-r--r--   0        0        0      952 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/utils/filesystem.py
--rw-r--r--   0        0        0     1179 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/utils/future.py
--rw-r--r--   0        0        0      166 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/utils/id.py
--rw-r--r--   0        0        0       34 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/utils/noop.py
--rw-r--r--   0        0        0      287 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/utils/str.py
--rw-r--r--   0        0        0      902 2023-10-20 23:32:22.675117 e2b-0.9.6/e2b/utils/threads.py
--rw-r--r--   0        0        0      912 2023-10-20 23:33:37.410575 e2b-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 e2b-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1493 2023-10-26 04:21:07.535476 e2b-0.9.7/README.md
+-rw-r--r--   0        0        0      468 2023-10-26 04:21:07.535476 e2b-0.9.7/e2b/__init__.py
+-rw-r--r--   0        0        0     1040 2023-10-26 04:21:07.535476 e2b-0.9.7/e2b/api/.openapi-generator-ignore
+-rw-r--r--   0        0        0      711 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/__init__.py
+-rw-r--r--   0        0        0     1792 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/__init__.py
+-rw-r--r--   0        0        0      214 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/api/__init__.py
+-rw-r--r--   0        0        0     6231 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/api/default_api.py
+-rw-r--r--   0        0        0    48260 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/api/envs_api.py
+-rw-r--r--   0        0        0    26370 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/api/sessions_api.py
+-rw-r--r--   0        0        0    28932 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/api_client.py
+-rw-r--r--   0        0        0      805 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/api_response.py
+-rw-r--r--   0        0        0    16716 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/configuration.py
+-rw-r--r--   0        0        0     5000 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/exceptions.py
+-rw-r--r--   0        0        0     1054 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/models/__init__.py
+-rw-r--r--   0        0        0     2232 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/models/environment.py
+-rw-r--r--   0        0        0      688 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/models/environment_state.py
+-rw-r--r--   0        0        0     2138 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/models/environment_state_update.py
+-rw-r--r--   0        0        0     2095 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/models/environment_title_update.py
+-rw-r--r--   0        0        0     2340 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/models/envs_get200_response_inner.py
+-rw-r--r--   0        0        0     2049 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/models/error.py
+-rw-r--r--   0        0        0     2134 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/models/new_environment.py
+-rw-r--r--   0        0        0     2574 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/models/new_session.py
+-rw-r--r--   0        0        0     2769 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/models/session.py
+-rw-r--r--   0        0        0     2949 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/models/sessions_get200_response_inner.py
+-rw-r--r--   0        0        0      752 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/models/template.py
+-rw-r--r--   0        0        0    13020 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client/rest.py
+-rw-r--r--   0        0        0     4245 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v1/client_README.md
+-rw-r--r--   0        0        0        0 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/__init__.py
+-rw-r--r--   0        0        0     1599 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/__init__.py
+-rw-r--r--   0        0        0      214 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/api/__init__.py
+-rw-r--r--   0        0        0     6176 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/api/default_api.py
+-rw-r--r--   0        0        0    47755 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/api/envs_api.py
+-rw-r--r--   0        0        0    25966 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/api/sessions_api.py
+-rw-r--r--   0        0        0    29311 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/api_client.py
+-rw-r--r--   0        0        0      827 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/api_response.py
+-rw-r--r--   0        0        0    16671 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/configuration.py
+-rw-r--r--   0        0        0     5280 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/exceptions.py
+-rw-r--r--   0        0        0      861 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/models/__init__.py
+-rw-r--r--   0        0        0     2212 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/models/environment.py
+-rw-r--r--   0        0        0      688 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/models/environment_state.py
+-rw-r--r--   0        0        0     2118 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/models/environment_state_update.py
+-rw-r--r--   0        0        0     2075 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/models/environment_title_update.py
+-rw-r--r--   0        0        0     2051 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/models/error.py
+-rw-r--r--   0        0        0     2114 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/models/new_environment.py
+-rw-r--r--   0        0        0     2554 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/models/new_session.py
+-rw-r--r--   0        0        0     2749 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/models/session.py
+-rw-r--r--   0        0        0      752 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/models/template.py
+-rw-r--r--   0        0        0    13141 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client/rest.py
+-rw-r--r--   0        0        0     4070 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/api/v2/client_README.md
+-rw-r--r--   0        0        0      178 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/constants.py
+-rw-r--r--   0        0        0      594 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/session/__init__.py
+-rw-r--r--   0        0        0     1720 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/session/code_snippet.py
+-rw-r--r--   0        0        0       50 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/session/env_vars.py
+-rw-r--r--   0        0        0      955 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/session/exception.py
+-rw-r--r--   0        0        0     6840 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/session/filesystem.py
+-rw-r--r--   0        0        0     3326 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/session/filesystem_watcher.py
+-rw-r--r--   0        0        0     7434 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/session/main.py
+-rw-r--r--   0        0        0      404 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/session/out.py
+-rw-r--r--   0        0        0    11303 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/session/process.py
+-rw-r--r--   0        0        0     2118 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/session/run_code.py
+-rw-r--r--   0        0        0    11796 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/session/session_connection.py
+-rw-r--r--   0        0        0     6194 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/session/session_rpc.py
+-rw-r--r--   0        0        0     8580 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/session/terminal.py
+-rw-r--r--   0        0        0     3224 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/session/websocket_client.py
+-rw-r--r--   0        0        0       40 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/templates/__init__.py
+-rw-r--r--   0        0        0     4070 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/templates/data_analysis.py
+-rw-r--r--   0        0        0      952 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/utils/filesystem.py
+-rw-r--r--   0        0        0     1179 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/utils/future.py
+-rw-r--r--   0        0        0      166 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/utils/id.py
+-rw-r--r--   0        0        0       34 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/utils/noop.py
+-rw-r--r--   0        0        0      287 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/utils/str.py
+-rw-r--r--   0        0        0      902 2023-10-26 04:21:07.539476 e2b-0.9.7/e2b/utils/threads.py
+-rw-r--r--   0        0        0      912 2023-10-26 04:22:02.875122 e2b-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 e2b-0.9.7/PKG-INFO
```

### Comparing `e2b-0.9.6/README.md` & `e2b-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/.openapi-generator-ignore` & `e2b-0.9.7/e2b/api/.openapi-generator-ignore`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/__init__.py` & `e2b-0.9.7/e2b/api/__init__.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/__init__.py` & `e2b-0.9.7/e2b/api/v1/client/__init__.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/api/default_api.py` & `e2b-0.9.7/e2b/api/v1/client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/api/envs_api.py` & `e2b-0.9.7/e2b/api/v1/client/api/envs_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/api/sessions_api.py` & `e2b-0.9.7/e2b/api/v1/client/api/sessions_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/api_client.py` & `e2b-0.9.7/e2b/api/v1/client/api_client.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/api_response.py` & `e2b-0.9.7/e2b/api/v1/client/api_response.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/configuration.py` & `e2b-0.9.7/e2b/api/v1/client/configuration.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/exceptions.py` & `e2b-0.9.7/e2b/api/v1/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/models/__init__.py` & `e2b-0.9.7/e2b/api/v1/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/models/environment.py` & `e2b-0.9.7/e2b/api/v1/client/models/environment.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/models/environment_state.py` & `e2b-0.9.7/e2b/api/v1/client/models/environment_state.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/models/environment_state_update.py` & `e2b-0.9.7/e2b/api/v1/client/models/environment_state_update.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/models/environment_title_update.py` & `e2b-0.9.7/e2b/api/v1/client/models/environment_title_update.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/models/envs_get200_response_inner.py` & `e2b-0.9.7/e2b/api/v1/client/models/envs_get200_response_inner.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/models/error.py` & `e2b-0.9.7/e2b/api/v1/client/models/error.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/models/new_environment.py` & `e2b-0.9.7/e2b/api/v1/client/models/new_environment.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/models/new_session.py` & `e2b-0.9.7/e2b/api/v1/client/models/new_session.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/models/session.py` & `e2b-0.9.7/e2b/api/v1/client/models/session.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/models/sessions_get200_response_inner.py` & `e2b-0.9.7/e2b/api/v1/client/models/sessions_get200_response_inner.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/models/template.py` & `e2b-0.9.7/e2b/api/v1/client/models/template.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client/rest.py` & `e2b-0.9.7/e2b/api/v1/client/rest.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v1/client_README.md` & `e2b-0.9.7/e2b/api/v1/client_README.md`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/__init__.py` & `e2b-0.9.7/e2b/api/v2/client/__init__.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/api/default_api.py` & `e2b-0.9.7/e2b/api/v2/client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/api/envs_api.py` & `e2b-0.9.7/e2b/api/v2/client/api/envs_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/api/sessions_api.py` & `e2b-0.9.7/e2b/api/v2/client/api/sessions_api.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/api_client.py` & `e2b-0.9.7/e2b/api/v2/client/api_client.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/api_response.py` & `e2b-0.9.7/e2b/api/v2/client/api_response.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/configuration.py` & `e2b-0.9.7/e2b/api/v2/client/configuration.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/exceptions.py` & `e2b-0.9.7/e2b/api/v2/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/models/__init__.py` & `e2b-0.9.7/e2b/api/v2/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/models/environment.py` & `e2b-0.9.7/e2b/api/v2/client/models/environment.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/models/environment_state.py` & `e2b-0.9.7/e2b/api/v2/client/models/environment_state.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/models/environment_state_update.py` & `e2b-0.9.7/e2b/api/v2/client/models/environment_state_update.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/models/environment_title_update.py` & `e2b-0.9.7/e2b/api/v2/client/models/environment_title_update.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/models/error.py` & `e2b-0.9.7/e2b/api/v2/client/models/error.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/models/new_environment.py` & `e2b-0.9.7/e2b/api/v2/client/models/new_environment.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/models/new_session.py` & `e2b-0.9.7/e2b/api/v2/client/models/new_session.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/models/session.py` & `e2b-0.9.7/e2b/api/v2/client/models/session.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/models/template.py` & `e2b-0.9.7/e2b/api/v2/client/models/template.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client/rest.py` & `e2b-0.9.7/e2b/api/v2/client/rest.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/api/v2/client_README.md` & `e2b-0.9.7/e2b/api/v2/client_README.md`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/session/__init__.py` & `e2b-0.9.7/e2b/session/__init__.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/session/code_snippet.py` & `e2b-0.9.7/e2b/session/code_snippet.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/session/exception.py` & `e2b-0.9.7/e2b/session/exception.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/session/filesystem.py` & `e2b-0.9.7/e2b/session/filesystem.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/session/filesystem_watcher.py` & `e2b-0.9.7/e2b/session/filesystem_watcher.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/session/main.py` & `e2b-0.9.7/e2b/session/main.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/session/process.py` & `e2b-0.9.7/e2b/session/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from asyncio.exceptions import TimeoutError
 from concurrent.futures import ThreadPoolExecutor
 from typing import (
     Any,
     Callable,
     ClassVar,
     Dict,
     List,
@@ -177,15 +176,15 @@
                 "stdin",
                 [self.process_id, data],
                 timeout=timeout,
             )
         except RpcException as e:
             raise ProcessException(e.message) from e
 
-    async def kill(self, timeout: Optional[float] = TIMEOUT) -> None:
+    def kill(self, timeout: Optional[float] = TIMEOUT) -> None:
         """
         Kills the process.
 
         :param timeout: Specify the duration, in seconds to give the method to finish its execution before it times out (default is 60 seconds). If set to None, the method will continue to wait until it completes, regardless of time
         """
         try:
             self._session._call(
```

### Comparing `e2b-0.9.6/e2b/session/run_code.py` & `e2b-0.9.7/e2b/session/run_code.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/session/session_connection.py` & `e2b-0.9.7/e2b/session/session_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import asyncio
 import functools
 import logging
 import traceback
 import warnings
-from concurrent.futures import ThreadPoolExecutor, TimeoutError
+from concurrent.futures import ThreadPoolExecutor, TimeoutError, Future
 from os import getenv
 from time import sleep
 from typing import Any, Callable, List, Literal, Optional, Union
 
 from pydantic import BaseModel
 from urllib3.exceptions import ReadTimeoutError, MaxRetryError, ConnectTimeoutError
 
@@ -84,15 +83,15 @@
         self._debug_port = _debug_port
         self._debug_dev_env = _debug_dev_env
         self._on_close_child = on_close
 
         self._session: Optional[models.Session] = None
         self._is_open = False
         self._process_cleanup: List[Callable[[], Any]] = []
-        self._refreshing_task: Optional[asyncio.Future] = None
+        self._refreshing_task: Optional[Future] = None
         self._subscribers = {}
         self._rpc: Optional[SessionRpc] = None
         self._finished = DeferredFuture(self._process_cleanup)
 
         logger.info(f"Session for code snippet {self._id} initialized")
 
         self._open(timeout=timeout)
@@ -175,15 +174,14 @@
                     api_key=self._api_key,
                     _request_timeout=timeout,
                 )
                 logger.info(
                     f"Session {self._session.code_snippet_id} created (id:{self._session.session_id})"
                 )
 
-                # We could potentially use asyncio.to_thread() but that requires Python 3.9+
                 executor = ThreadPoolExecutor(thread_name_prefix="e2b-refresh")
                 self._refreshing_task = executor.submit(
                     self._refresh, self._session.session_id
                 )
 
                 self._process_cleanup.append(self._refreshing_task.cancel)
                 self._process_cleanup.append(lambda: shutdown_executor(executor))
```

### Comparing `e2b-0.9.6/e2b/session/session_rpc.py` & `e2b-0.9.7/e2b/session/session_rpc.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/session/terminal.py` & `e2b-0.9.7/e2b/session/terminal.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/session/websocket_client.py` & `e2b-0.9.7/e2b/session/websocket_client.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/templates/data_analysis.py` & `e2b-0.9.7/e2b/templates/data_analysis.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/utils/filesystem.py` & `e2b-0.9.7/e2b/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/utils/future.py` & `e2b-0.9.7/e2b/utils/future.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/e2b/utils/threads.py` & `e2b-0.9.7/e2b/utils/threads.py`

 * *Files identical despite different names*

### Comparing `e2b-0.9.6/pyproject.toml` & `e2b-0.9.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "e2b"
-version = "0.9.6"
+version = "0.9.7"
 description = "E2B SDK that give agents cloud environments"
 authors = ["e2b <hello@e2b.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/e2b/tree/main/packages/python-sdk"
 packages = [{ include = "e2b" }]
```

### Comparing `e2b-0.9.6/PKG-INFO` & `e2b-0.9.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2b
-Version: 0.9.6
+Version: 0.9.7
 Summary: E2B SDK that give agents cloud environments
 Home-page: https://e2b.dev/
 License: MIT
 Author: e2b
 Author-email: hello@e2b.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: e2b Version: 0.9.6 Summary: E2B SDK that give
+Metadata-Version: 2.1 Name: e2b Version: 0.9.7 Summary: E2B SDK that give
 agents cloud environments Home-page: https://e2b.dev/ License: MIT Author: e2b
 Author-email: hello@e2b.dev Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aenum
 (>=3.1.11) Requires-Dist: aiohttp (>=3.8.4) Requires-Dist: jsonrpcclient
```

