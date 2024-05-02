# Comparing `tmp/sema4ai_action_server-0.5.3.tar.gz` & `tmp/sema4ai_action_server-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sema4ai_action_server-0.5.3.tar", max compression
+gzip compressed data, was "sema4ai_action_server-0.6.0.tar", max compression
```

## Comparing `sema4ai_action_server-0.5.3.tar` & `sema4ai_action_server-0.6.0.tar`

### file list

```diff
@@ -1,83 +1,87 @@
--rw-r--r--   0        0        0     4043 2024-04-24 19:35:25.878711 sema4ai_action_server-0.5.3/README.md
--rw-r--r--   0        0        0     2097 2024-04-24 19:35:25.878711 sema4ai_action_server-0.5.3/build.py
--rw-r--r--   0        0        0     1691 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      894 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/README.md
--rw-r--r--   0        0        0      128 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/__init__.py
--rw-r--r--   0        0        0      283 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/__main__.py
--rw-r--r--   0        0        0    20141 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_actions_import.py
--rw-r--r--   0        0        0    20508 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_actions_process_pool.py
--rw-r--r--   0        0        0    11348 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_actions_run.py
--rw-r--r--   0        0        0     1263 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_actions_run_helpers.py
--rw-r--r--   0        0        0     1237 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_api_action_package.py
--rw-r--r--   0        0        0     7722 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_api_run.py
--rw-r--r--   0        0        0     2623 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_app.py
--rw-r--r--   0        0        0      775 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_cli_helpers.py
--rw-r--r--   0        0        0    21166 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_database.py
--rw-r--r--   0        0        0     1875 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_download_rcc.py
--rw-r--r--   0        0        0     3764 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_errors.py
--rw-r--r--   0        0        0      113 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_errors_action_server.py
--rw-r--r--   0        0        0      642 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_gen_ids.py
--rw-r--r--   0        0        0     5210 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_models.py
--rw-r--r--   0        0        0     2764 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_new_project.py
--rw-r--r--   0        0        0        0 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_preload_actions/__init__.py
--rw-r--r--   0        0        0      714 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_preload_actions/preload_actions.py
--rw-r--r--   0        0        0    10693 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_preload_actions/preload_actions_server_main.py
--rw-r--r--   0        0        0     7857 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_preload_actions/preload_actions_streams.py
--rw-r--r--   0        0        0      691 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_preload_actions/preload_actions_teardown.py
--rw-r--r--   0        0        0     4322 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_protocols.py
--rw-r--r--   0        0        0    10440 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_rcc.py
--rw-r--r--   0        0        0      426 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/auth.py
--rw-r--r--   0        0        0     1526 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/callback.py
--rw-r--r--   0        0        0     1282 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/constants.py
--rw-r--r--   0        0        0     1027 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/log_custom_handler.py
--rw-r--r--   0        0        0     1397 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/log_formatter.py
--rw-r--r--   0        0        0    19023 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/process.py
--rw-r--r--   0        0        0      692 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/run_in_thread.py
--rw-r--r--   0        0        0    13510 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/system_mutex.py
--rw-r--r--   0        0        0     4031 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_runs_state_cache.py
--rw-r--r--   0        0        0    15891 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_selftest.py
--rw-r--r--   0        0        0    11163 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_server.py
--rw-r--r--   0        0        0    16734 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_server_expose.py
--rw-r--r--   0        0        0    10275 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_server_websockets.py
--rw-r--r--   0        0        0     4746 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_settings.py
--rw-r--r--   0        0        0     1650 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_slugify.py
--rw-r--r--   0        0        0   880128 2024-04-24 19:36:09.951016 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_static_contents.py
--rw-r--r--   0        0        0     2403 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/_whitelist.py
--rw-r--r--   0        0        0        6 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/bin/.gitignore
--rw-r--r--   0        0        0    25082 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/cli.py
--rw-r--r--   0        0        0     4725 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/migrations/__init__.py
--rw-r--r--   0        0        0      408 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/migrations/migration_add_action_enabled.py
--rw-r--r--   0        0        0      375 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/migrations/migration_add_action_managed_params.py
--rw-r--r--   0        0        0      372 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/migrations/migration_add_is_consequential.py
--rw-r--r--   0        0        0      259 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/migrations/migration_initial.py
--rw-r--r--   0        0        0        0 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/package/__init__.py
--rw-r--r--   0        0        0      468 2024-04-24 19:35:25.886711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/package/_ask_user.py
--rw-r--r--   0        0        0     7639 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/package/_package_build.py
--rw-r--r--   0        0        0     7658 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/package/_package_build_cli.py
--rw-r--r--   0        0        0     3292 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/package/_package_metadata.py
--rw-r--r--   0        0        0        0 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/py.typed
--rw-r--r--   0        0        0      349 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/README.md
--rw-r--r--   0        0        0        0 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/__init__.py
--rw-r--r--   0        0        0    14982 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/action_package_handling/__init__.py
--rw-r--r--   0        0        0      157 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/action_package_handling/cli_errors.py
--rw-r--r--   0        0        0        0 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/__init__.py
--rw-r--r--   0        0        0     1812 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/_conda_deps.py
--rw-r--r--   0        0        0     6112 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/_deps_protocols.py
--rw-r--r--   0        0        0     1405 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/_package_deps.py
--rw-r--r--   0        0        0     2333 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/_pip_deps.py
--rw-r--r--   0        0        0    23321 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/analyzer.py
--rw-r--r--   0        0        0    23813 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/conda_cloud.py
--rw-r--r--   0        0        0        0 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/__init__.py
--rw-r--r--   0        0        0      849 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py
--rw-r--r--   0        0        0    11440 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py
--rw-r--r--   0        0        0     9084 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_path.py
--rw-r--r--   0        0        0    13400 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_url.py
--rw-r--r--   0        0        0    25543 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_version.py
--rw-r--r--   0        0        0        0 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/__init__.py
--rw-r--r--   0        0        0     8976 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py
--rw-r--r--   0        0        0     1431 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py
--rw-r--r--   0        0        0    14693 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py
--rw-r--r--   0        0        0     7245 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/pypi_cloud.py
--rw-r--r--   0        0        0      319 2024-04-24 19:35:25.890711 sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/termcolors/__init__.py
--rw-r--r--   0        0        0     5914 1970-01-01 00:00:00.000000 sema4ai_action_server-0.5.3/setup.py
--rw-r--r--   0        0        0     5222 1970-01-01 00:00:00.000000 sema4ai_action_server-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     4043 2024-05-02 19:27:14.145207 sema4ai_action_server-0.6.0/README.md
+-rw-r--r--   0        0        0     2097 2024-05-02 19:27:14.145207 sema4ai_action_server-0.6.0/build.py
+-rw-r--r--   0        0        0     1691 2024-05-02 19:27:14.149207 sema4ai_action_server-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      894 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/README.md
+-rw-r--r--   0        0        0      128 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/__init__.py
+-rw-r--r--   0        0        0      283 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/__main__.py
+-rw-r--r--   0        0        0    20456 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_actions_import.py
+-rw-r--r--   0        0        0    20508 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_actions_process_pool.py
+-rw-r--r--   0        0        0    11265 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_actions_run.py
+-rw-r--r--   0        0        0     1263 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_actions_run_helpers.py
+-rw-r--r--   0        0        0     1237 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_api_action_package.py
+-rw-r--r--   0        0        0     7722 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_api_run.py
+-rw-r--r--   0        0        0     2623 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_app.py
+-rw-r--r--   0        0        0      775 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_cli_helpers.py
+-rw-r--r--   0        0        0    24161 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_cli_impl.py
+-rw-r--r--   0        0        0    21379 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_database.py
+-rw-r--r--   0        0        0     1875 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_download_rcc.py
+-rw-r--r--   0        0        0     3764 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_errors.py
+-rw-r--r--   0        0        0      113 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_errors_action_server.py
+-rw-r--r--   0        0        0      642 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_gen_ids.py
+-rw-r--r--   0        0        0     5233 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_models.py
+-rw-r--r--   0        0        0     2764 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_new_project.py
+-rw-r--r--   0        0        0        0 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_preload_actions/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_preload_actions/preload_actions.py
+-rw-r--r--   0        0        0    10693 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_preload_actions/preload_actions_server_main.py
+-rw-r--r--   0        0        0     7857 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_preload_actions/preload_actions_streams.py
+-rw-r--r--   0        0        0      691 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_preload_actions/preload_actions_teardown.py
+-rw-r--r--   0        0        0     4455 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_protocols.py
+-rw-r--r--   0        0        0    13075 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_rcc.py
+-rw-r--r--   0        0        0      426 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/auth.py
+-rw-r--r--   0        0        0     1526 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/callback.py
+-rw-r--r--   0        0        0     1282 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/constants.py
+-rw-r--r--   0        0        0     1027 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/log_custom_handler.py
+-rw-r--r--   0        0        0     1548 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/log_formatter.py
+-rw-r--r--   0        0        0    19023 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/process.py
+-rw-r--r--   0        0        0      692 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/run_in_thread.py
+-rw-r--r--   0        0        0    13510 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/system_mutex.py
+-rw-r--r--   0        0        0     4031 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_runs_state_cache.py
+-rw-r--r--   0        0        0    16410 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_selftest.py
+-rw-r--r--   0        0        0    11630 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_server.py
+-rw-r--r--   0        0        0    16734 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_server_expose.py
+-rw-r--r--   0        0        0    10275 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_server_websockets.py
+-rw-r--r--   0        0        0     4746 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_settings.py
+-rw-r--r--   0        0        0     1650 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_slugify.py
+-rw-r--r--   0        0        0   880128 2024-05-02 19:28:37.909124 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_static_contents.py
+-rw-r--r--   0        0        0     2403 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/_whitelist.py
+-rw-r--r--   0        0        0     1287 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/api.py
+-rw-r--r--   0        0        0        6 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/bin/.gitignore
+-rw-r--r--   0        0        0     1859 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/cli.py
+-rw-r--r--   0        0        0      870 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/env/__init__.py
+-rw-r--r--   0        0        0     4830 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/migrations/__init__.py
+-rw-r--r--   0        0        0      408 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/migrations/migration_add_action_enabled.py
+-rw-r--r--   0        0        0      375 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/migrations/migration_add_action_managed_params.py
+-rw-r--r--   0        0        0      381 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/migrations/migration_add_action_options.py
+-rw-r--r--   0        0        0      372 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/migrations/migration_add_is_consequential.py
+-rw-r--r--   0        0        0      259 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/migrations/migration_initial.py
+-rw-r--r--   0        0        0        0 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/package/__init__.py
+-rw-r--r--   0        0        0      468 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/package/_ask_user.py
+-rw-r--r--   0        0        0     7645 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/package/_package_build.py
+-rw-r--r--   0        0        0     7658 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/package/_package_build_cli.py
+-rw-r--r--   0        0        0     3298 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/package/_package_metadata.py
+-rw-r--r--   0        0        0        0 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/py.typed
+-rw-r--r--   0        0        0      349 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/__init__.py
+-rw-r--r--   0        0        0    14982 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/action_package_handling/__init__.py
+-rw-r--r--   0        0        0      157 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/action_package_handling/cli_errors.py
+-rw-r--r--   0        0        0        0 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/__init__.py
+-rw-r--r--   0        0        0     1812 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/_conda_deps.py
+-rw-r--r--   0        0        0     6112 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/_deps_protocols.py
+-rw-r--r--   0        0        0     1405 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/_package_deps.py
+-rw-r--r--   0        0        0     2333 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/_pip_deps.py
+-rw-r--r--   0        0        0    23321 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/analyzer.py
+-rw-r--r--   0        0        0    23813 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_cloud.py
+-rw-r--r--   0        0        0        0 2024-05-02 19:27:14.153207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/__init__.py
+-rw-r--r--   0        0        0      849 2024-05-02 19:27:14.157207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py
+-rw-r--r--   0        0        0    11440 2024-05-02 19:27:14.157207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py
+-rw-r--r--   0        0        0     9084 2024-05-02 19:27:14.157207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_path.py
+-rw-r--r--   0        0        0    13400 2024-05-02 19:27:14.157207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_url.py
+-rw-r--r--   0        0        0    25543 2024-05-02 19:27:14.157207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_version.py
+-rw-r--r--   0        0        0        0 2024-05-02 19:27:14.157207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/__init__.py
+-rw-r--r--   0        0        0     8976 2024-05-02 19:27:14.157207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py
+-rw-r--r--   0        0        0     1431 2024-05-02 19:27:14.157207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py
+-rw-r--r--   0        0        0    14693 2024-05-02 19:27:14.157207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py
+-rw-r--r--   0        0        0     7245 2024-05-02 19:27:14.157207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/pypi_cloud.py
+-rw-r--r--   0        0        0      319 2024-05-02 19:27:14.157207 sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/termcolors/__init__.py
+-rw-r--r--   0        0        0     5944 1970-01-01 00:00:00.000000 sema4ai_action_server-0.6.0/setup.py
+-rw-r--r--   0        0        0     5222 1970-01-01 00:00:00.000000 sema4ai_action_server-0.6.0/PKG-INFO
```

### Comparing `sema4ai_action_server-0.5.3/README.md` & `sema4ai_action_server-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/build.py` & `sema4ai_action_server-0.6.0/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from pathlib import Path
 from typing import Optional
 
 # No real build, just download RCC at this point.
 
 # Note: referenced here and in sema4ai.action_server._download_rcc
-RCC_VERSION = "17.23.2"
+RCC_VERSION = "17.28.4"
 
 RCC_URLS = {
     "Windows": f"https://sema4.ai/cdn/downloads/rcc/releases/v{RCC_VERSION}/windows64/rcc.exe",
     "Darwin": f"https://sema4.ai/cdn/downloads/rcc/releases/v{RCC_VERSION}/macos64/rcc",
     "Linux": f"https://sema4.ai/cdn/downloads/rcc/releases/v{RCC_VERSION}/linux64/rcc",
 }
```

### Comparing `sema4ai_action_server-0.5.3/pyproject.toml` & `sema4ai_action_server-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sema4ai-action-server"
-version = "0.5.3"
+version = "0.6.0"
 description = """Sema4AI Action Server"""
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/sema4ai/actions/"
 license = "Apache-2.0"
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/README.md` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/README.md`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_actions_import.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_actions_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         condahash = create_hash(repr(contents))
 
         log.info(
             "Action package seems ok. "
             "Bootstrapping RCC environment (please wait, this can take a long time)."
         )
         rcc = get_rcc()
-        env_info = rcc.create_env_and_get_vars(conda_yaml, condahash)
+        env_info = rcc.create_env_and_get_vars(datadir, conda_yaml, condahash)
         if not env_info.success:
             raise ActionPackageError(
                 f"It was not possible to bootstrap the RCC environment. "
                 f"Error: {env_info.message}"
             )
         if not env_info.result:
             raise ActionPackageError(
@@ -462,47 +462,55 @@
             except ValueError:
                 pass
 
             managed_params_str: str = ""
             if action_fields.get("managed_params_schema"):
                 managed_params_str = json.dumps(action_fields["managed_params_schema"])
 
+            options = action_fields.get("options") or {}
             actions.append(
                 Action(
                     id=gen_uuid("action"),
                     action_package_id=action_package.id,
                     name=action_name,
                     docs=action_fields["docs"],
                     file=filepath.as_posix(),
                     lineno=action_fields["line"],
                     input_schema=json.dumps(action_fields["input_schema"]),
                     output_schema=json.dumps(action_fields["output_schema"]),
                     enabled=True,
-                    is_consequential=(action_fields.get("options") or {}).get(
-                        "is_consequential", None
-                    ),
+                    is_consequential=options.get("is_consequential", None),
                     managed_params_schema=managed_params_str,
+                    options=json.dumps(options),
                 )
             )
 
     db = get_db()
+    if disable_not_imported:
+        all_previously_existing_actions = db.all(Action)
+
     try:
         existing_action_package = db.first(
             ActionPackage,
             "SELECT * FROM action_package WHERE name = ?",
             [action_package.name],
         )
     except KeyError:
         # ok, insert as new one
         with db.transaction():
             log.info("Found new action package: %s", action_package.name)
             db.insert(action_package)
             for action in actions:
                 log.info("Found new action: %s", action.name)
                 db.insert(action)
+
+            if disable_not_imported:
+                for action in all_previously_existing_actions:
+                    log.info("Disabling action: %s", action.name)
+                    db.update_by_id(Action, action.id, dict(enabled=False))
     else:
         # We already have an existing action package with the same name. This
         # means we'll have to update it instead of adding a new one.
         new_action_package_as_dict = asdict(action_package)
         # The id should not be updated.
         del new_action_package_as_dict["id"]
 
@@ -512,17 +520,14 @@
             [existing_action_package.id],
         )
 
         existing_action_name_to_action = {}
         for action in existing_actions:
             existing_action_name_to_action[action.name] = action
 
-        if disable_not_imported:
-            all_actions = db.all(Action)
-
         seen_action_ids = set()
         with db.transaction():
             log.debug("Updating action package: %s", action_package.name)
             db.update_by_id(
                 ActionPackage,
                 existing_action_package.id,
                 new_action_package_as_dict,
@@ -543,11 +548,11 @@
                 else:
                     # This is a new action, insert it.
                     log.info("Found new action: %s", action.name)
                     db.insert(action)
                     seen_action_ids.add(action.id)
 
             if disable_not_imported:
-                for action in all_actions:
+                for action in all_previously_existing_actions:
                     if action.id not in seen_action_ids:
                         log.info("Disabling action: %s", action.name)
                         db.update_by_id(Action, action.id, dict(enabled=False))
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_actions_process_pool.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_actions_process_pool.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_actions_run.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_actions_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,15 @@
 
 
 def _name_as_class_name(name):
     return name.replace("_", " ").title().replace(" ", "")
 
 
 def generate_func_from_action(
-    action: "Action",
+    action: "Action", display_name: str
 ) -> Tuple[Callable[[Response, Request], Any], dict[str, object]]:
     """
     This method generates the function which should be called from FastAPI.
 
     Initially it generated the function with the parameters required to build
     the openapi.json spec properly, but it was changed to deal with the body
     directly and provide the openapi.json bits needed as it's easier and more
@@ -288,17 +288,15 @@
         },
         "responses": {
             "200": {
                 "content": {
                     "application/json": {
                         "schema": {
                             **output_schema_dict,
-                            **{
-                                "title": f"Response {action.name.title().replace('_', ' ').replace('-', ' ')}"
-                            },
+                            **{"title": f"Response for {display_name}"},
                         }
                     }
                 },
                 "description": "Successful Response",
             },
             "422": {
                 "content": {
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_actions_run_helpers.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_actions_run_helpers.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_api_action_package.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_api_action_package.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_api_run.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_api_run.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_app.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_app.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_cli_helpers.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_cli_helpers.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_database.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -669,11 +669,19 @@
             raise RuntimeError(f"Unsupported type: {field_cls}")
 
         use = f"{name} {use}"
 
         if not_null and field_cls != bool:
             use = f"{use} NOT NULL"
 
+        try:
+            default_value = getattr(cls, name)
+        except AttributeError:
+            pass
+        else:
+            if field_cls == str:
+                use = f"{use} DEFAULT {default_value!r}"
+
         if primary_key:
             use = f"{use} PRIMARY KEY"
 
         return f"{use}"
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_download_rcc.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_download_rcc.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import sys
 from pathlib import Path
 from typing import Optional
 
 log = logging.getLogger(__name__)
 
 # Note: also referenced in action_server/build.py
-RCC_VERSION = "17.23.2"
+RCC_VERSION = "17.28.4"
 RCC_URLS = {
     "Windows": f"https://sema4.ai/cdn/downloads/rcc/releases/v{RCC_VERSION}/windows64/rcc.exe",
     "Darwin": f"https://sema4.ai/cdn/downloads/rcc/releases/v{RCC_VERSION}/macos64/rcc",
     "Linux": f"https://sema4.ai/cdn/downloads/rcc/releases/v{RCC_VERSION}/linux64/rcc",
 }
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_errors.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_errors.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_gen_ids.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_gen_ids.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_models.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
     enabled: bool = True
 
     is_consequential: Optional[bool] = None
 
     # The json content for the managed params schema
     managed_params_schema: Optional[str] = None
 
+    options: str = ""
+
 
 RUN_ID_COUNTER = "run_id"
 ALL_COUNTERS = (RUN_ID_COUNTER,)
 
 
 @dataclass
 class Counter:
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_new_project.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_new_project.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_preload_actions/preload_actions.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_preload_actions/preload_actions.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_preload_actions/preload_actions_server_main.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_preload_actions/preload_actions_server_main.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_preload_actions/preload_actions_streams.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_preload_actions/preload_actions_streams.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_preload_actions/preload_actions_teardown.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_preload_actions/preload_actions_teardown.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_protocols.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_protocols.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,24 +100,29 @@
 
 class ArgumentsNamespace(Protocol):
     """
     This is the argparse.Namespace with the arguments provided by the user.
     """
 
     command: Literal[
-        "download-rcc", "package", "import", "start", "version", "new", "migrate"
+        "download-rcc", "package", "import", "start", "version", "new", "migrate", "env"
     ]
     verbose: bool
 
 
 class ArgumentsNamespaceNew(ArgumentsNamespace):
     command: Literal["new"]
     name: str
 
 
+class ArgumentsNamespaceEnv(ArgumentsNamespace):
+    command: Literal["env"]
+    env_command: Literal["clean-tools-caches"]
+
+
 class ArgumentsNamespaceDownloadRcc(ArgumentsNamespace):
     command: Literal["download-rcc"]
     file: str
 
 
 class ArgumentsNamespacePackage(ArgumentsNamespace):
     command: Literal["package"]
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_rcc.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_rcc.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,30 +35,31 @@
 def as_str(s) -> str:
     if isinstance(s, bytes):
         return s.decode("utf-8", "replace")
     return str(s)
 
 
 class Rcc(object):
-    def __init__(self, rcc_location: Path, robocorp_home: Path):
+    def __init__(self, rcc_location: Path, robocorp_home: Optional[Path]):
         self._rcc_location = rcc_location
         self._robocorp_home = robocorp_home
         self.config_location = os.environ.get(
-            "RC_ACTION_SERVER_RCC_CONFIG_LOCATION", ""
+            "S4_ACTION_SERVER_RCC_CONFIG_LOCATION", ""
         )
 
     def _compute_env(self):
         env = os.environ.copy()
         env.pop("PYTHONPATH", "")
         env.pop("PYTHONHOME", "")
         env.pop("VIRTUAL_ENV", "")
         env["PYTHONIOENCODING"] = "utf-8"
         env["PYTHONUNBUFFERED"] = "1"
 
-        env["ROBOCORP_HOME"] = str(self._robocorp_home)
+        if self._robocorp_home:
+            env["ROBOCORP_HOME"] = str(self._robocorp_home)
         return env
 
     def _compute_launch_args_and_kwargs(
         self, cwd, env, args, stderr=Sentinel.SENTINEL
     ) -> Tuple[list, dict]:
         from sema4ai.action_server._robo_utils.process import build_subprocess_kwargs
 
@@ -94,15 +95,17 @@
             but users could change it to something as subprocess.STDOUT).
         """
         from subprocess import check_output, list2cmdline
 
         from sema4ai.action_server._robo_utils.process import check_output_interactive
 
         env = self._compute_env()
-        robocorp_home = env["ROBOCORP_HOME"]
+        robocorp_home = env.get("ROBOCORP_HOME")
+        if not robocorp_home:
+            robocorp_home = "<unset>"
 
         args, kwargs = self._compute_launch_args_and_kwargs(cwd, env, args, stderr)
         cmdline = list2cmdline([str(x) for x in args])
 
         try:
             if mutex_name:
                 from ._robo_utils.system_mutex import timed_acquire_mutex
@@ -198,24 +201,77 @@
             if hide_in_log:
                 msg = msg.replace(hide_in_log, "<HIDDEN_IN_LOG>")
             log.info(msg)
 
         return RCCActionResult(cmdline, success=True, message=None, result=output)
 
     def create_env_and_get_vars(
+        self, datadir: Path, conda_yaml: Path, conda_hash: str
+    ) -> ActionResult[EnvInfo]:
+        """
+        Creates the environment if needed. Note: this function needs to be
+        careful so that it doesn't call `_create_env_and_get_vars` unless
+        the environment file really changed, as that will build an environment
+        (with all the pypi/mamba caches it entails), meaning that if the user
+        did use `action-server env clean-tools-caches` the caches will be
+        rebuilt and the command will need to be called again.
+        """
+
+        env_info_dir = datadir / "env-info"
+        env_info_dir.mkdir(parents=True, exist_ok=True)
+
+        env_info_cache_file = env_info_dir / f"{conda_hash}.json"
+        if env_info_cache_file.exists():
+            try:
+                contents = env_info_cache_file.read_text(encoding="utf-8")
+                if contents:
+                    loaded = json.loads(contents)
+                    loaded["lastUsage"] = self._get_curr_time_as_str()
+                    return ActionResult(True, None, EnvInfo(loaded["environ"]))
+            except Exception:
+                return ActionResult(
+                    success=False,
+                    message=(
+                        f"It was not possible to get the environment info from:\n{env_info_cache_file}\n"
+                        "to proceed delete that file or fix it (note: if the caches\n"
+                        "were cleared they will need to be cleared again after restoring\n"
+                        "the environment)."
+                    ),
+                )
+
+        env_info = self._create_env_and_get_vars(conda_yaml, conda_hash)
+        if env_info.success:
+            assert isinstance(env_info.result, EnvInfo)
+            dump = {
+                "environ": env_info.result.env,
+                "lastUsage": self._get_curr_time_as_str(),
+            }
+            env_info_cache_file.write_text(json.dumps(dump), encoding="utf-8")
+        return env_info
+
+    def _get_curr_time_as_str(self):
+        from datetime import datetime
+
+        return datetime.now().strftime("%Y-%m-%d %H:%M:%S.%f%Z")
+
+    def _create_env_and_get_vars(
         self, conda_yaml: Path, conda_hash: str
     ) -> ActionResult[EnvInfo]:
+        """ """
         args = [
             "holotree",
             "variables",
             "--space",
             conda_hash,
             str(conda_yaml),
         ]
+        self._add_config_to_args(args)
         args.append("--json")
+        args.append("--no-retry-build")
+        args.append("--no-pyc-management")
         timeout = 60 * 60  # Wait up to 1 hour for the env...
         ret = self._run_rcc(
             args,
             mutex_name=RCC_CLOUD_ROBOT_MUTEX_NAME,
             cwd=str(conda_yaml.parent),
             timeout=timeout,  # Creating the env may be really slow!
             show_interactive_output=logging.root.level <= logging.DEBUG,
@@ -283,20 +339,25 @@
         cwd = None
         args, kwargs = self._compute_launch_args_and_kwargs(cwd, env, args)
         try:
             subprocess.Popen(args, **kwargs)
         except BaseException:
             log.exception("Error submitting feedback.")
 
+    def clean_tools_caches(self):
+        args = ["config", "cleanup", "--caches"]
+        self._add_config_to_args(args)
+        self._run_rcc(args, timeout=600, show_interactive_output=True)
+
 
 _rcc: Optional["Rcc"] = None
 
 
 @contextmanager
-def initialize_rcc(rcc_location: Path, robocorp_home: Path) -> Iterator[Rcc]:
+def initialize_rcc(rcc_location: Path, robocorp_home: Optional[Path]) -> Iterator[Rcc]:
     global _rcc
 
     rcc = Rcc(rcc_location, robocorp_home)
     _rcc = rcc
     try:
         yield rcc
     finally:
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/callback.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/callback.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/constants.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/constants.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/log_custom_handler.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/log_custom_handler.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/log_formatter.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/log_formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import re
 from datetime import datetime
 from logging import Filter, Formatter
 
 from termcolor import colored
 
 
@@ -17,15 +18,15 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         from uvicorn.logging import AccessFormatter
 
         self._access_formatter = AccessFormatter()
 
     def format(self, record):
-        if record.name.startswith("uvicorn"):
+        if record.name.startswith("uvicorn") and len(record.args) == 5:
             (
                 client_addr,
                 method,
                 full_path,
                 http_version,
                 status_code,
             ) = record.args
@@ -40,8 +41,12 @@
 
         return super().format(record)
 
 
 class UvicornLogFilter(Filter):
     def filter(self, record):
         # Log only Uvicorn Access messages
-        return not (record.name.startswith("uvicorn") and len(record.args) != 5)
+        if record.levelno > logging.INFO:
+            accept = True
+        else:
+            accept = not (record.name.startswith("uvicorn") and len(record.args) != 5)
+        return accept
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/process.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/process.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/run_in_thread.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/run_in_thread.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_robo_utils/system_mutex.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_robo_utils/system_mutex.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_runs_state_cache.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_runs_state_cache.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_selftest.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_selftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,31 @@
         import pydevd  # type:ignore
     except ImportError:
         return False
 
     return bool(pydevd.get_global_debugger())
 
 
+class ActionServerExitedError(RuntimeError):
+    pass
+
+
 class ActionServerProcess:
     SHOW_OUTPUT = True
 
     def __init__(self, datadir: Path) -> None:
+        from io import StringIO
+
         self._datadir = datadir.absolute()
         self._process: Optional["Process"] = None
         self._host: str = ""
         self._port: int = -1
         self.started: bool = False
+        self._stdout = StringIO()
+        self._stderr = StringIO()
 
     @property
     def datadir(self) -> Path:
         return self._datadir
 
     @property
     def host(self) -> str:
@@ -80,14 +88,16 @@
         add_shutdown_api: bool = False,
         min_processes: int = 0,
         max_processes: int = 20,
         reuse_processes: bool = False,
         lint: bool = False,
         additional_args: Optional[list[str]] = None,
         env: Optional[Dict[str, str]] = None,
+        port=0,
+        verbose="-v",
     ) -> None:
         from sema4ai.action_server._robo_utils.process import Process
         from sema4ai.action_server._settings import is_frozen
 
         if self.started:
             raise RuntimeError("The action process was already started.")
 
@@ -104,20 +114,22 @@
                 sys.executable,
                 "-m",
                 "sema4ai.action_server",
             ]
         new_args = base_args + [
             "start",
             "--actions-sync=false" if not actions_sync else "--actions-sync=true",
-            "--port=0",
-            "--verbose",
+            f"--port={port}",
             f"--datadir={str(self._datadir)}",
             f"--db-file={db_file}",
         ]
 
+        if verbose:
+            new_args.append(verbose)
+
         if not lint:
             new_args.append("--skip-lint")
 
         new_args.append(f"--min-processes={min_processes}")
         new_args.append(f"--max-processes={max_processes}")
         if reuse_processes:
             new_args.append("--reuse-processes")
@@ -140,18 +152,20 @@
             matches = re.findall(compiled, line)
 
             if matches:
                 host, port = matches[0]
                 future.set_result((host, port))
 
         def on_stdout(line):
+            self._stdout.write(line)
             if self.SHOW_OUTPUT:
                 sys.stdout.write(f"stdout: {line.rstrip()}\n")
 
         def on_stderr(line):
+            self._stderr.write(line)
             # Note: this is called in a thread.
             sys.stderr.write(f"stderr: {line.rstrip()}\n")
 
         process.on_stderr.register(on_stderr)
         process.on_stdout.register(on_stdout)
 
         with process.on_stderr.register(collect_port_from_stdout):
@@ -164,31 +178,40 @@
                         break
                     except TimeoutError:
                         if is_debugger_active():
                             continue
                         if time.monotonic() - initial_time >= timeout:
                             raise TimeoutError()
                         if not process.is_alive():
-                            raise RuntimeError(
+                            raise ActionServerExitedError(
                                 f"The process already exited with returncode: "
                                 f"{process.returncode}\n"
                                 f"Args: {new_args}"
                             )
             else:
                 host, port = future.result(timeout)
         assert host
         self._host = host
         assert int(port) > 0, f"Expected port to be > 0. Found: {port}"
         self._port = int(port)
 
     def stop(self):
+        """
+        Returns a tuple with stdout/stderr.
+        """
         if self._process is not None:
             self._process.stop()
             self._process = None
 
+    def get_stdout(self):
+        return self._stdout.getvalue()
+
+    def get_stderr(self):
+        return self._stderr.getvalue()
+
 
 class ActionServerClient:
     _base_url: Optional[str]
     action_server_process: Optional[ActionServerProcess]
 
     def __init__(self, action_server_process_or_base_url: ActionServerProcess | str):
         if isinstance(action_server_process_or_base_url, str):
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_server.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 def start_server(
     expose: bool,
     api_key: str | None,
     expose_session: str | None,
     whitelist: str | None,
     before_start: Sequence[IBeforeStartCallback],
 ) -> None:
+    import json
     from dataclasses import asdict
 
     import uvicorn
     from fastapi import Depends, HTTPException, Security
     from fastapi.security import HTTPAuthorizationCredentials, HTTPBearer
     from fastapi.staticfiles import StaticFiles
     from starlette.requests import Request
@@ -132,24 +133,34 @@
             if not accept_action(whitelist, action_package.name, action.name):
                 log.info(
                     "Skipping action %s / %s (not in whitelist)",
                     action_package.name,
                     action.name,
                 )
                 continue
+        display_name = _name_as_summary(action.name)
+        options = action.options
+        if options:
+            options_as_dict = json.loads(options)
+            if options_as_dict:
+                display_name_in_options = options_as_dict.get("display_name")
+                if display_name_in_options:
+                    display_name = display_name_in_options
 
-        func, openapi_extra = _actions_run.generate_func_from_action(action)
+        func, openapi_extra = _actions_run.generate_func_from_action(
+            action, display_name
+        )
         if action.is_consequential is not None:
             openapi_extra["x-openai-isConsequential"] = action.is_consequential
 
         app.add_api_route(
             build_url_api_run(action_package.name, action.name),
             func,
             name=action.name,
-            summary=_name_as_summary(action.name),
+            summary=display_name,
             description=doc_desc,
             operation_id=action.name,
             methods=["POST"],
             dependencies=endpoint_dependencies,
             openapi_extra=openapi_extra,
         )
 
@@ -330,15 +341,17 @@
         try:
             children_processes = list(p.children(recursive=True))
         except Exception:
             log.exception("Error listing subprocesses.")
 
         for child in children_processes:
             if child.pid != expose_pid:  # If it's still around, don't kill it again.
-                log.info("Killing sub-process when exiting action server: %s", child)
+                log.info(
+                    f"Killing sub-process when exiting action server: {child.name()} (pid: {child.pid})"
+                )
                 try:
                     kill_process_and_subprocesses(child.pid)
                 except Exception:
                     log.exception("Error killing subprocess: %s", child.pid)
 
     app.add_event_handler("startup", _on_startup)
     app.add_event_handler("shutdown", _on_shutdown)
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_server_expose.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_server_expose.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_server_websockets.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_server_websockets.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_settings.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_settings.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_slugify.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_slugify.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_static_contents.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_static_contents.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/_whitelist.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_whitelist.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/cli.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/_cli_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-"""
-Important: 
-
-sema4ai.action_server.cli.main() 
-
-is the only public API supported from the action-server.
-
-Everything else is considered private and can be broken/changed without
-being considered a backward-incompatible change!
-"""
-
 import argparse
 import logging
 import os.path
 import sys
 import time
 import typing
 from contextlib import contextmanager
@@ -40,19 +29,14 @@
     from sema4ai.action_server._database import Database
     from sema4ai.action_server._rcc import Rcc
 
     from ._settings import Settings
 
 log = logging.getLogger(__name__)
 
-# Important: main() is the only public API supported from the action-server.
-# Everything else is considered private and can be broken/changed without
-# being considered a backward-incompatible change!
-__all__ = ["main"]
-
 
 def _add_skip_lint(parser, defaults):
     parser.add_argument(
         "--skip-lint",
         default=False,
         help="Skip `@action` linting when an action is found (by default any "
         "`@action` is linted for errors when found).",
@@ -295,54 +279,28 @@
         help="Prints the version and exits",
     )
 
     _add_migrate_command(command_subparser, defaults)
 
     add_package_command(command_subparser, defaults)
 
-    return base_parser
-
-
-def main(args: Optional[list[str]] = None, *, exit=True) -> int:  # noqa
-    if args is None:
-        args = sys.argv[1:]
-
-    if not args:
-        if os.environ.get(
-            "RC_ACTION_SERVER_FORCE_DOWNLOAD_RCC", ""
-        ).strip().lower() in (
-            "1",
-            "true",
-        ):
-            log.info(
-                "As RC_ACTION_SERVER_FORCE_DOWNLOAD_RCC is set and no arguments were "
-                "passed, rcc will be downloaded."
-            )
-
-            from sema4ai.action_server._download_rcc import download_rcc
-
-            download_rcc(force=True)
-
-        if os.environ.get("RC_ACTION_SERVER_DO_SELFTEST", "").strip().lower() in (
-            "1",
-            "true",
-        ):
-            from . import _selftest
+    # Clean env caches
+    env_parser = command_subparser.add_parser(
+        "env",
+        help="Commands related to the environment handling",
+    )
 
-            log.info(
-                "As RC_ACTION_SERVER_DO_SELFTEST is set and no arguments were passed, "
-                "a selftest will be run."
-            )
+    env_subparser = env_parser.add_subparsers(dest="env_command")
 
-            sys.exit(_selftest.do_selftest())
+    env_parser = env_subparser.add_parser(
+        "clean-tools-caches",
+        help="Cleans up caches from tools used to build the environment (such as micromamba, pip and uv).",
+    )
 
-    retcode = _main_retcode(args)
-    if exit:
-        sys.exit(retcode)
-    return retcode
+    return base_parser
 
 
 def _setup_stderr_logging(log_level):
     from logging import StreamHandler
 
     # stderr is the default, but make it explicit.
     stream_handler = StreamHandler(sys.stderr)
@@ -529,14 +487,19 @@
     if command == "package":
         from sema4ai.action_server.package._package_build_cli import (
             handle_package_command,
         )
 
         return handle_package_command(base_args)
 
+    if command == "env":
+        from sema4ai.action_server.env import handle_env_command
+
+        return handle_env_command(base_args)
+
     if command not in (
         "migrate",
         "import",
         "start",
         "new",
     ):
         log.critical(f"Unexpected command: {command}.")
@@ -579,16 +542,18 @@
 ):
     from ._download_rcc import download_rcc
     from ._rcc import initialize_rcc
     from ._settings import setup_settings
 
     with setup_settings(base_args) as settings:
         settings.datadir.mkdir(parents=True, exist_ok=True)
-        robocorp_home = settings.datadir / ".robocorp_home"
-        robocorp_home.mkdir(parents=True, exist_ok=True)
+        # No longer set ROBOCORP_HOME inside of the datadir.
+        # robocorp_home = settings.datadir / ".robocorp_home"
+        # robocorp_home.mkdir(parents=True, exist_ok=True)
+        robocorp_home = None
 
         with initialize_rcc(download_rcc(force=False), robocorp_home) as rcc:
             yield _SetupInfo(rcc=rcc, settings=settings)
 
 
 def _make_import_migrate_or_start(
     base_args: ArgumentsNamespaceMigrateImportOrStart,
@@ -780,11 +745,7 @@
                     return 0
 
             else:
                 log.critical(f"Unexpected command: {command}.")
                 return 1
     finally:
         mutex.release_mutex()
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/migrations/__init__.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/migrations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     1: "initial",
     # we'll look for a 'migration_add_action_enabled' module based on this.
     2: "add_action_enabled",
     # we'll look for a 'migration_add_is_consequential' module based on this.
     3: "add_is_consequential",
     # we'll look for a 'migration_add_action_managed_params' module based on this.
     4: "add_action_managed_params",
+    # we'll look for a 'migration_add_action_options' module based on this.
+    5: "add_action_options",
 }
 
 CURRENT_VERSION: int = max(MIGRATION_ID_TO_NAME.keys())
 
 
 @dataclass
 class Migration:
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/package/_package_build.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/package/_package_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,17 +103,17 @@
         override: Whether an existing .zip can be overridden.
 
     Returns:
         The return code for the process (0 for success).
     """
     import yaml
 
+    from sema4ai.action_server._cli_impl import _main_retcode
     from sema4ai.action_server._models import Action, create_db
     from sema4ai.action_server._slugify import slugify
-    from sema4ai.action_server.cli import _main_retcode
     from sema4ai.action_server.package._ask_user import ask_user_input_to_proceed
 
     from .._errors_action_server import ActionServerValidationError
 
     # We expect a package.yaml to be there (we don't support just conda.yaml for
     # this).
     package_yaml = input_dir / "package.yaml"
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/package/_package_build_cli.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/package/_package_build_cli.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/package/_package_metadata.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/package/_package_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
     Returns: Either the package metadata to be printed or an error code.
     """
     from fastapi.applications import FastAPI
     from sema4ai.actions._protocols import ActionsListActionTypedDict
 
     from sema4ai.action_server._actions_import import hook_on_actions_list
+    from sema4ai.action_server._cli_impl import _main_retcode
     from sema4ai.action_server._errors_action_server import ActionServerValidationError
     from sema4ai.action_server._models import Action, ActionPackage, create_db
-    from sema4ai.action_server.cli import _main_retcode
 
     args = ["start", "--db-file", ":memory:"]
     if datadir:
         args.extend(["--datadir", datadir])
 
     metadata: Dict[str, Any] = {}
     secrets = {}
```

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/action_package_handling/__init__.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/action_package_handling/__init__.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/_conda_deps.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/_conda_deps.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/_deps_protocols.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/_deps_protocols.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/_package_deps.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/_package_deps.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/_pip_deps.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/_pip_deps.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/analyzer.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/analyzer.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/conda_cloud.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_cloud.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_channel.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_match_spec.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_path.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_path.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_url.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_url.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_version.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/conda_impl/conda_version.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_distlib_util.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_structure.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/pip_impl/pip_packaging_version.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/src/sema4ai/action_server/vendored_deps/package_deps/pypi_cloud.py` & `sema4ai_action_server-0.6.0/src/sema4ai/action_server/vendored_deps/package_deps/pypi_cloud.py`

 * *Files identical despite different names*

### Comparing `sema4ai_action_server-0.5.3/setup.py` & `sema4ai_action_server-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 {'': 'src'}
 
 packages = \
 ['sema4ai',
  'sema4ai.action_server',
  'sema4ai.action_server._preload_actions',
  'sema4ai.action_server._robo_utils',
+ 'sema4ai.action_server.env',
  'sema4ai.action_server.migrations',
  'sema4ai.action_server.package',
  'sema4ai.action_server.vendored_deps',
  'sema4ai.action_server.vendored_deps.action_package_handling',
  'sema4ai.action_server.vendored_deps.package_deps',
  'sema4ai.action_server.vendored_deps.package_deps.conda_impl',
  'sema4ai.action_server.vendored_deps.package_deps.pip_impl',
@@ -38,15 +39,15 @@
  'websockets>=12.0,<13.0']
 
 entry_points = \
 {'console_scripts': ['action-server = sema4ai.action_server.cli:main']}
 
 setup_kwargs = {
     'name': 'sema4ai-action-server',
-    'version': '0.5.3',
+    'version': '0.6.0',
     'description': 'Sema4AI Action Server',
     'long_description': '# sema4ai-action-server\n\n[Sema4.ai Action Server](https://github.com/sema4ai/actions#readme) is a Python framework designed to simplify the deployment of actions (AI or otherwise).\n\nAn `action` in this case is defined as a Python function (which has inputs/outputs defined), which is served by the `Sema4.ai Action Server`.\n\nThe `Sema4.ai Action Server` automatically generates an OpenAPI spec for your Python code, enabling different AI/LLM Agents to understand and call your Action. It also manages the Action lifecycle and provides full traceability of what happened during runs.\n\n## 1. Install Action Server\n\nAction Server is available as a stand-alone fully signed executable and via `pip install sema4ai-action-server`.\n> We recommend the executable to prevent confusion in case you have multiple/crowded Python environments, etc.\n\n#### For macOS\n\n```sh\n# Install Sema4.ai Action Server\nbrew update\nbrew install sema4ai/tools/action-server \n```\n\n#### For Windows\n\n```sh\n# Download Sema4.ai Action Server\ncurl -o action-server.exe https://sema4.ai/cdn/downloads/action-server/releases/latest/windows64/action-server.exe\n\n# Add to PATH or move to a folder that is in PATH\nsetx PATH=%PATH%;%CD%\n```\n\n#### For Linux\n\n```sh\n# Download Sema4.ai Action Server\ncurl -o action-server https://sema4.ai/cdn/downloads/action-server/releases/latest/linux64/action-server\nchmod a+x action-server\n\n# Add to PATH or move to a folder that is in PATH\nsudo mv action-server /usr/local/bin/\n```\n\n## 2. Run your first Action\n\n```sh\n# Bootstrap a new project using this template.\n# You\'ll be prompted for the name of the project (directory):\naction-server new\n\n# Start Action Server \ncd my-project\naction-server start --expose\n```\n\n👉 You should now have an Action Server running locally at: [http://localhost:8080](http://localhost:8080), so open that in your browser and the web UI will guide you further.\n\n👉 Using the `--expose` -flag, you also get a public internet-facing URL (something like "https://twently-cuddly-dinosaurs.robocorp.link") and the related token. These are the details that you need to configure your AI Agent to have access to your Action\n\n## What do you need in your Action Package\n\nAn `Action Package` is currently defined as a local folder that contains at least one Python file containing an action entry point (a Python function marked with `@action` -decorator from `sema4ai.actions`).\n\nThe `package.yaml` file is required for specifying the Python environment and dependencies for your Action ([RCC](https://github.com/robocorp/rcc/) will be used to automatically bootstrap it and keep it updated given the `package.yaml` contents).\n\n> Note: the `package.yaml` is optional if the action server is not being used as a standalone (i.e.: if it was pip-installed it can use the same python environment where it\'s installed).\n\n### Bootstrapping a new Action\n\nStart new projects with:\n\n`action-server new`\n\nNote: the `action-server` executable should be automatically added to your python installation after `pip install sema4ai-action-server`, but if for some reason it wasn\'t pip-installed, it\'s also possible to use `python -m sema4ai.action_server` instead of `action-server`.\n\nAfter creating the project, it\'s possible to serve the actions under the current directory with:\n\n`action-server start`\n\nFor example: When running `action-server start`, the action server will scan for existing actions under the current directory, and it\'ll start serving those.\n\nAfter it\'s started, it\'s possible to access the following URLs:\n\n- `/index.html`: UI for the Action Server.\n- `/openapi.json`: Provides the openapi spec for the action server.\n- `/docs`: Provides access to the APIs available in the server and a UI to test it.\n\n## Documentation\n\nExplore our [docs](https://github.com/sema4ai/actions/tree/master/action_server/docs) for extensive documentation.\n\n## Changelog\n\nA list of releases and corresponding changes can be found in the [changelog](https://github.com/sema4ai/actions/blob/master/action_server/docs/CHANGELOG.md).\n',
     'author': 'Fabio Z.',
     'author_email': 'fabio@robocorp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/sema4ai/actions/',
```

### Comparing `sema4ai_action_server-0.5.3/PKG-INFO` & `sema4ai_action_server-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema4ai-action-server
-Version: 0.5.3
+Version: 0.6.0
 Summary: Sema4AI Action Server
 Home-page: https://github.com/sema4ai/actions/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

