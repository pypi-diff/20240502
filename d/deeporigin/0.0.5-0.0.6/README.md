# Comparing `tmp/deeporigin-0.0.5.tar.gz` & `tmp/deeporigin-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeporigin-0.0.5.tar", last modified: Wed May  1 15:12:26 2024, max compression
+gzip compressed data, was "deeporigin-0.0.6.tar", last modified: Wed May  1 19:47:53 2024, max compression
```

## Comparing `deeporigin-0.0.5.tar` & `deeporigin-0.0.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.922603 deeporigin-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-01 15:12:23.000000 deeporigin-0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 15:12:23.000000 deeporigin-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-01 15:12:26.922603 deeporigin-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-01 15:12:23.000000 deeporigin-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.922603 deeporigin-0.0.5/deeporigin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-01 15:12:26.000000 deeporigin-0.0.5/deeporigin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-01 15:12:26.000000 deeporigin-0.0.5/deeporigin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:12:26.000000 deeporigin-0.0.5/deeporigin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 15:12:26.000000 deeporigin-0.0.5/deeporigin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 15:12:26.000000 deeporigin-0.0.5/deeporigin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 15:12:26.000000 deeporigin-0.0.5/deeporigin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-01 15:12:23.000000 deeporigin-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:12:26.922603 deeporigin-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.914602 deeporigin-0.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 15:12:24.000000 deeporigin-0.0.5/src/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.914602 deeporigin-0.0.5/src/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    11909 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/cli/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.914602 deeporigin-0.0.5/src/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/config/default.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/do_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/feature_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.914602 deeporigin-0.0.5/src/managed_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/managed_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/managed_data/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15869 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/managed_data/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/managed_data/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/managed_data/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.918603 deeporigin-0.0.5/src/variables/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/base_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    20324 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.918603 deeporigin-0.0.5/src/variables/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/anthropic_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/aws_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/git_http_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/gurobi_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/mosek_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/open_ai_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/private_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/private_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/secret_env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/secret_env_var_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/secret_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/secret_file_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/variables/types/xpress_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 15:12:23.000000 deeporigin-0.0.5/src/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:12:26.918603 deeporigin-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-01 15:12:23.000000 deeporigin-0.0.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-01 15:12:23.000000 deeporigin-0.0.5/tests/test_cli_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-01 15:12:23.000000 deeporigin-0.0.5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-01 15:12:23.000000 deeporigin-0.0.5/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-01 15:12:23.000000 deeporigin-0.0.5/tests/test_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-05-01 15:12:23.000000 deeporigin-0.0.5/tests/test_managed_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    90063 2024-05-01 15:12:23.000000 deeporigin-0.0.5/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.335903 deeporigin-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-01 19:47:49.000000 deeporigin-0.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 19:47:49.000000 deeporigin-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-01 19:47:53.335903 deeporigin-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-01 19:47:49.000000 deeporigin-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.335903 deeporigin-0.0.6/deeporigin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-01 19:47:53.000000 deeporigin-0.0.6/deeporigin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-01 19:47:53.000000 deeporigin-0.0.6/deeporigin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:47:53.000000 deeporigin-0.0.6/deeporigin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 19:47:53.000000 deeporigin-0.0.6/deeporigin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 19:47:53.000000 deeporigin-0.0.6/deeporigin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 19:47:53.000000 deeporigin-0.0.6/deeporigin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-01 19:47:49.000000 deeporigin-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 19:47:53.335903 deeporigin-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.327903 deeporigin-0.0.6/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 19:47:51.000000 deeporigin-0.0.6/src/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.327903 deeporigin-0.0.6/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/cli/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.327903 deeporigin-0.0.6/src/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/config/default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/do_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/feature_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.331903 deeporigin-0.0.6/src/managed_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/managed_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/managed_data/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15706 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/managed_data/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/managed_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/managed_data/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.331903 deeporigin-0.0.6/src/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/base_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20324 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.335903 deeporigin-0.0.6/src/variables/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/anthropic_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/aws_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/git_http_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/gurobi_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/mosek_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/open_ai_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/private_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/private_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/secret_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/secret_env_var_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/secret_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/secret_file_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/variables/types/xpress_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 19:47:49.000000 deeporigin-0.0.6/src/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:47:53.335903 deeporigin-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-01 19:47:49.000000 deeporigin-0.0.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-01 19:47:49.000000 deeporigin-0.0.6/tests/test_cli_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-05-01 19:47:49.000000 deeporigin-0.0.6/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-01 19:47:49.000000 deeporigin-0.0.6/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-01 19:47:49.000000 deeporigin-0.0.6/tests/test_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-01 19:47:49.000000 deeporigin-0.0.6/tests/test_managed_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90063 2024-05-01 19:47:49.000000 deeporigin-0.0.6/tests/test_variables.py
```

### Comparing `deeporigin-0.0.5/LICENSE.txt` & `deeporigin-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/PKG-INFO` & `deeporigin-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeporigin
-Version: 0.0.5
+Version: 0.0.6
 Summary: Command line tool and Python client for working with Deep Origin
 Author-email: Deep Origin <support@deeporigin.com>
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

### Comparing `deeporigin-0.0.5/README.md` & `deeporigin-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/deeporigin.egg-info/PKG-INFO` & `deeporigin-0.0.6/deeporigin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeporigin
-Version: 0.0.5
+Version: 0.0.6
 Summary: Command line tool and Python client for working with Deep Origin
 Author-email: Deep Origin <support@deeporigin.com>
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

### Comparing `deeporigin-0.0.5/deeporigin.egg-info/SOURCES.txt` & `deeporigin-0.0.6/deeporigin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/pyproject.toml` & `deeporigin-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/__init__.py` & `deeporigin-0.0.6/src/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,14 +25,14 @@
 with open(version_filename, "r") as file:
     __version__ = file.read()
 
     if __version__ == "0.0.0.dev0":
         # in dev mode. we use git to get a "version number"
         # that will change with tags and commits
         process = subprocess.run(
-            ["git", "describe", "--tags"],
+            ["git", "describe", "--tags", "--dirty", "--long"],
             capture_output=True,
             universal_newlines=True,
             cwd=Path(__file__).parent.parent,
         )
         if process.returncode == 0:
             __version__ = process.stdout.strip()
```

### Comparing `deeporigin-0.0.5/src/cli/__init__.py` & `deeporigin-0.0.6/src/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/cli/auth.py` & `deeporigin-0.0.6/src/cli/auth.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/cli/context.py` & `deeporigin-0.0.6/src/cli/context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/cli/data.py` & `deeporigin-0.0.6/src/cli/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,16 @@
     )
     def ls(self):
         """list rows in db"""
 
         tree = api.get_tree(
             client=self._get_client(),
         )
-        _print_tree(tree)
+        for branch in tree:
+            _print_tree(branch)
 
     @cement.ex(
         help="Show column names and values for a given row",
         arguments=[
             (
                 ["row_id"],
                 {"help": "Row ID", "action": "store"},
```

### Comparing `deeporigin-0.0.5/src/cli/variables.py` & `deeporigin-0.0.6/src/cli/variables.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/config/__init__.py` & `deeporigin-0.0.6/src/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/config/default.yml` & `deeporigin-0.0.6/src/config/default.yml`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/context.py` & `deeporigin-0.0.6/src/context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/do_api.py` & `deeporigin-0.0.6/src/do_api.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/feature_flags.py` & `deeporigin-0.0.6/src/feature_flags.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/managed_data/_api.py` & `deeporigin-0.0.6/src/managed_data/_api.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/managed_data/api.py` & `deeporigin-0.0.6/src/managed_data/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 @beartype
 def get_tree(
     *,
     include_rows: bool = True,
     client: Optional[Client] = None,
-) -> dict:
+) -> list[dict]:
     """Construct a tree of all workspaces, databases and rows.
 
     Returns a tree that contains all workspaces, databases and
     (optionally) rows. The tree is returned as a dictionary,
     and children of each object are contained in a field
     called `children`.
 
@@ -52,33 +52,26 @@
         workspaces = list_rows(row_type="workspace", client=client)
         databases = list_rows(row_type="database", client=client)
         objects = workspaces + databases
 
     for obj in workspaces + databases:
         obj["children"] = []
 
-    root_object = [obj for obj in objects if obj["parentId"] is None]
+    root_objects = [obj for obj in objects if obj["parentId"] is None]
 
-    # check that there is exactly one root
-    if len(root_object) != 1:
-        raise DeepOriginException(
-            f"Expected there to be exactly one root object. Instead, there were {len(root_object)}"
-        )
-
-    tree = root_object[0]
-
-    _add_children(tree, workspaces)
-    for workspace in workspaces:
-        _add_children(workspace, workspaces + databases)
+    for root_object in root_objects:
+        _add_children(root_object, workspaces)
+        for workspace in workspaces:
+            _add_children(workspace, workspaces + databases)
+
+        if include_rows:
+            for database in databases:
+                _add_children(database, rows)
 
-    if include_rows:
-        for database in databases:
-            _add_children(database, rows)
-
-    return tree
+    return root_objects
 
 
 @beartype
 def _add_children(node: dict, objects: list[dict]) -> None:
     """Internal function to add children to a node
```

### Comparing `deeporigin-0.0.5/src/managed_data/client.py` & `deeporigin-0.0.6/src/managed_data/client.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/managed_data/schema.py` & `deeporigin-0.0.6/src/managed_data/schema.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/utils.py` & `deeporigin-0.0.6/src/utils.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/variables/base_type.py` & `deeporigin-0.0.6/src/variables/base_type.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/variables/core.py` & `deeporigin-0.0.6/src/variables/core.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/variables/types/__init__.py` & `deeporigin-0.0.6/src/variables/types/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/variables/types/aws_profile.py` & `deeporigin-0.0.6/src/variables/types/aws_profile.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/variables/types/env_var.py` & `deeporigin-0.0.6/src/variables/types/env_var.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/variables/types/file.py` & `deeporigin-0.0.6/src/variables/types/file.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/variables/types/git_http_credentials.py` & `deeporigin-0.0.6/src/variables/types/git_http_credentials.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/variables/types/private_gpg_key.py` & `deeporigin-0.0.6/src/variables/types/private_gpg_key.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/variables/types/private_ssh_key.py` & `deeporigin-0.0.6/src/variables/types/private_ssh_key.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/variables/types/secret_env_var_value.py` & `deeporigin-0.0.6/src/variables/types/secret_env_var_value.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/variables/types/secret_file_value.py` & `deeporigin-0.0.6/src/variables/types/secret_file_value.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/src/variables/types/xpress_license_file.py` & `deeporigin-0.0.6/src/variables/types/xpress_license_file.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/tests/test_cli.py` & `deeporigin-0.0.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/tests/test_cli_data.py` & `deeporigin-0.0.6/tests/test_cli_data.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/tests/test_config.py` & `deeporigin-0.0.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/tests/test_context.py` & `deeporigin-0.0.6/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/tests/test_feature_flags.py` & `deeporigin-0.0.6/tests/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.0.5/tests/test_managed_data.py` & `deeporigin-0.0.6/tests/test_managed_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -266,20 +266,23 @@
 
     assert isinstance(data["mentions"], list), "Expected `mentions` to be a list"
 
 
 def test_get_tree(config):
     tree = api.get_tree(client=config["client"])
 
+    tree = tree[0]
+
     assert tree["parentId"] is None, "Expected the root of the tree to have no parent"
 
     tree.pop("children")
     ListRowsResponse(**tree)
 
     tree = api.get_tree(client=config["client"], include_rows=False)
+    tree = tree[0]
     assert tree["parentId"] is None, "Expected the root of the tree to have no parent"
 
     tree.pop("children")
     ListRowsResponse(**tree)
 
 
 def test_create_file_download_url(config):
```

### Comparing `deeporigin-0.0.5/tests/test_variables.py` & `deeporigin-0.0.6/tests/test_variables.py`

 * *Files identical despite different names*

