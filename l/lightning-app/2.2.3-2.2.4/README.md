# Comparing `tmp/lightning-app-2.2.3.tar.gz` & `tmp/lightning-app-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-app-2.2.3.tar", last modified: Tue Apr 23 18:46:05 2024, max compression
+gzip compressed data, was "lightning-app-2.2.4.tar", last modified: Wed May  1 22:51:54 2024, max compression
```

## Comparing `lightning-app-2.2.3.tar` & `lightning-app-2.2.4.tar`

### file list

```diff
@@ -1,361 +1,361 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.759478 lightning-app-2.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.707478 lightning-app-2.2.3/.actions/
--rw-r--r--   0 runner    (1001) docker     (127)    20994 2024-04-23 18:45:43.000000 lightning-app-2.2.3/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-23 18:45:43.000000 lightning-app-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-23 18:46:05.755478 lightning-app-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-04-23 18:45:43.000000 lightning-app-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-04-23 18:45:43.000000 lightning-app-2.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.699478 lightning-app-2.2.3/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.707478 lightning-app-2.2.3/requirements/app/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-23 18:45:43.000000 lightning-app-2.2.3/requirements/app/app.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 18:45:43.000000 lightning-app-2.2.3/requirements/app/cloud.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-23 18:45:43.000000 lightning-app-2.2.3/requirements/app/components.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 18:45:43.000000 lightning-app-2.2.3/requirements/app/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-23 18:45:43.000000 lightning-app-2.2.3/requirements/app/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:45:43.000000 lightning-app-2.2.3/requirements/app/ui.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:46:05.759478 lightning-app-2.2.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     7935 2024-04-23 18:45:43.000000 lightning-app-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.707478 lightning-app-2.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.711478 lightning-app-2.2.3/src/lightning_app/
--rw-r--r--   0 runner    (1001) docker     (127)    37365 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-23 18:45:43.000000 lightning-app-2.2.3/src/lightning_app/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-04-23 18:45:43.000000 lightning-app-2.2.3/src/lightning_app/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-23 18:45:43.000000 lightning-app-2.2.3/src/lightning_app/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-23 18:45:43.000000 lightning-app-2.2.3/src/lightning_app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-04-23 18:45:43.000000 lightning-app-2.2.3/src/lightning_app/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-23 18:45:43.000000 lightning-app-2.2.3/src/lightning_app/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.711478 lightning-app-2.2.3/src/lightning_app/api/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/api/http_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/api/request_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.711478 lightning-app-2.2.3/src/lightning_app/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.715478 lightning-app-2.2.3/src/lightning_app/cli/app-template/
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.715478 lightning-app-2.2.3/src/lightning_app/cli/app-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/placeholdername/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.699478 lightning-app-2.2.3/src/lightning_app/cli/app-template/placeholdername/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.715478 lightning-app-2.2.3/src/lightning_app/cli/app-template/placeholdername/components/component_a/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/placeholdername/components/component_a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/placeholdername/components/component_a/component_a.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.715478 lightning-app-2.2.3/src/lightning_app/cli/app-template/placeholdername/components/component_b/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/placeholdername/components/component_b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/placeholdername/components/component_b/component_a.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.715478 lightning-app-2.2.3/src/lightning_app/cli/app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/cmd_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    21517 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/cmd_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/cmd_pl_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/cmd_react_ui_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.715478 lightning-app-2.2.3/src/lightning_app/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/commands/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/commands/cd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/commands/cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/commands/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/commands/ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/commands/pwd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/commands/rm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.719478 lightning-app-2.2.3/src/lightning_app/cli/component-template/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.699478 lightning-app-2.2.3/src/lightning_app/cli/component-template/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.719478 lightning-app-2.2.3/src/lightning_app/cli/component-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/component-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/component-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/component-template/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/component-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.719478 lightning-app-2.2.3/src/lightning_app/cli/component-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/component-template/placeholdername/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/component-template/placeholdername/component.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/component-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/component-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.719478 lightning-app-2.2.3/src/lightning_app/cli/component-template/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/component-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/component-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/component-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/component-template/tests/test_placeholdername_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.719478 lightning-app-2.2.3/src/lightning_app/cli/connect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/connect/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/connect/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/lightning_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/lightning_cli_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/lightning_cli_launch.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/lightning_cli_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.719478 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/.lightningignore
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.719478 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.719478 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/components/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.719478 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/components/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/components/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.719478 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/components/script_runner/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/components/script_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.719478 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.723478 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/tests/test_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.723478 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/craco.config.js
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.723478 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/public/
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/public/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.723478 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/App.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.723478 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.727478 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/index.tsx
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/lightning-colors.ts
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/react-app-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/reportWebVitals.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.727478 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.727478 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/example_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.727478 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.727478 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/App.css
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/App.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.727478 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/main.tsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.727478 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/vite-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/tsconfig.node.json
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/vite.config.ts
--rw-r--r--   0 runner    (1001) docker     (127)    62319 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.727478 lightning-app-2.2.3/src/lightning_app/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.727478 lightning-app-2.2.3/src/lightning_app/components/database/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/database/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/database/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/database/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.731478 lightning-app-2.2.3/src/lightning_app/components/multi_node/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/multi_node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/multi_node/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/multi_node/fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/multi_node/pytorch_spawn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/multi_node/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.731478 lightning-app-2.2.3/src/lightning_app/components/python/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/python/popen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/python/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.731478 lightning-app-2.2.3/src/lightning_app/components/serve/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30437 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/serve/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)    20105 2024-04-23 18:46:03.000000 lightning-app-2.2.3/src/lightning_app/components/serve/catimage.png
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/serve/cold_start_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/serve/gradio_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/serve/python_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/serve/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/serve/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.731478 lightning-app-2.2.3/src/lightning_app/components/serve/types/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/serve/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/serve/types/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/serve/types/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/components/training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.731478 lightning-app-2.2.3/src/lightning_app/core/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/core/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29931 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/core/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    33041 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    21814 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/core/queues.py
--rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/core/work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.735478 lightning-app-2.2.3/src/lightning_app/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/frontend/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.735478 lightning-app-2.2.3/src/lightning_app/frontend/just_py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/frontend/just_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/frontend/just_py/just_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/frontend/just_py/just_py_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.735478 lightning-app-2.2.3/src/lightning_app/frontend/panel/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/frontend/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/frontend/panel/app_state_comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/frontend/panel/app_state_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/frontend/panel/panel_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/frontend/panel/panel_serve_render_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/frontend/stream_lit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/frontend/streamlit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/frontend/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/frontend/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.735478 lightning-app-2.2.3/src/lightning_app/launcher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15316 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/launcher/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    21529 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/launcher/lightning_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/launcher/lightning_hybrid_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.735478 lightning-app-2.2.3/src/lightning_app/pdb/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/pdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/pdb/pdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.735478 lightning-app-2.2.3/src/lightning_app/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:45:43.000000 lightning-app-2.2.3/src/lightning_app/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.739478 lightning-app-2.2.3/src/lightning_app/runners/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.739478 lightning-app-2.2.3/src/lightning_app/runners/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/runners/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/runners/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/runners/backends/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/runners/backends/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/runners/backends/mp_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    47781 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/runners/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/runners/multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/runners/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/runners/runtime_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.739478 lightning-app-2.2.3/src/lightning_app/source_code/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/source_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/source_code/copytree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/source_code/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/source_code/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/source_code/tar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/source_code/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.739478 lightning-app-2.2.3/src/lightning_app/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/storage/copier.py
--rw-r--r--   0 runner    (1001) docker     (127)    13120 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/storage/drive.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/storage/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/storage/mount.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/storage/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18334 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/storage/path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10975 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/storage/payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/storage/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.739478 lightning-app-2.2.3/src/lightning_app/structures/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/structures/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/structures/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.743478 lightning-app-2.2.3/src/lightning_app/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/testing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19345 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/testing/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.743478 lightning-app-2.2.3/src/lightning_app/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.743478 lightning-app-2.2.3/src/lightning_app/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.743478 lightning-app-2.2.3/src/lightning_app/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/css/main.fb7060be.css
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/css/main.fb7060be.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.743478 lightning-app-2.2.3/src/lightning_app/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/js/787.418637a8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10281 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   503634 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/js/main.c1f02aeb.js
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/js/main.c1f02aeb.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2068175 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/js/main.c1f02aeb.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/lightningState.js
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.751478 lightning-app-2.2.3/src/lightning_app/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/static/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-26 19:57:09.000000 lightning-app-2.2.3/src/lightning_app/ui/version.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.755478 lightning-app-2.2.3/src/lightning_app/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/app_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/app_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/app_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/cli_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.755478 lightning-app-2.2.3/src/lightning_app/utilities/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/dependency_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10724 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/load_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/log_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/logs_socket_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    60256 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.755478 lightning-app-2.2.3/src/lightning_app/utilities/packaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/packaging/app_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/packaging/build_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/packaging/cloud_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/packaging/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/packaging/lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/packaging/tarfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/port.py
--rw-r--r--   0 runner    (1001) docker     (127)    30254 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/safe_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-23 18:46:04.000000 lightning-app-2.2.3/src/lightning_app/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 18:45:43.000000 lightning-app-2.2.3/src/lightning_app/version.info
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:46:05.711478 lightning-app-2.2.3/src/lightning_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-23 18:46:05.000000 lightning-app-2.2.3/src/lightning_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13777 2024-04-23 18:46:05.000000 lightning-app-2.2.3/src/lightning_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:46:05.000000 lightning-app-2.2.3/src/lightning_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-23 18:46:05.000000 lightning-app-2.2.3/src/lightning_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:46:05.000000 lightning-app-2.2.3/src/lightning_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-23 18:46:05.000000 lightning-app-2.2.3/src/lightning_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 18:46:05.000000 lightning-app-2.2.3/src/lightning_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 18:45:43.000000 lightning-app-2.2.3/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.791739 lightning-app-2.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.743739 lightning-app-2.2.4/.actions/
+-rw-r--r--   0 runner    (1001) docker     (127)    20994 2024-05-01 22:51:36.000000 lightning-app-2.2.4/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-01 22:51:36.000000 lightning-app-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-05-01 22:51:54.791739 lightning-app-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-05-01 22:51:36.000000 lightning-app-2.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-01 22:51:36.000000 lightning-app-2.2.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.735738 lightning-app-2.2.4/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.743739 lightning-app-2.2.4/requirements/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-01 22:51:36.000000 lightning-app-2.2.4/requirements/app/app.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-01 22:51:36.000000 lightning-app-2.2.4/requirements/app/cloud.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-01 22:51:36.000000 lightning-app-2.2.4/requirements/app/components.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 22:51:36.000000 lightning-app-2.2.4/requirements/app/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-01 22:51:36.000000 lightning-app-2.2.4/requirements/app/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:36.000000 lightning-app-2.2.4/requirements/app/ui.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 22:51:54.791739 lightning-app-2.2.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7935 2024-05-01 22:51:36.000000 lightning-app-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.743739 lightning-app-2.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.743739 lightning-app-2.2.4/src/lightning_app/
+-rw-r--r--   0 runner    (1001) docker     (127)    37521 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-01 22:51:36.000000 lightning-app-2.2.4/src/lightning_app/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-05-01 22:51:36.000000 lightning-app-2.2.4/src/lightning_app/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-01 22:51:36.000000 lightning-app-2.2.4/src/lightning_app/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-01 22:51:36.000000 lightning-app-2.2.4/src/lightning_app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-05-01 22:51:36.000000 lightning-app-2.2.4/src/lightning_app/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-01 22:51:36.000000 lightning-app-2.2.4/src/lightning_app/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.747738 lightning-app-2.2.4/src/lightning_app/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/api/http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/api/request_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.747738 lightning-app-2.2.4/src/lightning_app/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.747738 lightning-app-2.2.4/src/lightning_app/cli/app-template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.747738 lightning-app-2.2.4/src/lightning_app/cli/app-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/placeholdername/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.735738 lightning-app-2.2.4/src/lightning_app/cli/app-template/placeholdername/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.747738 lightning-app-2.2.4/src/lightning_app/cli/app-template/placeholdername/components/component_a/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/placeholdername/components/component_a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/placeholdername/components/component_a/component_a.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.751738 lightning-app-2.2.4/src/lightning_app/cli/app-template/placeholdername/components/component_b/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/placeholdername/components/component_b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/placeholdername/components/component_b/component_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.751738 lightning-app-2.2.4/src/lightning_app/cli/app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/cmd_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21517 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/cmd_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/cmd_pl_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/cmd_react_ui_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.751738 lightning-app-2.2.4/src/lightning_app/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/commands/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/commands/cd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12590 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/commands/cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/commands/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/commands/ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/commands/pwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/commands/rm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.751738 lightning-app-2.2.4/src/lightning_app/cli/component-template/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.735738 lightning-app-2.2.4/src/lightning_app/cli/component-template/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.751738 lightning-app-2.2.4/src/lightning_app/cli/component-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/component-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/component-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/component-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/component-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.751738 lightning-app-2.2.4/src/lightning_app/cli/component-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/component-template/placeholdername/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/component-template/placeholdername/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/component-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/component-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.751738 lightning-app-2.2.4/src/lightning_app/cli/component-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/component-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/component-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/component-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/component-template/tests/test_placeholdername_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.755738 lightning-app-2.2.4/src/lightning_app/cli/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14428 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/connect/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/connect/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/lightning_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/lightning_cli_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/lightning_cli_launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/lightning_cli_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.755738 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/.lightningignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.755738 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.755738 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.755738 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/components/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/components/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.755738 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/components/script_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/components/script_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.755738 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.755738 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.755738 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/craco.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.759739 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/public/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.759739 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/App.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.759739 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.759739 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/lightning-colors.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/react-app-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/reportWebVitals.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.759739 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.759739 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/example_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.763738 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.763738 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/App.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.763738 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/main.tsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.763738 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/vite-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/tsconfig.node.json
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/vite.config.ts
+-rw-r--r--   0 runner    (1001) docker     (127)    62319 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.763738 lightning-app-2.2.4/src/lightning_app/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.763738 lightning-app-2.2.4/src/lightning_app/components/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/database/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/database/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/database/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.763738 lightning-app-2.2.4/src/lightning_app/components/multi_node/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/multi_node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/multi_node/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/multi_node/fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/multi_node/pytorch_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/multi_node/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.763738 lightning-app-2.2.4/src/lightning_app/components/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/python/popen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/python/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.767738 lightning-app-2.2.4/src/lightning_app/components/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30437 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/serve/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20105 2024-05-01 22:51:52.000000 lightning-app-2.2.4/src/lightning_app/components/serve/catimage.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/serve/cold_start_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/serve/gradio_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/serve/python_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/serve/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/serve/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.767738 lightning-app-2.2.4/src/lightning_app/components/serve/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/serve/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/serve/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/serve/types/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/components/training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.767738 lightning-app-2.2.4/src/lightning_app/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29931 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33041 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21814 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/core/queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/core/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.767738 lightning-app-2.2.4/src/lightning_app/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/frontend/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.771739 lightning-app-2.2.4/src/lightning_app/frontend/just_py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/frontend/just_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/frontend/just_py/just_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/frontend/just_py/just_py_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.771739 lightning-app-2.2.4/src/lightning_app/frontend/panel/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/frontend/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/frontend/panel/app_state_comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/frontend/panel/app_state_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/frontend/panel/panel_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/frontend/panel/panel_serve_render_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/frontend/stream_lit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/frontend/streamlit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/frontend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/frontend/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.771739 lightning-app-2.2.4/src/lightning_app/launcher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15316 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/launcher/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21529 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/launcher/lightning_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/launcher/lightning_hybrid_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.771739 lightning-app-2.2.4/src/lightning_app/pdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/pdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/pdb/pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.771739 lightning-app-2.2.4/src/lightning_app/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:36.000000 lightning-app-2.2.4/src/lightning_app/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.771739 lightning-app-2.2.4/src/lightning_app/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.771739 lightning-app-2.2.4/src/lightning_app/runners/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/runners/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/runners/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/runners/backends/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/runners/backends/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/runners/backends/mp_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47781 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/runners/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/runners/multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/runners/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/runners/runtime_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.775739 lightning-app-2.2.4/src/lightning_app/source_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/source_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/source_code/copytree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/source_code/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/source_code/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/source_code/tar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/source_code/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.775739 lightning-app-2.2.4/src/lightning_app/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/storage/copier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13120 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/storage/drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/storage/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/storage/mount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/storage/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18334 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/storage/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10975 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/storage/payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/storage/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.775739 lightning-app-2.2.4/src/lightning_app/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/structures/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-05-01 22:51:53.000000 lightning-app-2.2.4/src/lightning_app/structures/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.775739 lightning-app-2.2.4/src/lightning_app/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/testing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19345 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/testing/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.775739 lightning-app-2.2.4/src/lightning_app/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.779739 lightning-app-2.2.4/src/lightning_app/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.779739 lightning-app-2.2.4/src/lightning_app/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/css/main.fb7060be.css
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/css/main.fb7060be.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.779739 lightning-app-2.2.4/src/lightning_app/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/js/787.418637a8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   503634 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/js/main.c1f02aeb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/js/main.c1f02aeb.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2068175 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/js/main.c1f02aeb.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/lightningState.js
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.783738 lightning-app-2.2.4/src/lightning_app/ui/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/static/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-26 19:57:09.000000 lightning-app-2.2.4/src/lightning_app/ui/version.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.791739 lightning-app-2.2.4/src/lightning_app/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/app_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/app_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/app_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13146 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/cli_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.791739 lightning-app-2.2.4/src/lightning_app/utilities/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11195 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/dependency_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10724 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/load_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/logs_socket_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60256 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.791739 lightning-app-2.2.4/src/lightning_app/utilities/packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/packaging/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/packaging/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/packaging/cloud_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/packaging/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/packaging/lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/packaging/tarfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30254 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/safe_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12600 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 22:51:36.000000 lightning-app-2.2.4/src/lightning_app/version.info
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:51:54.747738 lightning-app-2.2.4/src/lightning_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13777 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 22:51:54.000000 lightning-app-2.2.4/src/lightning_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 22:51:36.000000 lightning-app-2.2.4/src/version.info
```

### Comparing `lightning-app-2.2.3/.actions/assistant.py` & `lightning-app-2.2.4/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/LICENSE` & `lightning-app-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/PKG-INFO` & `lightning-app-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-app
-Version: 2.2.3
+Version: 2.2.4
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightning-app Version: 2.2.3 Summary: Use Lightning
+Metadata-Version: 2.1 Name: lightning-app Version: 2.2.4 Summary: Use Lightning
 Apps to build everything from production-ready, multi-cloud ML systems to
 simple research demos. Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai License:
 Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning Project-URL:
 Bug Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
 Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
 https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
```

### Comparing `lightning-app-2.2.3/README.md` & `lightning-app-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/pyproject.toml` & `lightning-app-2.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/requirements/app/app.txt` & `lightning-app-2.2.4/requirements/app/app.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-lightning-cloud == 0.5.67  # Must be pinned to ensure compatibility
+lightning-cloud == 0.5.68  # Must be pinned to ensure compatibility
 packaging
 typing-extensions >=4.4.0, <4.10.0
 deepdiff >=5.7.0, <6.6.0
 fsspec[http] >=2022.5.0, <2023.11.0
 croniter >=1.3.0, <1.5.0  # strict; TODO: for now until we find something more robust.
 traitlets >=5.3.0, <5.12.0
 arrow >=1.2.0, <1.3.0
```

### Comparing `lightning-app-2.2.3/setup.py` & `lightning-app-2.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/CHANGELOG.md` & `lightning-app-2.2.4/src/lightning_app/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
+
+## [2.2.4] - 2024-05-02
+
+## Fixed
+
+- Fixed HTTPClient retry for flow/work queue ([#19837](https://github.com/Lightning-AI/pytorch-lightning/pull/19837))
+
+
 ## [2.2.0] - 2024-02-09
 
 ## Changed
 
 - Renames the `lightning` cli to `lightning_app` ([#19440](https://github.com/Lightning-AI/pytorch-lightning/pull/19440))
```

### Comparing `lightning-app-2.2.3/src/lightning_app/README.md` & `lightning-app-2.2.4/src/lightning_app/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/__about__.py` & `lightning-app-2.2.4/src/lightning_app/__about__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/__init__.py` & `lightning-app-2.2.4/src/lightning_app/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/__setup__.py` & `lightning-app-2.2.4/src/lightning_app/__setup__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/api/http_methods.py` & `lightning-app-2.2.4/src/lightning_app/api/http_methods.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/api/request_types.py` & `lightning-app-2.2.4/src/lightning_app/api/request_types.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/app-template/.gitignore` & `lightning-app-2.2.4/src/lightning_app/cli/app-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/app-template/LICENSE` & `lightning-app-2.2.4/src/lightning_app/cli/app-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/app-template/README.md` & `lightning-app-2.2.4/src/lightning_app/cli/app-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py` & `lightning-app-2.2.4/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/cmd_apps.py` & `lightning-app-2.2.4/src/lightning_app/cli/cmd_apps.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/cmd_init.py` & `lightning-app-2.2.4/src/lightning_app/cli/cmd_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/cmd_install.py` & `lightning-app-2.2.4/src/lightning_app/cli/cmd_install.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/cmd_pl_init.py` & `lightning-app-2.2.4/src/lightning_app/cli/cmd_pl_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/cmd_react_ui_init.py` & `lightning-app-2.2.4/src/lightning_app/cli/cmd_react_ui_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/commands/app_commands.py` & `lightning-app-2.2.4/src/lightning_app/cli/commands/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/commands/cd.py` & `lightning-app-2.2.4/src/lightning_app/cli/commands/cd.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/commands/cp.py` & `lightning-app-2.2.4/src/lightning_app/cli/commands/cp.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/commands/logs.py` & `lightning-app-2.2.4/src/lightning_app/cli/commands/logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/commands/ls.py` & `lightning-app-2.2.4/src/lightning_app/cli/commands/ls.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/commands/pwd.py` & `lightning-app-2.2.4/src/lightning_app/cli/commands/pwd.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/commands/rm.py` & `lightning-app-2.2.4/src/lightning_app/cli/commands/rm.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml` & `lightning-app-2.2.4/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/component-template/.gitignore` & `lightning-app-2.2.4/src/lightning_app/cli/component-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/component-template/LICENSE` & `lightning-app-2.2.4/src/lightning_app/cli/component-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/component-template/README.md` & `lightning-app-2.2.4/src/lightning_app/cli/component-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/connect/app.py` & `lightning-app-2.2.4/src/lightning_app/cli/connect/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/connect/data.py` & `lightning-app-2.2.4/src/lightning_app/cli/connect/data.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/core.py` & `lightning-app-2.2.4/src/lightning_app/cli/core.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/lightning_cli.py` & `lightning-app-2.2.4/src/lightning_app/cli/lightning_cli.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/lightning_cli_delete.py` & `lightning-app-2.2.4/src/lightning_app/cli/lightning_cli_delete.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/lightning_cli_launch.py` & `lightning-app-2.2.4/src/lightning_app/cli/lightning_cli_launch.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/lightning_cli_list.py` & `lightning-app-2.2.4/src/lightning_app/cli/lightning_cli_list.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/app.py` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/callbacks.py` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/core/state.py` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/core/state.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/setup.py` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/.prettierrc` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/.prettierrc`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/craco.config.js` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/craco.config.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/package.json` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/public/index.html` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/public/index.html`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/App.tsx` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/index.tsx` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/index.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/pl-app-template/ui/tsconfig.json` & `lightning-app-2.2.4/src/lightning_app/cli/pl-app-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/README.md` & `lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/example_app.py` & `lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/example_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/package.json` & `lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/App.tsx` & `lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg` & `lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts` & `lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts` & `lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/tsconfig.json` & `lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/cli/react-ui-template/ui/yarn.lock` & `lightning-app-2.2.4/src/lightning_app/cli/react-ui-template/ui/yarn.lock`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/__init__.py` & `lightning-app-2.2.4/src/lightning_app/components/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/database/client.py` & `lightning-app-2.2.4/src/lightning_app/components/database/client.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/database/server.py` & `lightning-app-2.2.4/src/lightning_app/components/database/server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/database/utilities.py` & `lightning-app-2.2.4/src/lightning_app/components/database/utilities.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/multi_node/base.py` & `lightning-app-2.2.4/src/lightning_app/components/multi_node/base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/multi_node/fabric.py` & `lightning-app-2.2.4/src/lightning_app/components/multi_node/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/multi_node/pytorch_spawn.py` & `lightning-app-2.2.4/src/lightning_app/components/multi_node/pytorch_spawn.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/multi_node/trainer.py` & `lightning-app-2.2.4/src/lightning_app/components/multi_node/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/python/popen.py` & `lightning-app-2.2.4/src/lightning_app/components/python/popen.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/python/tracer.py` & `lightning-app-2.2.4/src/lightning_app/components/python/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/serve/__init__.py` & `lightning-app-2.2.4/src/lightning_app/components/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/serve/auto_scaler.py` & `lightning-app-2.2.4/src/lightning_app/components/serve/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/serve/catimage.png` & `lightning-app-2.2.4/src/lightning_app/components/serve/catimage.png`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/serve/cold_start_proxy.py` & `lightning-app-2.2.4/src/lightning_app/components/serve/cold_start_proxy.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/serve/gradio_server.py` & `lightning-app-2.2.4/src/lightning_app/components/serve/gradio_server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/serve/python_server.py` & `lightning-app-2.2.4/src/lightning_app/components/serve/python_server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/serve/serve.py` & `lightning-app-2.2.4/src/lightning_app/components/serve/serve.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/serve/streamlit.py` & `lightning-app-2.2.4/src/lightning_app/components/serve/streamlit.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/serve/types/image.py` & `lightning-app-2.2.4/src/lightning_app/components/serve/types/image.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/serve/types/type.py` & `lightning-app-2.2.4/src/lightning_app/components/serve/types/type.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/components/training.py` & `lightning-app-2.2.4/src/lightning_app/components/training.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/core/api.py` & `lightning-app-2.2.4/src/lightning_app/core/api.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/core/app.py` & `lightning-app-2.2.4/src/lightning_app/core/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/core/constants.py` & `lightning-app-2.2.4/src/lightning_app/core/constants.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/core/flow.py` & `lightning-app-2.2.4/src/lightning_app/core/flow.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/core/queues.py` & `lightning-app-2.2.4/src/lightning_app/core/queues.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/core/work.py` & `lightning-app-2.2.4/src/lightning_app/core/work.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/frontend/frontend.py` & `lightning-app-2.2.4/src/lightning_app/frontend/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/frontend/just_py/just_py.py` & `lightning-app-2.2.4/src/lightning_app/frontend/just_py/just_py.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/frontend/just_py/just_py_base.py` & `lightning-app-2.2.4/src/lightning_app/frontend/just_py/just_py_base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/frontend/panel/app_state_comm.py` & `lightning-app-2.2.4/src/lightning_app/frontend/panel/app_state_comm.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/frontend/panel/app_state_watcher.py` & `lightning-app-2.2.4/src/lightning_app/frontend/panel/app_state_watcher.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/frontend/panel/panel_frontend.py` & `lightning-app-2.2.4/src/lightning_app/frontend/panel/panel_frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/frontend/panel/panel_serve_render_fn.py` & `lightning-app-2.2.4/src/lightning_app/frontend/panel/panel_serve_render_fn.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/frontend/stream_lit.py` & `lightning-app-2.2.4/src/lightning_app/frontend/stream_lit.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/frontend/streamlit_base.py` & `lightning-app-2.2.4/src/lightning_app/frontend/streamlit_base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/frontend/utils.py` & `lightning-app-2.2.4/src/lightning_app/frontend/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/frontend/web.py` & `lightning-app-2.2.4/src/lightning_app/frontend/web.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/launcher/launcher.py` & `lightning-app-2.2.4/src/lightning_app/launcher/launcher.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/launcher/lightning_backend.py` & `lightning-app-2.2.4/src/lightning_app/launcher/lightning_backend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/launcher/lightning_hybrid_backend.py` & `lightning-app-2.2.4/src/lightning_app/launcher/lightning_hybrid_backend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/pdb/pdb.py` & `lightning-app-2.2.4/src/lightning_app/pdb/pdb.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/plugin/plugin.py` & `lightning-app-2.2.4/src/lightning_app/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/runners/backends/__init__.py` & `lightning-app-2.2.4/src/lightning_app/runners/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/runners/backends/backend.py` & `lightning-app-2.2.4/src/lightning_app/runners/backends/backend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/runners/backends/cloud.py` & `lightning-app-2.2.4/src/lightning_app/runners/backends/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/runners/backends/docker.py` & `lightning-app-2.2.4/src/lightning_app/runners/backends/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/runners/backends/mp_process.py` & `lightning-app-2.2.4/src/lightning_app/runners/backends/mp_process.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/runners/cloud.py` & `lightning-app-2.2.4/src/lightning_app/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/runners/multiprocess.py` & `lightning-app-2.2.4/src/lightning_app/runners/multiprocess.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/runners/runtime.py` & `lightning-app-2.2.4/src/lightning_app/runners/runtime.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/runners/runtime_type.py` & `lightning-app-2.2.4/src/lightning_app/runners/runtime_type.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/source_code/copytree.py` & `lightning-app-2.2.4/src/lightning_app/source_code/copytree.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/source_code/hashing.py` & `lightning-app-2.2.4/src/lightning_app/source_code/hashing.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/source_code/local.py` & `lightning-app-2.2.4/src/lightning_app/source_code/local.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/source_code/tar.py` & `lightning-app-2.2.4/src/lightning_app/source_code/tar.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/source_code/uploader.py` & `lightning-app-2.2.4/src/lightning_app/source_code/uploader.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/storage/copier.py` & `lightning-app-2.2.4/src/lightning_app/storage/copier.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/storage/drive.py` & `lightning-app-2.2.4/src/lightning_app/storage/drive.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/storage/filesystem.py` & `lightning-app-2.2.4/src/lightning_app/storage/filesystem.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/storage/mount.py` & `lightning-app-2.2.4/src/lightning_app/storage/mount.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/storage/orchestrator.py` & `lightning-app-2.2.4/src/lightning_app/storage/orchestrator.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/storage/path.py` & `lightning-app-2.2.4/src/lightning_app/storage/path.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/storage/payload.py` & `lightning-app-2.2.4/src/lightning_app/storage/payload.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/storage/requests.py` & `lightning-app-2.2.4/src/lightning_app/storage/requests.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/structures/dict.py` & `lightning-app-2.2.4/src/lightning_app/structures/dict.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/structures/list.py` & `lightning-app-2.2.4/src/lightning_app/structures/list.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/testing/config.py` & `lightning-app-2.2.4/src/lightning_app/testing/config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/testing/helpers.py` & `lightning-app-2.2.4/src/lightning_app/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/testing/testing.py` & `lightning-app-2.2.4/src/lightning_app/testing/testing.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/ui/asset-manifest.json` & `lightning-app-2.2.4/src/lightning_app/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/ui/index.html` & `lightning-app-2.2.4/src/lightning_app/ui/index.html`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/ui/static/css/main.fb7060be.css` & `lightning-app-2.2.4/src/lightning_app/ui/static/css/main.fb7060be.css`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/ui/static/css/main.fb7060be.css.map` & `lightning-app-2.2.4/src/lightning_app/ui/static/css/main.fb7060be.css.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/ui/static/favicon.ico` & `lightning-app-2.2.4/src/lightning_app/ui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/ui/static/js/787.418637a8.chunk.js` & `lightning-app-2.2.4/src/lightning_app/ui/static/js/787.418637a8.chunk.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map` & `lightning-app-2.2.4/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/ui/static/js/main.c1f02aeb.js` & `lightning-app-2.2.4/src/lightning_app/ui/static/js/main.c1f02aeb.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/ui/static/js/main.c1f02aeb.js.LICENSE.txt` & `lightning-app-2.2.4/src/lightning_app/ui/static/js/main.c1f02aeb.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/ui/static/js/main.c1f02aeb.js.map` & `lightning-app-2.2.4/src/lightning_app/ui/static/js/main.c1f02aeb.js.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/ui/static/lightningState.js` & `lightning-app-2.2.4/src/lightning_app/ui/static/lightningState.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg` & `lightning-app-2.2.4/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg` & `lightning-app-2.2.4/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/app_commands.py` & `lightning-app-2.2.4/src/lightning_app/utilities/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/app_helpers.py` & `lightning-app-2.2.4/src/lightning_app/utilities/app_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/app_logs.py` & `lightning-app-2.2.4/src/lightning_app/utilities/app_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/app_status.py` & `lightning-app-2.2.4/src/lightning_app/utilities/app_status.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/auth.py` & `lightning-app-2.2.4/src/lightning_app/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/cli_helpers.py` & `lightning-app-2.2.4/src/lightning_app/utilities/cli_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/cloud.py` & `lightning-app-2.2.4/src/lightning_app/utilities/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/clusters.py` & `lightning-app-2.2.4/src/lightning_app/utilities/clusters.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/commands/base.py` & `lightning-app-2.2.4/src/lightning_app/utilities/commands/base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/component.py` & `lightning-app-2.2.4/src/lightning_app/utilities/component.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/data_structures.py` & `lightning-app-2.2.4/src/lightning_app/utilities/data_structures.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/dependency_caching.py` & `lightning-app-2.2.4/src/lightning_app/utilities/dependency_caching.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/enum.py` & `lightning-app-2.2.4/src/lightning_app/utilities/enum.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/exceptions.py` & `lightning-app-2.2.4/src/lightning_app/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/frontend.py` & `lightning-app-2.2.4/src/lightning_app/utilities/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/git.py` & `lightning-app-2.2.4/src/lightning_app/utilities/git.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/imports.py` & `lightning-app-2.2.4/src/lightning_app/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/introspection.py` & `lightning-app-2.2.4/src/lightning_app/utilities/introspection.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/layout.py` & `lightning-app-2.2.4/src/lightning_app/utilities/layout.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/load_app.py` & `lightning-app-2.2.4/src/lightning_app/utilities/load_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/log.py` & `lightning-app-2.2.4/src/lightning_app/utilities/log.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/log_helpers.py` & `lightning-app-2.2.4/src/lightning_app/utilities/log_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/login.py` & `lightning-app-2.2.4/src/lightning_app/utilities/login.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/logs_socket_api.py` & `lightning-app-2.2.4/src/lightning_app/utilities/logs_socket_api.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/name_generator.py` & `lightning-app-2.2.4/src/lightning_app/utilities/name_generator.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/network.py` & `lightning-app-2.2.4/src/lightning_app/utilities/network.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,26 +85,40 @@
 
 
 _CONNECTION_RETRY_TOTAL = 2880
 _CONNECTION_RETRY_BACKOFF_FACTOR = 0.5
 _DEFAULT_REQUEST_TIMEOUT = 30  # seconds
 
 
+def create_retry_strategy():
+    return Retry(
+        # wait time between retries increases exponentially according to: backoff_factor * (2 ** (retry - 1))
+        # but the the maximum wait time is 120 secs. By setting a large value (2880), we'll make sure clients
+        # are going to be alive for a very long time (~ 4 days) but retries every 120 seconds
+        total=_CONNECTION_RETRY_TOTAL,
+        backoff_factor=_CONNECTION_RETRY_BACKOFF_FACTOR,
+        status_forcelist={
+            408,  # Request Timeout
+            429,  # Too Many Requests
+            *range(500, 600),  # Any 5xx Server Error status
+        },
+        allowed_methods={
+            "POST",  # Default methods are idempotent, add POST here
+            *Retry.DEFAULT_ALLOWED_METHODS,
+        },
+    )
+
+
 def _configure_session() -> Session:
     """Configures the session for GET and POST requests.
 
     It enables a generous retrial strategy that waits for the application server to connect.
 
     """
-    retry_strategy = Retry(
-        # wait time between retries increases exponentially according to: backoff_factor * (2 ** (retry - 1))
-        total=_CONNECTION_RETRY_TOTAL,
-        backoff_factor=_CONNECTION_RETRY_BACKOFF_FACTOR,
-        status_forcelist=[429, 500, 502, 503, 504],
-    )
+    retry_strategy = create_retry_strategy()
     adapter = HTTPAdapter(max_retries=retry_strategy)
     http = requests.Session()
     http.mount("https://", adapter)
     http.mount("http://", adapter)
     return http
 
 
@@ -153,29 +167,15 @@
     """A wrapper class around the requests library which handles chores like logging, retries, and timeouts
     automatically."""
 
     def __init__(
         self, base_url: str, auth_token: Optional[str] = None, log_callback: Optional[Callable] = None
     ) -> None:
         self.base_url = base_url
-        retry_strategy = Retry(
-            # wait time between retries increases exponentially according to: backoff_factor * (2 ** (retry - 1))
-            # but the the maximum wait time is 120 secs. By setting a large value (2880), we'll make sure clients
-            # are going to be alive for a very long time (~ 4 days) but retries every 120 seconds
-            total=_CONNECTION_RETRY_TOTAL,
-            backoff_factor=_CONNECTION_RETRY_BACKOFF_FACTOR,
-            status_forcelist=[
-                408,  # Request Timeout
-                429,  # Too Many Requests
-                500,  # Internal Server Error
-                502,  # Bad Gateway
-                503,  # Service Unavailable
-                504,  # Gateway Timeout
-            ],
-        )
+        retry_strategy = create_retry_strategy()
         adapter = CustomRetryAdapter(max_retries=retry_strategy, timeout=_DEFAULT_REQUEST_TIMEOUT)
         self.session = requests.Session()
 
         self.session.hooks = {"response": _response}
 
         self.session.mount("http://", adapter)
         self.session.mount("https://", adapter)
```

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/openapi.py` & `lightning-app-2.2.4/src/lightning_app/utilities/openapi.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/packaging/app_config.py` & `lightning-app-2.2.4/src/lightning_app/utilities/packaging/app_config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/packaging/build_config.py` & `lightning-app-2.2.4/src/lightning_app/utilities/packaging/build_config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/packaging/cloud_compute.py` & `lightning-app-2.2.4/src/lightning_app/utilities/packaging/cloud_compute.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/packaging/docker.py` & `lightning-app-2.2.4/src/lightning_app/utilities/packaging/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/packaging/lightning_utils.py` & `lightning-app-2.2.4/src/lightning_app/utilities/packaging/lightning_utils.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/packaging/tarfile.py` & `lightning-app-2.2.4/src/lightning_app/utilities/packaging/tarfile.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/port.py` & `lightning-app-2.2.4/src/lightning_app/utilities/port.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/proxies.py` & `lightning-app-2.2.4/src/lightning_app/utilities/proxies.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/redis.py` & `lightning-app-2.2.4/src/lightning_app/utilities/redis.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/safe_pickle.py` & `lightning-app-2.2.4/src/lightning_app/utilities/safe_pickle.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/scheduler.py` & `lightning-app-2.2.4/src/lightning_app/utilities/scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/secrets.py` & `lightning-app-2.2.4/src/lightning_app/utilities/secrets.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/state.py` & `lightning-app-2.2.4/src/lightning_app/utilities/state.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/tracer.py` & `lightning-app-2.2.4/src/lightning_app/utilities/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/tree.py` & `lightning-app-2.2.4/src/lightning_app/utilities/tree.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/types.py` & `lightning-app-2.2.4/src/lightning_app/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app/utilities/warnings.py` & `lightning-app-2.2.4/src/lightning_app/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app.egg-info/PKG-INFO` & `lightning-app-2.2.4/src/lightning_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-app
-Version: 2.2.3
+Version: 2.2.4
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightning-app Version: 2.2.3 Summary: Use Lightning
+Metadata-Version: 2.1 Name: lightning-app Version: 2.2.4 Summary: Use Lightning
 Apps to build everything from production-ready, multi-cloud ML systems to
 simple research demos. Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai License:
 Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning Project-URL:
 Bug Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
 Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
 https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
```

### Comparing `lightning-app-2.2.3/src/lightning_app.egg-info/SOURCES.txt` & `lightning-app-2.2.4/src/lightning_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-app-2.2.3/src/lightning_app.egg-info/requires.txt` & `lightning-app-2.2.4/src/lightning_app.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-lightning-cloud==0.5.67
+lightning-cloud==0.5.68
 packaging
 typing-extensions<5.0,>=4.4.0
 deepdiff<7.0,>=5.7.0
 fsspec[http]<2024.0,>=2022.5.0
 croniter<1.5.0,>=1.3.0
 traitlets<6.0,>=5.3.0
 arrow<2.0,>=1.2.0
```

