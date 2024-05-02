# Comparing `tmp/launch_cli-0.5.0.tar.gz` & `tmp/launch_cli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launch_cli-0.5.0.tar", last modified: Mon Apr 29 17:07:21 2024, max compression
+gzip compressed data, was "launch_cli-0.6.0.tar", last modified: Thu May  2 21:16:47 2024, max compression
```

## Comparing `launch_cli-0.5.0.tar` & `launch_cli-0.6.0.tar`

### file list

```diff
@@ -1,79 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.414942 launch_cli-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 17:07:08.000000 launch_cli-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19229 2024-04-29 17:07:21.414942 launch_cli-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-04-29 17:07:08.000000 launch_cli-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.410942 launch_cli-0.5.0/launch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19229 2024-04-29 17:07:21.000000 launch_cli-0.5.0/launch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-29 17:07:21.000000 launch_cli-0.5.0/launch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:07:21.000000 launch_cli-0.5.0/launch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 17:07:21.000000 launch_cli-0.5.0/launch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-29 17:07:21.000000 launch_cli-0.5.0/launch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 17:07:21.000000 launch_cli-0.5.0/launch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-29 17:07:08.000000 launch_cli-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:07:21.414942 launch_cli-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.398942 launch_cli-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/automation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/automation/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/common/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/automation/helm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/helm/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/automation/provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/automation/provider/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/provider/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/provider/aws/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/automation/provider/az/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/provider/az/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/provider/az/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/automation/terragrunt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/terragrunt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/automation/terragrunt/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/cli/github/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/cli/github/access/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/access/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/cli/github/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/hooks/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/cli/github/repo/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/repo/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.406942 launch_cli-0.5.0/src/launch/cli/github/version/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/github/version/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.410942 launch_cli-0.5.0/src/launch/cli/helm/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/helm/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.410942 launch_cli-0.5.0/src/launch/cli/service/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/service/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.410942 launch_cli-0.5.0/src/launch/cli/terragrunt/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/terragrunt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/cli/terragrunt/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.410942 launch_cli-0.5.0/src/launch/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/github/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/github/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/github/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/github/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/github/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.410942 launch_cli-0.5.0/src/launch/local_repo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/local_repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/local_repo/branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/local_repo/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/local_repo/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/local_repo/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:21.410942 launch_cli-0.5.0/src/launch/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/service/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-29 17:07:08.000000 launch_cli-0.5.0/src/launch/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.359033 launch_cli-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 21:16:34.000000 launch_cli-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19229 2024-05-02 21:16:47.359033 launch_cli-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18217 2024-05-02 21:16:34.000000 launch_cli-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.355033 launch_cli-0.6.0/launch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19229 2024-05-02 21:16:47.000000 launch_cli-0.6.0/launch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-02 21:16:47.000000 launch_cli-0.6.0/launch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:16:47.000000 launch_cli-0.6.0/launch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 21:16:47.000000 launch_cli-0.6.0/launch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-02 21:16:47.000000 launch_cli-0.6.0/launch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 21:16:47.000000 launch_cli-0.6.0/launch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-02 21:16:34.000000 launch_cli-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 21:16:47.359033 launch_cli-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.347033 launch_cli-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.351034 launch_cli-0.6.0/src/launch/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.351034 launch_cli-0.6.0/src/launch/automation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/automation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.351034 launch_cli-0.6.0/src/launch/automation/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/automation/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13217 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/automation/common/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.351034 launch_cli-0.6.0/src/launch/automation/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/automation/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/automation/helm/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.351034 launch_cli-0.6.0/src/launch/automation/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/automation/provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.351034 launch_cli-0.6.0/src/launch/automation/provider/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/automation/provider/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/automation/provider/aws/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.351034 launch_cli-0.6.0/src/launch/automation/provider/az/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/automation/provider/az/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/automation/provider/az/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.351034 launch_cli-0.6.0/src/launch/automation/terragrunt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/automation/terragrunt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/automation/terragrunt/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.351034 launch_cli-0.6.0/src/launch/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.351034 launch_cli-0.6.0/src/launch/cli/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.351034 launch_cli-0.6.0/src/launch/cli/github/access/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/github/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/github/access/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.351034 launch_cli-0.6.0/src/launch/cli/github/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/github/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/github/hooks/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.351034 launch_cli-0.6.0/src/launch/cli/github/repo/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/github/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/github/repo/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.355033 launch_cli-0.6.0/src/launch/cli/github/version/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/github/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/github/version/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.355033 launch_cli-0.6.0/src/launch/cli/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/helm/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.355033 launch_cli-0.6.0/src/launch/cli/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/service/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.355033 launch_cli-0.6.0/src/launch/cli/terragrunt/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/terragrunt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/terragrunt/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.355033 launch_cli-0.6.0/src/launch/cli/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/cli/validate/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.355033 launch_cli-0.6.0/src/launch/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/github/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/github/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/github/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/github/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/github/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.355033 launch_cli-0.6.0/src/launch/local_repo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/local_repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/local_repo/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/local_repo/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/local_repo/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/local_repo/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:47.355033 launch_cli-0.6.0/src/launch/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/service/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-02 21:16:34.000000 launch_cli-0.6.0/src/launch/update.py
```

### Comparing `launch_cli-0.5.0/LICENSE` & `launch_cli-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/PKG-INFO` & `launch_cli-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launch-cli
-Version: 0.5.0
+Version: 0.6.0
 Summary: CLI tooling for common Launch functions
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/launchbynttdata/launch-cli
 Project-URL: Issues, https://github.com/launchbynttdata/launch-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `launch_cli-0.5.0/README.md` & `launch_cli-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/launch_cli.egg-info/PKG-INFO` & `launch_cli-0.6.0/launch_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: launch-cli
-Version: 0.5.0
+Version: 0.6.0
 Summary: CLI tooling for common Launch functions
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/launchbynttdata/launch-cli
 Project-URL: Issues, https://github.com/launchbynttdata/launch-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `launch_cli-0.5.0/launch_cli.egg-info/SOURCES.txt` & `launch_cli-0.6.0/launch_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 src/launch/cli/github/version/commands.py
 src/launch/cli/helm/__init__.py
 src/launch/cli/helm/commands.py
 src/launch/cli/service/__init__.py
 src/launch/cli/service/commands.py
 src/launch/cli/terragrunt/__init__.py
 src/launch/cli/terragrunt/commands.py
+src/launch/cli/validate/__init__.py
+src/launch/cli/validate/commands.py
 src/launch/github/__init__.py
 src/launch/github/access.py
 src/launch/github/auth.py
 src/launch/github/hooks.py
 src/launch/github/repo.py
 src/launch/github/tags.py
 src/launch/local_repo/__init__.py
```

### Comparing `launch_cli-0.5.0/pyproject.toml` & `launch_cli-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "launch-cli"
-version = "0.5.0"
+version = "0.6.0"
 description = "CLI tooling for common Launch functions"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "Apache 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `launch_cli-0.5.0/src/launch/__init__.py` & `launch_cli-0.6.0/src/launch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from semver import Version
 
-VERSION = "0.5.0"
+VERSION = "0.6.0"
 
 SEMANTIC_VERSION = Version.parse(VERSION)
 GITHUB_ORG_NAME = "launchbynttdata"
 GITHUB_REPO_NAME = "launch-cli"
 SERVICE_SKELETON = "https://github.com/launchbynttdata/lcaf-skeleton-terragrunt.git"
 SKELETON_BRANCH = "main"
 MAIN_BRANCH = "main"
```

### Comparing `launch_cli-0.5.0/src/launch/automation/common/functions.py` & `launch_cli-0.6.0/src/launch/automation/common/functions.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/automation/helm/functions.py` & `launch_cli-0.6.0/src/launch/automation/helm/functions.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/automation/provider/aws/functions.py` & `launch_cli-0.6.0/src/launch/automation/provider/aws/functions.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/automation/provider/az/functions.py` & `launch_cli-0.6.0/src/launch/automation/provider/az/functions.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/automation/terragrunt/functions.py` & `launch_cli-0.6.0/src/launch/automation/terragrunt/functions.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/cli/entrypoint.py` & `launch_cli-0.6.0/src/launch/cli/entrypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,13 +58,15 @@
         context.invoke(get_version)
 
 
 from .github import github_group
 from .helm import helm_group
 from .service import service_group
 from .terragrunt import terragrunt_group
+from .validate import validate_group
 
 cli.add_command(get_version)
 cli.add_command(github_group)
 cli.add_command(terragrunt_group)
 cli.add_command(service_group)
 cli.add_command(helm_group)
+cli.add_command(validate_group)
```

### Comparing `launch_cli-0.5.0/src/launch/cli/github/access/commands.py` & `launch_cli-0.6.0/src/launch/cli/github/access/commands.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/cli/github/hooks/commands.py` & `launch_cli-0.6.0/src/launch/cli/github/hooks/commands.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/cli/github/repo/commands.py` & `launch_cli-0.6.0/src/launch/cli/github/repo/commands.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/cli/github/version/commands.py` & `launch_cli-0.6.0/src/launch/cli/github/version/commands.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/cli/helm/commands.py` & `launch_cli-0.6.0/src/launch/cli/helm/commands.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/cli/service/commands.py` & `launch_cli-0.6.0/src/launch/cli/service/commands.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/cli/terragrunt/commands.py` & `launch_cli-0.6.0/src/launch/cli/terragrunt/commands.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/env.py` & `launch_cli-0.6.0/src/launch/env.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/github/access.py` & `launch_cli-0.6.0/src/launch/github/access.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/github/auth.py` & `launch_cli-0.6.0/src/launch/github/auth.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/github/hooks.py` & `launch_cli-0.6.0/src/launch/github/hooks.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/github/repo.py` & `launch_cli-0.6.0/src/launch/github/repo.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/github/tags.py` & `launch_cli-0.6.0/src/launch/github/tags.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/local_repo/predict.py` & `launch_cli-0.6.0/src/launch/local_repo/predict.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 BRANCH_DELIMITER = "/"
 
 PATCH_NAME_PARTS = ["fix", "bug", "patch"]
 MINOR_NAME_PARTS = ["feature"]
 MAJOR_NAME_PARTS = []
 
+ALL_NAME_PARTS = list(
+    itertools.chain(MAJOR_NAME_PARTS, MINOR_NAME_PARTS, PATCH_NAME_PARTS)
+)
+
 BREAKING_CHARS = ["!"]
 CAPITALIZE_FIRST_IS_BREAKING = True
 DEFAULT_VERSION = Version(major=0, minor=1, patch=0)
 
 
 class InvalidBranchNameException(Exception):
     pass
@@ -32,14 +36,37 @@
     return separated[0], delimiter.join(separated[1:])
 
 
 def latest_tag(tags: list[Version]) -> Version:
     return sorted(tags)[-1]
 
 
+def validate_name(branch_name: str) -> bool:
+    """Checks the contents of a branch name against this module's configuration and returns a success/failure boolean with the outcome.
+
+    Args:
+        branch_name (str): Name of the branch to validate.
+
+    Returns:
+        bool: Success indicator. A True value indicates that this branch name conforms to the expected convention, a False value indicates otherwise.
+    """
+    try:
+        revision_type, _ = split_delimiter(branch_name=branch_name)
+    except InvalidBranchNameException:
+        return False
+
+    for breaking_char in BREAKING_CHARS:
+        if breaking_char in revision_type:
+            revision_type = revision_type.replace(breaking_char, "")
+
+    if revision_type.lower().strip() not in map(str.lower, ALL_NAME_PARTS):
+        return False
+    return True
+
+
 def predict_version(
     existing_tags: list[Version],
     branch_name: str,
     breaking_chars: list[str] | None = None,
     capitalize_first_is_breaking: bool | None = None,
 ):
     breaking_change: bool = False
@@ -55,31 +82,27 @@
         breaking_chars = BREAKING_CHARS
 
     if capitalize_first_is_breaking is None:
         capitalize_first_is_breaking = CAPITALIZE_FIRST_IS_BREAKING
 
     revision_type, _ = split_delimiter(branch_name=branch_name)
 
-    valid_branch_revision_types = list(
-        itertools.chain(MAJOR_NAME_PARTS, MINOR_NAME_PARTS, PATCH_NAME_PARTS)
-    )
-
-    logger.debug(f"Evaluating {revision_type=} against {valid_branch_revision_types=}")
+    logger.debug(f"Evaluating {revision_type=} against {ALL_NAME_PARTS=}")
 
     for breaking_char in breaking_chars:
         if breaking_char in revision_type:
             logger.debug(
                 f"Detected {breaking_char=} in branch name, setting {breaking_change=}"
             )
             breaking_change = True
-            revision_type = revision_type.strip(breaking_char)
+            revision_type = revision_type.replace(breaking_char, "")
 
-    if revision_type.lower().strip() not in map(str.lower, valid_branch_revision_types):
+    if revision_type.lower().strip() not in map(str.lower, ALL_NAME_PARTS):
         raise InvalidBranchNameException(
-            f"Branch name {branch_name} is invalid, must case-insensitively match one of {valid_branch_revision_types}"
+            f"Branch name {branch_name} is invalid, must case-insensitively match one of {ALL_NAME_PARTS}"
         )
 
     if capitalize_first_is_breaking:
         if revision_type[0] == revision_type[0].upper():
             logger.debug(
                 f"Revision begins with a capital letter, setting {breaking_change=}"
             )
```

### Comparing `launch_cli-0.5.0/src/launch/local_repo/repo.py` & `launch_cli-0.6.0/src/launch/local_repo/repo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 import logging
-import subprocess
+import pathlib
 
 from git import GitCommandError, Repo
 
-from launch import INIT_BRANCH
-
 logger = logging.getLogger(__name__)
 
 
+def acquire_repo(repo_path: pathlib.Path) -> Repo:
+    try:
+        return Repo(path=repo_path)
+    except Exception as e:
+        raise RuntimeError(
+            f"Failed to get a Repo instance from path {repo_path}: {e}"
+        ) from e
+
+
 def checkout_branch(
     repository: Repo, target_branch: str, new_branch: bool = False
 ) -> None:
     command_args = []
     if new_branch:
         command_args.append("-b")
     command_args.append(target_branch)
```

### Comparing `launch_cli-0.5.0/src/launch/local_repo/tags.py` & `launch_cli-0.6.0/src/launch/local_repo/tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,27 @@
 import pathlib
 
 from git import TagReference
 from git.objects.commit import Commit
 from git.repo import Repo
 from semver import Version
 
+from launch.local_repo.repo import acquire_repo
+
 logger = logging.getLogger(__name__)
 
 
 class CommitNotTaggedException(Exception):
     pass
 
 
 class CommitTagNotSemanticVersionException(Exception):
     pass
 
 
-def acquire_repo(repo_path: pathlib.Path) -> Repo:
-    try:
-        return Repo(path=repo_path)
-    except Exception as e:
-        raise RuntimeError(
-            f"Failed to get a Repo instance from path {repo_path}: {e}"
-        ) from e
-
-
 def read_tags(repo_path: pathlib.Path) -> list[str]:
     repo_instance = acquire_repo(repo_path=repo_path)
     all_tags = [tag.name for tag in repo_instance.tags]
     logger.debug(f"Discovered {len(all_tags)} tags")
     return all_tags
```

### Comparing `launch_cli-0.5.0/src/launch/service/common.py` & `launch_cli-0.6.0/src/launch/service/common.py`

 * *Files identical despite different names*

### Comparing `launch_cli-0.5.0/src/launch/update.py` & `launch_cli-0.6.0/src/launch/update.py`

 * *Files identical despite different names*

