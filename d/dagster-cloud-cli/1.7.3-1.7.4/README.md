# Comparing `tmp/dagster-cloud-cli-1.7.3.tar.gz` & `tmp/dagster-cloud-cli-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-cli-1.7.3.tar", last modified: Thu Apr 25 20:21:43 2024, max compression
+gzip compressed data, was "dagster-cloud-cli-1.7.4.tar", last modified: Thu May  2 20:44:08 2024, max compression
```

## Comparing `dagster-cloud-cli-1.7.3.tar` & `dagster-cloud-cli-1.7.4.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.449393 dagster-cloud-cli-1.7.3/
--rw-r--r--   0 root         (0) root         (0)      132 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      314 2024-04-25 20:21:43.445393 dagster-cloud-cli-1.7.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.417393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.421393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.421393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/branch_deployment/
--rw-r--r--   0 root         (0) root         (0)     4947 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/branch_deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.425393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/ci/
--rw-r--r--   0 root         (0) root         (0)    30031 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4124 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/ci/checks.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/ci/report.py
--rw-r--r--   0 root         (0) root         (0)     4121 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/ci/state.py
--rw-r--r--   0 root         (0) root         (0)      508 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/ci/utils.py
--rw-r--r--   0 root         (0) root         (0)     8651 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.425393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/deployment/
--rw-r--r--   0 root         (0) root         (0)     2952 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.425393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/deployment/alert_policies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1657 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
--rw-r--r--   0 root         (0) root         (0)    17056 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.425393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/job/
--rw-r--r--   0 root         (0) root         (0)     1926 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4425 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.429393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/organization/
--rw-r--r--   0 root         (0) root         (0)     4001 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.429393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/organization/saml/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/organization/saml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2691 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/organization/saml/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.429393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/run/
--rw-r--r--   0 root         (0) root         (0)      669 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.429393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/serverless/
--rw-r--r--   0 root         (0) root         (0)     1499 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/serverless/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      628 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
--rw-r--r--   0 root         (0) root         (0)    18361 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.429393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/workspace/
--rw-r--r--   0 root         (0) root         (0)    12434 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18301 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/config_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.437393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      901 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/alert_types.py
--rw-r--r--   0 root         (0) root         (0)     4801 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/artifacts.py
--rw-r--r--   0 root         (0) root         (0)     1744 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/docker_runner.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    13677 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.437393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/headers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/headers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/headers/auth.py
--rw-r--r--   0 root         (0) root         (0)      924 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/headers/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.437393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/headers/versioning/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/headers/versioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/headers/versioning/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.441393 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/code_location.py
--rw-r--r--   0 root         (0) root         (0)     9423 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/deploy.py
--rw-r--r--   0 root         (0) root         (0)    14436 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/deps.py
--rw-r--r--   0 root         (0) root         (0)      949 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/git_context.py
--rw-r--r--   0 root         (0) root         (0)     6992 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/github_context.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/gitlab_context.py
--rw-r--r--   0 root         (0) root         (0)     1232 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/parse_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/pex_registry.py
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/selftest.py
--rw-r--r--   0 root         (0) root         (0)     5407 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/source.py
--rw-r--r--   0 root         (0) root         (0)     6220 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/util.py
--rw-r--r--   0 root         (0) root         (0)     2106 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pydantic_yaml.py
--rw-r--r--   0 root         (0) root         (0)     7106 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)     2463 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    20456 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/gql.py
--rw-r--r--   0 root         (0) root         (0)     5859 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/pex_utils.py
--rw-r--r--   0 root         (0) root         (0)     1845 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/types.py
--rw-r--r--   0 root         (0) root         (0)     2804 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/ui.py
--rw-r--r--   0 root         (0) root         (0)     3488 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.421393 dagster-cloud-cli-1.7.3/dagster_cloud_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2024-04-25 20:21:43.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3028 2024-04-25 20:21:43.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:21:43.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-25 20:21:43.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2024-04-25 20:21:43.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-04-25 20:21:43.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:21:43.445393 dagster-cloud-cli-1.7.3/dagster_cloud_cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      189 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli_tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     4130 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli_tests/test_check.py
--rw-r--r--   0 root         (0) root         (0)    16177 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli_tests/test_ci_commands.py
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli_tests/test_deps.py
--rw-r--r--   0 root         (0) root         (0)      683 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli_tests/test_gql.py
--rw-r--r--   0 root         (0) root         (0)     8872 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/dagster_cloud_cli_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 20:21:43.449393 dagster-cloud-cli-1.7.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1139 2024-04-25 20:08:52.000000 dagster-cloud-cli-1.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.818659 dagster-cloud-cli-1.7.4/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-02 20:44:08.818659 dagster-cloud-cli-1.7.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.802659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.806659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.806659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/branch_deployment/
+-rw-r--r--   0 root         (0) root         (0)     5173 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/branch_deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.806659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/
+-rw-r--r--   0 root         (0) root         (0)    30031 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/checks.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/report.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/state.py
+-rw-r--r--   0 root         (0) root         (0)      508 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8651 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.806659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/
+-rw-r--r--   0 root         (0) root         (0)     2952 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.806659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/alert_policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
+-rw-r--r--   0 root         (0) root         (0)    17056 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/job/
+-rw-r--r--   0 root         (0) root         (0)     1926 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/organization/
+-rw-r--r--   0 root         (0) root         (0)     4001 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/organization/saml/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/organization/saml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/organization/saml/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/run/
+-rw-r--r--   0 root         (0) root         (0)      669 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/serverless/
+-rw-r--r--   0 root         (0) root         (0)     1499 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/serverless/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      628 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
+-rw-r--r--   0 root         (0) root         (0)    18361 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/workspace/
+-rw-r--r--   0 root         (0) root         (0)    12434 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18301 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/config_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      901 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/alert_types.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/docker_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    13677 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/auth.py
+-rw-r--r--   0 root         (0) root         (0)      924 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.814659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/versioning/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/versioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/versioning/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.814659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/
+-rw-r--r--   0 root         (0) root         (0)      172 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     9423 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    14436 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/deps.py
+-rw-r--r--   0 root         (0) root         (0)      949 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/git_context.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/github_context.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/gitlab_context.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/parse_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/pex_registry.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/selftest.py
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/source.py
+-rw-r--r--   0 root         (0) root         (0)     6220 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/util.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)     7106 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    20701 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/gql.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/pex_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.806659 dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-02 20:44:08.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3028 2024-05-02 20:44:08.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:44:08.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-02 20:44:08.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2024-05-02 20:44:08.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-02 20:44:08.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.818659 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      189 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     4130 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_check.py
+-rw-r--r--   0 root         (0) root         (0)    16177 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_ci_commands.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_deps.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_gql.py
+-rw-r--r--   0 root         (0) root         (0)     8872 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 20:44:08.818659 dagster-cloud-cli-1.7.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/setup.py
```

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/branch_deployment/__init__.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/branch_deployment/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,14 +78,18 @@
         None, help="The URL for the avatar of the author for the latest commit, if any."
     ),
     read_git_state: bool = typer.Option(
         False,
         is_flag=True,
         help="Whether to commit data (timestamp, hash, author info) from Git state.",
     ),
+    base_deployment_name: str = typer.Option(
+        None,
+        help="The name of the deployment to use as the base deployment for the branch deployment.",
+    ),
 ) -> None:
     """Sets up or updates the branch deployment for the given git branch."""
     if not url and not organization:
         raise ui.error("Must provide either organization name or URL.")
     if not url:
         url = gql.url_from_config(organization=organization)
 
@@ -117,14 +121,15 @@
                 pull_request_url=pull_request_url,
                 pull_request_status=pull_request_status,
                 pull_request_number=pull_request_number,
                 commit_message=commit_message,
                 author_name=author_name,
                 author_email=author_email,
                 author_avatar_url=author_avatar_url,
+                base_deployment_name=base_deployment_name,
             )
         )
 
 
 @app.command(name="delete")
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 def delete(url: str, api_token: str, deployment: str):
```

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/ci/__init__.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/ci/checks.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/checks.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/ci/report.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/report.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/ci/state.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/state.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/config.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/deployment/__init__.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/deployment/alert_policies/commands.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/alert_policies/commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/job/__init__.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/job/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/metrics.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/organization/__init__.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/organization/saml/commands.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/organization/saml/commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/run/__init__.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/serverless/Dockerfile` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/serverless/Dockerfile`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/serverless/__init__.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/commands/workspace/__init__.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/config_utils.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/alert_types.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/alert_types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/artifacts.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/docker_runner.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/docker_runner.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/errors.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/graphql_client.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/graphql_client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/headers/impl.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/code_location.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/deploy.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/deploy.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/deps.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/deps.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/git_context.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/git_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/github_context.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/github_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/gitlab_context.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/gitlab_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/parse_workspace.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/parse_workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/pex_registry.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/pex_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/selftest.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/selftest.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/source.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/source.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pex_builder/util.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/util.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/pydantic_yaml.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pydantic_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/core/workspace.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/docker_utils.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/entrypoint.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/gql.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/gql.py`

 * *Files 2% similar despite different names*

```diff
@@ -454,24 +454,29 @@
     return result["data"]["organizationSettings"]["settings"]
 
 
 CREATE_OR_UPDATE_BRANCH_DEPLOYMENT = """
 mutation CliCreateOrUpdateBranchDeployment(
     $branchData: CreateOrUpdateBranchDeploymentInput!
     $commit: DeploymentCommitInput!
+    $baseDeploymentName: String
 ) {
     createOrUpdateBranchDeployment(
         branchData: $branchData,
-        commit: $commit
+        commit: $commit,
+        baseDeploymentName: $baseDeploymentName,
     ) {
         __typename
         ... on DagsterCloudDeployment {
             deploymentId
             deploymentName
         }
+        ... on PythonError {
+            message
+        }
     }
 }
 """
 
 
 def create_or_update_branch_deployment(
     client: DagsterCloudGraphQLClient,
@@ -484,14 +489,15 @@
     pull_request_status: Optional[str] = None,
     pull_request_number: Optional[str] = None,
     commit_message: Optional[str] = None,
     commit_url: Optional[str] = None,
     author_name: Optional[str] = None,
     author_email: Optional[str] = None,
     author_avatar_url: Optional[str] = None,
+    base_deployment_name: Optional[str] = None,
 ) -> str:
     result = client.execute(
         CREATE_OR_UPDATE_BRANCH_DEPLOYMENT,
         variable_values={
             "branchData": {
                 "repoName": repo_name,
                 "branchName": branch_name,
@@ -505,14 +511,15 @@
                 "timestamp": timestamp,
                 "commitMessage": commit_message,
                 "commitUrl": commit_url,
                 "authorName": author_name,
                 "authorEmail": author_email,
                 "authorAvatarUrl": author_avatar_url,
             },
+            "baseDeploymentName": base_deployment_name,
         },
     )
 
     name = result.get("data", {}).get("createOrUpdateBranchDeployment", {}).get("deploymentName")
     if name is None:
         raise Exception(f"Unable to create or update branch deployment: {result}")
```

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/pex_utils.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/pex_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/types.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/ui.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/ui.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli/utils.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli.egg-info/SOURCES.txt` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli_tests/test_check.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_check.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli_tests/test_ci_commands.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_ci_commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli_tests/test_deps.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli_tests/test_gql.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_gql.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/dagster_cloud_cli_tests/test_metrics.py` & `dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.3/setup.py` & `dagster-cloud-cli-1.7.4/setup.py`

 * *Files identical despite different names*

