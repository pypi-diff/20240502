# Comparing `tmp/dbt_core-1.8.0b3.tar.gz` & `tmp/dbt_core-1.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_core-1.8.0b3.tar", last modified: Thu Apr 18 16:22:42 2024, max compression
+gzip compressed data, was "dbt_core-1.8.0rc1.tar", last modified: Thu May  2 18:57:54 2024, max compression
```

## Comparing `dbt_core-1.8.0b3.tar` & `dbt_core-1.8.0rc1.tar`

### file list

```diff
@@ -1,266 +1,266 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.531873 dbt_core-1.8.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-18 16:22:42.531873 dbt_core-1.8.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.495873 dbt_core-1.8.0b3/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.495873 dbt_core-1.8.0b3/dbt/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.495873 dbt_core-1.8.0b3/dbt/artifacts/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/exceptions/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.495873 dbt_core-1.8.0b3/dbt/artifacts/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     9591 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/owner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/saved_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/semantic_layer_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/semantic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/source_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/sql_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/resources/v1/unit_test_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/catalog/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/catalog/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/catalog/v1/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/freshness/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/freshness/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/freshness/v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/freshness/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/freshness/v3/freshness.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/manifest/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/manifest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/manifest/v12/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/manifest/v12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/manifest/v12/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.499873 dbt_core-1.8.0b3/dbt/artifacts/schemas/run/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.503873 dbt_core-1.8.0b3/dbt/artifacts/schemas/run/v5/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/run/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/run/v5/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.503873 dbt_core-1.8.0b3/dbt/artifacts/schemas/upgrades/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/upgrades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/schemas/upgrades/upgrade_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.503873 dbt_core-1.8.0b3/dbt/artifacts/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/artifacts/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.503873 dbt_core-1.8.0b3/dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    18822 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/option_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    21775 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/requires.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.503873 dbt_core-1.8.0b3/dbt/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/clients/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/clients/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/clients/jinja_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/clients/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/clients/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23813 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/compilation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.507873 dbt_core-1.8.0b3/dbt/config/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    31410 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/config/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.507873 dbt_core-1.8.0b3/dbt/context/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23769 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/configured.py
--rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/context_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/exceptions_jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/macro_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/macros.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    67660 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/query_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/context/target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.511873 dbt_core-1.8.0b3/dbt/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.511873 dbt_core-1.8.0b3/dbt/contracts/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64188 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/model_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/node_args.py
--rw-r--r--   0 runner    (1001) docker     (127)    55031 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/semantic_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    22110 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/graph/unparsed.py
--rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/contracts/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.511873 dbt_core-1.8.0b3/dbt/deps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deps/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deps/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deps/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deps/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deps/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/deps/tarball.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.487873 dbt_core-1.8.0b3/dbt/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.511873 dbt_core-1.8.0b3/dbt/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.511873 dbt_core-1.8.0b3/dbt/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/docs/source/_ext/dbt_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.515873 dbt_core-1.8.0b3/dbt/events/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/events/base_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    99855 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/events/core_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/events/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    54812 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/events/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    49139 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.515873 dbt_core-1.8.0b3/dbt/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/graph/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/graph/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    14905 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/graph/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    35018 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/graph/selector_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/graph/selector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.515873 dbt_core-1.8.0b3/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.515873 dbt_core-1.8.0b3/dbt/include/starter_project/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.515873 dbt_core-1.8.0b3/dbt/include/starter_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.515873 dbt_core-1.8.0b3/dbt/include/starter_project/macros/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.487873 dbt_core-1.8.0b3/dbt/include/starter_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.519873 dbt_core-1.8.0b3/dbt/include/starter_project/models/example/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.519873 dbt_core-1.8.0b3/dbt/include/starter_project/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/seeds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.519873 dbt_core-1.8.0b3/dbt/include/starter_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.519873 dbt_core-1.8.0b3/dbt/include/starter_project/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/include/starter_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/internal_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/links.py
--rw-r--r--   0 runner    (1001) docker     (127)    16025 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/mp_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/node_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.523873 dbt_core-1.8.0b3/dbt/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    19106 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/generic_test_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/macros.py
--rw-r--r--   0 runner    (1001) docker     (127)    80055 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    23806 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    53594 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/partial.py
--rw-r--r--   0 runner    (1001) docker     (127)    17653 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/read_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/schema_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/schema_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/schema_yaml_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    43015 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/seeds.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    24969 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/parser/unit_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.523873 dbt_core-1.8.0b3/dbt/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/plugins/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/plugins/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/plugins/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/plugins/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/selected_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.527873 dbt_core-1.8.0b3/dbt/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17429 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/clone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/deps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.531873 dbt_core-1.8.0b3/dbt/task/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/docs/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)  1509632 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/docs/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)    10968 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/freshness.py
--rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    18691 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/run_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    27080 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/runnable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    15067 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/task/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.531873 dbt_core-1.8.0b3/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.531873 dbt_core-1.8.0b3/dbt/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20559 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/tests/fixtures/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    20813 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/dbt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:22:42.531873 dbt_core-1.8.0b3/dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-18 16:22:42.000000 dbt_core-1.8.0b3/dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-18 16:22:42.000000 dbt_core-1.8.0b3/dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:22:42.000000 dbt_core-1.8.0b3/dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 16:22:42.000000 dbt_core-1.8.0b3/dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:22:42.000000 dbt_core-1.8.0b3/dbt_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-18 16:22:42.000000 dbt_core-1.8.0b3/dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-18 16:22:42.000000 dbt_core-1.8.0b3/dbt_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:22:42.531873 dbt_core-1.8.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-18 16:22:31.000000 dbt_core-1.8.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.532992 dbt_core-1.8.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-02 18:57:54.532992 dbt_core-1.8.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.488993 dbt_core-1.8.0rc1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.488993 dbt_core-1.8.0rc1/dbt/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.488993 dbt_core-1.8.0rc1/dbt/artifacts/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/exceptions/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.488993 dbt_core-1.8.0rc1/dbt/artifacts/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.492992 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/owner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/saved_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/semantic_layer_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/semantic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/source_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/sql_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/unit_test_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.492992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.492992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/catalog/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/catalog/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/catalog/v1/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/freshness/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/freshness/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/freshness/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/freshness/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/freshness/v3/freshness.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/manifest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/manifest/v12/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/manifest/v12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/manifest/v12/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/run/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/run/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/run/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/run/v5/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/schemas/upgrades/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/upgrades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/schemas/upgrades/upgrade_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.496992 dbt_core-1.8.0rc1/dbt/artifacts/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/artifacts/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.500992 dbt_core-1.8.0rc1/dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20277 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18831 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/option_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21775 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/requires.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.500992 dbt_core-1.8.0rc1/dbt/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/clients/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/clients/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/clients/jinja_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/clients/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/clients/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23813 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/compilation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.500992 dbt_core-1.8.0rc1/dbt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32085 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/config/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.504993 dbt_core-1.8.0rc1/dbt/context/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24310 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/configured.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/exceptions_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/macro_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68635 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/query_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/context/target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.504993 dbt_core-1.8.0rc1/dbt/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.508993 dbt_core-1.8.0rc1/dbt/contracts/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65821 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/node_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55099 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/semantic_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22773 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/graph/unparsed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/contracts/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.508993 dbt_core-1.8.0rc1/dbt/deps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deps/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deps/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deps/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deps/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deps/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/deps/tarball.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.480993 dbt_core-1.8.0rc1/dbt/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.508993 dbt_core-1.8.0rc1/dbt/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.508993 dbt_core-1.8.0rc1/dbt/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/docs/source/_ext/dbt_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.512992 dbt_core-1.8.0rc1/dbt/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/events/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101044 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/events/core_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/events/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55599 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49209 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.512992 dbt_core-1.8.0rc1/dbt/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/graph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/graph/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14905 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/graph/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35223 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/graph/selector_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/graph/selector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.512992 dbt_core-1.8.0rc1/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.512992 dbt_core-1.8.0rc1/dbt/include/starter_project/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.512992 dbt_core-1.8.0rc1/dbt/include/starter_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.512992 dbt_core-1.8.0rc1/dbt/include/starter_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.484993 dbt_core-1.8.0rc1/dbt/include/starter_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.512992 dbt_core-1.8.0rc1/dbt/include/starter_project/models/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.516992 dbt_core-1.8.0rc1/dbt/include/starter_project/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/seeds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.516992 dbt_core-1.8.0rc1/dbt/include/starter_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.516992 dbt_core-1.8.0rc1/dbt/include/starter_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/include/starter_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/internal_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16025 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/mp_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/node_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.520992 dbt_core-1.8.0rc1/dbt/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19178 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/generic_test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80146 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23806 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53594 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17653 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/schema_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/schema_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29540 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/schema_yaml_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43568 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15421 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25079 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/parser/unit_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.520992 dbt_core-1.8.0rc1/dbt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/plugins/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/plugins/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/plugins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/plugins/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/selected_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.524992 dbt_core-1.8.0rc1/dbt/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17429 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/deps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.528992 dbt_core-1.8.0rc1/dbt/task/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/docs/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1509668 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/docs/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/freshness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18669 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/run_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26168 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15067 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/task/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.528992 dbt_core-1.8.0rc1/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.528992 dbt_core-1.8.0rc1/dbt/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20559 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/tests/fixtures/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20813 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/dbt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:57:54.532992 dbt_core-1.8.0rc1/dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-02 18:57:54.000000 dbt_core-1.8.0rc1/dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-02 18:57:54.000000 dbt_core-1.8.0rc1/dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:57:54.000000 dbt_core-1.8.0rc1/dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 18:57:54.000000 dbt_core-1.8.0rc1/dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:57:54.000000 dbt_core-1.8.0rc1/dbt_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-02 18:57:54.000000 dbt_core-1.8.0rc1/dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 18:57:54.000000 dbt_core-1.8.0rc1/dbt_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:57:54.532992 dbt_core-1.8.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-02 18:57:29.000000 dbt_core-1.8.0rc1/setup.py
```

### Comparing `dbt_core-1.8.0b3/PKG-INFO` & `dbt_core-1.8.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.8.0b3
+Version: 1.8.0rc1
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -13,28 +13,28 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: agate<1.8,>=1.7.0
+Requires-Dist: agate<1.10,>=1.7.0
 Requires-Dist: Jinja2<4,>=3.1.3
 Requires-Dist: mashumaro[msgpack]<4.0,>=3.9
 Requires-Dist: logbook<1.6,>=1.5
 Requires-Dist: click<9.0,>=8.0.2
 Requires-Dist: networkx<4.0,>=2.3
 Requires-Dist: protobuf<5,>=4.0.0
 Requires-Dist: requests<3.0.0
 Requires-Dist: pathspec<0.13,>=0.9
 Requires-Dist: sqlparse<0.6.0,>=0.5.0
 Requires-Dist: dbt-extractor<=0.6,>=0.5.0
 Requires-Dist: minimal-snowplow-tracker<0.1,>=0.0.2
 Requires-Dist: dbt-semantic-interfaces<0.6,>=0.5.1
-Requires-Dist: dbt-common<2.0,>=1.0.1
+Requires-Dist: dbt-common<2.0,>=1.0.2
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2
 Requires-Dist: packaging>20.9
 Requires-Dist: pytz>=2015.7
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: daff>=1.3.46
 Requires-Dist: typing-extensions>=4.4
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0b3 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0rc1 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Python: >=3.8 Description-Content-Type:
-text/markdown Requires-Dist: agate<1.8,>=1.7.0 Requires-Dist: Jinja2<4,>=3.1.3
+text/markdown Requires-Dist: agate<1.10,>=1.7.0 Requires-Dist: Jinja2<4,>=3.1.3
 Requires-Dist: mashumaro[msgpack]<4.0,>=3.9 Requires-Dist: logbook<1.6,>=1.5
 Requires-Dist: click<9.0,>=8.0.2 Requires-Dist: networkx<4.0,>=2.3 Requires-
 Dist: protobuf<5,>=4.0.0 Requires-Dist: requests<3.0.0 Requires-Dist:
 pathspec<0.13,>=0.9 Requires-Dist: sqlparse<0.6.0,>=0.5.0 Requires-Dist: dbt-
 extractor<=0.6,>=0.5.0 Requires-Dist: minimal-snowplow-tracker<0.1,>=0.0.2
 Requires-Dist: dbt-semantic-interfaces<0.6,>=0.5.1 Requires-Dist: dbt-
-common<2.0,>=1.0.1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2 Requires-Dist:
+common<2.0,>=1.0.2 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2 Requires-Dist:
 packaging>20.9 Requires-Dist: pytz>=2015.7 Requires-Dist: pyyaml>=6.0 Requires-
 Dist: daff>=1.3.46 Requires-Dist: typing-extensions>=4.4
                                   [dbt logo]
                                   _[_C_I_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. ![architecture](https://raw.githubusercontent.com/dbt-labs/
```

### Comparing `dbt_core-1.8.0b3/README.md` & `dbt_core-1.8.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/exceptions/schemas.py` & `dbt_core-1.8.0rc1/dbt/artifacts/exceptions/schemas.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/__init__.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/base.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/base.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/types.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/types.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/components.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 from dataclasses import dataclass, field
 from dbt.artifacts.resources.base import GraphResource, FileHash, Docs
+from dbt.artifacts.resources.types import NodeType
 from dbt.artifacts.resources.v1.config import NodeConfig
 from dbt_common.dataclass_schema import dbtClassMixin, ExtensibleDbtClassMixin
 from dbt_common.contracts.config.properties import AdditionalPropertiesMixin
 from dbt_common.contracts.constraints import ColumnLevelConstraint
 from typing import Dict, List, Optional, Union, Any
 from datetime import timedelta
 from dbt.artifacts.resources.types import TimePeriod
@@ -150,14 +151,22 @@
             return {}
 
 
 @dataclass
 class DeferRelation(HasRelationMetadata):
     alias: str
     relation_name: Optional[str]
+    # The rest of these fields match RelationConfig protocol exactly
+    resource_type: NodeType
+    name: str
+    description: str
+    compiled_code: Optional[str]
+    meta: Dict[str, Any]
+    tags: List[str]
+    config: Optional[NodeConfig]
 
     @property
     def identifier(self):
         return self.alias
 
 
 @dataclass
@@ -177,15 +186,14 @@
     description: str = field(default="")
     columns: Dict[str, ColumnInfo] = field(default_factory=dict)
     meta: Dict[str, Any] = field(default_factory=dict)
     group: Optional[str] = None
     docs: Docs = field(default_factory=Docs)
     patch_path: Optional[str] = None
     build_path: Optional[str] = None
-    deferred: bool = False
     unrendered_config: Dict[str, Any] = field(default_factory=dict)
     created_at: float = field(default_factory=lambda: time.time())
     config_call_dict: Dict[str, Any] = field(default_factory=dict)
     relation_name: Optional[str] = None
     raw_code: str = ""
```

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/config.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+
 from dbt_common.dataclass_schema import dbtClassMixin, ValidationError
 from typing import Optional, List, Any, Dict, Union
 from typing_extensions import Annotated
 from dataclasses import dataclass, field
 from dbt_common.contracts.config.base import (
     BaseConfig,
     CompareBehavior,
@@ -246,10 +248,16 @@
             if key in modifiers:
                 if not cls.compare_key(unrendered, other, key):
                     return False
         return True
 
     @classmethod
     def validate(cls, data):
+        if data.get("severity") and not re.match(SEVERITY_PATTERN, data.get("severity")):
+            raise ValidationError(
+                f"Severity must be either 'warn' or 'error'. Got '{data.get('severity')}'"
+            )
+
         super().validate(data)
+
         if data.get("materialized") and data.get("materialized") != "test":
             raise ValidationError("A test must have a materialized value of 'test'")
```

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/exposure.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/exposure.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/generic_test.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/macro.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/macro.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/metric.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/metric.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/model.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/model.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/saved_query.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/saved_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 @dataclass
 class ExportConfig(dbtClassMixin):
     """Nested configuration attributes for exports."""
 
     export_as: ExportDestinationType
     schema_name: Optional[str] = None
     alias: Optional[str] = None
+    database: Optional[str] = None
 
 
 @dataclass
 class Export(dbtClassMixin):
     """Configuration for writing query results to a table."""
 
     name: str
```

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/seed.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/seed.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/semantic_layer_components.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/semantic_layer_components.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/semantic_model.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/singular_test.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/snapshot.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/source_definition.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/source_definition.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/resources/v1/unit_test_definition.py` & `dbt_core-1.8.0rc1/dbt/artifacts/resources/v1/unit_test_definition.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/schemas/base.py` & `dbt_core-1.8.0rc1/dbt/artifacts/schemas/base.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/schemas/catalog/v1/catalog.py` & `dbt_core-1.8.0rc1/dbt/artifacts/schemas/catalog/v1/catalog.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/schemas/freshness/v3/freshness.py` & `dbt_core-1.8.0rc1/dbt/artifacts/schemas/freshness/v3/freshness.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/schemas/manifest/v12/manifest.py` & `dbt_core-1.8.0rc1/dbt/artifacts/schemas/manifest/v12/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/schemas/results.py` & `dbt_core-1.8.0rc1/dbt/artifacts/schemas/results.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/schemas/run/v5/run.py` & `dbt_core-1.8.0rc1/dbt/artifacts/schemas/run/v5/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import threading
 from typing import Any, Optional, Iterable, Tuple, Sequence, Dict, TYPE_CHECKING
 import copy
 from dataclasses import dataclass, field
 from datetime import datetime
 
 
-from dbt.constants import SECRET_ENV_PREFIX
+from dbt_common.constants import SECRET_ENV_PREFIX
 from dbt.artifacts.resources import CompiledResource
 from dbt.artifacts.schemas.base import (
     BaseArtifactMetadata,
     ArtifactMixin,
     schema_version,
     get_artifact_schema_version,
 )
```

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/schemas/upgrades/upgrade_manifest.py` & `dbt_core-1.8.0rc1/dbt/artifacts/schemas/upgrades/upgrade_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/artifacts/utils/validation.py` & `dbt_core-1.8.0rc1/dbt/artifacts/utils/validation.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/cli/exceptions.py` & `dbt_core-1.8.0rc1/dbt/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/cli/flags.py` & `dbt_core-1.8.0rc1/dbt/cli/flags.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
         # Set globals for common.jinja
         if getattr(self, "MACRO_DEBUGGING", None) is not None:
             jinja.MACRO_DEBUGGING = getattr(self, "MACRO_DEBUGGING")
 
     # This is here to prevent mypy from complaining about all of the
     # attributes which we added dynamically.
     def __getattr__(self, name: str) -> Any:
-        return super().__get_attribute__(name)  # type: ignore
+        return super().__getattribute__(name)  # type: ignore
 
 
 CommandParams = List[str]
 
 
 def command_params(command: CliCommand, args_dict: Dict[str, Any]) -> CommandParams:
     """Given a command and a dict, returns a list of strings representing
```

### Comparing `dbt_core-1.8.0b3/dbt/cli/main.py` & `dbt_core-1.8.0rc1/dbt/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,14 +166,15 @@
     """
 
 
 # dbt build
 @cli.command("build")
 @click.pass_context
 @global_flags
+@p.empty
 @p.exclude
 @p.export_saved_queries
 @p.full_refresh
 @p.deprecated_include_saved_query
 @p.profiles_dir
 @p.project_dir
 @p.resource_type
```

### Comparing `dbt_core-1.8.0b3/dbt/cli/option_types.py` & `dbt_core-1.8.0rc1/dbt/cli/option_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from click import ParamType, Choice
 
-from dbt.config.utils import parse_cli_yaml_string
+from dbt.config.utils import parse_cli_yaml_string, exclusive_primary_alt_value_setting
 from dbt.events import ALL_EVENT_NAMES
 from dbt.exceptions import ValidationError, OptionNotYamlDictError
 from dbt_common.exceptions import DbtValidationError
-
 from dbt_common.helper_types import WarnErrorOptions
 
 
 class YAML(ParamType):
     """The Click YAML type. Converts YAML strings into objects."""
 
     name = "YAML"
@@ -48,18 +47,25 @@
     """The Click WarnErrorOptions type. Converts YAML strings into objects."""
 
     name = "WarnErrorOptionsType"
 
     def convert(self, value, param, ctx):
         # this function is being used by param in click
         include_exclude = super().convert(value, param, ctx)
+        exclusive_primary_alt_value_setting(
+            include_exclude, "include", "error", "warn_error_options"
+        )
+        exclusive_primary_alt_value_setting(
+            include_exclude, "exclude", "warn", "warn_error_options"
+        )
 
         return WarnErrorOptions(
             include=include_exclude.get("include", []),
             exclude=include_exclude.get("exclude", []),
+            silence=include_exclude.get("silence", []),
             valid_error_names=ALL_EVENT_NAMES,
         )
 
 
 class Truthy(ParamType):
     """The Click Truthy type.  Converts strings into a "truthy" type"""
```

### Comparing `dbt_core-1.8.0b3/dbt/cli/options.py` & `dbt_core-1.8.0rc1/dbt/cli/options.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/cli/params.py` & `dbt_core-1.8.0rc1/dbt/cli/params.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/cli/requires.py` & `dbt_core-1.8.0rc1/dbt/cli/requires.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 
-import dbt.tracking
-from dbt_common.context import set_invocation_context
+from dbt_common.context import get_invocation_context, set_invocation_context
+from dbt_common.record import Recorder, RecorderMode, get_record_mode_from_env
+from dbt_common.clients.system import get_env
 from dbt_common.invocation import reset_invocation_id
 
+import dbt.tracking
 from dbt.version import installed as installed_version
 from dbt.adapters.factory import adapter_management, register_adapter, get_adapter
 from dbt.context.providers import generate_runtime_macro_context
 from dbt.flags import set_flags, get_flag_dict
 from dbt.cli.exceptions import (
     ExceptionExit,
     ResultExit,
@@ -40,23 +42,31 @@
 from dbt.mp_context import get_mp_context
 
 from click import Context
 from functools import update_wrapper
 import importlib.util
 import time
 import traceback
+from typing import Optional
 
 
 def preflight(func):
     def wrapper(*args, **kwargs):
         ctx = args[0]
         assert isinstance(ctx, Context)
         ctx.obj = ctx.obj or {}
 
-        set_invocation_context(os.environ)
+        set_invocation_context({})
+
+        # Record/Replay
+        setup_record_replay()
+
+        # Must be set after record/replay is set up so that the env can be
+        # recorded or replayed if needed.
+        get_invocation_context()._env = get_env()
 
         # Flags
         flags = Flags(ctx)
         ctx.obj["flags"] = flags
         set_flags(flags)
 
         # Reset invocation_id for each 'invocation' of a dbt command (can happen multiple times in a single process)
@@ -89,14 +99,36 @@
         ctx.with_resource(adapter_management())
 
         return func(*args, **kwargs)
 
     return update_wrapper(wrapper, func)
 
 
+def setup_record_replay():
+    rec_mode = get_record_mode_from_env()
+
+    recorder: Optional[Recorder] = None
+    if rec_mode == RecorderMode.REPLAY:
+        recording_path = os.environ["DBT_REPLAY"]
+        recorder = Recorder(RecorderMode.REPLAY, recording_path)
+    elif rec_mode == RecorderMode.RECORD:
+        recorder = Recorder(RecorderMode.RECORD)
+
+    get_invocation_context().recorder = recorder
+
+
+def tear_down_record_replay():
+    recorder = get_invocation_context().recorder
+    if recorder is not None:
+        if recorder.mode == RecorderMode.RECORD:
+            recorder.write("recording.json")
+        elif recorder.mode == RecorderMode.REPLAY:
+            recorder.write_diffs("replay_diffs.json")
+
+
 def postflight(func):
     """The decorator that handles all exception handling for the click commands.
     This decorator must be used before any other decorators that may throw an exception."""
 
     def wrapper(*args, **kwargs):
         ctx = args[0]
         start_func = time.perf_counter()
@@ -142,14 +174,16 @@
                     command=ctx.command_path,
                     success=success,
                     completed_at=get_json_string_utcnow(),
                     elapsed=time.perf_counter() - start_func,
                 )
             )
 
+            tear_down_record_replay()
+
         if not success:
             raise ResultExit(result)
 
         return (result, success)
 
     return update_wrapper(wrapper, func)
 
@@ -277,15 +311,15 @@
             reqs = [ctx.obj.get(dep) for dep in req_strs]
 
             if None in reqs:
                 raise DbtProjectError("profile, project, and runtime_config required for manifest")
 
             runtime_config = ctx.obj["runtime_config"]
 
-            # a manifest has already been set on the context, so don't overwrite it
+            # if a manifest has already been set on the context, don't overwrite it
             if ctx.obj.get("manifest") is None:
                 ctx.obj["manifest"] = parse_manifest(
                     runtime_config, write_perf_info, write, ctx.obj["flags"].write_json
                 )
             else:
                 register_adapter(runtime_config, get_mp_context())
                 adapter = get_adapter(runtime_config)
```

### Comparing `dbt_core-1.8.0b3/dbt/cli/resolvers.py` & `dbt_core-1.8.0rc1/dbt/cli/resolvers.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/cli/types.py` & `dbt_core-1.8.0rc1/dbt/cli/types.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/clients/git.py` & `dbt_core-1.8.0rc1/dbt/clients/git.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/clients/jinja.py` & `dbt_core-1.8.0rc1/dbt/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/clients/jinja_static.py` & `dbt_core-1.8.0rc1/dbt/clients/jinja_static.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/clients/registry.py` & `dbt_core-1.8.0rc1/dbt/clients/registry.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/clients/yaml_helper.py` & `dbt_core-1.8.0rc1/dbt/clients/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/compilation.py` & `dbt_core-1.8.0rc1/dbt/compilation.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/config/profile.py` & `dbt_core-1.8.0rc1/dbt/config/profile.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/config/project.py` & `dbt_core-1.8.0rc1/dbt/config/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,28 @@
     DBT_PROJECT_FILE_NAME,
 )
 from dbt_common.clients.system import path_exists, load_file_contents
 from dbt.clients.yaml_helper import load_yaml_text
 from dbt.adapters.contracts.connection import QueryComment
 from dbt.exceptions import (
     DbtProjectError,
+    DbtExclusivePropertyUseError,
     ProjectContractBrokenError,
     ProjectContractError,
     DbtRuntimeError,
 )
 from dbt_common.exceptions import SemverError
 from dbt.graph import SelectionSpec
 from dbt_common.helper_types import NoValue
 from dbt_common.semver import VersionSpecifier, versions_compatible
 from dbt.version import get_installed_version
 from dbt.utils import MultiDict, md5, coerce_dict_str
 from dbt.node_types import NodeType
 from dbt.config.selectors import SelectorDict
+from dbt.config.utils import exclusive_primary_alt_value_setting
 from dbt.contracts.project import (
     Project as ProjectContract,
     SemverString,
     ProjectFlags,
 )
 from dbt.contracts.project import PackageConfig, ProjectPackageMetadata
 from dbt_common.dataclass_schema import ValidationError
@@ -831,15 +833,26 @@
         if profile_project_flags:
             # This can't use WARN_ERROR or WARN_ERROR_OPTIONS because they're in
             # the config that we're loading. Uses special "warn" method.
             deprecations.warn("project-flags-moved")
             project_flags = profile_project_flags
 
         if project_flags is not None:
+            # handle collapsing `include` and `error` as well as collapsing `exclude` and `warn`
+            # for warn_error_options
+            warn_error_options = project_flags.get("warn_error_options")
+            exclusive_primary_alt_value_setting(
+                warn_error_options, "include", "error", "warn_error_options"
+            )
+            exclusive_primary_alt_value_setting(
+                warn_error_options, "exclude", "warn", "warn_error_options"
+            )
+
             ProjectFlags.validate(project_flags)
             return ProjectFlags.from_dict(project_flags)
-    except (DbtProjectError) as exc:
-        # We don't want to eat the DbtProjectError for UserConfig to ProjectFlags
+    except (DbtProjectError, DbtExclusivePropertyUseError) as exc:
+        # We don't want to eat the DbtProjectError for UserConfig to ProjectFlags or
+        # DbtConfigError for warn_error_options munging
         raise exc
     except (DbtRuntimeError, ValidationError):
         pass
     return ProjectFlags()
```

### Comparing `dbt_core-1.8.0b3/dbt/config/renderer.py` & `dbt_core-1.8.0rc1/dbt/config/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Dict, Any, Tuple, Optional, Union, Callable
 import re
 from datetime import date
 
 from dbt.clients.jinja import get_rendered
 from dbt_common.clients.jinja import catch_jinja
-from dbt.constants import SECRET_ENV_PREFIX, DEPENDENCIES_FILE_NAME
+from dbt_common.constants import SECRET_ENV_PREFIX
+from dbt.constants import DEPENDENCIES_FILE_NAME, SECRET_PLACEHOLDER
 from dbt.context.target import TargetContext
-from dbt.context.secret import SecretContext, SECRET_PLACEHOLDER
+from dbt.context.secret import SecretContext
 from dbt.context.base import BaseContext
 from dbt.adapters.contracts.connection import HasCredentials
 from dbt.exceptions import DbtProjectError
 from dbt_common.context import get_invocation_context
 from dbt_common.exceptions import CompilationError, RecursionError
 from dbt_common.utils import deep_map_render
```

### Comparing `dbt_core-1.8.0b3/dbt/config/runtime.py` & `dbt_core-1.8.0rc1/dbt/config/runtime.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/config/selectors.py` & `dbt_core-1.8.0rc1/dbt/config/selectors.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/constants.py` & `dbt_core-1.8.0rc1/dbt/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# TODO: remove SECRET_ENV_PREFIX and import from dbt_common
-SECRET_ENV_PREFIX = "DBT_ENV_SECRET_"
 DEFAULT_ENV_PLACEHOLDER = "DBT_DEFAULT_PLACEHOLDER"
 
+SECRET_PLACEHOLDER = "$$$DBT_SECRET_START$$${}$$$DBT_SECRET_END$$$"
+
 MAXIMUM_SEED_SIZE = 1 * 1024 * 1024
 MAXIMUM_SEED_SIZE_NAME = "1MB"
 
 PIN_PACKAGE_URL = (
     "https://docs.getdbt.com/docs/package-management#section-specifying-package-versions"
 )
```

### Comparing `dbt_core-1.8.0b3/dbt/context/base.py` & `dbt_core-1.8.0rc1/dbt/context/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 from dbt.flags import get_flags
 import dbt.flags as flags_module
 from dbt import tracking
 from dbt import utils
 from dbt.clients.jinja import get_rendered
 from dbt.clients.yaml_helper import yaml, safe_load, SafeLoader, Loader, Dumper  # noqa: F401
-from dbt.constants import SECRET_ENV_PREFIX, DEFAULT_ENV_PLACEHOLDER
+from dbt_common.constants import SECRET_ENV_PREFIX
+from dbt.constants import DEFAULT_ENV_PLACEHOLDER, SECRET_PLACEHOLDER
 from dbt.contracts.graph.nodes import Resource
 from dbt.exceptions import (
     SecretEnvVarLocationError,
     EnvVarMissingError,
     RequiredVarNotFoundError,
     SetStrictWrongTypeError,
     ZipStrictWrongTypeError,
@@ -557,14 +558,26 @@
 
         > macros/my_log_macro.sql
 
             {% macro some_macro(arg1, arg2) %}
               {{ log("Running some_macro: " ~ arg1 ~ ", " ~ arg2) }}
             {% endmacro %}"
         """
+        # Detect instances of the placeholder value ($$$DBT_SECRET_START...DBT_SECRET_END$$$)
+        # and replace it with the standard mask '*****'
+        if "DBT_SECRET_START" in str(msg):
+            search_group = f"({SECRET_ENV_PREFIX}(.*))"
+            pattern = SECRET_PLACEHOLDER.format(search_group).replace("$", r"\$")
+            m = re.search(
+                pattern,
+                msg,
+            )
+            if m:
+                msg = re.sub(pattern, "*****", msg)
+
         if info:
             fire_event(JinjaLogInfo(msg=msg, node_info=get_node_info()))
         else:
             fire_event(JinjaLogDebug(msg=msg, node_info=get_node_info()))
         return ""
 
     @contextproperty()
```

### Comparing `dbt_core-1.8.0b3/dbt/context/configured.py` & `dbt_core-1.8.0rc1/dbt/context/configured.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any, Dict, Optional
 
 from dbt_common.context import get_invocation_context
 
-from dbt.constants import SECRET_ENV_PREFIX, DEFAULT_ENV_PLACEHOLDER
+from dbt_common.constants import SECRET_ENV_PREFIX
+from dbt.constants import DEFAULT_ENV_PLACEHOLDER
 from dbt.adapters.contracts.connection import AdapterRequiredConfig
 from dbt.node_types import NodeType
 from dbt.utils import MultiDict
 
 from dbt.context.base import contextproperty, contextmember, Var
 from dbt.context.target import TargetContext
 from dbt.exceptions import EnvVarMissingError, SecretEnvVarLocationError
```

### Comparing `dbt_core-1.8.0b3/dbt/context/context_config.py` & `dbt_core-1.8.0rc1/dbt/context/context_config.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/context/docs.py` & `dbt_core-1.8.0rc1/dbt/context/docs.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/context/exceptions_jinja.py` & `dbt_core-1.8.0rc1/dbt/context/exceptions_jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/context/macro_resolver.py` & `dbt_core-1.8.0rc1/dbt/context/macro_resolver.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/context/macros.py` & `dbt_core-1.8.0rc1/dbt/context/macros.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/context/manifest.py` & `dbt_core-1.8.0rc1/dbt/context/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/context/providers.py` & `dbt_core-1.8.0rc1/dbt/context/providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 from dbt.adapters.base.column import Column
 from dbt.artifacts.resources import NodeVersion, RefArgs
 from dbt_common.clients.jinja import MacroProtocol
 from dbt_common.context import get_invocation_context
 from dbt.adapters.factory import get_adapter, get_adapter_package_names, get_adapter_type_names
 from dbt.clients.jinja import get_rendered, MacroGenerator, MacroStack, UnitTestMacroGenerator
 from dbt.config import RuntimeConfig, Project
-from dbt.constants import SECRET_ENV_PREFIX, DEFAULT_ENV_PLACEHOLDER
+from dbt_common.constants import SECRET_ENV_PREFIX
+from dbt.constants import DEFAULT_ENV_PLACEHOLDER
 from dbt.context.base import contextmember, contextproperty, Var
 from dbt.context.configured import FQNLookup
 from dbt.context.context_config import ContextConfig
 from dbt.context.exceptions_jinja import wrapped_exports
 from dbt.context.macro_resolver import MacroResolver, TestMacroNamespace
 from dbt.context.macros import MacroNamespaceBuilder, MacroNamespace
 from dbt.context.manifest import ManifestContext
@@ -499,49 +500,68 @@
             target_name,
             target_package,
             target_version,
             self.current_project,
             self.model.package_name,
         )
 
+        # Raise an error if the reference target is missing
         if target_model is None or isinstance(target_model, Disabled):
             raise TargetNotFoundError(
                 node=self.model,
                 target_name=target_name,
                 target_kind="node",
                 target_package=target_package,
                 target_version=target_version,
                 disabled=isinstance(target_model, Disabled),
             )
+
+        # Raise error if trying to reference a 'private' resource outside its 'group'
         elif self.manifest.is_invalid_private_ref(
             self.model, target_model, self.config.dependencies
         ):
             raise DbtReferenceError(
                 unique_id=self.model.unique_id,
                 ref_unique_id=target_model.unique_id,
                 access=AccessType.Private,
                 scope=cast_to_str(target_model.group),
             )
+        # Or a 'protected' resource outside its project/package namespace
         elif self.manifest.is_invalid_protected_ref(
             self.model, target_model, self.config.dependencies
         ):
             raise DbtReferenceError(
                 unique_id=self.model.unique_id,
                 ref_unique_id=target_model.unique_id,
                 access=AccessType.Protected,
                 scope=target_model.package_name,
             )
-
         self.validate(target_model, target_name, target_package, target_version)
         return self.create_relation(target_model)
 
     def create_relation(self, target_model: ManifestNode) -> RelationProxy:
         if target_model.is_ephemeral_model:
             self.model.set_cte(target_model.unique_id, None)
             return self.Relation.create_ephemeral_from(target_model, limit=self.resolve_limit)
+        elif (
+            hasattr(target_model, "defer_relation")
+            and target_model.defer_relation
+            and self.config.args.defer
+            and (
+                # User has explicitly opted to prefer defer_relation
+                self.config.args.favor_state
+                # Or, this node's relation does not exist in the expected target location (cache lookup)
+                or not get_adapter(self.config).get_relation(
+                    target_model.database, target_model.schema, target_model.identifier
+                )
+            )
+        ):
+            return self.Relation.create_from(
+                self.config, target_model.defer_relation, limit=self.resolve_limit
+            )
         else:
             return self.Relation.create_from(self.config, target_model, limit=self.resolve_limit)
 
     def validate(
         self,
         resolved: ManifestNode,
         target_name: str,
```

### Comparing `dbt_core-1.8.0b3/dbt/context/query_header.py` & `dbt_core-1.8.0rc1/dbt/context/query_header.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/context/secret.py` & `dbt_core-1.8.0rc1/dbt/context/secret.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from typing import Any, Dict, Optional
 
 from dbt_common.context import get_invocation_context
 
 from .base import BaseContext, contextmember
 
-from dbt.constants import SECRET_ENV_PREFIX, DEFAULT_ENV_PLACEHOLDER
+from dbt_common.constants import SECRET_ENV_PREFIX
+from dbt.constants import DEFAULT_ENV_PLACEHOLDER, SECRET_PLACEHOLDER
 from dbt.exceptions import EnvVarMissingError
 
 
-SECRET_PLACEHOLDER = "$$$DBT_SECRET_START$$${}$$$DBT_SECRET_END$$$"
-
-
 class SecretContext(BaseContext):
     """This context is used in profiles.yml + packages.yml. It can render secret
     env vars that aren't usable elsewhere"""
 
     @contextmember()
     def env_var(self, var: str, default: Optional[str] = None) -> str:
         """The env_var() function. Return the environment variable named 'var'.
```

### Comparing `dbt_core-1.8.0b3/dbt/context/target.py` & `dbt_core-1.8.0rc1/dbt/context/target.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/contracts/files.py` & `dbt_core-1.8.0rc1/dbt/contracts/files.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/contracts/graph/manifest.py` & `dbt_core-1.8.0rc1/dbt/contracts/graph/manifest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import enum
 from collections import defaultdict
 from dataclasses import dataclass, field, replace
-from itertools import chain, islice
+from itertools import chain
 from mashumaro.mixins.msgpack import DataClassMessagePackMixin
 from multiprocessing.synchronize import Lock
 from typing import (
     DefaultDict,
     Dict,
     List,
     Optional,
@@ -14,19 +14,19 @@
     MutableMapping,
     Any,
     Set,
     Tuple,
     TypeVar,
     Callable,
     Generic,
-    AbstractSet,
     ClassVar,
 )
 from typing_extensions import Protocol
 
+from dbt import deprecations
 from dbt import tracking
 from dbt.contracts.graph.nodes import (
     BaseNode,
     Documentation,
     Exposure,
     GenericTestNode,
     GraphMemberNode,
@@ -34,14 +34,15 @@
     Macro,
     ManifestNode,
     Metric,
     ModelNode,
     ResultNode,
     SavedQuery,
     SemanticModel,
+    SeedNode,
     SourceDefinition,
     UnpatchedSourceDefinition,
     UnitTestDefinition,
     UnitTestFileFixture,
     RESOURCE_CLASS_TO_NODE_CLASS,
 )
 from dbt.contracts.graph.unparsed import SourcePatch, UnparsedVersion
@@ -49,14 +50,15 @@
 
 # to preserve import paths
 from dbt.artifacts.resources import (
     NodeVersion,
     DeferRelation,
     BaseResource,
 )
+from dbt.artifacts.resources.v1.config import NodeConfig
 from dbt.artifacts.schemas.manifest import WritableManifest, ManifestMetadata, UniqueID
 from dbt.contracts.files import (
     SourceFile,
     SchemaSourceFile,
     FileHash,
     AnySourceFile,
     FixtureSourceFile,
@@ -69,15 +71,15 @@
     DuplicateResourceNameError,
     AmbiguousResourceNameRefError,
 )
 from dbt.adapters.exceptions import DuplicateMacroInPackageError, DuplicateMaterializationNameError
 from dbt_common.helper_types import PathSet
 from dbt_common.events.functions import fire_event
 from dbt_common.events.contextvars import get_node_info
-from dbt.events.types import MergedFromState, UnpinnedRefNewVersionAvailable
+from dbt.events.types import UnpinnedRefNewVersionAvailable
 from dbt.node_types import NodeType, AccessType, REFABLE_NODE_TYPES, VERSIONED_NODE_TYPES
 from dbt.mp_context import get_mp_context
 import dbt_common.utils
 import dbt_common.exceptions
 
 
 PackageName = str
@@ -566,19 +568,37 @@
         return False
 
 
 M = TypeVar("M", bound=MacroCandidate)
 
 
 class CandidateList(List[M]):
-    def last(self) -> Optional[Macro]:
+    def last_candidate(
+        self, valid_localities: Optional[List[Locality]] = None
+    ) -> Optional[MacroCandidate]:
+        """
+        Obtain the last (highest precedence) MacroCandidate from the CandidateList of any locality in valid_localities.
+        If valid_localities is not specified, return the last MacroCandidate of any locality.
+        """
         if not self:
             return None
         self.sort()
-        return self[-1].macro
+
+        if valid_localities is None:
+            return self[-1]
+
+        for candidate in reversed(self):
+            if candidate.locality in valid_localities:
+                return candidate
+
+        return None
+
+    def last(self) -> Optional[Macro]:
+        last_candidate = self.last_candidate()
+        return last_candidate.macro if last_candidate is not None else None
 
 
 def _get_locality(macro: Macro, root_project_name: str, internal_packages: Set[str]) -> Locality:
     if macro.package_name == root_project_name:
         return Locality.Root
     elif macro.package_name in internal_packages:
         return Locality.Core
@@ -926,15 +946,41 @@
                     materialization_name=materialization_name,
                     adapter_type=atype,
                     specificity=specificity,  # where in the inheritance chain this candidate is
                 )
                 for specificity, atype in enumerate(self._get_parent_adapter_types(adapter_type))
             )
         )
-        return candidates.last()
+        core_candidates = [
+            candidate for candidate in candidates if candidate.locality == Locality.Core
+        ]
+
+        materialization_candidate = candidates.last_candidate()
+        # If an imported materialization macro was found that also had a core candidate, fire a deprecation
+        if (
+            materialization_candidate is not None
+            and materialization_candidate.locality == Locality.Imported
+            and core_candidates
+        ):
+            # preserve legacy behaviour - allow materialization override
+            if (
+                get_flags().require_explicit_package_overrides_for_builtin_materializations
+                is False
+            ):
+                deprecations.warn(
+                    "package-materialization-override",
+                    package_name=materialization_candidate.macro.package_name,
+                    materialization_name=materialization_name,
+                )
+            else:
+                materialization_candidate = candidates.last_candidate(
+                    valid_localities=[Locality.Core, Locality.Root]
+                )
+
+        return materialization_candidate.macro if materialization_candidate else None
 
     def get_resource_fqns(self) -> Mapping[str, PathSet]:
         resource_fqns: Dict[str, Set[Tuple[str, ...]]] = {}
         all_resources = chain(
             self.exposures.values(),
             self.nodes.values(),
             self.sources.values(),
@@ -1417,58 +1463,44 @@
         target_dependency = dependencies.get(target_model.package_name)
         restrict_package_access = target_dependency.restrict_access if target_dependency else False
 
         return is_protected_ref and (
             node.package_name != target_model.package_name and restrict_package_access
         )
 
-    # Called by GraphRunnableTask.defer_to_manifest
-    def merge_from_artifact(
-        self,
-        adapter,
-        other: "Manifest",
-        selected: AbstractSet[UniqueID],
-        favor_state: bool = False,
-    ) -> None:
-        """Given the selected unique IDs and a writable manifest, update this
-        manifest by replacing any unselected nodes with their counterpart.
+    # Called in GraphRunnableTask.before_run, RunTask.before_run, CloneTask.before_run
+    def merge_from_artifact(self, other: "Manifest") -> None:
+        """Update this manifest by adding the 'defer_relation' attribute to all nodes
+        with a counterpart in the stateful manifest used for deferral.
 
         Only non-ephemeral refable nodes are examined.
         """
         refables = set(REFABLE_NODE_TYPES)
-        merged = set()
         for unique_id, node in other.nodes.items():
             current = self.nodes.get(unique_id)
-            if current and (
-                node.resource_type in refables
-                and not node.is_ephemeral
-                and unique_id not in selected
-                and (
-                    not adapter.get_relation(current.database, current.schema, current.identifier)
-                    or favor_state
-                )
-            ):
-                merged.add(unique_id)
-                self.nodes[unique_id] = replace(node, deferred=True)
-
-            # for all other nodes, add 'defer_relation'
-            elif current and node.resource_type in refables and not node.is_ephemeral:
+            if current and node.resource_type in refables and not node.is_ephemeral:
+                assert isinstance(node.config, NodeConfig)  # this makes mypy happy
                 defer_relation = DeferRelation(
-                    node.database, node.schema, node.alias, node.relation_name
+                    database=node.database,
+                    schema=node.schema,
+                    alias=node.alias,
+                    relation_name=node.relation_name,
+                    resource_type=node.resource_type,
+                    name=node.name,
+                    description=node.description,
+                    compiled_code=(node.compiled_code if not isinstance(node, SeedNode) else None),
+                    meta=node.meta,
+                    tags=node.tags,
+                    config=node.config,
                 )
                 self.nodes[unique_id] = replace(current, defer_relation=defer_relation)
 
-        # Rebuild the flat_graph, which powers the 'graph' context variable,
-        # now that we've deferred some nodes
+        # Rebuild the flat_graph, which powers the 'graph' context variable
         self.build_flat_graph()
 
-        # log up to 5 items
-        sample = list(islice(merged, 5))
-        fire_event(MergedFromState(num_merged=len(merged), sample=sample))
-
     # Methods that were formerly in ParseResult
     def add_macro(self, source_file: SourceFile, macro: Macro):
         if macro.unique_id in self.macros:
             # detect that the macro exists and emit an error
             raise DuplicateMacroInPackageError(macro=macro, macro_mapping=self.macros)
 
         self.macros[macro.unique_id] = macro
```

### Comparing `dbt_core-1.8.0b3/dbt/contracts/graph/metrics.py` & `dbt_core-1.8.0rc1/dbt/contracts/graph/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/contracts/graph/model_config.py` & `dbt_core-1.8.0rc1/dbt/contracts/graph/model_config.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/contracts/graph/node_args.py` & `dbt_core-1.8.0rc1/dbt/contracts/graph/node_args.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/contracts/graph/nodes.py` & `dbt_core-1.8.0rc1/dbt/contracts/graph/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -873,14 +873,19 @@
         return False
 
     @property
     def language(self):
         return "sql"
 
 
+#    @property
+#    def compiled_code(self):
+#        return None
+
+
 # ====================================
 # Singular Test node
 # ====================================
 
 
 class TestShouldStoreFailures:
     @property
```

### Comparing `dbt_core-1.8.0b3/dbt/contracts/graph/semantic_manifest.py` & `dbt_core-1.8.0rc1/dbt/contracts/graph/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/contracts/graph/unparsed.py` & `dbt_core-1.8.0rc1/dbt/contracts/graph/unparsed.py`

 * *Files 4% similar despite different names*

```diff
@@ -265,14 +265,15 @@
     arguments: List[MacroArgument] = field(default_factory=list)
 
 
 @dataclass
 class UnparsedSourceTableDefinition(HasColumnTests, HasColumnAndTestProps):
     config: Dict[str, Any] = field(default_factory=dict)
     loaded_at_field: Optional[str] = None
+    loaded_at_field_present: Optional[bool] = None
     identifier: Optional[str] = None
     quoting: Quoting = field(default_factory=Quoting)
     freshness: Optional[FreshnessThreshold] = field(default_factory=FreshnessThreshold)
     external: Optional[ExternalTable] = None
     tags: List[str] = field(default_factory=list)
 
     def __post_serialize__(self, dct):
@@ -289,18 +290,30 @@
     meta: Dict[str, Any] = field(default_factory=dict)
     database: Optional[str] = None
     schema: Optional[str] = None
     loader: str = ""
     quoting: Quoting = field(default_factory=Quoting)
     freshness: Optional[FreshnessThreshold] = field(default_factory=FreshnessThreshold)
     loaded_at_field: Optional[str] = None
+    loaded_at_field_present: Optional[bool] = None
     tables: List[UnparsedSourceTableDefinition] = field(default_factory=list)
     tags: List[str] = field(default_factory=list)
     config: Dict[str, Any] = field(default_factory=dict)
 
+    @classmethod
+    def validate(cls, data):
+        super(UnparsedSourceDefinition, cls).validate(data)
+
+        if data.get("loaded_at_field", None) == "":
+            raise ValidationError("loaded_at_field cannot be an empty string.")
+        if "tables" in data:
+            for table in data["tables"]:
+                if table.get("loaded_at_field", None) == "":
+                    raise ValidationError("loaded_at_field cannot be an empty string.")
+
     @property
     def yaml_key(self) -> "str":
         return "sources"
 
     def __post_serialize__(self, dct):
         dct = super().__post_serialize__(dct)
         if "freshness" not in dct and self.freshness is None:
@@ -312,14 +325,15 @@
 class SourceTablePatch(dbtClassMixin):
     name: str
     description: Optional[str] = None
     meta: Optional[Dict[str, Any]] = None
     data_type: Optional[str] = None
     docs: Optional[Docs] = None
     loaded_at_field: Optional[str] = None
+    loaded_at_field_present: Optional[bool] = None
     identifier: Optional[str] = None
     quoting: Quoting = field(default_factory=Quoting)
     freshness: Optional[FreshnessThreshold] = field(default_factory=FreshnessThreshold)
     external: Optional[ExternalTable] = None
     tags: Optional[List[str]] = None
     data_tests: Optional[List[TestDef]] = None
     tests: Optional[List[TestDef]] = None  # back compat for previous name of 'data_tests'
@@ -354,14 +368,15 @@
     meta: Optional[Dict[str, Any]] = None
     database: Optional[str] = None
     schema: Optional[str] = None
     loader: Optional[str] = None
     quoting: Optional[Quoting] = None
     freshness: Optional[Optional[FreshnessThreshold]] = field(default_factory=FreshnessThreshold)
     loaded_at_field: Optional[str] = None
+    loaded_at_field_present: Optional[bool] = None
     tables: Optional[List[SourceTablePatch]] = None
     tags: Optional[List[str]] = None
 
     def to_patch_dict(self) -> Dict[str, Any]:
         dct = self.to_dict(omit_none=True)
         remove_keys = ("name", "overrides", "tables", "path")
         for key in remove_keys:
```

### Comparing `dbt_core-1.8.0b3/dbt/contracts/project.py` & `dbt_core-1.8.0rc1/dbt/contracts/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,21 +97,34 @@
 @dataclass
 class PackageConfig(dbtClassMixin):
     packages: List[PackageSpec]
 
     @classmethod
     def validate(cls, data):
         for package in data.get("packages", data):
+            # This can happen when the target is a variable that is not filled and results in hangs
+            if isinstance(package, dict):
+                if package.get("package") == "":
+                    raise ValidationError(
+                        "A hub package is missing the value. It is a required property."
+                    )
+                if package.get("local") == "":
+                    raise ValidationError(
+                        "A local package is missing the value. It is a required property."
+                    )
+                if package.get("git") == "":
+                    raise ValidationError(
+                        "A git package is missing the value. It is a required property."
+                    )
             if isinstance(package, dict) and package.get("package"):
                 if not package["version"]:
                     raise ValidationError(
                         f"{package['package']} is missing the version. When installing from the Hub "
                         "package index, version is a required property"
                     )
-
                 if "/" not in package["package"]:
                     raise ValidationError(
                         f"{package['package']} was not found in the package index. Packages on the index "
                         "require a namespace, e.g dbt-labs/dbt_utils"
                     )
         super().validate(data)
 
@@ -292,42 +305,46 @@
             deprecations.warn(
                 "project-test-config", deprecated_path="tests", exp_path="data_tests"
             )
 
 
 @dataclass
 class ProjectFlags(ExtensibleDbtClassMixin):
-    allow_spaces_in_model_names: Optional[bool] = True
     cache_selected_only: Optional[bool] = None
     debug: Optional[bool] = None
     fail_fast: Optional[bool] = None
     indirect_selection: Optional[str] = None
     log_format: Optional[str] = None
     log_format_file: Optional[str] = None
     log_level: Optional[str] = None
     log_level_file: Optional[str] = None
     partial_parse: Optional[bool] = None
     populate_cache: Optional[bool] = None
     printer_width: Optional[int] = None
     send_anonymous_usage_stats: bool = DEFAULT_SEND_ANONYMOUS_USAGE_STATS
-    source_freshness_run_project_hooks: bool = False
     static_parser: Optional[bool] = None
     use_colors: Optional[bool] = None
     use_colors_file: Optional[bool] = None
     use_experimental_parser: Optional[bool] = None
     version_check: Optional[bool] = None
     warn_error: Optional[bool] = None
     warn_error_options: Optional[Dict[str, Union[str, List[str]]]] = None
     write_json: Optional[bool] = None
 
+    # legacy behaviors
+    require_explicit_package_overrides_for_builtin_materializations: bool = True
+    require_resource_names_without_spaces: bool = False
+    source_freshness_run_project_hooks: bool = False
+
     @property
     def project_only_flags(self) -> Dict[str, Any]:
         return {
+            "require_explicit_package_overrides_for_builtin_materializations": self.require_explicit_package_overrides_for_builtin_materializations,
+            "require_resource_names_without_spaces": self.require_resource_names_without_spaces,
             "source_freshness_run_project_hooks": self.source_freshness_run_project_hooks,
-            "allow_spaces_in_model_names": self.allow_spaces_in_model_names,
         }
 
 
 @dataclass
 class ProfileConfig(dbtClassMixin):
     profile_name: str
     target_name: str
```

### Comparing `dbt_core-1.8.0b3/dbt/contracts/results.py` & `dbt_core-1.8.0rc1/dbt/contracts/results.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/contracts/selection.py` & `dbt_core-1.8.0rc1/dbt/contracts/selection.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/contracts/sql.py` & `dbt_core-1.8.0rc1/dbt/contracts/sql.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/contracts/state.py` & `dbt_core-1.8.0rc1/dbt/contracts/state.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/contracts/util.py` & `dbt_core-1.8.0rc1/dbt/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/deprecations.py` & `dbt_core-1.8.0rc1/dbt/deprecations.py`

 * *Files 10% similar despite different names*

```diff
@@ -114,14 +114,29 @@
             # We can't do warn_or_error because the ProjectFlags
             # is where that is set up and we're just reading it.
             fire_event(event)
             self.track_deprecation_warn()
             active_deprecations.add(self.name)
 
 
+class PackageMaterializationOverrideDeprecation(DBTDeprecation):
+    _name = "package-materialization-override"
+    _event = "PackageMaterializationOverrideDeprecation"
+
+
+class ResourceNamesWithSpacesDeprecation(DBTDeprecation):
+    _name = "resource-names-with-spaces"
+    _event = "ResourceNamesWithSpacesDeprecation"
+
+
+class SourceFreshnessProjectHooksNotRun(DBTDeprecation):
+    _name = "source-freshness-project-hooks"
+    _event = "SourceFreshnessProjectHooksNotRun"
+
+
 def renamed_env_var(old_name: str, new_name: str):
     class EnvironmentVariableRenamed(DBTDeprecation):
         _name = f"environment-variable-renamed:{old_name}"
         _event = "EnvironmentVariableRenamed"
 
     dep = EnvironmentVariableRenamed()
     deprecations_list.append(dep)
@@ -153,14 +168,17 @@
     ConfigDataPathDeprecation(),
     ExposureNameDeprecation(),
     ConfigLogPathDeprecation(),
     ConfigTargetPathDeprecation(),
     CollectFreshnessReturnSignature(),
     TestsConfigDeprecation(),
     ProjectFlagsMovedDeprecation(),
+    PackageMaterializationOverrideDeprecation(),
+    ResourceNamesWithSpacesDeprecation(),
+    SourceFreshnessProjectHooksNotRun(),
 ]
 
 deprecations: Dict[str, DBTDeprecation] = {d.name: d for d in deprecations_list}
 
 
 def reset_deprecations():
     active_deprecations.clear()
```

### Comparing `dbt_core-1.8.0b3/dbt/deps/base.py` & `dbt_core-1.8.0rc1/dbt/deps/base.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/deps/git.py` & `dbt_core-1.8.0rc1/dbt/deps/git.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/deps/local.py` & `dbt_core-1.8.0rc1/dbt/deps/local.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/deps/registry.py` & `dbt_core-1.8.0rc1/dbt/deps/registry.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/deps/resolver.py` & `dbt_core-1.8.0rc1/dbt/deps/resolver.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/deps/tarball.py` & `dbt_core-1.8.0rc1/dbt/deps/tarball.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/docs/source/_ext/dbt_click.py` & `dbt_core-1.8.0rc1/dbt/docs/source/_ext/dbt_click.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/docs/source/conf.py` & `dbt_core-1.8.0rc1/dbt/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/events/base_types.py` & `dbt_core-1.8.0rc1/dbt/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/events/core_types_pb2.py` & `dbt_core-1.8.0rc1/dbt/events/core_types_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x63ore_types.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x99\x02\n\rCoreEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x05\x65xtra\x18\t \x03(\x0b\x32%.proto_types.CoreEventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"V\n\x0cNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x91\x02\n\x08NodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\rnode_relation\x18\n \x01(\x0b\x32\x19.proto_types.NodeRelation\"\x7f\n\rTimingInfoMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xd1\x01\n\x0cRunResultMsg\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x0btiming_info\x18\x03 \x03(\x0b\x32\x1a.proto_types.TimingInfoMsg\x12\x0e\n\x06thread\x18\x04 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x31\n\x10\x61\x64\x61pter_response\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"\\\n\nColumnType\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12\x1c\n\x14previous_column_type\x18\x02 \x01(\t\x12\x1b\n\x13\x63urrent_column_type\x18\x03 \x01(\t\"Y\n\x10\x43olumnConstraint\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63onstraint_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63onstraint_type\x18\x03 \x01(\t\"T\n\x0fModelConstraint\x12\x17\n\x0f\x63onstraint_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63onstraint_type\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\"9\n\x11MainReportVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0blog_version\x18\x02 \x01(\x05\"n\n\x14MainReportVersionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.MainReportVersion\"r\n\x0eMainReportArgs\x12\x33\n\x04\x61rgs\x18\x01 \x03(\x0b\x32%.proto_types.MainReportArgs.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"h\n\x11MainReportArgsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainReportArgs\"+\n\x15MainTrackingUserState\x12\x12\n\nuser_state\x18\x01 \x01(\t\"v\n\x18MainTrackingUserStateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainTrackingUserState\"5\n\x0fMergedFromState\x12\x12\n\nnum_merged\x18\x01 \x01(\x05\x12\x0e\n\x06sample\x18\x02 \x03(\t\"j\n\x12MergedFromStateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.MergedFromState\"A\n\x14MissingProfileTarget\x12\x14\n\x0cprofile_name\x18\x01 \x01(\t\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\"t\n\x17MissingProfileTargetMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MissingProfileTarget\"(\n\x11InvalidOptionYAML\x12\x13\n\x0boption_name\x18\x01 \x01(\t\"n\n\x14InvalidOptionYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InvalidOptionYAML\"!\n\x12LogDbtProjectError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x15LogDbtProjectErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProjectError\"3\n\x12LogDbtProfileError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08profiles\x18\x02 \x03(\t\"p\n\x15LogDbtProfileErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProfileError\"!\n\x12StarterProjectPath\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"p\n\x15StarterProjectPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StarterProjectPath\"$\n\x15\x43onfigFolderDirectory\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"v\n\x18\x43onfigFolderDirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConfigFolderDirectory\"\'\n\x14NoSampleProfileFound\x12\x0f\n\x07\x61\x64\x61pter\x18\x01 \x01(\t\"t\n\x17NoSampleProfileFoundMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NoSampleProfileFound\"6\n\x18ProfileWrittenWithSample\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"|\n\x1bProfileWrittenWithSampleMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProfileWrittenWithSample\"B\n$ProfileWrittenWithTargetTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x94\x01\n\'ProfileWrittenWithTargetTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.ProfileWrittenWithTargetTemplateYAML\"C\n%ProfileWrittenWithProjectTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x96\x01\n(ProfileWrittenWithProjectTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.ProfileWrittenWithProjectTemplateYAML\"\x12\n\x10SettingUpProfile\"l\n\x13SettingUpProfileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SettingUpProfile\"\x1c\n\x1aInvalidProfileTemplateYAML\"\x80\x01\n\x1dInvalidProfileTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.InvalidProfileTemplateYAML\"(\n\x18ProjectNameAlreadyExists\x12\x0c\n\x04name\x18\x01 \x01(\t\"|\n\x1bProjectNameAlreadyExistsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProjectNameAlreadyExists\"K\n\x0eProjectCreated\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocs_url\x18\x02 \x01(\t\x12\x11\n\tslack_url\x18\x03 \x01(\t\"h\n\x11ProjectCreatedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ProjectCreated\"@\n\x1aPackageRedirectDeprecation\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"\x80\x01\n\x1dPackageRedirectDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PackageRedirectDeprecation\"\x1f\n\x1dPackageInstallPathDeprecation\"\x86\x01\n PackageInstallPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.PackageInstallPathDeprecation\"H\n\x1b\x43onfigSourcePathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"\x82\x01\n\x1e\x43onfigSourcePathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigSourcePathDeprecation\"F\n\x19\x43onfigDataPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"~\n\x1c\x43onfigDataPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConfigDataPathDeprecation\".\n\x17MetricAttributesRenamed\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\"z\n\x1aMetricAttributesRenamedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.MetricAttributesRenamed\"+\n\x17\x45xposureNameDeprecation\x12\x10\n\x08\x65xposure\x18\x01 \x01(\t\"z\n\x1a\x45xposureNameDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.ExposureNameDeprecation\"^\n\x13InternalDeprecation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x18\n\x10suggested_action\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"r\n\x16InternalDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.InternalDeprecation\"@\n\x1a\x45nvironmentVariableRenamed\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"\x80\x01\n\x1d\x45nvironmentVariableRenamedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.EnvironmentVariableRenamed\"3\n\x18\x43onfigLogPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"|\n\x1b\x43onfigLogPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ConfigLogPathDeprecation\"6\n\x1b\x43onfigTargetPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"\x82\x01\n\x1e\x43onfigTargetPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigTargetPathDeprecation\"C\n\x16TestsConfigDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"x\n\x19TestsConfigDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.TestsConfigDeprecation\"\x1e\n\x1cProjectFlagsMovedDeprecation\"\x84\x01\n\x1fProjectFlagsMovedDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.ProjectFlagsMovedDeprecation\"X\n\x1cSpacesInModelNameDeprecation\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\r\n\x05level\x18\x03 \x01(\t\"\x84\x01\n\x1fSpacesInModelNameDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.SpacesInModelNameDeprecation\"k\n$TotalModelNamesWithSpacesDeprecation\x12\x1b\n\x13\x63ount_invalid_names\x18\x01 \x01(\x05\x12\x17\n\x0fshow_debug_hint\x18\x02 \x01(\x08\x12\r\n\x05level\x18\x03 \x01(\t\"\x94\x01\n\'TotalModelNamesWithSpacesDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.TotalModelNamesWithSpacesDeprecation\"V\n\x0f\x44\x65precatedModel\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65precation_date\x18\x03 \x01(\t\"j\n\x12\x44\x65precatedModelMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DeprecatedModel\"7\n\x12InputFileDiffError\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"p\n\x15InputFileDiffErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InputFileDiffError\"?\n\x14InvalidValueForField\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_value\x18\x02 \x01(\t\"t\n\x17InvalidValueForFieldMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.InvalidValueForField\"Q\n\x11ValidationWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12\x11\n\tnode_name\x18\x03 \x01(\t\"n\n\x14ValidationWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ValidationWarning\"!\n\x11ParsePerfInfoPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"n\n\x14ParsePerfInfoPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ParsePerfInfoPath\"1\n!PartialParsingErrorProcessingFile\x12\x0c\n\x04\x66ile\x18\x01 \x01(\t\"\x8e\x01\n$PartialParsingErrorProcessingFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.PartialParsingErrorProcessingFile\"\x86\x01\n\x13PartialParsingError\x12?\n\x08\x65xc_info\x18\x01 \x03(\x0b\x32-.proto_types.PartialParsingError.ExcInfoEntry\x1a.\n\x0c\x45xcInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x16PartialParsingErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.PartialParsingError\"\x1b\n\x19PartialParsingSkipParsing\"~\n\x1cPartialParsingSkipParsingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.PartialParsingSkipParsing\"&\n\x14UnableToPartialParse\x12\x0e\n\x06reason\x18\x01 \x01(\t\"t\n\x17UnableToPartialParseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.UnableToPartialParse\"f\n\x12StateCheckVarsHash\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\x12\x0c\n\x04vars\x18\x02 \x01(\t\x12\x0f\n\x07profile\x18\x03 \x01(\t\x12\x0e\n\x06target\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\"p\n\x15StateCheckVarsHashMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StateCheckVarsHash\"\x1a\n\x18PartialParsingNotEnabled\"|\n\x1bPartialParsingNotEnabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.PartialParsingNotEnabled\"C\n\x14ParsedFileLoadFailed\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"t\n\x17ParsedFileLoadFailedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParsedFileLoadFailed\"H\n\x15PartialParsingEnabled\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x05\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hanged\x18\x03 \x01(\x05\"v\n\x18PartialParsingEnabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.PartialParsingEnabled\"8\n\x12PartialParsingFile\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\"p\n\x15PartialParsingFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.PartialParsingFile\"\xaf\x01\n\x1fInvalidDisabledTargetInTestNode\x12\x1b\n\x13resource_type_title\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1a\n\x12original_file_path\x18\x03 \x01(\t\x12\x13\n\x0btarget_kind\x18\x04 \x01(\t\x12\x13\n\x0btarget_name\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\"\x8a\x01\n\"InvalidDisabledTargetInTestNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.InvalidDisabledTargetInTestNode\"7\n\x18UnusedResourceConfigPath\x12\x1b\n\x13unused_config_paths\x18\x01 \x03(\t\"|\n\x1bUnusedResourceConfigPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.UnusedResourceConfigPath\"3\n\rSeedIncreased\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"f\n\x10SeedIncreasedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.SeedIncreased\">\n\x18SeedExceedsLimitSamePath\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"|\n\x1bSeedExceedsLimitSamePathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.SeedExceedsLimitSamePath\"D\n\x1eSeedExceedsLimitAndPathChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x88\x01\n!SeedExceedsLimitAndPathChangedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.SeedExceedsLimitAndPathChanged\"\\\n\x1fSeedExceedsLimitChecksumChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rchecksum_name\x18\x03 \x01(\t\"\x8a\x01\n\"SeedExceedsLimitChecksumChangedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SeedExceedsLimitChecksumChanged\"%\n\x0cUnusedTables\x12\x15\n\runused_tables\x18\x01 \x03(\t\"d\n\x0fUnusedTablesMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.UnusedTables\"\x87\x01\n\x17WrongResourceSchemaFile\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x1c\n\x14plural_resource_type\x18\x03 \x01(\t\x12\x10\n\x08yaml_key\x18\x04 \x01(\t\x12\x11\n\tfile_path\x18\x05 \x01(\t\"z\n\x1aWrongResourceSchemaFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.WrongResourceSchemaFile\"K\n\x10NoNodeForYamlKey\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x10\n\x08yaml_key\x18\x02 \x01(\t\x12\x11\n\tfile_path\x18\x03 \x01(\t\"l\n\x13NoNodeForYamlKeyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.NoNodeForYamlKey\"+\n\x15MacroNotFoundForPatch\x12\x12\n\npatch_name\x18\x01 \x01(\t\"v\n\x18MacroNotFoundForPatchMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MacroNotFoundForPatch\"\xb8\x01\n\x16NodeNotFoundOrDisabled\x12\x1a\n\x12original_file_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1b\n\x13resource_type_title\x18\x03 \x01(\t\x12\x13\n\x0btarget_name\x18\x04 \x01(\t\x12\x13\n\x0btarget_kind\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\x12\x10\n\x08\x64isabled\x18\x07 \x01(\t\"x\n\x19NodeNotFoundOrDisabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.NodeNotFoundOrDisabled\"H\n\x0fJinjaLogWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"j\n\x12JinjaLogWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.JinjaLogWarning\"E\n\x0cJinjaLogInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"d\n\x0fJinjaLogInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.JinjaLogInfo\"F\n\rJinjaLogDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"f\n\x10JinjaLogDebugMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.JinjaLogDebug\"\xae\x01\n\x1eUnpinnedRefNewVersionAvailable\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rref_node_name\x18\x02 \x01(\t\x12\x18\n\x10ref_node_package\x18\x03 \x01(\t\x12\x18\n\x10ref_node_version\x18\x04 \x01(\t\x12\x17\n\x0fref_max_version\x18\x05 \x01(\t\"\x88\x01\n!UnpinnedRefNewVersionAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.UnpinnedRefNewVersionAvailable\"\xc6\x01\n\x1cUpcomingReferenceDeprecation\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"\x84\x01\n\x1fUpcomingReferenceDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.UpcomingReferenceDeprecation\"\xbd\x01\n\x13\x44\x65precatedReference\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"r\n\x16\x44\x65precatedReferenceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DeprecatedReference\"<\n$UnsupportedConstraintMaterialization\x12\x14\n\x0cmaterialized\x18\x01 \x01(\t\"\x94\x01\n\'UnsupportedConstraintMaterializationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.UnsupportedConstraintMaterialization\"M\n\x14ParseInlineNodeError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\"t\n\x17ParseInlineNodeErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParseInlineNodeError\"(\n\x19SemanticValidationFailure\x12\x0b\n\x03msg\x18\x02 \x01(\t\"~\n\x1cSemanticValidationFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.SemanticValidationFailure\"\x8a\x03\n\x19UnversionedBreakingChange\x12\x18\n\x10\x62reaking_changes\x18\x01 \x03(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x17\n\x0fmodel_file_path\x18\x03 \x01(\t\x12\"\n\x1a\x63ontract_enforced_disabled\x18\x04 \x01(\x08\x12\x17\n\x0f\x63olumns_removed\x18\x05 \x03(\t\x12\x34\n\x13\x63olumn_type_changes\x18\x06 \x03(\x0b\x32\x17.proto_types.ColumnType\x12I\n\"enforced_column_constraint_removed\x18\x07 \x03(\x0b\x32\x1d.proto_types.ColumnConstraint\x12G\n!enforced_model_constraint_removed\x18\x08 \x03(\x0b\x32\x1c.proto_types.ModelConstraint\x12\x1f\n\x17materialization_changed\x18\t \x03(\t\"~\n\x1cUnversionedBreakingChangeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.UnversionedBreakingChange\"*\n\x14WarnStateTargetEqual\x12\x12\n\nstate_path\x18\x01 \x01(\t\"t\n\x17WarnStateTargetEqualMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.WarnStateTargetEqual\"%\n\x16\x46reshnessConfigProblem\x12\x0b\n\x03msg\x18\x01 \x01(\t\"x\n\x19\x46reshnessConfigProblemMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessConfigProblem\"/\n\x1dGitSparseCheckoutSubdirectory\x12\x0e\n\x06subdir\x18\x01 \x01(\t\"\x86\x01\n GitSparseCheckoutSubdirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.GitSparseCheckoutSubdirectory\"/\n\x1bGitProgressCheckoutRevision\x12\x10\n\x08revision\x18\x01 \x01(\t\"\x82\x01\n\x1eGitProgressCheckoutRevisionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.GitProgressCheckoutRevision\"4\n%GitProgressUpdatingExistingDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x96\x01\n(GitProgressUpdatingExistingDependencyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.GitProgressUpdatingExistingDependency\".\n\x1fGitProgressPullingNewDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x8a\x01\n\"GitProgressPullingNewDependencyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressPullingNewDependency\"\x1d\n\x0eGitNothingToDo\x12\x0b\n\x03sha\x18\x01 \x01(\t\"h\n\x11GitNothingToDoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.GitNothingToDo\"E\n\x1fGitProgressUpdatedCheckoutRange\x12\x11\n\tstart_sha\x18\x01 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x02 \x01(\t\"\x8a\x01\n\"GitProgressUpdatedCheckoutRangeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressUpdatedCheckoutRange\"*\n\x17GitProgressCheckedOutAt\x12\x0f\n\x07\x65nd_sha\x18\x01 \x01(\t\"z\n\x1aGitProgressCheckedOutAtMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.GitProgressCheckedOutAt\")\n\x1aRegistryProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x80\x01\n\x1dRegistryProgressGETRequestMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.RegistryProgressGETRequest\"=\n\x1bRegistryProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x82\x01\n\x1eRegistryProgressGETResponseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RegistryProgressGETResponse\"_\n\x1dSelectorReportInvalidSelector\x12\x17\n\x0fvalid_selectors\x18\x01 \x01(\t\x12\x13\n\x0bspec_method\x18\x02 \x01(\t\x12\x10\n\x08raw_spec\x18\x03 \x01(\t\"\x86\x01\n SelectorReportInvalidSelectorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.SelectorReportInvalidSelector\"\x15\n\x13\x44\x65psNoPackagesFound\"r\n\x16\x44\x65psNoPackagesFoundMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsNoPackagesFound\"/\n\x17\x44\x65psStartPackageInstall\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"z\n\x1a\x44\x65psStartPackageInstallMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsStartPackageInstall\"\'\n\x0f\x44\x65psInstallInfo\x12\x14\n\x0cversion_name\x18\x01 \x01(\t\"j\n\x12\x44\x65psInstallInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DepsInstallInfo\"-\n\x13\x44\x65psUpdateAvailable\x12\x16\n\x0eversion_latest\x18\x01 \x01(\t\"r\n\x16\x44\x65psUpdateAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsUpdateAvailable\"\x0e\n\x0c\x44\x65psUpToDate\"d\n\x0f\x44\x65psUpToDateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUpToDate\",\n\x14\x44\x65psListSubdirectory\x12\x14\n\x0csubdirectory\x18\x01 \x01(\t\"t\n\x17\x44\x65psListSubdirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.DepsListSubdirectory\".\n\x1a\x44\x65psNotifyUpdatesAvailable\x12\x10\n\x08packages\x18\x01 \x03(\t\"\x80\x01\n\x1d\x44\x65psNotifyUpdatesAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.DepsNotifyUpdatesAvailable\".\n\x1fRegistryIndexProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x8a\x01\n\"RegistryIndexProgressGETRequestMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryIndexProgressGETRequest\"B\n RegistryIndexProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x8c\x01\n#RegistryIndexProgressGETResponseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12;\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32-.proto_types.RegistryIndexProgressGETResponse\"2\n\x1eRegistryResponseUnexpectedType\x12\x10\n\x08response\x18\x01 \x01(\t\"\x88\x01\n!RegistryResponseUnexpectedTypeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseUnexpectedType\"2\n\x1eRegistryResponseMissingTopKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x88\x01\n!RegistryResponseMissingTopKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseMissingTopKeys\"5\n!RegistryResponseMissingNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8e\x01\n$RegistryResponseMissingNestedKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.RegistryResponseMissingNestedKeys\"3\n\x1fRegistryResponseExtraNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8a\x01\n\"RegistryResponseExtraNestedKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryResponseExtraNestedKeys\"(\n\x18\x44\x65psSetDownloadDirectory\x12\x0c\n\x04path\x18\x01 \x01(\t\"|\n\x1b\x44\x65psSetDownloadDirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsSetDownloadDirectory\"-\n\x0c\x44\x65psUnpinned\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0b\n\x03git\x18\x02 \x01(\t\"d\n\x0f\x44\x65psUnpinnedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUnpinned\"/\n\x1bNoNodesForSelectionCriteria\x12\x10\n\x08spec_raw\x18\x01 \x01(\t\"\x82\x01\n\x1eNoNodesForSelectionCriteriaMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.NoNodesForSelectionCriteria\")\n\x10\x44\x65psLockUpdating\x12\x15\n\rlock_filepath\x18\x01 \x01(\t\"l\n\x13\x44\x65psLockUpdatingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.DepsLockUpdating\"R\n\x0e\x44\x65psAddPackage\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x19\n\x11packages_filepath\x18\x03 \x01(\t\"h\n\x11\x44\x65psAddPackageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DepsAddPackage\"\xa7\x01\n\x19\x44\x65psFoundDuplicatePackage\x12S\n\x0fremoved_package\x18\x01 \x03(\x0b\x32:.proto_types.DepsFoundDuplicatePackage.RemovedPackageEntry\x1a\x35\n\x13RemovedPackageEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"~\n\x1c\x44\x65psFoundDuplicatePackageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.DepsFoundDuplicatePackage\"$\n\x12\x44\x65psVersionMissing\x12\x0e\n\x06source\x18\x01 \x01(\t\"p\n\x15\x44\x65psVersionMissingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.DepsVersionMissing\"/\n\x17\x44\x65psScrubbedPackageName\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"z\n\x1a\x44\x65psScrubbedPackageNameMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsScrubbedPackageName\"*\n\x1bRunningOperationCaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x82\x01\n\x1eRunningOperationCaughtErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RunningOperationCaughtError\"\x11\n\x0f\x43ompileComplete\"j\n\x12\x43ompileCompleteMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.CompileComplete\"\x18\n\x16\x46reshnessCheckComplete\"x\n\x19\x46reshnessCheckCompleteMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessCheckComplete\"\x1c\n\nSeedHeader\x12\x0e\n\x06header\x18\x01 \x01(\t\"`\n\rSeedHeaderMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SeedHeader\"]\n\x12SQLRunnerException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x02 \x01(\t\x12(\n\tnode_info\x18\x03 \x01(\x0b\x32\x15.proto_types.NodeInfo\"p\n\x15SQLRunnerExceptionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SQLRunnerException\"\xa8\x01\n\rLogTestResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x12\n\nnum_models\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"f\n\x10LogTestResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogTestResult\"k\n\x0cLogStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"d\n\x0fLogStartLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.LogStartLine\"\x95\x01\n\x0eLogModelResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"h\n\x11LogModelResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogModelResult\"\x92\x02\n\x11LogSnapshotResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x34\n\x03\x63\x66g\x18\x07 \x03(\x0b\x32\'.proto_types.LogSnapshotResult.CfgEntry\x12\x16\n\x0eresult_message\x18\x08 \x01(\t\x1a*\n\x08\x43\x66gEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"n\n\x14LogSnapshotResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogSnapshotResult\"\xb9\x01\n\rLogSeedResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x16\n\x0eresult_message\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12\x10\n\x08relation\x18\x08 \x01(\t\"f\n\x10LogSeedResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogSeedResult\"\xad\x01\n\x12LogFreshnessResult\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x13\n\x0bsource_name\x18\x06 \x01(\t\x12\x12\n\ntable_name\x18\x07 \x01(\t\"p\n\x15LogFreshnessResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogFreshnessResult\"\x98\x01\n\x11LogNodeNoOpResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"n\n\x14LogNodeNoOpResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogNodeNoOpResult\"\"\n\rLogCancelLine\x12\x11\n\tconn_name\x18\x01 \x01(\t\"f\n\x10LogCancelLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogCancelLine\"\x1f\n\x0f\x44\x65\x66\x61ultSelector\x12\x0c\n\x04name\x18\x01 \x01(\t\"j\n\x12\x44\x65\x66\x61ultSelectorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DefaultSelector\"5\n\tNodeStart\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"^\n\x0cNodeStartMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.NodeStart\"g\n\x0cNodeFinished\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12-\n\nrun_result\x18\x02 \x01(\x0b\x32\x19.proto_types.RunResultMsg\"d\n\x0fNodeFinishedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.NodeFinished\"+\n\x1bQueryCancelationUnsupported\x12\x0c\n\x04type\x18\x01 \x01(\t\"\x82\x01\n\x1eQueryCancelationUnsupportedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.QueryCancelationUnsupported\"O\n\x0f\x43oncurrencyLine\x12\x13\n\x0bnum_threads\x18\x01 \x01(\x05\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\x12\x12\n\nnode_count\x18\x03 \x01(\x05\"j\n\x12\x43oncurrencyLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ConcurrencyLine\"E\n\x19WritingInjectedSQLForNode\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"~\n\x1cWritingInjectedSQLForNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.WritingInjectedSQLForNode\"9\n\rNodeCompiling\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"f\n\x10NodeCompilingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeCompiling\"9\n\rNodeExecuting\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"f\n\x10NodeExecutingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeExecuting\"m\n\x10LogHookStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"l\n\x13LogHookStartLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.LogHookStartLine\"\x93\x01\n\x0eLogHookEndLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"h\n\x11LogHookEndLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogHookEndLine\"\x93\x01\n\x0fSkippingDetails\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x11\n\tnode_name\x18\x04 \x01(\t\x12\r\n\x05index\x18\x05 \x01(\x05\x12\r\n\x05total\x18\x06 \x01(\x05\"j\n\x12SkippingDetailsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SkippingDetails\"\r\n\x0bNothingToDo\"b\n\x0eNothingToDoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.NothingToDo\",\n\x1dRunningOperationUncaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x86\x01\n RunningOperationUncaughtErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.RunningOperationUncaughtError\"\x93\x01\n\x0c\x45ndRunResult\x12*\n\x07results\x18\x01 \x03(\x0b\x32\x19.proto_types.RunResultMsg\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x02\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07success\x18\x04 \x01(\x08\"d\n\x0f\x45ndRunResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.EndRunResult\"\x11\n\x0fNoNodesSelected\"j\n\x12NoNodesSelectedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.NoNodesSelected\"w\n\x10\x43ommandCompleted\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x65lapsed\x18\x04 \x01(\x02\"l\n\x13\x43ommandCompletedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.CommandCompleted\"k\n\x08ShowNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0f\n\x07preview\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"\\\n\x0bShowNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.ShowNode\"p\n\x0c\x43ompiledNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x10\n\x08\x63ompiled\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"d\n\x0f\x43ompiledNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.CompiledNode\"b\n\x17\x43\x61tchableExceptionOnRun\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"z\n\x1a\x43\x61tchableExceptionOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.CatchableExceptionOnRun\"_\n\x12InternalErrorOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12(\n\tnode_info\x18\x03 \x01(\x0b\x32\x15.proto_types.NodeInfo\"p\n\x15InternalErrorOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InternalErrorOnRun\"u\n\x15GenericExceptionOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"v\n\x18GenericExceptionOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.GenericExceptionOnRun\"N\n\x1aNodeConnectionReleaseError\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"\x80\x01\n\x1dNodeConnectionReleaseErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.NodeConnectionReleaseError\"\x1f\n\nFoundStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\"`\n\rFoundStatsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.FoundStats\"\x17\n\x15MainKeyboardInterrupt\"v\n\x18MainKeyboardInterruptMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainKeyboardInterrupt\"#\n\x14MainEncounteredError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"t\n\x17MainEncounteredErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MainEncounteredError\"%\n\x0eMainStackTrace\x12\x13\n\x0bstack_trace\x18\x01 \x01(\t\"h\n\x11MainStackTraceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainStackTrace\"p\n\x13TimingInfoCollected\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12/\n\x0btiming_info\x18\x02 \x01(\x0b\x32\x1a.proto_types.TimingInfoMsg\"r\n\x16TimingInfoCollectedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.TimingInfoCollected\"&\n\x12LogDebugStackTrace\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"p\n\x15LogDebugStackTraceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDebugStackTrace\"\x1e\n\x0e\x43heckCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"h\n\x11\x43heckCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CheckCleanPath\" \n\x10\x43onfirmCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"l\n\x13\x43onfirmCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConfirmCleanPath\"\"\n\x12ProtectedCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"p\n\x15ProtectedCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ProtectedCleanPath\"\x14\n\x12\x46inishedCleanPaths\"p\n\x15\x46inishedCleanPathsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FinishedCleanPaths\"5\n\x0bOpenCommand\x12\x10\n\x08open_cmd\x18\x01 \x01(\t\x12\x14\n\x0cprofiles_dir\x18\x02 \x01(\t\"b\n\x0eOpenCommandMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.OpenCommand\"0\n\x0fServingDocsPort\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"j\n\x12ServingDocsPortMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ServingDocsPort\"%\n\x15ServingDocsAccessInfo\x12\x0c\n\x04port\x18\x01 \x01(\t\"v\n\x18ServingDocsAccessInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ServingDocsAccessInfo\"\x15\n\x13ServingDocsExitInfo\"r\n\x16ServingDocsExitInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.ServingDocsExitInfo\"t\n\x10RunResultWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"l\n\x13RunResultWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultWarning\"t\n\x10RunResultFailure\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"l\n\x13RunResultFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultFailure\"k\n\tStatsLine\x12\x30\n\x05stats\x18\x01 \x03(\x0b\x32!.proto_types.StatsLine.StatsEntry\x1a,\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"^\n\x0cStatsLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.StatsLine\"G\n\x0eRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"h\n\x11RunResultErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RunResultError\"S\n\x17RunResultErrorNoMessage\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1aRunResultErrorNoMessageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultErrorNoMessage\"I\n\x0fSQLCompiledPath\x12\x0c\n\x04path\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"j\n\x12SQLCompiledPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SQLCompiledPath\"W\n\x14\x43heckNodeTestFailure\x12\x15\n\rrelation_name\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"t\n\x17\x43heckNodeTestFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.CheckNodeTestFailure\"W\n\x0f\x45ndOfRunSummary\x12\x12\n\nnum_errors\x18\x01 \x01(\x05\x12\x14\n\x0cnum_warnings\x18\x02 \x01(\x05\x12\x1a\n\x12keyboard_interrupt\x18\x03 \x01(\x08\"j\n\x12\x45ndOfRunSummaryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.EndOfRunSummary\"U\n\x13LogSkipBecauseError\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x10\n\x08relation\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"r\n\x16LogSkipBecauseErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.LogSkipBecauseError\"\x14\n\x12\x45nsureGitInstalled\"p\n\x15\x45nsureGitInstalledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.EnsureGitInstalled\"\x1a\n\x18\x44\x65psCreatingLocalSymlink\"|\n\x1b\x44\x65psCreatingLocalSymlinkMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsCreatingLocalSymlink\"\x19\n\x17\x44\x65psSymlinkNotAvailable\"z\n\x1a\x44\x65psSymlinkNotAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsSymlinkNotAvailable\"\x11\n\x0f\x44isableTracking\"j\n\x12\x44isableTrackingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DisableTracking\"\x1e\n\x0cSendingEvent\x12\x0e\n\x06kwargs\x18\x01 \x01(\t\"d\n\x0fSendingEventMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SendingEvent\"\x12\n\x10SendEventFailure\"l\n\x13SendEventFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SendEventFailure\"\r\n\x0b\x46lushEvents\"b\n\x0e\x46lushEventsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.FlushEvents\"\x14\n\x12\x46lushEventsFailure\"p\n\x15\x46lushEventsFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FlushEventsFailure\"-\n\x19TrackingInitializeFailure\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"~\n\x1cTrackingInitializeFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.TrackingInitializeFailure\"P\n\x17RunResultWarningMessage\x12\x0b\n\x03msg\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1aRunResultWarningMessageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultWarningMessage\"\x1a\n\x0b\x44\x65\x62ugCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"b\n\x0e\x44\x65\x62ugCmdOutMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.DebugCmdOut\"\x1d\n\x0e\x44\x65\x62ugCmdResult\x12\x0b\n\x03msg\x18\x01 \x01(\t\"h\n\x11\x44\x65\x62ugCmdResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DebugCmdResult\"\x19\n\nListCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"`\n\rListCmdOutMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.ListCmdOut\"\xec\x01\n\x0eResourceReport\x12\x14\n\x0c\x63ommand_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ommand_success\x18\x03 \x01(\x08\x12\x1f\n\x17\x63ommand_wall_clock_time\x18\x04 \x01(\x02\x12\x19\n\x11process_user_time\x18\x05 \x01(\x02\x12\x1b\n\x13process_kernel_time\x18\x06 \x01(\x02\x12\x1b\n\x13process_mem_max_rss\x18\x07 \x01(\x03\x12\x19\n\x11process_in_blocks\x18\x08 \x01(\x03\x12\x1a\n\x12process_out_blocks\x18\t \x01(\x03\"h\n\x11ResourceReportMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ResourceReportb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x63ore_types.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x99\x02\n\rCoreEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x05\x65xtra\x18\t \x03(\x0b\x32%.proto_types.CoreEventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"V\n\x0cNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x91\x02\n\x08NodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\rnode_relation\x18\n \x01(\x0b\x32\x19.proto_types.NodeRelation\"\x7f\n\rTimingInfoMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xd1\x01\n\x0cRunResultMsg\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x0btiming_info\x18\x03 \x03(\x0b\x32\x1a.proto_types.TimingInfoMsg\x12\x0e\n\x06thread\x18\x04 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x31\n\x10\x61\x64\x61pter_response\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"\\\n\nColumnType\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12\x1c\n\x14previous_column_type\x18\x02 \x01(\t\x12\x1b\n\x13\x63urrent_column_type\x18\x03 \x01(\t\"Y\n\x10\x43olumnConstraint\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63onstraint_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63onstraint_type\x18\x03 \x01(\t\"T\n\x0fModelConstraint\x12\x17\n\x0f\x63onstraint_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63onstraint_type\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\"9\n\x11MainReportVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0blog_version\x18\x02 \x01(\x05\"n\n\x14MainReportVersionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.MainReportVersion\"r\n\x0eMainReportArgs\x12\x33\n\x04\x61rgs\x18\x01 \x03(\x0b\x32%.proto_types.MainReportArgs.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"h\n\x11MainReportArgsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainReportArgs\"+\n\x15MainTrackingUserState\x12\x12\n\nuser_state\x18\x01 \x01(\t\"v\n\x18MainTrackingUserStateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainTrackingUserState\"5\n\x0fMergedFromState\x12\x12\n\nnum_merged\x18\x01 \x01(\x05\x12\x0e\n\x06sample\x18\x02 \x03(\t\"j\n\x12MergedFromStateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.MergedFromState\"A\n\x14MissingProfileTarget\x12\x14\n\x0cprofile_name\x18\x01 \x01(\t\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\"t\n\x17MissingProfileTargetMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MissingProfileTarget\"(\n\x11InvalidOptionYAML\x12\x13\n\x0boption_name\x18\x01 \x01(\t\"n\n\x14InvalidOptionYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InvalidOptionYAML\"!\n\x12LogDbtProjectError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x15LogDbtProjectErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProjectError\"3\n\x12LogDbtProfileError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08profiles\x18\x02 \x03(\t\"p\n\x15LogDbtProfileErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProfileError\"!\n\x12StarterProjectPath\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"p\n\x15StarterProjectPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StarterProjectPath\"$\n\x15\x43onfigFolderDirectory\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"v\n\x18\x43onfigFolderDirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConfigFolderDirectory\"\'\n\x14NoSampleProfileFound\x12\x0f\n\x07\x61\x64\x61pter\x18\x01 \x01(\t\"t\n\x17NoSampleProfileFoundMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NoSampleProfileFound\"6\n\x18ProfileWrittenWithSample\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"|\n\x1bProfileWrittenWithSampleMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProfileWrittenWithSample\"B\n$ProfileWrittenWithTargetTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x94\x01\n\'ProfileWrittenWithTargetTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.ProfileWrittenWithTargetTemplateYAML\"C\n%ProfileWrittenWithProjectTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x96\x01\n(ProfileWrittenWithProjectTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.ProfileWrittenWithProjectTemplateYAML\"\x12\n\x10SettingUpProfile\"l\n\x13SettingUpProfileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SettingUpProfile\"\x1c\n\x1aInvalidProfileTemplateYAML\"\x80\x01\n\x1dInvalidProfileTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.InvalidProfileTemplateYAML\"(\n\x18ProjectNameAlreadyExists\x12\x0c\n\x04name\x18\x01 \x01(\t\"|\n\x1bProjectNameAlreadyExistsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProjectNameAlreadyExists\"K\n\x0eProjectCreated\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocs_url\x18\x02 \x01(\t\x12\x11\n\tslack_url\x18\x03 \x01(\t\"h\n\x11ProjectCreatedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ProjectCreated\"@\n\x1aPackageRedirectDeprecation\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"\x80\x01\n\x1dPackageRedirectDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PackageRedirectDeprecation\"\x1f\n\x1dPackageInstallPathDeprecation\"\x86\x01\n PackageInstallPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.PackageInstallPathDeprecation\"H\n\x1b\x43onfigSourcePathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"\x82\x01\n\x1e\x43onfigSourcePathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigSourcePathDeprecation\"F\n\x19\x43onfigDataPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"~\n\x1c\x43onfigDataPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConfigDataPathDeprecation\".\n\x17MetricAttributesRenamed\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\"z\n\x1aMetricAttributesRenamedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.MetricAttributesRenamed\"+\n\x17\x45xposureNameDeprecation\x12\x10\n\x08\x65xposure\x18\x01 \x01(\t\"z\n\x1a\x45xposureNameDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.ExposureNameDeprecation\"^\n\x13InternalDeprecation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x18\n\x10suggested_action\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"r\n\x16InternalDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.InternalDeprecation\"@\n\x1a\x45nvironmentVariableRenamed\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"\x80\x01\n\x1d\x45nvironmentVariableRenamedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.EnvironmentVariableRenamed\"3\n\x18\x43onfigLogPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"|\n\x1b\x43onfigLogPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ConfigLogPathDeprecation\"6\n\x1b\x43onfigTargetPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"\x82\x01\n\x1e\x43onfigTargetPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigTargetPathDeprecation\"C\n\x16TestsConfigDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"x\n\x19TestsConfigDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.TestsConfigDeprecation\"\x1e\n\x1cProjectFlagsMovedDeprecation\"\x84\x01\n\x1fProjectFlagsMovedDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.ProjectFlagsMovedDeprecation\"C\n\x1fSpacesInResourceNameDeprecation\x12\x11\n\tunique_id\x18\x01 \x01(\t\x12\r\n\x05level\x18\x02 \x01(\t\"\x8a\x01\n\"SpacesInResourceNameDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SpacesInResourceNameDeprecation\"i\n\"ResourceNamesWithSpacesDeprecation\x12\x1b\n\x13\x63ount_invalid_names\x18\x01 \x01(\x05\x12\x17\n\x0fshow_debug_hint\x18\x02 \x01(\x08\x12\r\n\x05level\x18\x03 \x01(\t\"\x90\x01\n%ResourceNamesWithSpacesDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12=\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32/.proto_types.ResourceNamesWithSpacesDeprecation\"_\n)PackageMaterializationOverrideDeprecation\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x1c\n\x14materialization_name\x18\x02 \x01(\t\"\x9e\x01\n,PackageMaterializationOverrideDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x44\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x36.proto_types.PackageMaterializationOverrideDeprecation\"#\n!SourceFreshnessProjectHooksNotRun\"\x8e\x01\n$SourceFreshnessProjectHooksNotRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.SourceFreshnessProjectHooksNotRun\"V\n\x0f\x44\x65precatedModel\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65precation_date\x18\x03 \x01(\t\"j\n\x12\x44\x65precatedModelMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DeprecatedModel\"7\n\x12InputFileDiffError\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"p\n\x15InputFileDiffErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InputFileDiffError\"?\n\x14InvalidValueForField\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_value\x18\x02 \x01(\t\"t\n\x17InvalidValueForFieldMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.InvalidValueForField\"Q\n\x11ValidationWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12\x11\n\tnode_name\x18\x03 \x01(\t\"n\n\x14ValidationWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ValidationWarning\"!\n\x11ParsePerfInfoPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"n\n\x14ParsePerfInfoPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ParsePerfInfoPath\"1\n!PartialParsingErrorProcessingFile\x12\x0c\n\x04\x66ile\x18\x01 \x01(\t\"\x8e\x01\n$PartialParsingErrorProcessingFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.PartialParsingErrorProcessingFile\"\x86\x01\n\x13PartialParsingError\x12?\n\x08\x65xc_info\x18\x01 \x03(\x0b\x32-.proto_types.PartialParsingError.ExcInfoEntry\x1a.\n\x0c\x45xcInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x16PartialParsingErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.PartialParsingError\"\x1b\n\x19PartialParsingSkipParsing\"~\n\x1cPartialParsingSkipParsingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.PartialParsingSkipParsing\"&\n\x14UnableToPartialParse\x12\x0e\n\x06reason\x18\x01 \x01(\t\"t\n\x17UnableToPartialParseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.UnableToPartialParse\"f\n\x12StateCheckVarsHash\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\x12\x0c\n\x04vars\x18\x02 \x01(\t\x12\x0f\n\x07profile\x18\x03 \x01(\t\x12\x0e\n\x06target\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\"p\n\x15StateCheckVarsHashMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StateCheckVarsHash\"\x1a\n\x18PartialParsingNotEnabled\"|\n\x1bPartialParsingNotEnabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.PartialParsingNotEnabled\"C\n\x14ParsedFileLoadFailed\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"t\n\x17ParsedFileLoadFailedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParsedFileLoadFailed\"H\n\x15PartialParsingEnabled\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x05\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hanged\x18\x03 \x01(\x05\"v\n\x18PartialParsingEnabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.PartialParsingEnabled\"8\n\x12PartialParsingFile\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\"p\n\x15PartialParsingFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.PartialParsingFile\"\xaf\x01\n\x1fInvalidDisabledTargetInTestNode\x12\x1b\n\x13resource_type_title\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1a\n\x12original_file_path\x18\x03 \x01(\t\x12\x13\n\x0btarget_kind\x18\x04 \x01(\t\x12\x13\n\x0btarget_name\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\"\x8a\x01\n\"InvalidDisabledTargetInTestNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.InvalidDisabledTargetInTestNode\"7\n\x18UnusedResourceConfigPath\x12\x1b\n\x13unused_config_paths\x18\x01 \x03(\t\"|\n\x1bUnusedResourceConfigPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.UnusedResourceConfigPath\"3\n\rSeedIncreased\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"f\n\x10SeedIncreasedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.SeedIncreased\">\n\x18SeedExceedsLimitSamePath\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"|\n\x1bSeedExceedsLimitSamePathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.SeedExceedsLimitSamePath\"D\n\x1eSeedExceedsLimitAndPathChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x88\x01\n!SeedExceedsLimitAndPathChangedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.SeedExceedsLimitAndPathChanged\"\\\n\x1fSeedExceedsLimitChecksumChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rchecksum_name\x18\x03 \x01(\t\"\x8a\x01\n\"SeedExceedsLimitChecksumChangedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SeedExceedsLimitChecksumChanged\"%\n\x0cUnusedTables\x12\x15\n\runused_tables\x18\x01 \x03(\t\"d\n\x0fUnusedTablesMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.UnusedTables\"\x87\x01\n\x17WrongResourceSchemaFile\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x1c\n\x14plural_resource_type\x18\x03 \x01(\t\x12\x10\n\x08yaml_key\x18\x04 \x01(\t\x12\x11\n\tfile_path\x18\x05 \x01(\t\"z\n\x1aWrongResourceSchemaFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.WrongResourceSchemaFile\"K\n\x10NoNodeForYamlKey\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x10\n\x08yaml_key\x18\x02 \x01(\t\x12\x11\n\tfile_path\x18\x03 \x01(\t\"l\n\x13NoNodeForYamlKeyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.NoNodeForYamlKey\"+\n\x15MacroNotFoundForPatch\x12\x12\n\npatch_name\x18\x01 \x01(\t\"v\n\x18MacroNotFoundForPatchMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MacroNotFoundForPatch\"\xb8\x01\n\x16NodeNotFoundOrDisabled\x12\x1a\n\x12original_file_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1b\n\x13resource_type_title\x18\x03 \x01(\t\x12\x13\n\x0btarget_name\x18\x04 \x01(\t\x12\x13\n\x0btarget_kind\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\x12\x10\n\x08\x64isabled\x18\x07 \x01(\t\"x\n\x19NodeNotFoundOrDisabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.NodeNotFoundOrDisabled\"H\n\x0fJinjaLogWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"j\n\x12JinjaLogWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.JinjaLogWarning\"E\n\x0cJinjaLogInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"d\n\x0fJinjaLogInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.JinjaLogInfo\"F\n\rJinjaLogDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"f\n\x10JinjaLogDebugMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.JinjaLogDebug\"\xae\x01\n\x1eUnpinnedRefNewVersionAvailable\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rref_node_name\x18\x02 \x01(\t\x12\x18\n\x10ref_node_package\x18\x03 \x01(\t\x12\x18\n\x10ref_node_version\x18\x04 \x01(\t\x12\x17\n\x0fref_max_version\x18\x05 \x01(\t\"\x88\x01\n!UnpinnedRefNewVersionAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.UnpinnedRefNewVersionAvailable\"\xc6\x01\n\x1cUpcomingReferenceDeprecation\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"\x84\x01\n\x1fUpcomingReferenceDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.UpcomingReferenceDeprecation\"\xbd\x01\n\x13\x44\x65precatedReference\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"r\n\x16\x44\x65precatedReferenceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DeprecatedReference\"<\n$UnsupportedConstraintMaterialization\x12\x14\n\x0cmaterialized\x18\x01 \x01(\t\"\x94\x01\n\'UnsupportedConstraintMaterializationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.UnsupportedConstraintMaterialization\"M\n\x14ParseInlineNodeError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\"t\n\x17ParseInlineNodeErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParseInlineNodeError\"(\n\x19SemanticValidationFailure\x12\x0b\n\x03msg\x18\x02 \x01(\t\"~\n\x1cSemanticValidationFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.SemanticValidationFailure\"\x8a\x03\n\x19UnversionedBreakingChange\x12\x18\n\x10\x62reaking_changes\x18\x01 \x03(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x17\n\x0fmodel_file_path\x18\x03 \x01(\t\x12\"\n\x1a\x63ontract_enforced_disabled\x18\x04 \x01(\x08\x12\x17\n\x0f\x63olumns_removed\x18\x05 \x03(\t\x12\x34\n\x13\x63olumn_type_changes\x18\x06 \x03(\x0b\x32\x17.proto_types.ColumnType\x12I\n\"enforced_column_constraint_removed\x18\x07 \x03(\x0b\x32\x1d.proto_types.ColumnConstraint\x12G\n!enforced_model_constraint_removed\x18\x08 \x03(\x0b\x32\x1c.proto_types.ModelConstraint\x12\x1f\n\x17materialization_changed\x18\t \x03(\t\"~\n\x1cUnversionedBreakingChangeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.UnversionedBreakingChange\"*\n\x14WarnStateTargetEqual\x12\x12\n\nstate_path\x18\x01 \x01(\t\"t\n\x17WarnStateTargetEqualMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.WarnStateTargetEqual\"%\n\x16\x46reshnessConfigProblem\x12\x0b\n\x03msg\x18\x01 \x01(\t\"x\n\x19\x46reshnessConfigProblemMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessConfigProblem\"/\n\x1dGitSparseCheckoutSubdirectory\x12\x0e\n\x06subdir\x18\x01 \x01(\t\"\x86\x01\n GitSparseCheckoutSubdirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.GitSparseCheckoutSubdirectory\"/\n\x1bGitProgressCheckoutRevision\x12\x10\n\x08revision\x18\x01 \x01(\t\"\x82\x01\n\x1eGitProgressCheckoutRevisionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.GitProgressCheckoutRevision\"4\n%GitProgressUpdatingExistingDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x96\x01\n(GitProgressUpdatingExistingDependencyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.GitProgressUpdatingExistingDependency\".\n\x1fGitProgressPullingNewDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x8a\x01\n\"GitProgressPullingNewDependencyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressPullingNewDependency\"\x1d\n\x0eGitNothingToDo\x12\x0b\n\x03sha\x18\x01 \x01(\t\"h\n\x11GitNothingToDoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.GitNothingToDo\"E\n\x1fGitProgressUpdatedCheckoutRange\x12\x11\n\tstart_sha\x18\x01 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x02 \x01(\t\"\x8a\x01\n\"GitProgressUpdatedCheckoutRangeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressUpdatedCheckoutRange\"*\n\x17GitProgressCheckedOutAt\x12\x0f\n\x07\x65nd_sha\x18\x01 \x01(\t\"z\n\x1aGitProgressCheckedOutAtMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.GitProgressCheckedOutAt\")\n\x1aRegistryProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x80\x01\n\x1dRegistryProgressGETRequestMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.RegistryProgressGETRequest\"=\n\x1bRegistryProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x82\x01\n\x1eRegistryProgressGETResponseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RegistryProgressGETResponse\"_\n\x1dSelectorReportInvalidSelector\x12\x17\n\x0fvalid_selectors\x18\x01 \x01(\t\x12\x13\n\x0bspec_method\x18\x02 \x01(\t\x12\x10\n\x08raw_spec\x18\x03 \x01(\t\"\x86\x01\n SelectorReportInvalidSelectorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.SelectorReportInvalidSelector\"\x15\n\x13\x44\x65psNoPackagesFound\"r\n\x16\x44\x65psNoPackagesFoundMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsNoPackagesFound\"/\n\x17\x44\x65psStartPackageInstall\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"z\n\x1a\x44\x65psStartPackageInstallMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsStartPackageInstall\"\'\n\x0f\x44\x65psInstallInfo\x12\x14\n\x0cversion_name\x18\x01 \x01(\t\"j\n\x12\x44\x65psInstallInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DepsInstallInfo\"-\n\x13\x44\x65psUpdateAvailable\x12\x16\n\x0eversion_latest\x18\x01 \x01(\t\"r\n\x16\x44\x65psUpdateAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsUpdateAvailable\"\x0e\n\x0c\x44\x65psUpToDate\"d\n\x0f\x44\x65psUpToDateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUpToDate\",\n\x14\x44\x65psListSubdirectory\x12\x14\n\x0csubdirectory\x18\x01 \x01(\t\"t\n\x17\x44\x65psListSubdirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.DepsListSubdirectory\".\n\x1a\x44\x65psNotifyUpdatesAvailable\x12\x10\n\x08packages\x18\x01 \x03(\t\"\x80\x01\n\x1d\x44\x65psNotifyUpdatesAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.DepsNotifyUpdatesAvailable\".\n\x1fRegistryIndexProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x8a\x01\n\"RegistryIndexProgressGETRequestMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryIndexProgressGETRequest\"B\n RegistryIndexProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x8c\x01\n#RegistryIndexProgressGETResponseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12;\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32-.proto_types.RegistryIndexProgressGETResponse\"2\n\x1eRegistryResponseUnexpectedType\x12\x10\n\x08response\x18\x01 \x01(\t\"\x88\x01\n!RegistryResponseUnexpectedTypeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseUnexpectedType\"2\n\x1eRegistryResponseMissingTopKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x88\x01\n!RegistryResponseMissingTopKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseMissingTopKeys\"5\n!RegistryResponseMissingNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8e\x01\n$RegistryResponseMissingNestedKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.RegistryResponseMissingNestedKeys\"3\n\x1fRegistryResponseExtraNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8a\x01\n\"RegistryResponseExtraNestedKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryResponseExtraNestedKeys\"(\n\x18\x44\x65psSetDownloadDirectory\x12\x0c\n\x04path\x18\x01 \x01(\t\"|\n\x1b\x44\x65psSetDownloadDirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsSetDownloadDirectory\"-\n\x0c\x44\x65psUnpinned\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0b\n\x03git\x18\x02 \x01(\t\"d\n\x0f\x44\x65psUnpinnedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUnpinned\"/\n\x1bNoNodesForSelectionCriteria\x12\x10\n\x08spec_raw\x18\x01 \x01(\t\"\x82\x01\n\x1eNoNodesForSelectionCriteriaMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.NoNodesForSelectionCriteria\")\n\x10\x44\x65psLockUpdating\x12\x15\n\rlock_filepath\x18\x01 \x01(\t\"l\n\x13\x44\x65psLockUpdatingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.DepsLockUpdating\"R\n\x0e\x44\x65psAddPackage\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x19\n\x11packages_filepath\x18\x03 \x01(\t\"h\n\x11\x44\x65psAddPackageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DepsAddPackage\"\xa7\x01\n\x19\x44\x65psFoundDuplicatePackage\x12S\n\x0fremoved_package\x18\x01 \x03(\x0b\x32:.proto_types.DepsFoundDuplicatePackage.RemovedPackageEntry\x1a\x35\n\x13RemovedPackageEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"~\n\x1c\x44\x65psFoundDuplicatePackageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.DepsFoundDuplicatePackage\"$\n\x12\x44\x65psVersionMissing\x12\x0e\n\x06source\x18\x01 \x01(\t\"p\n\x15\x44\x65psVersionMissingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.DepsVersionMissing\"/\n\x17\x44\x65psScrubbedPackageName\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"z\n\x1a\x44\x65psScrubbedPackageNameMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsScrubbedPackageName\"*\n\x1bRunningOperationCaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x82\x01\n\x1eRunningOperationCaughtErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RunningOperationCaughtError\"\x11\n\x0f\x43ompileComplete\"j\n\x12\x43ompileCompleteMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.CompileComplete\"\x18\n\x16\x46reshnessCheckComplete\"x\n\x19\x46reshnessCheckCompleteMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessCheckComplete\"\x1c\n\nSeedHeader\x12\x0e\n\x06header\x18\x01 \x01(\t\"`\n\rSeedHeaderMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SeedHeader\"]\n\x12SQLRunnerException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x02 \x01(\t\x12(\n\tnode_info\x18\x03 \x01(\x0b\x32\x15.proto_types.NodeInfo\"p\n\x15SQLRunnerExceptionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SQLRunnerException\"\xa8\x01\n\rLogTestResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x12\n\nnum_models\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"f\n\x10LogTestResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogTestResult\"k\n\x0cLogStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"d\n\x0fLogStartLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.LogStartLine\"\x95\x01\n\x0eLogModelResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"h\n\x11LogModelResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogModelResult\"\x92\x02\n\x11LogSnapshotResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x34\n\x03\x63\x66g\x18\x07 \x03(\x0b\x32\'.proto_types.LogSnapshotResult.CfgEntry\x12\x16\n\x0eresult_message\x18\x08 \x01(\t\x1a*\n\x08\x43\x66gEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"n\n\x14LogSnapshotResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogSnapshotResult\"\xb9\x01\n\rLogSeedResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x16\n\x0eresult_message\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12\x10\n\x08relation\x18\x08 \x01(\t\"f\n\x10LogSeedResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogSeedResult\"\xad\x01\n\x12LogFreshnessResult\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x13\n\x0bsource_name\x18\x06 \x01(\t\x12\x12\n\ntable_name\x18\x07 \x01(\t\"p\n\x15LogFreshnessResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogFreshnessResult\"\x98\x01\n\x11LogNodeNoOpResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"n\n\x14LogNodeNoOpResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogNodeNoOpResult\"\"\n\rLogCancelLine\x12\x11\n\tconn_name\x18\x01 \x01(\t\"f\n\x10LogCancelLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogCancelLine\"\x1f\n\x0f\x44\x65\x66\x61ultSelector\x12\x0c\n\x04name\x18\x01 \x01(\t\"j\n\x12\x44\x65\x66\x61ultSelectorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DefaultSelector\"5\n\tNodeStart\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"^\n\x0cNodeStartMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.NodeStart\"g\n\x0cNodeFinished\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12-\n\nrun_result\x18\x02 \x01(\x0b\x32\x19.proto_types.RunResultMsg\"d\n\x0fNodeFinishedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.NodeFinished\"+\n\x1bQueryCancelationUnsupported\x12\x0c\n\x04type\x18\x01 \x01(\t\"\x82\x01\n\x1eQueryCancelationUnsupportedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.QueryCancelationUnsupported\"O\n\x0f\x43oncurrencyLine\x12\x13\n\x0bnum_threads\x18\x01 \x01(\x05\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\x12\x12\n\nnode_count\x18\x03 \x01(\x05\"j\n\x12\x43oncurrencyLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ConcurrencyLine\"E\n\x19WritingInjectedSQLForNode\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"~\n\x1cWritingInjectedSQLForNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.WritingInjectedSQLForNode\"9\n\rNodeCompiling\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"f\n\x10NodeCompilingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeCompiling\"9\n\rNodeExecuting\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"f\n\x10NodeExecutingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeExecuting\"m\n\x10LogHookStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"l\n\x13LogHookStartLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.LogHookStartLine\"\x93\x01\n\x0eLogHookEndLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"h\n\x11LogHookEndLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogHookEndLine\"\x93\x01\n\x0fSkippingDetails\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x11\n\tnode_name\x18\x04 \x01(\t\x12\r\n\x05index\x18\x05 \x01(\x05\x12\r\n\x05total\x18\x06 \x01(\x05\"j\n\x12SkippingDetailsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SkippingDetails\"\r\n\x0bNothingToDo\"b\n\x0eNothingToDoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.NothingToDo\",\n\x1dRunningOperationUncaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x86\x01\n RunningOperationUncaughtErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.RunningOperationUncaughtError\"\x93\x01\n\x0c\x45ndRunResult\x12*\n\x07results\x18\x01 \x03(\x0b\x32\x19.proto_types.RunResultMsg\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x02\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07success\x18\x04 \x01(\x08\"d\n\x0f\x45ndRunResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.EndRunResult\"\x11\n\x0fNoNodesSelected\"j\n\x12NoNodesSelectedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.NoNodesSelected\"w\n\x10\x43ommandCompleted\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x65lapsed\x18\x04 \x01(\x02\"l\n\x13\x43ommandCompletedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.CommandCompleted\"k\n\x08ShowNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0f\n\x07preview\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"\\\n\x0bShowNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.ShowNode\"p\n\x0c\x43ompiledNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x10\n\x08\x63ompiled\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"d\n\x0f\x43ompiledNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.CompiledNode\"b\n\x17\x43\x61tchableExceptionOnRun\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"z\n\x1a\x43\x61tchableExceptionOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.CatchableExceptionOnRun\"_\n\x12InternalErrorOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12(\n\tnode_info\x18\x03 \x01(\x0b\x32\x15.proto_types.NodeInfo\"p\n\x15InternalErrorOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InternalErrorOnRun\"u\n\x15GenericExceptionOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"v\n\x18GenericExceptionOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.GenericExceptionOnRun\"N\n\x1aNodeConnectionReleaseError\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"\x80\x01\n\x1dNodeConnectionReleaseErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.NodeConnectionReleaseError\"\x1f\n\nFoundStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\"`\n\rFoundStatsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.FoundStats\"\x17\n\x15MainKeyboardInterrupt\"v\n\x18MainKeyboardInterruptMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainKeyboardInterrupt\"#\n\x14MainEncounteredError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"t\n\x17MainEncounteredErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MainEncounteredError\"%\n\x0eMainStackTrace\x12\x13\n\x0bstack_trace\x18\x01 \x01(\t\"h\n\x11MainStackTraceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainStackTrace\"p\n\x13TimingInfoCollected\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12/\n\x0btiming_info\x18\x02 \x01(\x0b\x32\x1a.proto_types.TimingInfoMsg\"r\n\x16TimingInfoCollectedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.TimingInfoCollected\"&\n\x12LogDebugStackTrace\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"p\n\x15LogDebugStackTraceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDebugStackTrace\"\x1e\n\x0e\x43heckCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"h\n\x11\x43heckCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CheckCleanPath\" \n\x10\x43onfirmCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"l\n\x13\x43onfirmCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConfirmCleanPath\"\"\n\x12ProtectedCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"p\n\x15ProtectedCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ProtectedCleanPath\"\x14\n\x12\x46inishedCleanPaths\"p\n\x15\x46inishedCleanPathsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FinishedCleanPaths\"5\n\x0bOpenCommand\x12\x10\n\x08open_cmd\x18\x01 \x01(\t\x12\x14\n\x0cprofiles_dir\x18\x02 \x01(\t\"b\n\x0eOpenCommandMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.OpenCommand\"0\n\x0fServingDocsPort\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"j\n\x12ServingDocsPortMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ServingDocsPort\"%\n\x15ServingDocsAccessInfo\x12\x0c\n\x04port\x18\x01 \x01(\t\"v\n\x18ServingDocsAccessInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ServingDocsAccessInfo\"\x15\n\x13ServingDocsExitInfo\"r\n\x16ServingDocsExitInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.ServingDocsExitInfo\"t\n\x10RunResultWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"l\n\x13RunResultWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultWarning\"t\n\x10RunResultFailure\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"l\n\x13RunResultFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultFailure\"k\n\tStatsLine\x12\x30\n\x05stats\x18\x01 \x03(\x0b\x32!.proto_types.StatsLine.StatsEntry\x1a,\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"^\n\x0cStatsLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.StatsLine\"G\n\x0eRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"h\n\x11RunResultErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RunResultError\"S\n\x17RunResultErrorNoMessage\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1aRunResultErrorNoMessageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultErrorNoMessage\"I\n\x0fSQLCompiledPath\x12\x0c\n\x04path\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"j\n\x12SQLCompiledPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SQLCompiledPath\"W\n\x14\x43heckNodeTestFailure\x12\x15\n\rrelation_name\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"t\n\x17\x43heckNodeTestFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.CheckNodeTestFailure\"W\n\x0f\x45ndOfRunSummary\x12\x12\n\nnum_errors\x18\x01 \x01(\x05\x12\x14\n\x0cnum_warnings\x18\x02 \x01(\x05\x12\x1a\n\x12keyboard_interrupt\x18\x03 \x01(\x08\"j\n\x12\x45ndOfRunSummaryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.EndOfRunSummary\"U\n\x13LogSkipBecauseError\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x10\n\x08relation\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"r\n\x16LogSkipBecauseErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.LogSkipBecauseError\"\x14\n\x12\x45nsureGitInstalled\"p\n\x15\x45nsureGitInstalledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.EnsureGitInstalled\"\x1a\n\x18\x44\x65psCreatingLocalSymlink\"|\n\x1b\x44\x65psCreatingLocalSymlinkMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsCreatingLocalSymlink\"\x19\n\x17\x44\x65psSymlinkNotAvailable\"z\n\x1a\x44\x65psSymlinkNotAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsSymlinkNotAvailable\"\x11\n\x0f\x44isableTracking\"j\n\x12\x44isableTrackingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DisableTracking\"\x1e\n\x0cSendingEvent\x12\x0e\n\x06kwargs\x18\x01 \x01(\t\"d\n\x0fSendingEventMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SendingEvent\"\x12\n\x10SendEventFailure\"l\n\x13SendEventFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SendEventFailure\"\r\n\x0b\x46lushEvents\"b\n\x0e\x46lushEventsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.FlushEvents\"\x14\n\x12\x46lushEventsFailure\"p\n\x15\x46lushEventsFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FlushEventsFailure\"-\n\x19TrackingInitializeFailure\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"~\n\x1cTrackingInitializeFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.TrackingInitializeFailure\"P\n\x17RunResultWarningMessage\x12\x0b\n\x03msg\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1aRunResultWarningMessageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultWarningMessage\"\x1a\n\x0b\x44\x65\x62ugCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"b\n\x0e\x44\x65\x62ugCmdOutMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.DebugCmdOut\"\x1d\n\x0e\x44\x65\x62ugCmdResult\x12\x0b\n\x03msg\x18\x01 \x01(\t\"h\n\x11\x44\x65\x62ugCmdResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DebugCmdResult\"\x19\n\nListCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"`\n\rListCmdOutMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.ListCmdOut\"\xec\x01\n\x0eResourceReport\x12\x14\n\x0c\x63ommand_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ommand_success\x18\x03 \x01(\x08\x12\x1f\n\x17\x63ommand_wall_clock_time\x18\x04 \x01(\x02\x12\x19\n\x11process_user_time\x18\x05 \x01(\x02\x12\x1b\n\x13process_kernel_time\x18\x06 \x01(\x02\x12\x1b\n\x13process_mem_max_rss\x18\x07 \x01(\x03\x12\x19\n\x11process_in_blocks\x18\x08 \x01(\x03\x12\x1a\n\x12process_out_blocks\x18\t \x01(\x03\"h\n\x11ResourceReportMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ResourceReportb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'core_types_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_COREEVENTINFO_EXTRAENTRY']._options = None
@@ -171,584 +171,592 @@
   _globals['_TESTSCONFIGDEPRECATION']._serialized_end=6422
   _globals['_TESTSCONFIGDEPRECATIONMSG']._serialized_start=6424
   _globals['_TESTSCONFIGDEPRECATIONMSG']._serialized_end=6544
   _globals['_PROJECTFLAGSMOVEDDEPRECATION']._serialized_start=6546
   _globals['_PROJECTFLAGSMOVEDDEPRECATION']._serialized_end=6576
   _globals['_PROJECTFLAGSMOVEDDEPRECATIONMSG']._serialized_start=6579
   _globals['_PROJECTFLAGSMOVEDDEPRECATIONMSG']._serialized_end=6711
-  _globals['_SPACESINMODELNAMEDEPRECATION']._serialized_start=6713
-  _globals['_SPACESINMODELNAMEDEPRECATION']._serialized_end=6801
-  _globals['_SPACESINMODELNAMEDEPRECATIONMSG']._serialized_start=6804
-  _globals['_SPACESINMODELNAMEDEPRECATIONMSG']._serialized_end=6936
-  _globals['_TOTALMODELNAMESWITHSPACESDEPRECATION']._serialized_start=6938
-  _globals['_TOTALMODELNAMESWITHSPACESDEPRECATION']._serialized_end=7045
-  _globals['_TOTALMODELNAMESWITHSPACESDEPRECATIONMSG']._serialized_start=7048
-  _globals['_TOTALMODELNAMESWITHSPACESDEPRECATIONMSG']._serialized_end=7196
-  _globals['_DEPRECATEDMODEL']._serialized_start=7198
-  _globals['_DEPRECATEDMODEL']._serialized_end=7284
-  _globals['_DEPRECATEDMODELMSG']._serialized_start=7286
-  _globals['_DEPRECATEDMODELMSG']._serialized_end=7392
-  _globals['_INPUTFILEDIFFERROR']._serialized_start=7394
-  _globals['_INPUTFILEDIFFERROR']._serialized_end=7449
-  _globals['_INPUTFILEDIFFERRORMSG']._serialized_start=7451
-  _globals['_INPUTFILEDIFFERRORMSG']._serialized_end=7563
-  _globals['_INVALIDVALUEFORFIELD']._serialized_start=7565
-  _globals['_INVALIDVALUEFORFIELD']._serialized_end=7628
-  _globals['_INVALIDVALUEFORFIELDMSG']._serialized_start=7630
-  _globals['_INVALIDVALUEFORFIELDMSG']._serialized_end=7746
-  _globals['_VALIDATIONWARNING']._serialized_start=7748
-  _globals['_VALIDATIONWARNING']._serialized_end=7829
-  _globals['_VALIDATIONWARNINGMSG']._serialized_start=7831
-  _globals['_VALIDATIONWARNINGMSG']._serialized_end=7941
-  _globals['_PARSEPERFINFOPATH']._serialized_start=7943
-  _globals['_PARSEPERFINFOPATH']._serialized_end=7976
-  _globals['_PARSEPERFINFOPATHMSG']._serialized_start=7978
-  _globals['_PARSEPERFINFOPATHMSG']._serialized_end=8088
-  _globals['_PARTIALPARSINGERRORPROCESSINGFILE']._serialized_start=8090
-  _globals['_PARTIALPARSINGERRORPROCESSINGFILE']._serialized_end=8139
-  _globals['_PARTIALPARSINGERRORPROCESSINGFILEMSG']._serialized_start=8142
-  _globals['_PARTIALPARSINGERRORPROCESSINGFILEMSG']._serialized_end=8284
-  _globals['_PARTIALPARSINGERROR']._serialized_start=8287
-  _globals['_PARTIALPARSINGERROR']._serialized_end=8421
-  _globals['_PARTIALPARSINGERROR_EXCINFOENTRY']._serialized_start=8375
-  _globals['_PARTIALPARSINGERROR_EXCINFOENTRY']._serialized_end=8421
-  _globals['_PARTIALPARSINGERRORMSG']._serialized_start=8423
-  _globals['_PARTIALPARSINGERRORMSG']._serialized_end=8537
-  _globals['_PARTIALPARSINGSKIPPARSING']._serialized_start=8539
-  _globals['_PARTIALPARSINGSKIPPARSING']._serialized_end=8566
-  _globals['_PARTIALPARSINGSKIPPARSINGMSG']._serialized_start=8568
-  _globals['_PARTIALPARSINGSKIPPARSINGMSG']._serialized_end=8694
-  _globals['_UNABLETOPARTIALPARSE']._serialized_start=8696
-  _globals['_UNABLETOPARTIALPARSE']._serialized_end=8734
-  _globals['_UNABLETOPARTIALPARSEMSG']._serialized_start=8736
-  _globals['_UNABLETOPARTIALPARSEMSG']._serialized_end=8852
-  _globals['_STATECHECKVARSHASH']._serialized_start=8854
-  _globals['_STATECHECKVARSHASH']._serialized_end=8956
-  _globals['_STATECHECKVARSHASHMSG']._serialized_start=8958
-  _globals['_STATECHECKVARSHASHMSG']._serialized_end=9070
-  _globals['_PARTIALPARSINGNOTENABLED']._serialized_start=9072
-  _globals['_PARTIALPARSINGNOTENABLED']._serialized_end=9098
-  _globals['_PARTIALPARSINGNOTENABLEDMSG']._serialized_start=9100
-  _globals['_PARTIALPARSINGNOTENABLEDMSG']._serialized_end=9224
-  _globals['_PARSEDFILELOADFAILED']._serialized_start=9226
-  _globals['_PARSEDFILELOADFAILED']._serialized_end=9293
-  _globals['_PARSEDFILELOADFAILEDMSG']._serialized_start=9295
-  _globals['_PARSEDFILELOADFAILEDMSG']._serialized_end=9411
-  _globals['_PARTIALPARSINGENABLED']._serialized_start=9413
-  _globals['_PARTIALPARSINGENABLED']._serialized_end=9485
-  _globals['_PARTIALPARSINGENABLEDMSG']._serialized_start=9487
-  _globals['_PARTIALPARSINGENABLEDMSG']._serialized_end=9605
-  _globals['_PARTIALPARSINGFILE']._serialized_start=9607
-  _globals['_PARTIALPARSINGFILE']._serialized_end=9663
-  _globals['_PARTIALPARSINGFILEMSG']._serialized_start=9665
-  _globals['_PARTIALPARSINGFILEMSG']._serialized_end=9777
-  _globals['_INVALIDDISABLEDTARGETINTESTNODE']._serialized_start=9780
-  _globals['_INVALIDDISABLEDTARGETINTESTNODE']._serialized_end=9955
-  _globals['_INVALIDDISABLEDTARGETINTESTNODEMSG']._serialized_start=9958
-  _globals['_INVALIDDISABLEDTARGETINTESTNODEMSG']._serialized_end=10096
-  _globals['_UNUSEDRESOURCECONFIGPATH']._serialized_start=10098
-  _globals['_UNUSEDRESOURCECONFIGPATH']._serialized_end=10153
-  _globals['_UNUSEDRESOURCECONFIGPATHMSG']._serialized_start=10155
-  _globals['_UNUSEDRESOURCECONFIGPATHMSG']._serialized_end=10279
-  _globals['_SEEDINCREASED']._serialized_start=10281
-  _globals['_SEEDINCREASED']._serialized_end=10332
-  _globals['_SEEDINCREASEDMSG']._serialized_start=10334
-  _globals['_SEEDINCREASEDMSG']._serialized_end=10436
-  _globals['_SEEDEXCEEDSLIMITSAMEPATH']._serialized_start=10438
-  _globals['_SEEDEXCEEDSLIMITSAMEPATH']._serialized_end=10500
-  _globals['_SEEDEXCEEDSLIMITSAMEPATHMSG']._serialized_start=10502
-  _globals['_SEEDEXCEEDSLIMITSAMEPATHMSG']._serialized_end=10626
-  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGED']._serialized_start=10628
-  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGED']._serialized_end=10696
-  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGEDMSG']._serialized_start=10699
-  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGEDMSG']._serialized_end=10835
-  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGED']._serialized_start=10837
-  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGED']._serialized_end=10929
-  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG']._serialized_start=10932
-  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG']._serialized_end=11070
-  _globals['_UNUSEDTABLES']._serialized_start=11072
-  _globals['_UNUSEDTABLES']._serialized_end=11109
-  _globals['_UNUSEDTABLESMSG']._serialized_start=11111
-  _globals['_UNUSEDTABLESMSG']._serialized_end=11211
-  _globals['_WRONGRESOURCESCHEMAFILE']._serialized_start=11214
-  _globals['_WRONGRESOURCESCHEMAFILE']._serialized_end=11349
-  _globals['_WRONGRESOURCESCHEMAFILEMSG']._serialized_start=11351
-  _globals['_WRONGRESOURCESCHEMAFILEMSG']._serialized_end=11473
-  _globals['_NONODEFORYAMLKEY']._serialized_start=11475
-  _globals['_NONODEFORYAMLKEY']._serialized_end=11550
-  _globals['_NONODEFORYAMLKEYMSG']._serialized_start=11552
-  _globals['_NONODEFORYAMLKEYMSG']._serialized_end=11660
-  _globals['_MACRONOTFOUNDFORPATCH']._serialized_start=11662
-  _globals['_MACRONOTFOUNDFORPATCH']._serialized_end=11705
-  _globals['_MACRONOTFOUNDFORPATCHMSG']._serialized_start=11707
-  _globals['_MACRONOTFOUNDFORPATCHMSG']._serialized_end=11825
-  _globals['_NODENOTFOUNDORDISABLED']._serialized_start=11828
-  _globals['_NODENOTFOUNDORDISABLED']._serialized_end=12012
-  _globals['_NODENOTFOUNDORDISABLEDMSG']._serialized_start=12014
-  _globals['_NODENOTFOUNDORDISABLEDMSG']._serialized_end=12134
-  _globals['_JINJALOGWARNING']._serialized_start=12136
-  _globals['_JINJALOGWARNING']._serialized_end=12208
-  _globals['_JINJALOGWARNINGMSG']._serialized_start=12210
-  _globals['_JINJALOGWARNINGMSG']._serialized_end=12316
-  _globals['_JINJALOGINFO']._serialized_start=12318
-  _globals['_JINJALOGINFO']._serialized_end=12387
-  _globals['_JINJALOGINFOMSG']._serialized_start=12389
-  _globals['_JINJALOGINFOMSG']._serialized_end=12489
-  _globals['_JINJALOGDEBUG']._serialized_start=12491
-  _globals['_JINJALOGDEBUG']._serialized_end=12561
-  _globals['_JINJALOGDEBUGMSG']._serialized_start=12563
-  _globals['_JINJALOGDEBUGMSG']._serialized_end=12665
-  _globals['_UNPINNEDREFNEWVERSIONAVAILABLE']._serialized_start=12668
-  _globals['_UNPINNEDREFNEWVERSIONAVAILABLE']._serialized_end=12842
-  _globals['_UNPINNEDREFNEWVERSIONAVAILABLEMSG']._serialized_start=12845
-  _globals['_UNPINNEDREFNEWVERSIONAVAILABLEMSG']._serialized_end=12981
-  _globals['_UPCOMINGREFERENCEDEPRECATION']._serialized_start=12984
-  _globals['_UPCOMINGREFERENCEDEPRECATION']._serialized_end=13182
-  _globals['_UPCOMINGREFERENCEDEPRECATIONMSG']._serialized_start=13185
-  _globals['_UPCOMINGREFERENCEDEPRECATIONMSG']._serialized_end=13317
-  _globals['_DEPRECATEDREFERENCE']._serialized_start=13320
-  _globals['_DEPRECATEDREFERENCE']._serialized_end=13509
-  _globals['_DEPRECATEDREFERENCEMSG']._serialized_start=13511
-  _globals['_DEPRECATEDREFERENCEMSG']._serialized_end=13625
-  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATION']._serialized_start=13627
-  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATION']._serialized_end=13687
-  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATIONMSG']._serialized_start=13690
-  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATIONMSG']._serialized_end=13838
-  _globals['_PARSEINLINENODEERROR']._serialized_start=13840
-  _globals['_PARSEINLINENODEERROR']._serialized_end=13917
-  _globals['_PARSEINLINENODEERRORMSG']._serialized_start=13919
-  _globals['_PARSEINLINENODEERRORMSG']._serialized_end=14035
-  _globals['_SEMANTICVALIDATIONFAILURE']._serialized_start=14037
-  _globals['_SEMANTICVALIDATIONFAILURE']._serialized_end=14077
-  _globals['_SEMANTICVALIDATIONFAILUREMSG']._serialized_start=14079
-  _globals['_SEMANTICVALIDATIONFAILUREMSG']._serialized_end=14205
-  _globals['_UNVERSIONEDBREAKINGCHANGE']._serialized_start=14208
-  _globals['_UNVERSIONEDBREAKINGCHANGE']._serialized_end=14602
-  _globals['_UNVERSIONEDBREAKINGCHANGEMSG']._serialized_start=14604
-  _globals['_UNVERSIONEDBREAKINGCHANGEMSG']._serialized_end=14730
-  _globals['_WARNSTATETARGETEQUAL']._serialized_start=14732
-  _globals['_WARNSTATETARGETEQUAL']._serialized_end=14774
-  _globals['_WARNSTATETARGETEQUALMSG']._serialized_start=14776
-  _globals['_WARNSTATETARGETEQUALMSG']._serialized_end=14892
-  _globals['_FRESHNESSCONFIGPROBLEM']._serialized_start=14894
-  _globals['_FRESHNESSCONFIGPROBLEM']._serialized_end=14931
-  _globals['_FRESHNESSCONFIGPROBLEMMSG']._serialized_start=14933
-  _globals['_FRESHNESSCONFIGPROBLEMMSG']._serialized_end=15053
-  _globals['_GITSPARSECHECKOUTSUBDIRECTORY']._serialized_start=15055
-  _globals['_GITSPARSECHECKOUTSUBDIRECTORY']._serialized_end=15102
-  _globals['_GITSPARSECHECKOUTSUBDIRECTORYMSG']._serialized_start=15105
-  _globals['_GITSPARSECHECKOUTSUBDIRECTORYMSG']._serialized_end=15239
-  _globals['_GITPROGRESSCHECKOUTREVISION']._serialized_start=15241
-  _globals['_GITPROGRESSCHECKOUTREVISION']._serialized_end=15288
-  _globals['_GITPROGRESSCHECKOUTREVISIONMSG']._serialized_start=15291
-  _globals['_GITPROGRESSCHECKOUTREVISIONMSG']._serialized_end=15421
-  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCY']._serialized_start=15423
-  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCY']._serialized_end=15475
-  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG']._serialized_start=15478
-  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG']._serialized_end=15628
-  _globals['_GITPROGRESSPULLINGNEWDEPENDENCY']._serialized_start=15630
-  _globals['_GITPROGRESSPULLINGNEWDEPENDENCY']._serialized_end=15676
-  _globals['_GITPROGRESSPULLINGNEWDEPENDENCYMSG']._serialized_start=15679
-  _globals['_GITPROGRESSPULLINGNEWDEPENDENCYMSG']._serialized_end=15817
-  _globals['_GITNOTHINGTODO']._serialized_start=15819
-  _globals['_GITNOTHINGTODO']._serialized_end=15848
-  _globals['_GITNOTHINGTODOMSG']._serialized_start=15850
-  _globals['_GITNOTHINGTODOMSG']._serialized_end=15954
-  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGE']._serialized_start=15956
-  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGE']._serialized_end=16025
-  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGEMSG']._serialized_start=16028
-  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGEMSG']._serialized_end=16166
-  _globals['_GITPROGRESSCHECKEDOUTAT']._serialized_start=16168
-  _globals['_GITPROGRESSCHECKEDOUTAT']._serialized_end=16210
-  _globals['_GITPROGRESSCHECKEDOUTATMSG']._serialized_start=16212
-  _globals['_GITPROGRESSCHECKEDOUTATMSG']._serialized_end=16334
-  _globals['_REGISTRYPROGRESSGETREQUEST']._serialized_start=16336
-  _globals['_REGISTRYPROGRESSGETREQUEST']._serialized_end=16377
-  _globals['_REGISTRYPROGRESSGETREQUESTMSG']._serialized_start=16380
-  _globals['_REGISTRYPROGRESSGETREQUESTMSG']._serialized_end=16508
-  _globals['_REGISTRYPROGRESSGETRESPONSE']._serialized_start=16510
-  _globals['_REGISTRYPROGRESSGETRESPONSE']._serialized_end=16571
-  _globals['_REGISTRYPROGRESSGETRESPONSEMSG']._serialized_start=16574
-  _globals['_REGISTRYPROGRESSGETRESPONSEMSG']._serialized_end=16704
-  _globals['_SELECTORREPORTINVALIDSELECTOR']._serialized_start=16706
-  _globals['_SELECTORREPORTINVALIDSELECTOR']._serialized_end=16801
-  _globals['_SELECTORREPORTINVALIDSELECTORMSG']._serialized_start=16804
-  _globals['_SELECTORREPORTINVALIDSELECTORMSG']._serialized_end=16938
-  _globals['_DEPSNOPACKAGESFOUND']._serialized_start=16940
-  _globals['_DEPSNOPACKAGESFOUND']._serialized_end=16961
-  _globals['_DEPSNOPACKAGESFOUNDMSG']._serialized_start=16963
-  _globals['_DEPSNOPACKAGESFOUNDMSG']._serialized_end=17077
-  _globals['_DEPSSTARTPACKAGEINSTALL']._serialized_start=17079
-  _globals['_DEPSSTARTPACKAGEINSTALL']._serialized_end=17126
-  _globals['_DEPSSTARTPACKAGEINSTALLMSG']._serialized_start=17128
-  _globals['_DEPSSTARTPACKAGEINSTALLMSG']._serialized_end=17250
-  _globals['_DEPSINSTALLINFO']._serialized_start=17252
-  _globals['_DEPSINSTALLINFO']._serialized_end=17291
-  _globals['_DEPSINSTALLINFOMSG']._serialized_start=17293
-  _globals['_DEPSINSTALLINFOMSG']._serialized_end=17399
-  _globals['_DEPSUPDATEAVAILABLE']._serialized_start=17401
-  _globals['_DEPSUPDATEAVAILABLE']._serialized_end=17446
-  _globals['_DEPSUPDATEAVAILABLEMSG']._serialized_start=17448
-  _globals['_DEPSUPDATEAVAILABLEMSG']._serialized_end=17562
-  _globals['_DEPSUPTODATE']._serialized_start=17564
-  _globals['_DEPSUPTODATE']._serialized_end=17578
-  _globals['_DEPSUPTODATEMSG']._serialized_start=17580
-  _globals['_DEPSUPTODATEMSG']._serialized_end=17680
-  _globals['_DEPSLISTSUBDIRECTORY']._serialized_start=17682
-  _globals['_DEPSLISTSUBDIRECTORY']._serialized_end=17726
-  _globals['_DEPSLISTSUBDIRECTORYMSG']._serialized_start=17728
-  _globals['_DEPSLISTSUBDIRECTORYMSG']._serialized_end=17844
-  _globals['_DEPSNOTIFYUPDATESAVAILABLE']._serialized_start=17846
-  _globals['_DEPSNOTIFYUPDATESAVAILABLE']._serialized_end=17892
-  _globals['_DEPSNOTIFYUPDATESAVAILABLEMSG']._serialized_start=17895
-  _globals['_DEPSNOTIFYUPDATESAVAILABLEMSG']._serialized_end=18023
-  _globals['_REGISTRYINDEXPROGRESSGETREQUEST']._serialized_start=18025
-  _globals['_REGISTRYINDEXPROGRESSGETREQUEST']._serialized_end=18071
-  _globals['_REGISTRYINDEXPROGRESSGETREQUESTMSG']._serialized_start=18074
-  _globals['_REGISTRYINDEXPROGRESSGETREQUESTMSG']._serialized_end=18212
-  _globals['_REGISTRYINDEXPROGRESSGETRESPONSE']._serialized_start=18214
-  _globals['_REGISTRYINDEXPROGRESSGETRESPONSE']._serialized_end=18280
-  _globals['_REGISTRYINDEXPROGRESSGETRESPONSEMSG']._serialized_start=18283
-  _globals['_REGISTRYINDEXPROGRESSGETRESPONSEMSG']._serialized_end=18423
-  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPE']._serialized_start=18425
-  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPE']._serialized_end=18475
-  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPEMSG']._serialized_start=18478
-  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPEMSG']._serialized_end=18614
-  _globals['_REGISTRYRESPONSEMISSINGTOPKEYS']._serialized_start=18616
-  _globals['_REGISTRYRESPONSEMISSINGTOPKEYS']._serialized_end=18666
-  _globals['_REGISTRYRESPONSEMISSINGTOPKEYSMSG']._serialized_start=18669
-  _globals['_REGISTRYRESPONSEMISSINGTOPKEYSMSG']._serialized_end=18805
-  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYS']._serialized_start=18807
-  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYS']._serialized_end=18860
-  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYSMSG']._serialized_start=18863
-  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYSMSG']._serialized_end=19005
-  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYS']._serialized_start=19007
-  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYS']._serialized_end=19058
-  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYSMSG']._serialized_start=19061
-  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYSMSG']._serialized_end=19199
-  _globals['_DEPSSETDOWNLOADDIRECTORY']._serialized_start=19201
-  _globals['_DEPSSETDOWNLOADDIRECTORY']._serialized_end=19241
-  _globals['_DEPSSETDOWNLOADDIRECTORYMSG']._serialized_start=19243
-  _globals['_DEPSSETDOWNLOADDIRECTORYMSG']._serialized_end=19367
-  _globals['_DEPSUNPINNED']._serialized_start=19369
-  _globals['_DEPSUNPINNED']._serialized_end=19414
-  _globals['_DEPSUNPINNEDMSG']._serialized_start=19416
-  _globals['_DEPSUNPINNEDMSG']._serialized_end=19516
-  _globals['_NONODESFORSELECTIONCRITERIA']._serialized_start=19518
-  _globals['_NONODESFORSELECTIONCRITERIA']._serialized_end=19565
-  _globals['_NONODESFORSELECTIONCRITERIAMSG']._serialized_start=19568
-  _globals['_NONODESFORSELECTIONCRITERIAMSG']._serialized_end=19698
-  _globals['_DEPSLOCKUPDATING']._serialized_start=19700
-  _globals['_DEPSLOCKUPDATING']._serialized_end=19741
-  _globals['_DEPSLOCKUPDATINGMSG']._serialized_start=19743
-  _globals['_DEPSLOCKUPDATINGMSG']._serialized_end=19851
-  _globals['_DEPSADDPACKAGE']._serialized_start=19853
-  _globals['_DEPSADDPACKAGE']._serialized_end=19935
-  _globals['_DEPSADDPACKAGEMSG']._serialized_start=19937
-  _globals['_DEPSADDPACKAGEMSG']._serialized_end=20041
-  _globals['_DEPSFOUNDDUPLICATEPACKAGE']._serialized_start=20044
-  _globals['_DEPSFOUNDDUPLICATEPACKAGE']._serialized_end=20211
-  _globals['_DEPSFOUNDDUPLICATEPACKAGE_REMOVEDPACKAGEENTRY']._serialized_start=20158
-  _globals['_DEPSFOUNDDUPLICATEPACKAGE_REMOVEDPACKAGEENTRY']._serialized_end=20211
-  _globals['_DEPSFOUNDDUPLICATEPACKAGEMSG']._serialized_start=20213
-  _globals['_DEPSFOUNDDUPLICATEPACKAGEMSG']._serialized_end=20339
-  _globals['_DEPSVERSIONMISSING']._serialized_start=20341
-  _globals['_DEPSVERSIONMISSING']._serialized_end=20377
-  _globals['_DEPSVERSIONMISSINGMSG']._serialized_start=20379
-  _globals['_DEPSVERSIONMISSINGMSG']._serialized_end=20491
-  _globals['_DEPSSCRUBBEDPACKAGENAME']._serialized_start=20493
-  _globals['_DEPSSCRUBBEDPACKAGENAME']._serialized_end=20540
-  _globals['_DEPSSCRUBBEDPACKAGENAMEMSG']._serialized_start=20542
-  _globals['_DEPSSCRUBBEDPACKAGENAMEMSG']._serialized_end=20664
-  _globals['_RUNNINGOPERATIONCAUGHTERROR']._serialized_start=20666
-  _globals['_RUNNINGOPERATIONCAUGHTERROR']._serialized_end=20708
-  _globals['_RUNNINGOPERATIONCAUGHTERRORMSG']._serialized_start=20711
-  _globals['_RUNNINGOPERATIONCAUGHTERRORMSG']._serialized_end=20841
-  _globals['_COMPILECOMPLETE']._serialized_start=20843
-  _globals['_COMPILECOMPLETE']._serialized_end=20860
-  _globals['_COMPILECOMPLETEMSG']._serialized_start=20862
-  _globals['_COMPILECOMPLETEMSG']._serialized_end=20968
-  _globals['_FRESHNESSCHECKCOMPLETE']._serialized_start=20970
-  _globals['_FRESHNESSCHECKCOMPLETE']._serialized_end=20994
-  _globals['_FRESHNESSCHECKCOMPLETEMSG']._serialized_start=20996
-  _globals['_FRESHNESSCHECKCOMPLETEMSG']._serialized_end=21116
-  _globals['_SEEDHEADER']._serialized_start=21118
-  _globals['_SEEDHEADER']._serialized_end=21146
-  _globals['_SEEDHEADERMSG']._serialized_start=21148
-  _globals['_SEEDHEADERMSG']._serialized_end=21244
-  _globals['_SQLRUNNEREXCEPTION']._serialized_start=21246
-  _globals['_SQLRUNNEREXCEPTION']._serialized_end=21339
-  _globals['_SQLRUNNEREXCEPTIONMSG']._serialized_start=21341
-  _globals['_SQLRUNNEREXCEPTIONMSG']._serialized_end=21453
-  _globals['_LOGTESTRESULT']._serialized_start=21456
-  _globals['_LOGTESTRESULT']._serialized_end=21624
-  _globals['_LOGTESTRESULTMSG']._serialized_start=21626
-  _globals['_LOGTESTRESULTMSG']._serialized_end=21728
-  _globals['_LOGSTARTLINE']._serialized_start=21730
-  _globals['_LOGSTARTLINE']._serialized_end=21837
-  _globals['_LOGSTARTLINEMSG']._serialized_start=21839
-  _globals['_LOGSTARTLINEMSG']._serialized_end=21939
-  _globals['_LOGMODELRESULT']._serialized_start=21942
-  _globals['_LOGMODELRESULT']._serialized_end=22091
-  _globals['_LOGMODELRESULTMSG']._serialized_start=22093
-  _globals['_LOGMODELRESULTMSG']._serialized_end=22197
-  _globals['_LOGSNAPSHOTRESULT']._serialized_start=22200
-  _globals['_LOGSNAPSHOTRESULT']._serialized_end=22474
-  _globals['_LOGSNAPSHOTRESULT_CFGENTRY']._serialized_start=22432
-  _globals['_LOGSNAPSHOTRESULT_CFGENTRY']._serialized_end=22474
-  _globals['_LOGSNAPSHOTRESULTMSG']._serialized_start=22476
-  _globals['_LOGSNAPSHOTRESULTMSG']._serialized_end=22586
-  _globals['_LOGSEEDRESULT']._serialized_start=22589
-  _globals['_LOGSEEDRESULT']._serialized_end=22774
-  _globals['_LOGSEEDRESULTMSG']._serialized_start=22776
-  _globals['_LOGSEEDRESULTMSG']._serialized_end=22878
-  _globals['_LOGFRESHNESSRESULT']._serialized_start=22881
-  _globals['_LOGFRESHNESSRESULT']._serialized_end=23054
-  _globals['_LOGFRESHNESSRESULTMSG']._serialized_start=23056
-  _globals['_LOGFRESHNESSRESULTMSG']._serialized_end=23168
-  _globals['_LOGNODENOOPRESULT']._serialized_start=23171
-  _globals['_LOGNODENOOPRESULT']._serialized_end=23323
-  _globals['_LOGNODENOOPRESULTMSG']._serialized_start=23325
-  _globals['_LOGNODENOOPRESULTMSG']._serialized_end=23435
-  _globals['_LOGCANCELLINE']._serialized_start=23437
-  _globals['_LOGCANCELLINE']._serialized_end=23471
-  _globals['_LOGCANCELLINEMSG']._serialized_start=23473
-  _globals['_LOGCANCELLINEMSG']._serialized_end=23575
-  _globals['_DEFAULTSELECTOR']._serialized_start=23577
-  _globals['_DEFAULTSELECTOR']._serialized_end=23608
-  _globals['_DEFAULTSELECTORMSG']._serialized_start=23610
-  _globals['_DEFAULTSELECTORMSG']._serialized_end=23716
-  _globals['_NODESTART']._serialized_start=23718
-  _globals['_NODESTART']._serialized_end=23771
-  _globals['_NODESTARTMSG']._serialized_start=23773
-  _globals['_NODESTARTMSG']._serialized_end=23867
-  _globals['_NODEFINISHED']._serialized_start=23869
-  _globals['_NODEFINISHED']._serialized_end=23972
-  _globals['_NODEFINISHEDMSG']._serialized_start=23974
-  _globals['_NODEFINISHEDMSG']._serialized_end=24074
-  _globals['_QUERYCANCELATIONUNSUPPORTED']._serialized_start=24076
-  _globals['_QUERYCANCELATIONUNSUPPORTED']._serialized_end=24119
-  _globals['_QUERYCANCELATIONUNSUPPORTEDMSG']._serialized_start=24122
-  _globals['_QUERYCANCELATIONUNSUPPORTEDMSG']._serialized_end=24252
-  _globals['_CONCURRENCYLINE']._serialized_start=24254
-  _globals['_CONCURRENCYLINE']._serialized_end=24333
-  _globals['_CONCURRENCYLINEMSG']._serialized_start=24335
-  _globals['_CONCURRENCYLINEMSG']._serialized_end=24441
-  _globals['_WRITINGINJECTEDSQLFORNODE']._serialized_start=24443
-  _globals['_WRITINGINJECTEDSQLFORNODE']._serialized_end=24512
-  _globals['_WRITINGINJECTEDSQLFORNODEMSG']._serialized_start=24514
-  _globals['_WRITINGINJECTEDSQLFORNODEMSG']._serialized_end=24640
-  _globals['_NODECOMPILING']._serialized_start=24642
-  _globals['_NODECOMPILING']._serialized_end=24699
-  _globals['_NODECOMPILINGMSG']._serialized_start=24701
-  _globals['_NODECOMPILINGMSG']._serialized_end=24803
-  _globals['_NODEEXECUTING']._serialized_start=24805
-  _globals['_NODEEXECUTING']._serialized_end=24862
-  _globals['_NODEEXECUTINGMSG']._serialized_start=24864
-  _globals['_NODEEXECUTINGMSG']._serialized_end=24966
-  _globals['_LOGHOOKSTARTLINE']._serialized_start=24968
-  _globals['_LOGHOOKSTARTLINE']._serialized_end=25077
-  _globals['_LOGHOOKSTARTLINEMSG']._serialized_start=25079
-  _globals['_LOGHOOKSTARTLINEMSG']._serialized_end=25187
-  _globals['_LOGHOOKENDLINE']._serialized_start=25190
-  _globals['_LOGHOOKENDLINE']._serialized_end=25337
-  _globals['_LOGHOOKENDLINEMSG']._serialized_start=25339
-  _globals['_LOGHOOKENDLINEMSG']._serialized_end=25443
-  _globals['_SKIPPINGDETAILS']._serialized_start=25446
-  _globals['_SKIPPINGDETAILS']._serialized_end=25593
-  _globals['_SKIPPINGDETAILSMSG']._serialized_start=25595
-  _globals['_SKIPPINGDETAILSMSG']._serialized_end=25701
-  _globals['_NOTHINGTODO']._serialized_start=25703
-  _globals['_NOTHINGTODO']._serialized_end=25716
-  _globals['_NOTHINGTODOMSG']._serialized_start=25718
-  _globals['_NOTHINGTODOMSG']._serialized_end=25816
-  _globals['_RUNNINGOPERATIONUNCAUGHTERROR']._serialized_start=25818
-  _globals['_RUNNINGOPERATIONUNCAUGHTERROR']._serialized_end=25862
-  _globals['_RUNNINGOPERATIONUNCAUGHTERRORMSG']._serialized_start=25865
-  _globals['_RUNNINGOPERATIONUNCAUGHTERRORMSG']._serialized_end=25999
-  _globals['_ENDRUNRESULT']._serialized_start=26002
-  _globals['_ENDRUNRESULT']._serialized_end=26149
-  _globals['_ENDRUNRESULTMSG']._serialized_start=26151
-  _globals['_ENDRUNRESULTMSG']._serialized_end=26251
-  _globals['_NONODESSELECTED']._serialized_start=26253
-  _globals['_NONODESSELECTED']._serialized_end=26270
-  _globals['_NONODESSELECTEDMSG']._serialized_start=26272
-  _globals['_NONODESSELECTEDMSG']._serialized_end=26378
-  _globals['_COMMANDCOMPLETED']._serialized_start=26380
-  _globals['_COMMANDCOMPLETED']._serialized_end=26499
-  _globals['_COMMANDCOMPLETEDMSG']._serialized_start=26501
-  _globals['_COMMANDCOMPLETEDMSG']._serialized_end=26609
-  _globals['_SHOWNODE']._serialized_start=26611
-  _globals['_SHOWNODE']._serialized_end=26718
-  _globals['_SHOWNODEMSG']._serialized_start=26720
-  _globals['_SHOWNODEMSG']._serialized_end=26812
-  _globals['_COMPILEDNODE']._serialized_start=26814
-  _globals['_COMPILEDNODE']._serialized_end=26926
-  _globals['_COMPILEDNODEMSG']._serialized_start=26928
-  _globals['_COMPILEDNODEMSG']._serialized_end=27028
-  _globals['_CATCHABLEEXCEPTIONONRUN']._serialized_start=27030
-  _globals['_CATCHABLEEXCEPTIONONRUN']._serialized_end=27128
-  _globals['_CATCHABLEEXCEPTIONONRUNMSG']._serialized_start=27130
-  _globals['_CATCHABLEEXCEPTIONONRUNMSG']._serialized_end=27252
-  _globals['_INTERNALERRORONRUN']._serialized_start=27254
-  _globals['_INTERNALERRORONRUN']._serialized_end=27349
-  _globals['_INTERNALERRORONRUNMSG']._serialized_start=27351
-  _globals['_INTERNALERRORONRUNMSG']._serialized_end=27463
-  _globals['_GENERICEXCEPTIONONRUN']._serialized_start=27465
-  _globals['_GENERICEXCEPTIONONRUN']._serialized_end=27582
-  _globals['_GENERICEXCEPTIONONRUNMSG']._serialized_start=27584
-  _globals['_GENERICEXCEPTIONONRUNMSG']._serialized_end=27702
-  _globals['_NODECONNECTIONRELEASEERROR']._serialized_start=27704
-  _globals['_NODECONNECTIONRELEASEERROR']._serialized_end=27782
-  _globals['_NODECONNECTIONRELEASEERRORMSG']._serialized_start=27785
-  _globals['_NODECONNECTIONRELEASEERRORMSG']._serialized_end=27913
-  _globals['_FOUNDSTATS']._serialized_start=27915
-  _globals['_FOUNDSTATS']._serialized_end=27946
-  _globals['_FOUNDSTATSMSG']._serialized_start=27948
-  _globals['_FOUNDSTATSMSG']._serialized_end=28044
-  _globals['_MAINKEYBOARDINTERRUPT']._serialized_start=28046
-  _globals['_MAINKEYBOARDINTERRUPT']._serialized_end=28069
-  _globals['_MAINKEYBOARDINTERRUPTMSG']._serialized_start=28071
-  _globals['_MAINKEYBOARDINTERRUPTMSG']._serialized_end=28189
-  _globals['_MAINENCOUNTEREDERROR']._serialized_start=28191
-  _globals['_MAINENCOUNTEREDERROR']._serialized_end=28226
-  _globals['_MAINENCOUNTEREDERRORMSG']._serialized_start=28228
-  _globals['_MAINENCOUNTEREDERRORMSG']._serialized_end=28344
-  _globals['_MAINSTACKTRACE']._serialized_start=28346
-  _globals['_MAINSTACKTRACE']._serialized_end=28383
-  _globals['_MAINSTACKTRACEMSG']._serialized_start=28385
-  _globals['_MAINSTACKTRACEMSG']._serialized_end=28489
-  _globals['_TIMINGINFOCOLLECTED']._serialized_start=28491
-  _globals['_TIMINGINFOCOLLECTED']._serialized_end=28603
-  _globals['_TIMINGINFOCOLLECTEDMSG']._serialized_start=28605
-  _globals['_TIMINGINFOCOLLECTEDMSG']._serialized_end=28719
-  _globals['_LOGDEBUGSTACKTRACE']._serialized_start=28721
-  _globals['_LOGDEBUGSTACKTRACE']._serialized_end=28759
-  _globals['_LOGDEBUGSTACKTRACEMSG']._serialized_start=28761
-  _globals['_LOGDEBUGSTACKTRACEMSG']._serialized_end=28873
-  _globals['_CHECKCLEANPATH']._serialized_start=28875
-  _globals['_CHECKCLEANPATH']._serialized_end=28905
-  _globals['_CHECKCLEANPATHMSG']._serialized_start=28907
-  _globals['_CHECKCLEANPATHMSG']._serialized_end=29011
-  _globals['_CONFIRMCLEANPATH']._serialized_start=29013
-  _globals['_CONFIRMCLEANPATH']._serialized_end=29045
-  _globals['_CONFIRMCLEANPATHMSG']._serialized_start=29047
-  _globals['_CONFIRMCLEANPATHMSG']._serialized_end=29155
-  _globals['_PROTECTEDCLEANPATH']._serialized_start=29157
-  _globals['_PROTECTEDCLEANPATH']._serialized_end=29191
-  _globals['_PROTECTEDCLEANPATHMSG']._serialized_start=29193
-  _globals['_PROTECTEDCLEANPATHMSG']._serialized_end=29305
-  _globals['_FINISHEDCLEANPATHS']._serialized_start=29307
-  _globals['_FINISHEDCLEANPATHS']._serialized_end=29327
-  _globals['_FINISHEDCLEANPATHSMSG']._serialized_start=29329
-  _globals['_FINISHEDCLEANPATHSMSG']._serialized_end=29441
-  _globals['_OPENCOMMAND']._serialized_start=29443
-  _globals['_OPENCOMMAND']._serialized_end=29496
-  _globals['_OPENCOMMANDMSG']._serialized_start=29498
-  _globals['_OPENCOMMANDMSG']._serialized_end=29596
-  _globals['_SERVINGDOCSPORT']._serialized_start=29598
-  _globals['_SERVINGDOCSPORT']._serialized_end=29646
-  _globals['_SERVINGDOCSPORTMSG']._serialized_start=29648
-  _globals['_SERVINGDOCSPORTMSG']._serialized_end=29754
-  _globals['_SERVINGDOCSACCESSINFO']._serialized_start=29756
-  _globals['_SERVINGDOCSACCESSINFO']._serialized_end=29793
-  _globals['_SERVINGDOCSACCESSINFOMSG']._serialized_start=29795
-  _globals['_SERVINGDOCSACCESSINFOMSG']._serialized_end=29913
-  _globals['_SERVINGDOCSEXITINFO']._serialized_start=29915
-  _globals['_SERVINGDOCSEXITINFO']._serialized_end=29936
-  _globals['_SERVINGDOCSEXITINFOMSG']._serialized_start=29938
-  _globals['_SERVINGDOCSEXITINFOMSG']._serialized_end=30052
-  _globals['_RUNRESULTWARNING']._serialized_start=30054
-  _globals['_RUNRESULTWARNING']._serialized_end=30170
-  _globals['_RUNRESULTWARNINGMSG']._serialized_start=30172
-  _globals['_RUNRESULTWARNINGMSG']._serialized_end=30280
-  _globals['_RUNRESULTFAILURE']._serialized_start=30282
-  _globals['_RUNRESULTFAILURE']._serialized_end=30398
-  _globals['_RUNRESULTFAILUREMSG']._serialized_start=30400
-  _globals['_RUNRESULTFAILUREMSG']._serialized_end=30508
-  _globals['_STATSLINE']._serialized_start=30510
-  _globals['_STATSLINE']._serialized_end=30617
-  _globals['_STATSLINE_STATSENTRY']._serialized_start=30573
-  _globals['_STATSLINE_STATSENTRY']._serialized_end=30617
-  _globals['_STATSLINEMSG']._serialized_start=30619
-  _globals['_STATSLINEMSG']._serialized_end=30713
-  _globals['_RUNRESULTERROR']._serialized_start=30715
-  _globals['_RUNRESULTERROR']._serialized_end=30786
-  _globals['_RUNRESULTERRORMSG']._serialized_start=30788
-  _globals['_RUNRESULTERRORMSG']._serialized_end=30892
-  _globals['_RUNRESULTERRORNOMESSAGE']._serialized_start=30894
-  _globals['_RUNRESULTERRORNOMESSAGE']._serialized_end=30977
-  _globals['_RUNRESULTERRORNOMESSAGEMSG']._serialized_start=30979
-  _globals['_RUNRESULTERRORNOMESSAGEMSG']._serialized_end=31101
-  _globals['_SQLCOMPILEDPATH']._serialized_start=31103
-  _globals['_SQLCOMPILEDPATH']._serialized_end=31176
-  _globals['_SQLCOMPILEDPATHMSG']._serialized_start=31178
-  _globals['_SQLCOMPILEDPATHMSG']._serialized_end=31284
-  _globals['_CHECKNODETESTFAILURE']._serialized_start=31286
-  _globals['_CHECKNODETESTFAILURE']._serialized_end=31373
-  _globals['_CHECKNODETESTFAILUREMSG']._serialized_start=31375
-  _globals['_CHECKNODETESTFAILUREMSG']._serialized_end=31491
-  _globals['_ENDOFRUNSUMMARY']._serialized_start=31493
-  _globals['_ENDOFRUNSUMMARY']._serialized_end=31580
-  _globals['_ENDOFRUNSUMMARYMSG']._serialized_start=31582
-  _globals['_ENDOFRUNSUMMARYMSG']._serialized_end=31688
-  _globals['_LOGSKIPBECAUSEERROR']._serialized_start=31690
-  _globals['_LOGSKIPBECAUSEERROR']._serialized_end=31775
-  _globals['_LOGSKIPBECAUSEERRORMSG']._serialized_start=31777
-  _globals['_LOGSKIPBECAUSEERRORMSG']._serialized_end=31891
-  _globals['_ENSUREGITINSTALLED']._serialized_start=31893
-  _globals['_ENSUREGITINSTALLED']._serialized_end=31913
-  _globals['_ENSUREGITINSTALLEDMSG']._serialized_start=31915
-  _globals['_ENSUREGITINSTALLEDMSG']._serialized_end=32027
-  _globals['_DEPSCREATINGLOCALSYMLINK']._serialized_start=32029
-  _globals['_DEPSCREATINGLOCALSYMLINK']._serialized_end=32055
-  _globals['_DEPSCREATINGLOCALSYMLINKMSG']._serialized_start=32057
-  _globals['_DEPSCREATINGLOCALSYMLINKMSG']._serialized_end=32181
-  _globals['_DEPSSYMLINKNOTAVAILABLE']._serialized_start=32183
-  _globals['_DEPSSYMLINKNOTAVAILABLE']._serialized_end=32208
-  _globals['_DEPSSYMLINKNOTAVAILABLEMSG']._serialized_start=32210
-  _globals['_DEPSSYMLINKNOTAVAILABLEMSG']._serialized_end=32332
-  _globals['_DISABLETRACKING']._serialized_start=32334
-  _globals['_DISABLETRACKING']._serialized_end=32351
-  _globals['_DISABLETRACKINGMSG']._serialized_start=32353
-  _globals['_DISABLETRACKINGMSG']._serialized_end=32459
-  _globals['_SENDINGEVENT']._serialized_start=32461
-  _globals['_SENDINGEVENT']._serialized_end=32491
-  _globals['_SENDINGEVENTMSG']._serialized_start=32493
-  _globals['_SENDINGEVENTMSG']._serialized_end=32593
-  _globals['_SENDEVENTFAILURE']._serialized_start=32595
-  _globals['_SENDEVENTFAILURE']._serialized_end=32613
-  _globals['_SENDEVENTFAILUREMSG']._serialized_start=32615
-  _globals['_SENDEVENTFAILUREMSG']._serialized_end=32723
-  _globals['_FLUSHEVENTS']._serialized_start=32725
-  _globals['_FLUSHEVENTS']._serialized_end=32738
-  _globals['_FLUSHEVENTSMSG']._serialized_start=32740
-  _globals['_FLUSHEVENTSMSG']._serialized_end=32838
-  _globals['_FLUSHEVENTSFAILURE']._serialized_start=32840
-  _globals['_FLUSHEVENTSFAILURE']._serialized_end=32860
-  _globals['_FLUSHEVENTSFAILUREMSG']._serialized_start=32862
-  _globals['_FLUSHEVENTSFAILUREMSG']._serialized_end=32974
-  _globals['_TRACKINGINITIALIZEFAILURE']._serialized_start=32976
-  _globals['_TRACKINGINITIALIZEFAILURE']._serialized_end=33021
-  _globals['_TRACKINGINITIALIZEFAILUREMSG']._serialized_start=33023
-  _globals['_TRACKINGINITIALIZEFAILUREMSG']._serialized_end=33149
-  _globals['_RUNRESULTWARNINGMESSAGE']._serialized_start=33151
-  _globals['_RUNRESULTWARNINGMESSAGE']._serialized_end=33231
-  _globals['_RUNRESULTWARNINGMESSAGEMSG']._serialized_start=33233
-  _globals['_RUNRESULTWARNINGMESSAGEMSG']._serialized_end=33355
-  _globals['_DEBUGCMDOUT']._serialized_start=33357
-  _globals['_DEBUGCMDOUT']._serialized_end=33383
-  _globals['_DEBUGCMDOUTMSG']._serialized_start=33385
-  _globals['_DEBUGCMDOUTMSG']._serialized_end=33483
-  _globals['_DEBUGCMDRESULT']._serialized_start=33485
-  _globals['_DEBUGCMDRESULT']._serialized_end=33514
-  _globals['_DEBUGCMDRESULTMSG']._serialized_start=33516
-  _globals['_DEBUGCMDRESULTMSG']._serialized_end=33620
-  _globals['_LISTCMDOUT']._serialized_start=33622
-  _globals['_LISTCMDOUT']._serialized_end=33647
-  _globals['_LISTCMDOUTMSG']._serialized_start=33649
-  _globals['_LISTCMDOUTMSG']._serialized_end=33745
-  _globals['_RESOURCEREPORT']._serialized_start=33748
-  _globals['_RESOURCEREPORT']._serialized_end=33984
-  _globals['_RESOURCEREPORTMSG']._serialized_start=33986
-  _globals['_RESOURCEREPORTMSG']._serialized_end=34090
+  _globals['_SPACESINRESOURCENAMEDEPRECATION']._serialized_start=6713
+  _globals['_SPACESINRESOURCENAMEDEPRECATION']._serialized_end=6780
+  _globals['_SPACESINRESOURCENAMEDEPRECATIONMSG']._serialized_start=6783
+  _globals['_SPACESINRESOURCENAMEDEPRECATIONMSG']._serialized_end=6921
+  _globals['_RESOURCENAMESWITHSPACESDEPRECATION']._serialized_start=6923
+  _globals['_RESOURCENAMESWITHSPACESDEPRECATION']._serialized_end=7028
+  _globals['_RESOURCENAMESWITHSPACESDEPRECATIONMSG']._serialized_start=7031
+  _globals['_RESOURCENAMESWITHSPACESDEPRECATIONMSG']._serialized_end=7175
+  _globals['_PACKAGEMATERIALIZATIONOVERRIDEDEPRECATION']._serialized_start=7177
+  _globals['_PACKAGEMATERIALIZATIONOVERRIDEDEPRECATION']._serialized_end=7272
+  _globals['_PACKAGEMATERIALIZATIONOVERRIDEDEPRECATIONMSG']._serialized_start=7275
+  _globals['_PACKAGEMATERIALIZATIONOVERRIDEDEPRECATIONMSG']._serialized_end=7433
+  _globals['_SOURCEFRESHNESSPROJECTHOOKSNOTRUN']._serialized_start=7435
+  _globals['_SOURCEFRESHNESSPROJECTHOOKSNOTRUN']._serialized_end=7470
+  _globals['_SOURCEFRESHNESSPROJECTHOOKSNOTRUNMSG']._serialized_start=7473
+  _globals['_SOURCEFRESHNESSPROJECTHOOKSNOTRUNMSG']._serialized_end=7615
+  _globals['_DEPRECATEDMODEL']._serialized_start=7617
+  _globals['_DEPRECATEDMODEL']._serialized_end=7703
+  _globals['_DEPRECATEDMODELMSG']._serialized_start=7705
+  _globals['_DEPRECATEDMODELMSG']._serialized_end=7811
+  _globals['_INPUTFILEDIFFERROR']._serialized_start=7813
+  _globals['_INPUTFILEDIFFERROR']._serialized_end=7868
+  _globals['_INPUTFILEDIFFERRORMSG']._serialized_start=7870
+  _globals['_INPUTFILEDIFFERRORMSG']._serialized_end=7982
+  _globals['_INVALIDVALUEFORFIELD']._serialized_start=7984
+  _globals['_INVALIDVALUEFORFIELD']._serialized_end=8047
+  _globals['_INVALIDVALUEFORFIELDMSG']._serialized_start=8049
+  _globals['_INVALIDVALUEFORFIELDMSG']._serialized_end=8165
+  _globals['_VALIDATIONWARNING']._serialized_start=8167
+  _globals['_VALIDATIONWARNING']._serialized_end=8248
+  _globals['_VALIDATIONWARNINGMSG']._serialized_start=8250
+  _globals['_VALIDATIONWARNINGMSG']._serialized_end=8360
+  _globals['_PARSEPERFINFOPATH']._serialized_start=8362
+  _globals['_PARSEPERFINFOPATH']._serialized_end=8395
+  _globals['_PARSEPERFINFOPATHMSG']._serialized_start=8397
+  _globals['_PARSEPERFINFOPATHMSG']._serialized_end=8507
+  _globals['_PARTIALPARSINGERRORPROCESSINGFILE']._serialized_start=8509
+  _globals['_PARTIALPARSINGERRORPROCESSINGFILE']._serialized_end=8558
+  _globals['_PARTIALPARSINGERRORPROCESSINGFILEMSG']._serialized_start=8561
+  _globals['_PARTIALPARSINGERRORPROCESSINGFILEMSG']._serialized_end=8703
+  _globals['_PARTIALPARSINGERROR']._serialized_start=8706
+  _globals['_PARTIALPARSINGERROR']._serialized_end=8840
+  _globals['_PARTIALPARSINGERROR_EXCINFOENTRY']._serialized_start=8794
+  _globals['_PARTIALPARSINGERROR_EXCINFOENTRY']._serialized_end=8840
+  _globals['_PARTIALPARSINGERRORMSG']._serialized_start=8842
+  _globals['_PARTIALPARSINGERRORMSG']._serialized_end=8956
+  _globals['_PARTIALPARSINGSKIPPARSING']._serialized_start=8958
+  _globals['_PARTIALPARSINGSKIPPARSING']._serialized_end=8985
+  _globals['_PARTIALPARSINGSKIPPARSINGMSG']._serialized_start=8987
+  _globals['_PARTIALPARSINGSKIPPARSINGMSG']._serialized_end=9113
+  _globals['_UNABLETOPARTIALPARSE']._serialized_start=9115
+  _globals['_UNABLETOPARTIALPARSE']._serialized_end=9153
+  _globals['_UNABLETOPARTIALPARSEMSG']._serialized_start=9155
+  _globals['_UNABLETOPARTIALPARSEMSG']._serialized_end=9271
+  _globals['_STATECHECKVARSHASH']._serialized_start=9273
+  _globals['_STATECHECKVARSHASH']._serialized_end=9375
+  _globals['_STATECHECKVARSHASHMSG']._serialized_start=9377
+  _globals['_STATECHECKVARSHASHMSG']._serialized_end=9489
+  _globals['_PARTIALPARSINGNOTENABLED']._serialized_start=9491
+  _globals['_PARTIALPARSINGNOTENABLED']._serialized_end=9517
+  _globals['_PARTIALPARSINGNOTENABLEDMSG']._serialized_start=9519
+  _globals['_PARTIALPARSINGNOTENABLEDMSG']._serialized_end=9643
+  _globals['_PARSEDFILELOADFAILED']._serialized_start=9645
+  _globals['_PARSEDFILELOADFAILED']._serialized_end=9712
+  _globals['_PARSEDFILELOADFAILEDMSG']._serialized_start=9714
+  _globals['_PARSEDFILELOADFAILEDMSG']._serialized_end=9830
+  _globals['_PARTIALPARSINGENABLED']._serialized_start=9832
+  _globals['_PARTIALPARSINGENABLED']._serialized_end=9904
+  _globals['_PARTIALPARSINGENABLEDMSG']._serialized_start=9906
+  _globals['_PARTIALPARSINGENABLEDMSG']._serialized_end=10024
+  _globals['_PARTIALPARSINGFILE']._serialized_start=10026
+  _globals['_PARTIALPARSINGFILE']._serialized_end=10082
+  _globals['_PARTIALPARSINGFILEMSG']._serialized_start=10084
+  _globals['_PARTIALPARSINGFILEMSG']._serialized_end=10196
+  _globals['_INVALIDDISABLEDTARGETINTESTNODE']._serialized_start=10199
+  _globals['_INVALIDDISABLEDTARGETINTESTNODE']._serialized_end=10374
+  _globals['_INVALIDDISABLEDTARGETINTESTNODEMSG']._serialized_start=10377
+  _globals['_INVALIDDISABLEDTARGETINTESTNODEMSG']._serialized_end=10515
+  _globals['_UNUSEDRESOURCECONFIGPATH']._serialized_start=10517
+  _globals['_UNUSEDRESOURCECONFIGPATH']._serialized_end=10572
+  _globals['_UNUSEDRESOURCECONFIGPATHMSG']._serialized_start=10574
+  _globals['_UNUSEDRESOURCECONFIGPATHMSG']._serialized_end=10698
+  _globals['_SEEDINCREASED']._serialized_start=10700
+  _globals['_SEEDINCREASED']._serialized_end=10751
+  _globals['_SEEDINCREASEDMSG']._serialized_start=10753
+  _globals['_SEEDINCREASEDMSG']._serialized_end=10855
+  _globals['_SEEDEXCEEDSLIMITSAMEPATH']._serialized_start=10857
+  _globals['_SEEDEXCEEDSLIMITSAMEPATH']._serialized_end=10919
+  _globals['_SEEDEXCEEDSLIMITSAMEPATHMSG']._serialized_start=10921
+  _globals['_SEEDEXCEEDSLIMITSAMEPATHMSG']._serialized_end=11045
+  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGED']._serialized_start=11047
+  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGED']._serialized_end=11115
+  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGEDMSG']._serialized_start=11118
+  _globals['_SEEDEXCEEDSLIMITANDPATHCHANGEDMSG']._serialized_end=11254
+  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGED']._serialized_start=11256
+  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGED']._serialized_end=11348
+  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG']._serialized_start=11351
+  _globals['_SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG']._serialized_end=11489
+  _globals['_UNUSEDTABLES']._serialized_start=11491
+  _globals['_UNUSEDTABLES']._serialized_end=11528
+  _globals['_UNUSEDTABLESMSG']._serialized_start=11530
+  _globals['_UNUSEDTABLESMSG']._serialized_end=11630
+  _globals['_WRONGRESOURCESCHEMAFILE']._serialized_start=11633
+  _globals['_WRONGRESOURCESCHEMAFILE']._serialized_end=11768
+  _globals['_WRONGRESOURCESCHEMAFILEMSG']._serialized_start=11770
+  _globals['_WRONGRESOURCESCHEMAFILEMSG']._serialized_end=11892
+  _globals['_NONODEFORYAMLKEY']._serialized_start=11894
+  _globals['_NONODEFORYAMLKEY']._serialized_end=11969
+  _globals['_NONODEFORYAMLKEYMSG']._serialized_start=11971
+  _globals['_NONODEFORYAMLKEYMSG']._serialized_end=12079
+  _globals['_MACRONOTFOUNDFORPATCH']._serialized_start=12081
+  _globals['_MACRONOTFOUNDFORPATCH']._serialized_end=12124
+  _globals['_MACRONOTFOUNDFORPATCHMSG']._serialized_start=12126
+  _globals['_MACRONOTFOUNDFORPATCHMSG']._serialized_end=12244
+  _globals['_NODENOTFOUNDORDISABLED']._serialized_start=12247
+  _globals['_NODENOTFOUNDORDISABLED']._serialized_end=12431
+  _globals['_NODENOTFOUNDORDISABLEDMSG']._serialized_start=12433
+  _globals['_NODENOTFOUNDORDISABLEDMSG']._serialized_end=12553
+  _globals['_JINJALOGWARNING']._serialized_start=12555
+  _globals['_JINJALOGWARNING']._serialized_end=12627
+  _globals['_JINJALOGWARNINGMSG']._serialized_start=12629
+  _globals['_JINJALOGWARNINGMSG']._serialized_end=12735
+  _globals['_JINJALOGINFO']._serialized_start=12737
+  _globals['_JINJALOGINFO']._serialized_end=12806
+  _globals['_JINJALOGINFOMSG']._serialized_start=12808
+  _globals['_JINJALOGINFOMSG']._serialized_end=12908
+  _globals['_JINJALOGDEBUG']._serialized_start=12910
+  _globals['_JINJALOGDEBUG']._serialized_end=12980
+  _globals['_JINJALOGDEBUGMSG']._serialized_start=12982
+  _globals['_JINJALOGDEBUGMSG']._serialized_end=13084
+  _globals['_UNPINNEDREFNEWVERSIONAVAILABLE']._serialized_start=13087
+  _globals['_UNPINNEDREFNEWVERSIONAVAILABLE']._serialized_end=13261
+  _globals['_UNPINNEDREFNEWVERSIONAVAILABLEMSG']._serialized_start=13264
+  _globals['_UNPINNEDREFNEWVERSIONAVAILABLEMSG']._serialized_end=13400
+  _globals['_UPCOMINGREFERENCEDEPRECATION']._serialized_start=13403
+  _globals['_UPCOMINGREFERENCEDEPRECATION']._serialized_end=13601
+  _globals['_UPCOMINGREFERENCEDEPRECATIONMSG']._serialized_start=13604
+  _globals['_UPCOMINGREFERENCEDEPRECATIONMSG']._serialized_end=13736
+  _globals['_DEPRECATEDREFERENCE']._serialized_start=13739
+  _globals['_DEPRECATEDREFERENCE']._serialized_end=13928
+  _globals['_DEPRECATEDREFERENCEMSG']._serialized_start=13930
+  _globals['_DEPRECATEDREFERENCEMSG']._serialized_end=14044
+  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATION']._serialized_start=14046
+  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATION']._serialized_end=14106
+  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATIONMSG']._serialized_start=14109
+  _globals['_UNSUPPORTEDCONSTRAINTMATERIALIZATIONMSG']._serialized_end=14257
+  _globals['_PARSEINLINENODEERROR']._serialized_start=14259
+  _globals['_PARSEINLINENODEERROR']._serialized_end=14336
+  _globals['_PARSEINLINENODEERRORMSG']._serialized_start=14338
+  _globals['_PARSEINLINENODEERRORMSG']._serialized_end=14454
+  _globals['_SEMANTICVALIDATIONFAILURE']._serialized_start=14456
+  _globals['_SEMANTICVALIDATIONFAILURE']._serialized_end=14496
+  _globals['_SEMANTICVALIDATIONFAILUREMSG']._serialized_start=14498
+  _globals['_SEMANTICVALIDATIONFAILUREMSG']._serialized_end=14624
+  _globals['_UNVERSIONEDBREAKINGCHANGE']._serialized_start=14627
+  _globals['_UNVERSIONEDBREAKINGCHANGE']._serialized_end=15021
+  _globals['_UNVERSIONEDBREAKINGCHANGEMSG']._serialized_start=15023
+  _globals['_UNVERSIONEDBREAKINGCHANGEMSG']._serialized_end=15149
+  _globals['_WARNSTATETARGETEQUAL']._serialized_start=15151
+  _globals['_WARNSTATETARGETEQUAL']._serialized_end=15193
+  _globals['_WARNSTATETARGETEQUALMSG']._serialized_start=15195
+  _globals['_WARNSTATETARGETEQUALMSG']._serialized_end=15311
+  _globals['_FRESHNESSCONFIGPROBLEM']._serialized_start=15313
+  _globals['_FRESHNESSCONFIGPROBLEM']._serialized_end=15350
+  _globals['_FRESHNESSCONFIGPROBLEMMSG']._serialized_start=15352
+  _globals['_FRESHNESSCONFIGPROBLEMMSG']._serialized_end=15472
+  _globals['_GITSPARSECHECKOUTSUBDIRECTORY']._serialized_start=15474
+  _globals['_GITSPARSECHECKOUTSUBDIRECTORY']._serialized_end=15521
+  _globals['_GITSPARSECHECKOUTSUBDIRECTORYMSG']._serialized_start=15524
+  _globals['_GITSPARSECHECKOUTSUBDIRECTORYMSG']._serialized_end=15658
+  _globals['_GITPROGRESSCHECKOUTREVISION']._serialized_start=15660
+  _globals['_GITPROGRESSCHECKOUTREVISION']._serialized_end=15707
+  _globals['_GITPROGRESSCHECKOUTREVISIONMSG']._serialized_start=15710
+  _globals['_GITPROGRESSCHECKOUTREVISIONMSG']._serialized_end=15840
+  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCY']._serialized_start=15842
+  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCY']._serialized_end=15894
+  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG']._serialized_start=15897
+  _globals['_GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG']._serialized_end=16047
+  _globals['_GITPROGRESSPULLINGNEWDEPENDENCY']._serialized_start=16049
+  _globals['_GITPROGRESSPULLINGNEWDEPENDENCY']._serialized_end=16095
+  _globals['_GITPROGRESSPULLINGNEWDEPENDENCYMSG']._serialized_start=16098
+  _globals['_GITPROGRESSPULLINGNEWDEPENDENCYMSG']._serialized_end=16236
+  _globals['_GITNOTHINGTODO']._serialized_start=16238
+  _globals['_GITNOTHINGTODO']._serialized_end=16267
+  _globals['_GITNOTHINGTODOMSG']._serialized_start=16269
+  _globals['_GITNOTHINGTODOMSG']._serialized_end=16373
+  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGE']._serialized_start=16375
+  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGE']._serialized_end=16444
+  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGEMSG']._serialized_start=16447
+  _globals['_GITPROGRESSUPDATEDCHECKOUTRANGEMSG']._serialized_end=16585
+  _globals['_GITPROGRESSCHECKEDOUTAT']._serialized_start=16587
+  _globals['_GITPROGRESSCHECKEDOUTAT']._serialized_end=16629
+  _globals['_GITPROGRESSCHECKEDOUTATMSG']._serialized_start=16631
+  _globals['_GITPROGRESSCHECKEDOUTATMSG']._serialized_end=16753
+  _globals['_REGISTRYPROGRESSGETREQUEST']._serialized_start=16755
+  _globals['_REGISTRYPROGRESSGETREQUEST']._serialized_end=16796
+  _globals['_REGISTRYPROGRESSGETREQUESTMSG']._serialized_start=16799
+  _globals['_REGISTRYPROGRESSGETREQUESTMSG']._serialized_end=16927
+  _globals['_REGISTRYPROGRESSGETRESPONSE']._serialized_start=16929
+  _globals['_REGISTRYPROGRESSGETRESPONSE']._serialized_end=16990
+  _globals['_REGISTRYPROGRESSGETRESPONSEMSG']._serialized_start=16993
+  _globals['_REGISTRYPROGRESSGETRESPONSEMSG']._serialized_end=17123
+  _globals['_SELECTORREPORTINVALIDSELECTOR']._serialized_start=17125
+  _globals['_SELECTORREPORTINVALIDSELECTOR']._serialized_end=17220
+  _globals['_SELECTORREPORTINVALIDSELECTORMSG']._serialized_start=17223
+  _globals['_SELECTORREPORTINVALIDSELECTORMSG']._serialized_end=17357
+  _globals['_DEPSNOPACKAGESFOUND']._serialized_start=17359
+  _globals['_DEPSNOPACKAGESFOUND']._serialized_end=17380
+  _globals['_DEPSNOPACKAGESFOUNDMSG']._serialized_start=17382
+  _globals['_DEPSNOPACKAGESFOUNDMSG']._serialized_end=17496
+  _globals['_DEPSSTARTPACKAGEINSTALL']._serialized_start=17498
+  _globals['_DEPSSTARTPACKAGEINSTALL']._serialized_end=17545
+  _globals['_DEPSSTARTPACKAGEINSTALLMSG']._serialized_start=17547
+  _globals['_DEPSSTARTPACKAGEINSTALLMSG']._serialized_end=17669
+  _globals['_DEPSINSTALLINFO']._serialized_start=17671
+  _globals['_DEPSINSTALLINFO']._serialized_end=17710
+  _globals['_DEPSINSTALLINFOMSG']._serialized_start=17712
+  _globals['_DEPSINSTALLINFOMSG']._serialized_end=17818
+  _globals['_DEPSUPDATEAVAILABLE']._serialized_start=17820
+  _globals['_DEPSUPDATEAVAILABLE']._serialized_end=17865
+  _globals['_DEPSUPDATEAVAILABLEMSG']._serialized_start=17867
+  _globals['_DEPSUPDATEAVAILABLEMSG']._serialized_end=17981
+  _globals['_DEPSUPTODATE']._serialized_start=17983
+  _globals['_DEPSUPTODATE']._serialized_end=17997
+  _globals['_DEPSUPTODATEMSG']._serialized_start=17999
+  _globals['_DEPSUPTODATEMSG']._serialized_end=18099
+  _globals['_DEPSLISTSUBDIRECTORY']._serialized_start=18101
+  _globals['_DEPSLISTSUBDIRECTORY']._serialized_end=18145
+  _globals['_DEPSLISTSUBDIRECTORYMSG']._serialized_start=18147
+  _globals['_DEPSLISTSUBDIRECTORYMSG']._serialized_end=18263
+  _globals['_DEPSNOTIFYUPDATESAVAILABLE']._serialized_start=18265
+  _globals['_DEPSNOTIFYUPDATESAVAILABLE']._serialized_end=18311
+  _globals['_DEPSNOTIFYUPDATESAVAILABLEMSG']._serialized_start=18314
+  _globals['_DEPSNOTIFYUPDATESAVAILABLEMSG']._serialized_end=18442
+  _globals['_REGISTRYINDEXPROGRESSGETREQUEST']._serialized_start=18444
+  _globals['_REGISTRYINDEXPROGRESSGETREQUEST']._serialized_end=18490
+  _globals['_REGISTRYINDEXPROGRESSGETREQUESTMSG']._serialized_start=18493
+  _globals['_REGISTRYINDEXPROGRESSGETREQUESTMSG']._serialized_end=18631
+  _globals['_REGISTRYINDEXPROGRESSGETRESPONSE']._serialized_start=18633
+  _globals['_REGISTRYINDEXPROGRESSGETRESPONSE']._serialized_end=18699
+  _globals['_REGISTRYINDEXPROGRESSGETRESPONSEMSG']._serialized_start=18702
+  _globals['_REGISTRYINDEXPROGRESSGETRESPONSEMSG']._serialized_end=18842
+  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPE']._serialized_start=18844
+  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPE']._serialized_end=18894
+  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPEMSG']._serialized_start=18897
+  _globals['_REGISTRYRESPONSEUNEXPECTEDTYPEMSG']._serialized_end=19033
+  _globals['_REGISTRYRESPONSEMISSINGTOPKEYS']._serialized_start=19035
+  _globals['_REGISTRYRESPONSEMISSINGTOPKEYS']._serialized_end=19085
+  _globals['_REGISTRYRESPONSEMISSINGTOPKEYSMSG']._serialized_start=19088
+  _globals['_REGISTRYRESPONSEMISSINGTOPKEYSMSG']._serialized_end=19224
+  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYS']._serialized_start=19226
+  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYS']._serialized_end=19279
+  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYSMSG']._serialized_start=19282
+  _globals['_REGISTRYRESPONSEMISSINGNESTEDKEYSMSG']._serialized_end=19424
+  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYS']._serialized_start=19426
+  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYS']._serialized_end=19477
+  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYSMSG']._serialized_start=19480
+  _globals['_REGISTRYRESPONSEEXTRANESTEDKEYSMSG']._serialized_end=19618
+  _globals['_DEPSSETDOWNLOADDIRECTORY']._serialized_start=19620
+  _globals['_DEPSSETDOWNLOADDIRECTORY']._serialized_end=19660
+  _globals['_DEPSSETDOWNLOADDIRECTORYMSG']._serialized_start=19662
+  _globals['_DEPSSETDOWNLOADDIRECTORYMSG']._serialized_end=19786
+  _globals['_DEPSUNPINNED']._serialized_start=19788
+  _globals['_DEPSUNPINNED']._serialized_end=19833
+  _globals['_DEPSUNPINNEDMSG']._serialized_start=19835
+  _globals['_DEPSUNPINNEDMSG']._serialized_end=19935
+  _globals['_NONODESFORSELECTIONCRITERIA']._serialized_start=19937
+  _globals['_NONODESFORSELECTIONCRITERIA']._serialized_end=19984
+  _globals['_NONODESFORSELECTIONCRITERIAMSG']._serialized_start=19987
+  _globals['_NONODESFORSELECTIONCRITERIAMSG']._serialized_end=20117
+  _globals['_DEPSLOCKUPDATING']._serialized_start=20119
+  _globals['_DEPSLOCKUPDATING']._serialized_end=20160
+  _globals['_DEPSLOCKUPDATINGMSG']._serialized_start=20162
+  _globals['_DEPSLOCKUPDATINGMSG']._serialized_end=20270
+  _globals['_DEPSADDPACKAGE']._serialized_start=20272
+  _globals['_DEPSADDPACKAGE']._serialized_end=20354
+  _globals['_DEPSADDPACKAGEMSG']._serialized_start=20356
+  _globals['_DEPSADDPACKAGEMSG']._serialized_end=20460
+  _globals['_DEPSFOUNDDUPLICATEPACKAGE']._serialized_start=20463
+  _globals['_DEPSFOUNDDUPLICATEPACKAGE']._serialized_end=20630
+  _globals['_DEPSFOUNDDUPLICATEPACKAGE_REMOVEDPACKAGEENTRY']._serialized_start=20577
+  _globals['_DEPSFOUNDDUPLICATEPACKAGE_REMOVEDPACKAGEENTRY']._serialized_end=20630
+  _globals['_DEPSFOUNDDUPLICATEPACKAGEMSG']._serialized_start=20632
+  _globals['_DEPSFOUNDDUPLICATEPACKAGEMSG']._serialized_end=20758
+  _globals['_DEPSVERSIONMISSING']._serialized_start=20760
+  _globals['_DEPSVERSIONMISSING']._serialized_end=20796
+  _globals['_DEPSVERSIONMISSINGMSG']._serialized_start=20798
+  _globals['_DEPSVERSIONMISSINGMSG']._serialized_end=20910
+  _globals['_DEPSSCRUBBEDPACKAGENAME']._serialized_start=20912
+  _globals['_DEPSSCRUBBEDPACKAGENAME']._serialized_end=20959
+  _globals['_DEPSSCRUBBEDPACKAGENAMEMSG']._serialized_start=20961
+  _globals['_DEPSSCRUBBEDPACKAGENAMEMSG']._serialized_end=21083
+  _globals['_RUNNINGOPERATIONCAUGHTERROR']._serialized_start=21085
+  _globals['_RUNNINGOPERATIONCAUGHTERROR']._serialized_end=21127
+  _globals['_RUNNINGOPERATIONCAUGHTERRORMSG']._serialized_start=21130
+  _globals['_RUNNINGOPERATIONCAUGHTERRORMSG']._serialized_end=21260
+  _globals['_COMPILECOMPLETE']._serialized_start=21262
+  _globals['_COMPILECOMPLETE']._serialized_end=21279
+  _globals['_COMPILECOMPLETEMSG']._serialized_start=21281
+  _globals['_COMPILECOMPLETEMSG']._serialized_end=21387
+  _globals['_FRESHNESSCHECKCOMPLETE']._serialized_start=21389
+  _globals['_FRESHNESSCHECKCOMPLETE']._serialized_end=21413
+  _globals['_FRESHNESSCHECKCOMPLETEMSG']._serialized_start=21415
+  _globals['_FRESHNESSCHECKCOMPLETEMSG']._serialized_end=21535
+  _globals['_SEEDHEADER']._serialized_start=21537
+  _globals['_SEEDHEADER']._serialized_end=21565
+  _globals['_SEEDHEADERMSG']._serialized_start=21567
+  _globals['_SEEDHEADERMSG']._serialized_end=21663
+  _globals['_SQLRUNNEREXCEPTION']._serialized_start=21665
+  _globals['_SQLRUNNEREXCEPTION']._serialized_end=21758
+  _globals['_SQLRUNNEREXCEPTIONMSG']._serialized_start=21760
+  _globals['_SQLRUNNEREXCEPTIONMSG']._serialized_end=21872
+  _globals['_LOGTESTRESULT']._serialized_start=21875
+  _globals['_LOGTESTRESULT']._serialized_end=22043
+  _globals['_LOGTESTRESULTMSG']._serialized_start=22045
+  _globals['_LOGTESTRESULTMSG']._serialized_end=22147
+  _globals['_LOGSTARTLINE']._serialized_start=22149
+  _globals['_LOGSTARTLINE']._serialized_end=22256
+  _globals['_LOGSTARTLINEMSG']._serialized_start=22258
+  _globals['_LOGSTARTLINEMSG']._serialized_end=22358
+  _globals['_LOGMODELRESULT']._serialized_start=22361
+  _globals['_LOGMODELRESULT']._serialized_end=22510
+  _globals['_LOGMODELRESULTMSG']._serialized_start=22512
+  _globals['_LOGMODELRESULTMSG']._serialized_end=22616
+  _globals['_LOGSNAPSHOTRESULT']._serialized_start=22619
+  _globals['_LOGSNAPSHOTRESULT']._serialized_end=22893
+  _globals['_LOGSNAPSHOTRESULT_CFGENTRY']._serialized_start=22851
+  _globals['_LOGSNAPSHOTRESULT_CFGENTRY']._serialized_end=22893
+  _globals['_LOGSNAPSHOTRESULTMSG']._serialized_start=22895
+  _globals['_LOGSNAPSHOTRESULTMSG']._serialized_end=23005
+  _globals['_LOGSEEDRESULT']._serialized_start=23008
+  _globals['_LOGSEEDRESULT']._serialized_end=23193
+  _globals['_LOGSEEDRESULTMSG']._serialized_start=23195
+  _globals['_LOGSEEDRESULTMSG']._serialized_end=23297
+  _globals['_LOGFRESHNESSRESULT']._serialized_start=23300
+  _globals['_LOGFRESHNESSRESULT']._serialized_end=23473
+  _globals['_LOGFRESHNESSRESULTMSG']._serialized_start=23475
+  _globals['_LOGFRESHNESSRESULTMSG']._serialized_end=23587
+  _globals['_LOGNODENOOPRESULT']._serialized_start=23590
+  _globals['_LOGNODENOOPRESULT']._serialized_end=23742
+  _globals['_LOGNODENOOPRESULTMSG']._serialized_start=23744
+  _globals['_LOGNODENOOPRESULTMSG']._serialized_end=23854
+  _globals['_LOGCANCELLINE']._serialized_start=23856
+  _globals['_LOGCANCELLINE']._serialized_end=23890
+  _globals['_LOGCANCELLINEMSG']._serialized_start=23892
+  _globals['_LOGCANCELLINEMSG']._serialized_end=23994
+  _globals['_DEFAULTSELECTOR']._serialized_start=23996
+  _globals['_DEFAULTSELECTOR']._serialized_end=24027
+  _globals['_DEFAULTSELECTORMSG']._serialized_start=24029
+  _globals['_DEFAULTSELECTORMSG']._serialized_end=24135
+  _globals['_NODESTART']._serialized_start=24137
+  _globals['_NODESTART']._serialized_end=24190
+  _globals['_NODESTARTMSG']._serialized_start=24192
+  _globals['_NODESTARTMSG']._serialized_end=24286
+  _globals['_NODEFINISHED']._serialized_start=24288
+  _globals['_NODEFINISHED']._serialized_end=24391
+  _globals['_NODEFINISHEDMSG']._serialized_start=24393
+  _globals['_NODEFINISHEDMSG']._serialized_end=24493
+  _globals['_QUERYCANCELATIONUNSUPPORTED']._serialized_start=24495
+  _globals['_QUERYCANCELATIONUNSUPPORTED']._serialized_end=24538
+  _globals['_QUERYCANCELATIONUNSUPPORTEDMSG']._serialized_start=24541
+  _globals['_QUERYCANCELATIONUNSUPPORTEDMSG']._serialized_end=24671
+  _globals['_CONCURRENCYLINE']._serialized_start=24673
+  _globals['_CONCURRENCYLINE']._serialized_end=24752
+  _globals['_CONCURRENCYLINEMSG']._serialized_start=24754
+  _globals['_CONCURRENCYLINEMSG']._serialized_end=24860
+  _globals['_WRITINGINJECTEDSQLFORNODE']._serialized_start=24862
+  _globals['_WRITINGINJECTEDSQLFORNODE']._serialized_end=24931
+  _globals['_WRITINGINJECTEDSQLFORNODEMSG']._serialized_start=24933
+  _globals['_WRITINGINJECTEDSQLFORNODEMSG']._serialized_end=25059
+  _globals['_NODECOMPILING']._serialized_start=25061
+  _globals['_NODECOMPILING']._serialized_end=25118
+  _globals['_NODECOMPILINGMSG']._serialized_start=25120
+  _globals['_NODECOMPILINGMSG']._serialized_end=25222
+  _globals['_NODEEXECUTING']._serialized_start=25224
+  _globals['_NODEEXECUTING']._serialized_end=25281
+  _globals['_NODEEXECUTINGMSG']._serialized_start=25283
+  _globals['_NODEEXECUTINGMSG']._serialized_end=25385
+  _globals['_LOGHOOKSTARTLINE']._serialized_start=25387
+  _globals['_LOGHOOKSTARTLINE']._serialized_end=25496
+  _globals['_LOGHOOKSTARTLINEMSG']._serialized_start=25498
+  _globals['_LOGHOOKSTARTLINEMSG']._serialized_end=25606
+  _globals['_LOGHOOKENDLINE']._serialized_start=25609
+  _globals['_LOGHOOKENDLINE']._serialized_end=25756
+  _globals['_LOGHOOKENDLINEMSG']._serialized_start=25758
+  _globals['_LOGHOOKENDLINEMSG']._serialized_end=25862
+  _globals['_SKIPPINGDETAILS']._serialized_start=25865
+  _globals['_SKIPPINGDETAILS']._serialized_end=26012
+  _globals['_SKIPPINGDETAILSMSG']._serialized_start=26014
+  _globals['_SKIPPINGDETAILSMSG']._serialized_end=26120
+  _globals['_NOTHINGTODO']._serialized_start=26122
+  _globals['_NOTHINGTODO']._serialized_end=26135
+  _globals['_NOTHINGTODOMSG']._serialized_start=26137
+  _globals['_NOTHINGTODOMSG']._serialized_end=26235
+  _globals['_RUNNINGOPERATIONUNCAUGHTERROR']._serialized_start=26237
+  _globals['_RUNNINGOPERATIONUNCAUGHTERROR']._serialized_end=26281
+  _globals['_RUNNINGOPERATIONUNCAUGHTERRORMSG']._serialized_start=26284
+  _globals['_RUNNINGOPERATIONUNCAUGHTERRORMSG']._serialized_end=26418
+  _globals['_ENDRUNRESULT']._serialized_start=26421
+  _globals['_ENDRUNRESULT']._serialized_end=26568
+  _globals['_ENDRUNRESULTMSG']._serialized_start=26570
+  _globals['_ENDRUNRESULTMSG']._serialized_end=26670
+  _globals['_NONODESSELECTED']._serialized_start=26672
+  _globals['_NONODESSELECTED']._serialized_end=26689
+  _globals['_NONODESSELECTEDMSG']._serialized_start=26691
+  _globals['_NONODESSELECTEDMSG']._serialized_end=26797
+  _globals['_COMMANDCOMPLETED']._serialized_start=26799
+  _globals['_COMMANDCOMPLETED']._serialized_end=26918
+  _globals['_COMMANDCOMPLETEDMSG']._serialized_start=26920
+  _globals['_COMMANDCOMPLETEDMSG']._serialized_end=27028
+  _globals['_SHOWNODE']._serialized_start=27030
+  _globals['_SHOWNODE']._serialized_end=27137
+  _globals['_SHOWNODEMSG']._serialized_start=27139
+  _globals['_SHOWNODEMSG']._serialized_end=27231
+  _globals['_COMPILEDNODE']._serialized_start=27233
+  _globals['_COMPILEDNODE']._serialized_end=27345
+  _globals['_COMPILEDNODEMSG']._serialized_start=27347
+  _globals['_COMPILEDNODEMSG']._serialized_end=27447
+  _globals['_CATCHABLEEXCEPTIONONRUN']._serialized_start=27449
+  _globals['_CATCHABLEEXCEPTIONONRUN']._serialized_end=27547
+  _globals['_CATCHABLEEXCEPTIONONRUNMSG']._serialized_start=27549
+  _globals['_CATCHABLEEXCEPTIONONRUNMSG']._serialized_end=27671
+  _globals['_INTERNALERRORONRUN']._serialized_start=27673
+  _globals['_INTERNALERRORONRUN']._serialized_end=27768
+  _globals['_INTERNALERRORONRUNMSG']._serialized_start=27770
+  _globals['_INTERNALERRORONRUNMSG']._serialized_end=27882
+  _globals['_GENERICEXCEPTIONONRUN']._serialized_start=27884
+  _globals['_GENERICEXCEPTIONONRUN']._serialized_end=28001
+  _globals['_GENERICEXCEPTIONONRUNMSG']._serialized_start=28003
+  _globals['_GENERICEXCEPTIONONRUNMSG']._serialized_end=28121
+  _globals['_NODECONNECTIONRELEASEERROR']._serialized_start=28123
+  _globals['_NODECONNECTIONRELEASEERROR']._serialized_end=28201
+  _globals['_NODECONNECTIONRELEASEERRORMSG']._serialized_start=28204
+  _globals['_NODECONNECTIONRELEASEERRORMSG']._serialized_end=28332
+  _globals['_FOUNDSTATS']._serialized_start=28334
+  _globals['_FOUNDSTATS']._serialized_end=28365
+  _globals['_FOUNDSTATSMSG']._serialized_start=28367
+  _globals['_FOUNDSTATSMSG']._serialized_end=28463
+  _globals['_MAINKEYBOARDINTERRUPT']._serialized_start=28465
+  _globals['_MAINKEYBOARDINTERRUPT']._serialized_end=28488
+  _globals['_MAINKEYBOARDINTERRUPTMSG']._serialized_start=28490
+  _globals['_MAINKEYBOARDINTERRUPTMSG']._serialized_end=28608
+  _globals['_MAINENCOUNTEREDERROR']._serialized_start=28610
+  _globals['_MAINENCOUNTEREDERROR']._serialized_end=28645
+  _globals['_MAINENCOUNTEREDERRORMSG']._serialized_start=28647
+  _globals['_MAINENCOUNTEREDERRORMSG']._serialized_end=28763
+  _globals['_MAINSTACKTRACE']._serialized_start=28765
+  _globals['_MAINSTACKTRACE']._serialized_end=28802
+  _globals['_MAINSTACKTRACEMSG']._serialized_start=28804
+  _globals['_MAINSTACKTRACEMSG']._serialized_end=28908
+  _globals['_TIMINGINFOCOLLECTED']._serialized_start=28910
+  _globals['_TIMINGINFOCOLLECTED']._serialized_end=29022
+  _globals['_TIMINGINFOCOLLECTEDMSG']._serialized_start=29024
+  _globals['_TIMINGINFOCOLLECTEDMSG']._serialized_end=29138
+  _globals['_LOGDEBUGSTACKTRACE']._serialized_start=29140
+  _globals['_LOGDEBUGSTACKTRACE']._serialized_end=29178
+  _globals['_LOGDEBUGSTACKTRACEMSG']._serialized_start=29180
+  _globals['_LOGDEBUGSTACKTRACEMSG']._serialized_end=29292
+  _globals['_CHECKCLEANPATH']._serialized_start=29294
+  _globals['_CHECKCLEANPATH']._serialized_end=29324
+  _globals['_CHECKCLEANPATHMSG']._serialized_start=29326
+  _globals['_CHECKCLEANPATHMSG']._serialized_end=29430
+  _globals['_CONFIRMCLEANPATH']._serialized_start=29432
+  _globals['_CONFIRMCLEANPATH']._serialized_end=29464
+  _globals['_CONFIRMCLEANPATHMSG']._serialized_start=29466
+  _globals['_CONFIRMCLEANPATHMSG']._serialized_end=29574
+  _globals['_PROTECTEDCLEANPATH']._serialized_start=29576
+  _globals['_PROTECTEDCLEANPATH']._serialized_end=29610
+  _globals['_PROTECTEDCLEANPATHMSG']._serialized_start=29612
+  _globals['_PROTECTEDCLEANPATHMSG']._serialized_end=29724
+  _globals['_FINISHEDCLEANPATHS']._serialized_start=29726
+  _globals['_FINISHEDCLEANPATHS']._serialized_end=29746
+  _globals['_FINISHEDCLEANPATHSMSG']._serialized_start=29748
+  _globals['_FINISHEDCLEANPATHSMSG']._serialized_end=29860
+  _globals['_OPENCOMMAND']._serialized_start=29862
+  _globals['_OPENCOMMAND']._serialized_end=29915
+  _globals['_OPENCOMMANDMSG']._serialized_start=29917
+  _globals['_OPENCOMMANDMSG']._serialized_end=30015
+  _globals['_SERVINGDOCSPORT']._serialized_start=30017
+  _globals['_SERVINGDOCSPORT']._serialized_end=30065
+  _globals['_SERVINGDOCSPORTMSG']._serialized_start=30067
+  _globals['_SERVINGDOCSPORTMSG']._serialized_end=30173
+  _globals['_SERVINGDOCSACCESSINFO']._serialized_start=30175
+  _globals['_SERVINGDOCSACCESSINFO']._serialized_end=30212
+  _globals['_SERVINGDOCSACCESSINFOMSG']._serialized_start=30214
+  _globals['_SERVINGDOCSACCESSINFOMSG']._serialized_end=30332
+  _globals['_SERVINGDOCSEXITINFO']._serialized_start=30334
+  _globals['_SERVINGDOCSEXITINFO']._serialized_end=30355
+  _globals['_SERVINGDOCSEXITINFOMSG']._serialized_start=30357
+  _globals['_SERVINGDOCSEXITINFOMSG']._serialized_end=30471
+  _globals['_RUNRESULTWARNING']._serialized_start=30473
+  _globals['_RUNRESULTWARNING']._serialized_end=30589
+  _globals['_RUNRESULTWARNINGMSG']._serialized_start=30591
+  _globals['_RUNRESULTWARNINGMSG']._serialized_end=30699
+  _globals['_RUNRESULTFAILURE']._serialized_start=30701
+  _globals['_RUNRESULTFAILURE']._serialized_end=30817
+  _globals['_RUNRESULTFAILUREMSG']._serialized_start=30819
+  _globals['_RUNRESULTFAILUREMSG']._serialized_end=30927
+  _globals['_STATSLINE']._serialized_start=30929
+  _globals['_STATSLINE']._serialized_end=31036
+  _globals['_STATSLINE_STATSENTRY']._serialized_start=30992
+  _globals['_STATSLINE_STATSENTRY']._serialized_end=31036
+  _globals['_STATSLINEMSG']._serialized_start=31038
+  _globals['_STATSLINEMSG']._serialized_end=31132
+  _globals['_RUNRESULTERROR']._serialized_start=31134
+  _globals['_RUNRESULTERROR']._serialized_end=31205
+  _globals['_RUNRESULTERRORMSG']._serialized_start=31207
+  _globals['_RUNRESULTERRORMSG']._serialized_end=31311
+  _globals['_RUNRESULTERRORNOMESSAGE']._serialized_start=31313
+  _globals['_RUNRESULTERRORNOMESSAGE']._serialized_end=31396
+  _globals['_RUNRESULTERRORNOMESSAGEMSG']._serialized_start=31398
+  _globals['_RUNRESULTERRORNOMESSAGEMSG']._serialized_end=31520
+  _globals['_SQLCOMPILEDPATH']._serialized_start=31522
+  _globals['_SQLCOMPILEDPATH']._serialized_end=31595
+  _globals['_SQLCOMPILEDPATHMSG']._serialized_start=31597
+  _globals['_SQLCOMPILEDPATHMSG']._serialized_end=31703
+  _globals['_CHECKNODETESTFAILURE']._serialized_start=31705
+  _globals['_CHECKNODETESTFAILURE']._serialized_end=31792
+  _globals['_CHECKNODETESTFAILUREMSG']._serialized_start=31794
+  _globals['_CHECKNODETESTFAILUREMSG']._serialized_end=31910
+  _globals['_ENDOFRUNSUMMARY']._serialized_start=31912
+  _globals['_ENDOFRUNSUMMARY']._serialized_end=31999
+  _globals['_ENDOFRUNSUMMARYMSG']._serialized_start=32001
+  _globals['_ENDOFRUNSUMMARYMSG']._serialized_end=32107
+  _globals['_LOGSKIPBECAUSEERROR']._serialized_start=32109
+  _globals['_LOGSKIPBECAUSEERROR']._serialized_end=32194
+  _globals['_LOGSKIPBECAUSEERRORMSG']._serialized_start=32196
+  _globals['_LOGSKIPBECAUSEERRORMSG']._serialized_end=32310
+  _globals['_ENSUREGITINSTALLED']._serialized_start=32312
+  _globals['_ENSUREGITINSTALLED']._serialized_end=32332
+  _globals['_ENSUREGITINSTALLEDMSG']._serialized_start=32334
+  _globals['_ENSUREGITINSTALLEDMSG']._serialized_end=32446
+  _globals['_DEPSCREATINGLOCALSYMLINK']._serialized_start=32448
+  _globals['_DEPSCREATINGLOCALSYMLINK']._serialized_end=32474
+  _globals['_DEPSCREATINGLOCALSYMLINKMSG']._serialized_start=32476
+  _globals['_DEPSCREATINGLOCALSYMLINKMSG']._serialized_end=32600
+  _globals['_DEPSSYMLINKNOTAVAILABLE']._serialized_start=32602
+  _globals['_DEPSSYMLINKNOTAVAILABLE']._serialized_end=32627
+  _globals['_DEPSSYMLINKNOTAVAILABLEMSG']._serialized_start=32629
+  _globals['_DEPSSYMLINKNOTAVAILABLEMSG']._serialized_end=32751
+  _globals['_DISABLETRACKING']._serialized_start=32753
+  _globals['_DISABLETRACKING']._serialized_end=32770
+  _globals['_DISABLETRACKINGMSG']._serialized_start=32772
+  _globals['_DISABLETRACKINGMSG']._serialized_end=32878
+  _globals['_SENDINGEVENT']._serialized_start=32880
+  _globals['_SENDINGEVENT']._serialized_end=32910
+  _globals['_SENDINGEVENTMSG']._serialized_start=32912
+  _globals['_SENDINGEVENTMSG']._serialized_end=33012
+  _globals['_SENDEVENTFAILURE']._serialized_start=33014
+  _globals['_SENDEVENTFAILURE']._serialized_end=33032
+  _globals['_SENDEVENTFAILUREMSG']._serialized_start=33034
+  _globals['_SENDEVENTFAILUREMSG']._serialized_end=33142
+  _globals['_FLUSHEVENTS']._serialized_start=33144
+  _globals['_FLUSHEVENTS']._serialized_end=33157
+  _globals['_FLUSHEVENTSMSG']._serialized_start=33159
+  _globals['_FLUSHEVENTSMSG']._serialized_end=33257
+  _globals['_FLUSHEVENTSFAILURE']._serialized_start=33259
+  _globals['_FLUSHEVENTSFAILURE']._serialized_end=33279
+  _globals['_FLUSHEVENTSFAILUREMSG']._serialized_start=33281
+  _globals['_FLUSHEVENTSFAILUREMSG']._serialized_end=33393
+  _globals['_TRACKINGINITIALIZEFAILURE']._serialized_start=33395
+  _globals['_TRACKINGINITIALIZEFAILURE']._serialized_end=33440
+  _globals['_TRACKINGINITIALIZEFAILUREMSG']._serialized_start=33442
+  _globals['_TRACKINGINITIALIZEFAILUREMSG']._serialized_end=33568
+  _globals['_RUNRESULTWARNINGMESSAGE']._serialized_start=33570
+  _globals['_RUNRESULTWARNINGMESSAGE']._serialized_end=33650
+  _globals['_RUNRESULTWARNINGMESSAGEMSG']._serialized_start=33652
+  _globals['_RUNRESULTWARNINGMESSAGEMSG']._serialized_end=33774
+  _globals['_DEBUGCMDOUT']._serialized_start=33776
+  _globals['_DEBUGCMDOUT']._serialized_end=33802
+  _globals['_DEBUGCMDOUTMSG']._serialized_start=33804
+  _globals['_DEBUGCMDOUTMSG']._serialized_end=33902
+  _globals['_DEBUGCMDRESULT']._serialized_start=33904
+  _globals['_DEBUGCMDRESULT']._serialized_end=33933
+  _globals['_DEBUGCMDRESULTMSG']._serialized_start=33935
+  _globals['_DEBUGCMDRESULTMSG']._serialized_end=34039
+  _globals['_LISTCMDOUT']._serialized_start=34041
+  _globals['_LISTCMDOUT']._serialized_end=34066
+  _globals['_LISTCMDOUTMSG']._serialized_start=34068
+  _globals['_LISTCMDOUTMSG']._serialized_end=34164
+  _globals['_RESOURCEREPORT']._serialized_start=34167
+  _globals['_RESOURCEREPORT']._serialized_end=34403
+  _globals['_RESOURCEREPORTMSG']._serialized_start=34405
+  _globals['_RESOURCEREPORTMSG']._serialized_end=34509
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dbt_core-1.8.0b3/dbt/events/logging.py` & `dbt_core-1.8.0rc1/dbt/events/logging.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/events/types.py` & `dbt_core-1.8.0rc1/dbt/events/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,20 +53,15 @@
     def code(self) -> str:
         return "A003"
 
     def message(self) -> str:
         return f"Tracking: {self.user_state}"
 
 
-class MergedFromState(DebugLevel):
-    def code(self) -> str:
-        return "A004"
-
-    def message(self) -> str:
-        return f"Merged {self.num_merged} items from state (sample: {self.sample})"
+# Removed A004: MergedFromState
 
 
 class MissingProfileTarget(InfoLevel):
     def code(self) -> str:
         return "A005"
 
     def message(self) -> str:
@@ -409,49 +404,60 @@
             "User config should be moved from the 'config' key in profiles.yml to the 'flags' "
             "key in dbt_project.yml."
         )
         # Can't use line_wrap_message here because flags.printer_width isn't available yet
         return warning_tag(f"Deprecated functionality\n\n{description}")
 
 
-class SpacesInModelNameDeprecation(DynamicLevel):
+class SpacesInResourceNameDeprecation(DynamicLevel):
     def code(self) -> str:
         return "D014"
 
     def message(self) -> str:
-        version = ".v" + self.model_version if self.model_version else ""
-        description = (
-            f"Model `{self.model_name}{version}` has spaces in its name. This is deprecated and "
-            "may cause errors when using dbt."
-        )
+        description = f"Found spaces in the name of `{self.unique_id}`"
 
         if self.level == EventLevel.ERROR.value:
             description = error_tag(description)
         elif self.level == EventLevel.WARN.value:
             description = warning_tag(description)
 
         return line_wrap_message(description)
 
 
-class TotalModelNamesWithSpacesDeprecation(DynamicLevel):
+class ResourceNamesWithSpacesDeprecation(WarnLevel):
     def code(self) -> str:
         return "D015"
 
     def message(self) -> str:
-        description = f"Spaces in model names found in {self.count_invalid_names} model(s), which is deprecated."
+        description = f"Spaces found in {self.count_invalid_names} resource name(s). This is deprecated, and may lead to errors when using dbt. For more information: https://docs.getdbt.com/reference/global-configs/legacy-behaviors#require_resource_names_without_spaces"
 
         if self.show_debug_hint:
             description += " Run again with `--debug` to see them all."
 
-        if self.level == EventLevel.ERROR.value:
-            description = error_tag(description)
-        elif self.level == EventLevel.WARN.value:
-            description = warning_tag(description)
+        return line_wrap_message(warning_tag(description))
 
-        return line_wrap_message(description)
+
+class PackageMaterializationOverrideDeprecation(WarnLevel):
+    def code(self) -> str:
+        return "D016"
+
+    def message(self) -> str:
+        description = f"Installed package '{self.package_name}' is overriding the built-in materialization '{self.materialization_name}'. Overrides of built-in materializations from installed packages will be deprecated in future versions of dbt. Please refer to https://docs.getdbt.com/reference/global-configs/legacy-behaviors#require_explicit_package_overrides_for_builtin_materializations for detailed documentation and suggested workarounds."
+
+        return line_wrap_message(warning_tag(description))
+
+
+class SourceFreshnessProjectHooksNotRun(WarnLevel):
+    def code(self) -> str:
+        return "D017"
+
+    def message(self) -> str:
+        description = "In a future version of dbt, the `source freshness` command will start running `on-run-start` and `on-run-end` hooks by default. Please refer to https://docs.getdbt.com/reference/global-configs/legacy-behaviors#source_freshness_run_project_hooks for detailed documentation and suggested workarounds."
+
+        return line_wrap_message(warning_tag(description))
 
 
 # =======================================================
 # I - Project parsing
 # =======================================================
```

### Comparing `dbt_core-1.8.0b3/dbt/exceptions.py` & `dbt_core-1.8.0rc1/dbt/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     DbtValidationError,
     CommandResultError,
 )
 from dbt.node_types import NodeType, AccessType, REFABLE_NODE_TYPES
 
 from dbt_common.dataclass_schema import ValidationError
 
-from dbt.constants import SECRET_ENV_PREFIX
+from dbt_common.constants import SECRET_ENV_PREFIX
 
 
 if TYPE_CHECKING:
     import agate
 
 
 class ContractBreakingChangeError(DbtRuntimeError):
@@ -109,14 +109,18 @@
     pass
 
 
 class DbtProfileError(DbtConfigError):
     pass
 
 
+class DbtExclusivePropertyUseError(DbtConfigError):
+    pass
+
+
 class InvalidSelectorError(DbtRuntimeError):
     def __init__(self, name: str) -> None:
         self.name = name
         super().__init__(name)
 
 
 class DuplicateYamlKeyError(CompilationError):
```

### Comparing `dbt_core-1.8.0b3/dbt/flags.py` & `dbt_core-1.8.0rc1/dbt/flags.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/graph/cli.py` & `dbt_core-1.8.0rc1/dbt/graph/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,24 +24,23 @@
 DEFAULT_INCLUDES: List[str] = ["fqn:*", "source:*", "exposure:*", "metric:*", "semantic_model:*"]
 DEFAULT_EXCLUDES: List[str] = []
 
 
 def parse_union(
     components: List[str],
     expect_exists: bool,
-    indirect_selection: IndirectSelection = IndirectSelection.Eager,
 ) -> SelectionUnion:
     # turn ['a b', 'c'] -> ['a', 'b', 'c']
     raw_specs = itertools.chain.from_iterable(r.split(" ") for r in components)
     union_components: List[SelectionSpec] = []
     flags = get_flags()
     # ['a', 'b', 'c,d'] -> union('a', 'b', intersection('c', 'd'))
     for raw_spec in raw_specs:
         intersection_components: List[SelectionSpec] = [
-            SelectionCriteria.from_single_spec(part, indirect_selection=indirect_selection)
+            SelectionCriteria.from_single_spec(part)
             for part in raw_spec.split(INTERSECTION_DELIMITER)
         ]
         union_components.append(
             SelectionIntersection(
                 components=intersection_components,
                 expect_exists=expect_exists,
                 raw=raw_spec,
@@ -52,49 +51,33 @@
         components=union_components,
         expect_exists=False,
         raw=components,
         indirect_selection=IndirectSelection(flags.INDIRECT_SELECTION),
     )
 
 
-def parse_union_from_default(
-    raw: Optional[List[str]],
-    default: List[str],
-    indirect_selection: IndirectSelection = IndirectSelection.Eager,
-) -> SelectionUnion:
+def parse_union_from_default(raw: Optional[List[str]], default: List[str]) -> SelectionUnion:
     components: List[str]
     expect_exists: bool
     if raw is None:
-        return parse_union(
-            components=default, expect_exists=False, indirect_selection=indirect_selection
-        )
+        return parse_union(components=default, expect_exists=False)
     else:
-        return parse_union(
-            components=raw, expect_exists=True, indirect_selection=indirect_selection
-        )
+        return parse_union(components=raw, expect_exists=True)
 
 
 def parse_difference(
-    include: Optional[List[str]], exclude: Optional[List[str]], indirect_selection: Any
+    include: Optional[List[str]], exclude: Optional[List[str]]
 ) -> SelectionDifference:
 
     if include == ():
         include = None
 
-    included = parse_union_from_default(
-        include, DEFAULT_INCLUDES, indirect_selection=IndirectSelection(indirect_selection)
-    )
-    flags = get_flags()
-    excluded = parse_union_from_default(
-        exclude, DEFAULT_EXCLUDES, indirect_selection=IndirectSelection(flags.INDIRECT_SELECTION)
-    )
-    return SelectionDifference(
-        components=[included, excluded],
-        indirect_selection=IndirectSelection(flags.INDIRECT_SELECTION),
-    )
+    included = parse_union_from_default(include, DEFAULT_INCLUDES)
+    excluded = parse_union_from_default(exclude, DEFAULT_EXCLUDES)
+    return SelectionDifference(components=[included, excluded])
 
 
 RawDefinition = Union[str, Dict[str, Any]]
 
 
 def _get_list_dicts(dct: Dict[str, Any], key: str) -> List[RawDefinition]:
     result: List[RawDefinition] = []
```

### Comparing `dbt_core-1.8.0b3/dbt/graph/graph.py` & `dbt_core-1.8.0rc1/dbt/graph/graph.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/graph/queue.py` & `dbt_core-1.8.0rc1/dbt/graph/queue.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/graph/selector.py` & `dbt_core-1.8.0rc1/dbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/graph/selector_methods.py` & `dbt_core-1.8.0rc1/dbt/graph/selector_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,14 +451,18 @@
             elif fnmatch(Path(node.original_file_path).stem, selector):
                 yield unique_id
 
 
 class PackageSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """Yields nodes from included that have the specified package"""
+        # `this` is an alias for the current dbt project name
+        if selector == "this" and self.manifest.metadata.project_name is not None:
+            selector = self.manifest.metadata.project_name
+
         for unique_id, node in self.all_nodes(included_nodes):
             if fnmatch(node.package_name, selector):
                 yield unique_id
 
 
 def _getattr_descend(obj: Any, attrs: List[str]) -> Any:
     value = obj
```

### Comparing `dbt_core-1.8.0b3/dbt/graph/selector_spec.py` & `dbt_core-1.8.0rc1/dbt/graph/selector_spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
 import re
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 from dbt_common.dataclass_schema import StrEnum, dbtClassMixin
 
+
 from typing import Set, Iterator, List, Optional, Dict, Union, Any, Iterable, Tuple
 from .graph import UniqueId
 from .selector_methods import MethodName
 from dbt_common.exceptions import DbtRuntimeError
 from dbt.exceptions import InvalidSelectorError
+from dbt.flags import get_flags
 
 
 RAW_SELECTOR_PATTERN = re.compile(
     r"\A"
     r"(?P<childrens_parents>(\@))?"
     r"(?P<parents>((?P<parents_depth>(\d*))\+))?"
     r"((?P<method>([\w.]+)):)?(?P<value>(.*?))"
@@ -106,26 +108,25 @@
         return method_name, method_arguments
 
     @classmethod
     def selection_criteria_from_dict(
         cls,
         raw: Any,
         dct: Dict[str, Any],
-        indirect_selection: IndirectSelection = IndirectSelection.Eager,
     ) -> "SelectionCriteria":
         if "value" not in dct:
             raise DbtRuntimeError(f'Invalid node spec "{raw}" - no search value!')
         method_name, method_arguments = cls.parse_method(dct)
 
         parents_depth = _match_to_int(dct, "parents_depth")
         children_depth = _match_to_int(dct, "children_depth")
 
         # If defined field in selector, override CLI flag
         indirect_selection = IndirectSelection(
-            dct.get("indirect_selection", None) or indirect_selection
+            dct.get("indirect_selection", get_flags().INDIRECT_SELECTION)
         )
 
         return cls(
             raw=raw,
             method=method_name,
             method_arguments=method_arguments,
             value=dct["value"],
@@ -154,25 +155,21 @@
         if "parents" in dct:
             dct["parents"] = bool(dct.get("parents"))
         if "children" in dct:
             dct["children"] = bool(dct.get("children"))
         return dct
 
     @classmethod
-    def from_single_spec(
-        cls, raw: str, indirect_selection: IndirectSelection = IndirectSelection.Eager
-    ) -> "SelectionCriteria":
+    def from_single_spec(cls, raw: str) -> "SelectionCriteria":
         result = RAW_SELECTOR_PATTERN.match(raw)
         if result is None:
             # bad spec!
             raise DbtRuntimeError(f'Invalid selector spec "{raw}"')
 
-        return cls.selection_criteria_from_dict(
-            raw, result.groupdict(), indirect_selection=indirect_selection
-        )
+        return cls.selection_criteria_from_dict(raw, result.groupdict())
 
 
 class BaseSelectionGroup(dbtClassMixin, Iterable[SelectionSpec], metaclass=ABCMeta):
     def __init__(
         self,
         components: Iterable[SelectionSpec],
         indirect_selection: IndirectSelection = IndirectSelection.Eager,
```

### Comparing `dbt_core-1.8.0b3/dbt/include/README.md` & `dbt_core-1.8.0rc1/dbt/include/README.md`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/include/starter_project/README.md` & `dbt_core-1.8.0rc1/dbt/include/starter_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/include/starter_project/dbt_project.yml` & `dbt_core-1.8.0rc1/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/internal_deprecations.py` & `dbt_core-1.8.0rc1/dbt/internal_deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/logger.py` & `dbt_core-1.8.0rc1/dbt/logger.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/node_types.py` & `dbt_core-1.8.0rc1/dbt/node_types.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/__init__.py` & `dbt_core-1.8.0rc1/dbt/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/analysis.py` & `dbt_core-1.8.0rc1/dbt/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/base.py` & `dbt_core-1.8.0rc1/dbt/parser/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                     package_macro, imported_macro_context
                 )
 
         self.package_updaters = package_updaters
         self.component = component
 
     def __call__(self, parsed_node: Any, override: Optional[str]) -> None:
-        if parsed_node.package_name in self.package_updaters:
+        if getattr(parsed_node, "package_name", None) in self.package_updaters:
             new_value = self.package_updaters[parsed_node.package_name](override, parsed_node)
         else:
             new_value = self.default_updater(override, parsed_node)
 
         if isinstance(new_value, str):
             new_value = new_value.strip()
         setattr(parsed_node, self.component, new_value)
@@ -289,15 +289,15 @@
 
         # These call the RelationUpdate callable to go through generate_name macros
         self._update_node_database(parsed_node, config_dict.get("database"))
         self._update_node_schema(parsed_node, config_dict.get("schema"))
         self._update_node_alias(parsed_node, config_dict.get("alias"))
 
         # Snapshot nodes use special "target_database" and "target_schema" fields for some reason
-        if parsed_node.resource_type == NodeType.Snapshot:
+        if getattr(parsed_node, "resource_type", None) == NodeType.Snapshot:
             if "target_database" in config_dict and config_dict["target_database"]:
                 parsed_node.database = config_dict["target_database"]
             if "target_schema" in config_dict and config_dict["target_schema"]:
                 parsed_node.schema = config_dict["target_schema"]
 
         self._update_node_relation_name(parsed_node)
 
@@ -448,15 +448,15 @@
         return result
 
     def _update_node_relation_name(self, node: ManifestNode):
         # Seed and Snapshot nodes and Models that are not ephemeral,
         # and TestNodes that store_failures.
         # TestNodes do not get a relation_name without store failures
         # because no schema is created.
-        if node.is_relational and not node.is_ephemeral_model:
+        if getattr(node, "is_relational", None) and not getattr(node, "is_ephemeral_model", None):
             adapter = get_adapter(self.root_project)
             relation_cls = adapter.Relation
             node.relation_name = str(relation_cls.create_from(self.root_project, node))
         else:
             # Set it to None in case it changed with a config update
             node.relation_name = None
```

### Comparing `dbt_core-1.8.0b3/dbt/parser/common.py` & `dbt_core-1.8.0rc1/dbt/parser/common.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/docs.py` & `dbt_core-1.8.0rc1/dbt/parser/docs.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/fixtures.py` & `dbt_core-1.8.0rc1/dbt/parser/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/generic_test.py` & `dbt_core-1.8.0rc1/dbt/parser/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/generic_test_builders.py` & `dbt_core-1.8.0rc1/dbt/parser/generic_test_builders.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/hooks.py` & `dbt_core-1.8.0rc1/dbt/parser/hooks.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/macros.py` & `dbt_core-1.8.0rc1/dbt/parser/macros.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/manifest.py` & `dbt_core-1.8.0rc1/dbt/parser/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from dbt_common.exceptions.base import DbtValidationError
 import dbt_common.utils
 import json
 import pprint
 from dbt.mp_context import get_mp_context
 import msgpack
 
+import dbt.deprecations
 import dbt.exceptions
 import dbt.tracking
 import dbt.utils
 from dbt.flags import get_flags
 
 from dbt.adapters.factory import (
     get_adapter,
@@ -40,16 +41,16 @@
     get_adapter_package_names,
     register_adapter,
 )
 from dbt.constants import (
     MANIFEST_FILE_NAME,
     PARTIAL_PARSE_FILE_NAME,
     SEMANTIC_MANIFEST_FILE_NAME,
-    SECRET_ENV_PREFIX,
 )
+from dbt_common.constants import SECRET_ENV_PREFIX
 from dbt_common.helper_types import PathSet
 from dbt_common.events.functions import fire_event, get_invocation_id, warn_or_error
 from dbt_common.events.types import (
     Note,
 )
 from dbt.events.types import (
     PartialParsingErrorProcessingFile,
@@ -60,17 +61,16 @@
     PartialParsingNotEnabled,
     ParsedFileLoadFailed,
     InvalidDisabledTargetInTestNode,
     NodeNotFoundOrDisabled,
     StateCheckVarsHash,
     DeprecatedModel,
     DeprecatedReference,
-    SpacesInModelNameDeprecation,
-    TotalModelNamesWithSpacesDeprecation,
     UpcomingReferenceDeprecation,
+    SpacesInResourceNameDeprecation,
 )
 from dbt.logger import DbtProcessState
 from dbt.node_types import NodeType, AccessType
 from dbt.clients.jinja import get_rendered, MacroStack
 from dbt.clients.jinja_static import statically_extract_macro_calls
 from dbt_common.clients.system import (
     make_directory,
@@ -521,15 +521,15 @@
                 # parent and child maps will be rebuilt by write_manifest
 
         if not self.skip_parsing or external_nodes_modified:
             # write out the fully parsed manifest
             self.write_manifest_for_partial_parse()
 
         self.check_for_model_deprecations()
-        self.check_for_spaces_in_model_names()
+        self.check_for_spaces_in_resource_names()
 
         return self.manifest
 
     def safe_update_project_parser_files_partially(self, project_parser_files: Dict) -> Dict:
         if self.saved_manifest is None:
             return project_parser_files
 
@@ -623,54 +623,51 @@
                                 ref_model_name=resolved_ref.name,
                                 ref_model_version=version_to_str(resolved_ref.version),
                                 ref_model_latest_version=str(resolved_ref.latest_version),
                                 ref_model_deprecation_date=resolved_ref.deprecation_date.isoformat(),
                             )
                         )
 
-    def check_for_spaces_in_model_names(self):
-        """Validates that model names do not contain spaces
+    def check_for_spaces_in_resource_names(self):
+        """Validates that resource names do not contain spaces
 
         If `DEBUG` flag is `False`, logs only first bad model name
         If `DEBUG` flag is `True`, logs every bad model name
-        If `ALLOW_SPACES_IN_MODEL_NAMES` is `False`, logs are `ERROR` level and an exception is raised if any names are bad
-        If `ALLOW_SPACES_IN_MODEL_NAMES` is `True`, logs are `WARN` level
+        If `REQUIRE_RESOURCE_NAMES_WITHOUT_SPACES` is `True`, logs are `ERROR` level and an exception is raised if any names are bad
+        If `REQUIRE_RESOURCE_NAMES_WITHOUT_SPACES` is `False`, logs are `WARN` level
         """
-        improper_model_names = 0
+        improper_resource_names = 0
         level = (
-            EventLevel.WARN
-            if self.root_project.args.ALLOW_SPACES_IN_MODEL_NAMES
-            else EventLevel.ERROR
+            EventLevel.ERROR
+            if self.root_project.args.REQUIRE_RESOURCE_NAMES_WITHOUT_SPACES
+            else EventLevel.WARN
         )
 
         for node in self.manifest.nodes.values():
-            if isinstance(node, ModelNode) and " " in node.name:
-                if improper_model_names == 0 or self.root_project.args.DEBUG:
+            if " " in node.name:
+                if improper_resource_names == 0 or self.root_project.args.DEBUG:
                     fire_event(
-                        SpacesInModelNameDeprecation(
-                            model_name=node.name,
-                            model_version=version_to_str(node.version),
+                        SpacesInResourceNameDeprecation(
+                            unique_id=node.unique_id,
                             level=level.value,
                         ),
                         level=level,
                     )
-                improper_model_names += 1
+                improper_resource_names += 1
 
-        if improper_model_names > 0:
-            fire_event(
-                TotalModelNamesWithSpacesDeprecation(
-                    count_invalid_names=improper_model_names,
-                    show_debug_hint=(not self.root_project.args.DEBUG),
-                    level=level.value,
-                ),
-                level=level,
-            )
-
-            if level == EventLevel.ERROR:
-                raise DbtValidationError("Model names cannot contain spaces")
+        if improper_resource_names > 0:
+            if level == EventLevel.WARN:
+                flags = get_flags()
+                dbt.deprecations.warn(
+                    "resource-names-with-spaces",
+                    count_invalid_names=improper_resource_names,
+                    show_debug_hint=(not flags.DEBUG),
+                )
+            else:  # ERROR level
+                raise DbtValidationError("Resource names cannot contain spaces")
 
     def load_and_parse_macros(self, project_parser_files):
         for project in self.all_projects.values():
             if project.project_name not in project_parser_files:
                 continue
             parser_files = project_parser_files[project.project_name]
             if "MacroParser" in parser_files:
@@ -1885,23 +1882,29 @@
     file_name = MANIFEST_FILE_NAME
     path = os.path.join(target_path, file_name)
     manifest.write(path)
 
     write_semantic_manifest(manifest=manifest, target_path=target_path)
 
 
-def parse_manifest(runtime_config, write_perf_info, write, write_json):
+def parse_manifest(
+    runtime_config: RuntimeConfig,
+    write_perf_info: bool,
+    write: bool,
+    write_json: bool,
+) -> Manifest:
     register_adapter(runtime_config, get_mp_context())
     adapter = get_adapter(runtime_config)
     adapter.set_macro_context_generator(generate_runtime_macro_context)
     manifest = ManifestLoader.get_full_manifest(
         runtime_config,
         write_perf_info=write_perf_info,
     )
 
+    # If we should (over)write the manifest in the target path, do that now
     if write and write_json:
         write_manifest(manifest, runtime_config.project_target_path)
         pm = plugins.get_plugin_manager(runtime_config.project_name)
         plugin_artifacts = pm.get_manifest_artifacts(manifest)
         for path, plugin_artifact in plugin_artifacts.items():
             plugin_artifact.write(path)
     return manifest
```

### Comparing `dbt_core-1.8.0b3/dbt/parser/models.py` & `dbt_core-1.8.0rc1/dbt/parser/models.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/partial.py` & `dbt_core-1.8.0rc1/dbt/parser/partial.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/read_files.py` & `dbt_core-1.8.0rc1/dbt/parser/read_files.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/schema_generic_tests.py` & `dbt_core-1.8.0rc1/dbt/parser/schema_generic_tests.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/schema_renderer.py` & `dbt_core-1.8.0rc1/dbt/parser/schema_renderer.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/schema_yaml_readers.py` & `dbt_core-1.8.0rc1/dbt/parser/schema_yaml_readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -760,14 +760,30 @@
             query_params=self._get_query_params(unparsed.query_params),
             exports=[self._get_export(export, config) for export in unparsed.exports],
             config=config,
             unrendered_config=unrendered_config,
             group=config.group,
         )
 
+        for export in parsed.exports:
+            self.schema_parser.update_parsed_node_relation_names(export, export.config.to_dict())  # type: ignore
+
+            if not export.config.schema_name:
+                export.config.schema_name = getattr(export, "schema", None)
+            delattr(export, "schema")
+
+            export.config.database = getattr(export, "database", None) or export.config.database
+            delattr(export, "database")
+
+            if not export.config.alias:
+                export.config.alias = getattr(export, "alias", None)
+            delattr(export, "alias")
+
+            delattr(export, "relation_name")
+
         # Only add thes saved query if it's enabled, otherwise we track it with other diabled nodes
         if parsed.config.enabled:
             self.manifest.add_saved_query(self.yaml.file, parsed)
         else:
             self.manifest.add_disabled(self.yaml.file, parsed)
 
     def parse(self) -> ParseResult:
```

### Comparing `dbt_core-1.8.0b3/dbt/parser/schemas.py` & `dbt_core-1.8.0rc1/dbt/parser/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,19 +107,32 @@
 #              ModelPatchParser (models)
 #              AnalysisPatchParser (analyses)
 #              TestablePatchParser (seeds, snapshots)
 #
 # ===============================================================================
 
 
-def yaml_from_file(source_file: SchemaSourceFile) -> Dict[str, Any]:
+def yaml_from_file(source_file: SchemaSourceFile) -> Optional[Dict[str, Any]]:
     """If loading the yaml fails, raise an exception."""
     try:
         # source_file.contents can sometimes be None
-        return load_yaml_text(source_file.contents or "", source_file.path)
+        contents = load_yaml_text(source_file.contents or "", source_file.path)
+
+        if contents is None:
+            return contents
+
+        # When loaded_loaded_at_field is defined as None or null, it shows up in
+        # the dict but when it is not defined, it does not show up in the dict
+        # We need to capture this to be able to override source level settings later.
+        for source in contents.get("sources", []):
+            for table in source.get("tables", []):
+                if "loaded_at_field" in table:
+                    table["loaded_at_field_present"] = True
+
+        return contents
     except DbtValidationError as e:
         raise YamlLoadError(
             project_name=source_file.project_name, path=source_file.path.relative_path, exc=e
         )
 
 
 # This is the main schema file parser, but almost everything happens in the
```

### Comparing `dbt_core-1.8.0b3/dbt/parser/search.py` & `dbt_core-1.8.0rc1/dbt/parser/search.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/seeds.py` & `dbt_core-1.8.0rc1/dbt/parser/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/singular_test.py` & `dbt_core-1.8.0rc1/dbt/parser/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/snapshots.py` & `dbt_core-1.8.0rc1/dbt/parser/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/sources.py` & `dbt_core-1.8.0rc1/dbt/parser/sources.py`

 * *Files 8% similar despite different names*

```diff
@@ -129,15 +129,22 @@
     def parse_source(self, target: UnpatchedSourceDefinition) -> SourceDefinition:
         source = target.source
         table = target.table
         refs = ParserRef.from_target(table)
         unique_id = target.unique_id
         description = table.description or ""
         source_description = source.description or ""
-        loaded_at_field = table.loaded_at_field or source.loaded_at_field
+
+        # We need to be able to tell the difference between explicitly setting the loaded_at_field to None/null
+        # and when it's simply not set.  This allows a user to override the source level loaded_at_field so that
+        # specific table can default to metadata-based freshness.
+        if table.loaded_at_field_present or table.loaded_at_field is not None:
+            loaded_at_field = table.loaded_at_field
+        else:
+            loaded_at_field = source.loaded_at_field  # may be None, that's okay
 
         freshness = merge_freshness(source.freshness, table.freshness)
         quoting = source.quoting.merged(table.quoting)
         # path = block.path.original_file_path
         table_meta = table.meta or {}
         source_meta = source.meta or {}
         meta = {**source_meta, **table_meta}
```

### Comparing `dbt_core-1.8.0b3/dbt/parser/sql.py` & `dbt_core-1.8.0rc1/dbt/parser/sql.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/parser/unit_tests.py` & `dbt_core-1.8.0rc1/dbt/parser/unit_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,18 @@
             }
 
             if original_input_node.resource_type in (
                 NodeType.Model,
                 NodeType.Seed,
                 NodeType.Snapshot,
             ):
-                input_node = ModelNode(**common_fields)
+                input_node = ModelNode(
+                    **common_fields,
+                    defer_relation=original_input_node.defer_relation,
+                )
                 if (
                     original_input_node.resource_type == NodeType.Model
                     and original_input_node.version
                 ):
                     input_node.version = original_input_node.version
 
             elif original_input_node.resource_type == NodeType.Source:
```

### Comparing `dbt_core-1.8.0b3/dbt/plugins/__init__.py` & `dbt_core-1.8.0rc1/dbt/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/plugins/manager.py` & `dbt_core-1.8.0rc1/dbt/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/plugins/manifest.py` & `dbt_core-1.8.0rc1/dbt/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/base.py` & `dbt_core-1.8.0rc1/dbt/task/base.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/build.py` & `dbt_core-1.8.0rc1/dbt/task/build.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/clean.py` & `dbt_core-1.8.0rc1/dbt/task/clean.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/clone.py` & `dbt_core-1.8.0rc1/dbt/task/clone.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,17 +118,16 @@
                     )
                     result.add(other_relation.without_identifier())
 
         return result
 
     def before_run(self, adapter, selected_uids: AbstractSet[str]):
         with adapter.connection_named("master"):
-            # unlike in other tasks, we want to add information from the --state manifest *before* caching!
-            self.defer_to_manifest(adapter, selected_uids)
-            # only create *our* schemas, but cache *other* schemas in addition
+            self.defer_to_manifest()
+            # only create target schemas, but also cache defer_relation schemas
             schemas_to_create = super().get_model_schemas(adapter, selected_uids)
             self.create_schemas(adapter, schemas_to_create)
             schemas_to_cache = self.get_model_schemas(adapter, selected_uids)
             self.populate_adapter_cache(adapter, schemas_to_cache)
 
     @property
     def resource_types(self):
```

### Comparing `dbt_core-1.8.0b3/dbt/task/compile.py` & `dbt_core-1.8.0rc1/dbt/task/compile.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/debug.py` & `dbt_core-1.8.0rc1/dbt/task/debug.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/deps.py` & `dbt_core-1.8.0rc1/dbt/task/deps.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/docs/generate.py` & `dbt_core-1.8.0rc1/dbt/task/docs/generate.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/docs/index.html` & `dbt_core-1.8.0rc1/dbt/task/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -89968,4385 +89968,4388 @@
 0015f6f0: 5b22 6d6f 6465 6c22 2c22 7365 6564 222c  ["model","seed",
 0015f700: 2273 6f75 7263 6522 2c22 736e 6170 7368  "source","snapsh
 0015f710: 6f74 222c 2261 6e61 6c79 7369 7322 2c22  ot","analysis","
 0015f720: 6578 706f 7375 7265 222c 226d 6574 7269  exposure","metri
 0015f730: 6322 2c22 7365 6d61 6e74 6963 5f6d 6f64  c","semantic_mod
 0015f740: 656c 222c 226f 7065 7261 7469 6f6e 225d  el","operation"]
 0015f750: 2c65 2e72 6573 6f75 7263 655f 7479 7065  ,e.resource_type
-0015f760: 292c 6e3d 2274 6573 7422 3d3d 652e 7265  ),n="test"==e.re
-0015f770: 736f 7572 6365 5f74 7970 6526 2621 652e  source_type&&!e.
-0015f780: 6861 734f 776e 5072 6f70 6572 7479 2822  hasOwnProperty("
-0015f790: 7465 7374 5f6d 6574 6164 6174 6122 293b  test_metadata");
-0015f7a0: 7265 7475 726e 2074 7c7c 6e7d 2929 2c28  return t||n})),(
-0015f7b0: 6675 6e63 7469 6f6e 2865 297b 7661 7220  function(e){var 
-0015f7c0: 743d 7b67 726f 7570 3a22 6e6f 6465 7322  t={group:"nodes"
-0015f7d0: 2c64 6174 613a 722e 6173 7369 676e 2865  ,data:r.assign(e
-0015f7e0: 2c7b 7061 7265 6e74 3a65 2e70 6163 6b61  ,{parent:e.packa
-0015f7f0: 6765 5f6e 616d 652c 6964 3a65 2e75 6e69  ge_name,id:e.uni
-0015f800: 7175 655f 6964 2c69 735f 6772 6f75 703a  que_id,is_group:
-0015f810: 2266 616c 7365 227d 297d 3b70 2e67 7261  "false"})};p.gra
-0015f820: 7068 2e70 7269 7374 696e 652e 6e6f 6465  ph.pristine.node
-0015f830: 735b 652e 756e 6971 7565 5f69 645d 3d74  s[e.unique_id]=t
-0015f840: 7d29 292c 722e 6561 6368 2870 2e6d 616e  })),r.each(p.man
-0015f850: 6966 6573 742e 7061 7265 6e74 5f6d 6170  ifest.parent_map
-0015f860: 2c28 6675 6e63 7469 6f6e 2865 2c74 297b  ,(function(e,t){
-0015f870: 722e 6561 6368 2865 2c28 6675 6e63 7469  r.each(e,(functi
-0015f880: 6f6e 2865 297b 7661 7220 6e3d 702e 6d61  on(e){var n=p.ma
-0015f890: 6e69 6665 7374 2e6e 6f64 6573 5b65 5d2c  nifest.nodes[e],
-0015f8a0: 693d 702e 6d61 6e69 6665 7374 2e6e 6f64  i=p.manifest.nod
-0015f8b0: 6573 5b74 5d3b 6966 2872 2e69 6e63 6c75  es[t];if(r.inclu
-0015f8c0: 6465 7328 5b22 6d6f 6465 6c22 2c22 736f  des(["model","so
-0015f8d0: 7572 6365 222c 2273 6565 6422 2c22 736e  urce","seed","sn
-0015f8e0: 6170 7368 6f74 222c 226d 6574 7269 6322  apshot","metric"
-0015f8f0: 2c22 7365 6d61 6e74 6963 5f6d 6f64 656c  ,"semantic_model
-0015f900: 225d 2c6e 2e72 6573 6f75 7263 655f 7479  "],n.resource_ty
-0015f910: 7065 2926 2628 2274 6573 7422 213d 692e  pe)&&("test"!=i.
-0015f920: 7265 736f 7572 6365 5f74 7970 657c 7c21  resource_type||!
-0015f930: 692e 6861 734f 776e 5072 6f70 6572 7479  i.hasOwnProperty
-0015f940: 2822 7465 7374 5f6d 6574 6164 6174 6122  ("test_metadata"
-0015f950: 2929 297b 7661 7220 6f3d 6e2e 756e 6971  ))){var o=n.uniq
-0015f960: 7565 5f69 642b 227c 222b 692e 756e 6971  ue_id+"|"+i.uniq
-0015f970: 7565 5f69 642c 613d 7b67 726f 7570 3a22  ue_id,a={group:"
-0015f980: 6564 6765 7322 2c64 6174 613a 7b73 6f75  edges",data:{sou
-0015f990: 7263 653a 6e2e 756e 6971 7565 5f69 642c  rce:n.unique_id,
-0015f9a0: 7461 7267 6574 3a69 2e75 6e69 7175 655f  target:i.unique_
-0015f9b0: 6964 2c75 6e69 7175 655f 6964 3a6f 7d7d  id,unique_id:o}}
-0015f9c0: 2c73 3d69 2e75 6e69 7175 655f 6964 3b70  ,s=i.unique_id;p
-0015f9d0: 2e67 7261 7068 2e70 7269 7374 696e 652e  .graph.pristine.
-0015f9e0: 6564 6765 735b 735d 7c7c 2870 2e67 7261  edges[s]||(p.gra
-0015f9f0: 7068 2e70 7269 7374 696e 652e 6564 6765  ph.pristine.edge
-0015fa00: 735b 735d 3d5b 5d29 2c70 2e67 7261 7068  s[s]=[]),p.graph
-0015fa10: 2e70 7269 7374 696e 652e 6564 6765 735b  .pristine.edges[
-0015fa20: 735d 2e70 7573 6828 6129 7d7d 2929 7d29  s].push(a)}}))})
-0015fa30: 293b 7661 7220 743d 6e65 7720 692e 4772  );var t=new i.Gr
-0015fa40: 6170 6828 7b64 6972 6563 7465 643a 2130  aph({directed:!0
-0015fa50: 7d29 3b72 2e65 6163 6828 702e 6772 6170  });r.each(p.grap
-0015fa60: 682e 7072 6973 7469 6e65 2e6e 6f64 6573  h.pristine.nodes
-0015fa70: 2c28 6675 6e63 7469 6f6e 2865 297b 742e  ,(function(e){t.
-0015fa80: 7365 744e 6f64 6528 652e 6461 7461 2e75  setNode(e.data.u
-0015fa90: 6e69 7175 655f 6964 2c65 2e64 6174 612e  nique_id,e.data.
-0015faa0: 6e61 6d65 297d 2929 2c72 2e65 6163 6828  name)})),r.each(
-0015fab0: 702e 6772 6170 682e 7072 6973 7469 6e65  p.graph.pristine
-0015fac0: 2e65 6467 6573 2c28 6675 6e63 7469 6f6e  .edges,(function
-0015fad0: 2865 297b 722e 6561 6368 2865 2c28 6675  (e){r.each(e,(fu
-0015fae0: 6e63 7469 6f6e 2865 297b 742e 7365 7445  nction(e){t.setE
-0015faf0: 6467 6528 652e 6461 7461 2e73 6f75 7263  dge(e.data.sourc
-0015fb00: 652c 652e 6461 7461 2e74 6172 6765 7429  e,e.data.target)
-0015fb10: 7d29 297d 2929 2c70 2e67 7261 7068 2e70  }))})),p.graph.p
-0015fb20: 7269 7374 696e 652e 6461 673d 742c 702e  ristine.dag=t,p.
-0015fb30: 6772 6170 682e 656c 656d 656e 7473 3d72  graph.elements=r
-0015fb40: 2e66 6c61 7474 656e 2872 2e76 616c 7565  .flatten(r.value
-0015fb50: 7328 702e 6772 6170 682e 7072 6973 7469  s(p.graph.pristi
-0015fb60: 6e65 2e6e 6f64 6573 292e 636f 6e63 6174  ne.nodes).concat
-0015fb70: 2872 2e76 616c 7565 7328 702e 6772 6170  (r.values(p.grap
-0015fb80: 682e 7072 6973 7469 6e65 2e65 6467 6573  h.pristine.edges
-0015fb90: 2929 292c 6628 742e 6e6f 6465 7328 2929  ))),f(t.nodes())
-0015fba0: 7d29 292c 702e 6869 6465 4772 6170 683d  })),p.hideGraph=
-0015fbb0: 6675 6e63 7469 6f6e 2829 7b70 2e6f 7269  function(){p.ori
-0015fbc0: 656e 7461 7469 6f6e 3d22 7369 6465 6261  entation="sideba
-0015fbd0: 7222 2c70 2e65 7870 616e 6465 643d 2131  r",p.expanded=!1
-0015fbe0: 7d2c 702e 7368 6f77 5665 7274 6963 616c  },p.showVertical
-0015fbf0: 4772 6170 683d 6675 6e63 7469 6f6e 2865  Graph=function(e
-0015fc00: 2c74 297b 702e 6f72 6965 6e74 6174 696f  ,t){p.orientatio
-0015fc10: 6e3d 2273 6964 6562 6172 222c 7426 2628  n="sidebar",t&&(
-0015fc20: 702e 6578 7061 6e64 6564 3d21 3029 3b76  p.expanded=!0);v
-0015fc30: 6172 206e 3d68 2872 2e61 7373 6967 6e28  ar n=h(r.assign(
-0015fc40: 7b7d 2c73 2e6f 7074 696f 6e73 2c7b 696e  {},s.options,{in
-0015fc50: 636c 7564 653a 222b 222b 652b 222b 222c  clude:"+"+e+"+",
-0015fc60: 6578 636c 7564 653a 2222 2c68 6f70 733a  exclude:"",hops:
-0015fc70: 317d 292c 2276 6572 7469 6361 6c22 2c21  1}),"vertical",!
-0015fc80: 3029 3b72 6574 7572 6e20 702e 6772 6170  0);return p.grap
-0015fc90: 682e 6c61 796f 7574 3d64 2e74 6f70 5f64  h.layout=d.top_d
-0015fca0: 6f77 6e2c 702e 6772 6170 682e 6f70 7469  own,p.graph.opti
-0015fcb0: 6f6e 733d 752e 7665 7274 6963 616c 2c6e  ons=u.vertical,n
-0015fcc0: 7d2c 702e 7368 6f77 4675 6c6c 4772 6170  },p.showFullGrap
-0015fcd0: 683d 6675 6e63 7469 6f6e 2865 297b 702e  h=function(e){p.
-0015fce0: 6f72 6965 6e74 6174 696f 6e3d 2266 756c  orientation="ful
-0015fcf0: 6c73 6372 6565 6e22 2c70 2e65 7870 616e  lscreen",p.expan
-0015fd00: 6465 643d 2130 3b76 6172 2074 3d72 2e61  ded=!0;var t=r.a
-0015fd10: 7373 6967 6e28 7b7d 2c73 2e6f 7074 696f  ssign({},s.optio
-0015fd20: 6e73 293b 653f 2874 2e69 6e63 6c75 6465  ns);e?(t.include
-0015fd30: 3d22 2b22 2b65 2b22 2b22 2c74 2e65 7863  ="+"+e+"+",t.exc
-0015fd40: 6c75 6465 3d22 2229 3a28 742e 696e 636c  lude=""):(t.incl
-0015fd50: 7564 653d 2222 2c74 2e65 7863 6c75 6465  ude="",t.exclude
-0015fd60: 3d22 2229 3b76 6172 206e 3d68 2874 2c22  ="");var n=h(t,"
-0015fd70: 686f 7269 7a6f 6e74 616c 222c 2130 293b  horizontal",!0);
-0015fd80: 7265 7475 726e 2070 2e67 7261 7068 2e6c  return p.graph.l
-0015fd90: 6179 6f75 743d 642e 6c65 6674 5f72 6967  ayout=d.left_rig
-0015fda0: 6874 2c70 2e67 7261 7068 2e6f 7074 696f  ht,p.graph.optio
-0015fdb0: 6e73 3d75 2e68 6f72 697a 6f6e 7461 6c2c  ns=u.horizontal,
-0015fdc0: 632e 7365 7453 7461 7465 2874 292c 6e7d  c.setState(t),n}
-0015fdd0: 2c70 2e75 7064 6174 6547 7261 7068 3d66  ,p.updateGraph=f
-0015fde0: 756e 6374 696f 6e28 6529 7b70 2e6f 7269  unction(e){p.ori
-0015fdf0: 656e 7461 7469 6f6e 3d22 6675 6c6c 7363  entation="fullsc
-0015fe00: 7265 656e 222c 702e 6578 7061 6e64 6564  reen",p.expanded
-0015fe10: 3d21 303b 7661 7220 743d 6828 652c 2268  =!0;var t=h(e,"h
-0015fe20: 6f72 697a 6f6e 7461 6c22 2c21 3129 3b72  orizontal",!1);r
-0015fe30: 6574 7572 6e20 702e 6772 6170 682e 6c61  eturn p.graph.la
-0015fe40: 796f 7574 3d64 2e6c 6566 745f 7269 6768  yout=d.left_righ
-0015fe50: 742c 702e 6772 6170 682e 6f70 7469 6f6e  t,p.graph.option
-0015fe60: 733d 752e 686f 7269 7a6f 6e74 616c 2c63  s=u.horizontal,c
-0015fe70: 2e73 6574 5374 6174 6528 6529 2c74 7d2c  .setState(e),t},
-0015fe80: 702e 6465 7365 6c65 6374 4e6f 6465 733d  p.deselectNodes=
-0015fe90: 6675 6e63 7469 6f6e 2829 7b22 6675 6c6c  function(){"full
-0015fea0: 7363 7265 656e 223d 3d70 2e6f 7269 656e  screen"==p.orien
-0015feb0: 7461 7469 6f6e 2626 702e 6772 6170 685f  tation&&p.graph_
-0015fec0: 656c 656d 656e 742e 656c 656d 656e 7473  element.elements
-0015fed0: 2829 2e64 6174 6128 2273 656c 6563 7465  ().data("selecte
-0015fee0: 6422 2c30 297d 2c70 2e73 656c 6563 744e  d",0)},p.selectN
-0015fef0: 6f64 653d 6675 6e63 7469 6f6e 2865 297b  ode=function(e){
-0015ff00: 6966 2822 6675 6c6c 7363 7265 656e 223d  if("fullscreen"=
-0015ff10: 3d70 2e6f 7269 656e 7461 7469 6f6e 297b  =p.orientation){
-0015ff20: 702e 6772 6170 682e 7072 6973 7469 6e65  p.graph.pristine
-0015ff30: 2e6e 6f64 6573 5b65 5d3b 7661 7220 743d  .nodes[e];var t=
-0015ff40: 702e 6772 6170 682e 7072 6973 7469 6e65  p.graph.pristine
-0015ff50: 2e64 6167 2c6e 3d72 2e69 6e64 6578 4279  .dag,n=r.indexBy
-0015ff60: 286f 2e61 6e63 6573 746f 724e 6f64 6573  (o.ancestorNodes
-0015ff70: 2874 2c65 2929 2c69 3d72 2e69 6e64 6578  (t,e)),i=r.index
-0015ff80: 4279 286f 2e64 6573 6365 6e64 656e 744e  By(o.descendentN
-0015ff90: 6f64 6573 2874 2c65 2929 3b6e 5b65 5d3d  odes(t,e));n[e]=
-0015ffa0: 652c 695b 655d 3d65 3b76 6172 2061 3d70  e,i[e]=e;var a=p
-0015ffb0: 2e67 7261 7068 5f65 6c65 6d65 6e74 3b72  .graph_element;r
-0015ffc0: 2e65 6163 6828 702e 6772 6170 682e 656c  .each(p.graph.el
-0015ffd0: 656d 656e 7473 2c28 6675 6e63 7469 6f6e  ements,(function
-0015ffe0: 2874 297b 7661 7220 723d 612e 2469 6428  (t){var r=a.$id(
-0015fff0: 742e 6461 7461 2e69 6429 3b6e 5b74 2e64  t.data.id);n[t.d
-00160000: 6174 612e 736f 7572 6365 5d26 266e 5b74  ata.source]&&n[t
-00160010: 2e64 6174 612e 7461 7267 6574 5d7c 7c69  .data.target]||i
+0015f760: 292c 6e3d 2274 6573 7422 3d3d 3d65 2e72  ),n="test"===e.r
+0015f770: 6573 6f75 7263 655f 7479 7065 2626 2165  esource_type&&!e
+0015f780: 2e68 6173 4f77 6e50 726f 7065 7274 7928  .hasOwnProperty(
+0015f790: 2274 6573 745f 6d65 7461 6461 7461 2229  "test_metadata")
+0015f7a0: 2c69 3d22 756e 6974 5f74 6573 7422 3d3d  ,i="unit_test"==
+0015f7b0: 3d65 2e72 6573 6f75 7263 655f 7479 7065  =e.resource_type
+0015f7c0: 3b72 6574 7572 6e20 747c 7c6e 7c7c 697d  ;return t||n||i}
+0015f7d0: 2929 2c28 6675 6e63 7469 6f6e 2865 297b  )),(function(e){
+0015f7e0: 7661 7220 743d 7b67 726f 7570 3a22 6e6f  var t={group:"no
+0015f7f0: 6465 7322 2c64 6174 613a 722e 6173 7369  des",data:r.assi
+0015f800: 676e 2865 2c7b 7061 7265 6e74 3a65 2e70  gn(e,{parent:e.p
+0015f810: 6163 6b61 6765 5f6e 616d 652c 6964 3a65  ackage_name,id:e
+0015f820: 2e75 6e69 7175 655f 6964 2c69 735f 6772  .unique_id,is_gr
+0015f830: 6f75 703a 2266 616c 7365 227d 297d 3b70  oup:"false"})};p
+0015f840: 2e67 7261 7068 2e70 7269 7374 696e 652e  .graph.pristine.
+0015f850: 6e6f 6465 735b 652e 756e 6971 7565 5f69  nodes[e.unique_i
+0015f860: 645d 3d74 7d29 292c 722e 6561 6368 2870  d]=t})),r.each(p
+0015f870: 2e6d 616e 6966 6573 742e 7061 7265 6e74  .manifest.parent
+0015f880: 5f6d 6170 2c28 6675 6e63 7469 6f6e 2865  _map,(function(e
+0015f890: 2c74 297b 722e 6561 6368 2865 2c28 6675  ,t){r.each(e,(fu
+0015f8a0: 6e63 7469 6f6e 2865 297b 7661 7220 6e3d  nction(e){var n=
+0015f8b0: 702e 6d61 6e69 6665 7374 2e6e 6f64 6573  p.manifest.nodes
+0015f8c0: 5b65 5d2c 693d 702e 6d61 6e69 6665 7374  [e],i=p.manifest
+0015f8d0: 2e6e 6f64 6573 5b74 5d3b 6966 2872 2e69  .nodes[t];if(r.i
+0015f8e0: 6e63 6c75 6465 7328 5b22 6d6f 6465 6c22  ncludes(["model"
+0015f8f0: 2c22 736f 7572 6365 222c 2273 6565 6422  ,"source","seed"
+0015f900: 2c22 736e 6170 7368 6f74 222c 226d 6574  ,"snapshot","met
+0015f910: 7269 6322 2c22 7365 6d61 6e74 6963 5f6d  ric","semantic_m
+0015f920: 6f64 656c 225d 2c6e 2e72 6573 6f75 7263  odel"],n.resourc
+0015f930: 655f 7479 7065 2926 2628 2274 6573 7422  e_type)&&("test"
+0015f940: 213d 692e 7265 736f 7572 6365 5f74 7970  !=i.resource_typ
+0015f950: 657c 7c21 692e 6861 734f 776e 5072 6f70  e||!i.hasOwnProp
+0015f960: 6572 7479 2822 7465 7374 5f6d 6574 6164  erty("test_metad
+0015f970: 6174 6122 2929 297b 7661 7220 6f3d 6e2e  ata"))){var o=n.
+0015f980: 756e 6971 7565 5f69 642b 227c 222b 692e  unique_id+"|"+i.
+0015f990: 756e 6971 7565 5f69 642c 613d 7b67 726f  unique_id,a={gro
+0015f9a0: 7570 3a22 6564 6765 7322 2c64 6174 613a  up:"edges",data:
+0015f9b0: 7b73 6f75 7263 653a 6e2e 756e 6971 7565  {source:n.unique
+0015f9c0: 5f69 642c 7461 7267 6574 3a69 2e75 6e69  _id,target:i.uni
+0015f9d0: 7175 655f 6964 2c75 6e69 7175 655f 6964  que_id,unique_id
+0015f9e0: 3a6f 7d7d 2c73 3d69 2e75 6e69 7175 655f  :o}},s=i.unique_
+0015f9f0: 6964 3b70 2e67 7261 7068 2e70 7269 7374  id;p.graph.prist
+0015fa00: 696e 652e 6564 6765 735b 735d 7c7c 2870  ine.edges[s]||(p
+0015fa10: 2e67 7261 7068 2e70 7269 7374 696e 652e  .graph.pristine.
+0015fa20: 6564 6765 735b 735d 3d5b 5d29 2c70 2e67  edges[s]=[]),p.g
+0015fa30: 7261 7068 2e70 7269 7374 696e 652e 6564  raph.pristine.ed
+0015fa40: 6765 735b 735d 2e70 7573 6828 6129 7d7d  ges[s].push(a)}}
+0015fa50: 2929 7d29 293b 7661 7220 743d 6e65 7720  ))}));var t=new 
+0015fa60: 692e 4772 6170 6828 7b64 6972 6563 7465  i.Graph({directe
+0015fa70: 643a 2130 7d29 3b72 2e65 6163 6828 702e  d:!0});r.each(p.
+0015fa80: 6772 6170 682e 7072 6973 7469 6e65 2e6e  graph.pristine.n
+0015fa90: 6f64 6573 2c28 6675 6e63 7469 6f6e 2865  odes,(function(e
+0015faa0: 297b 742e 7365 744e 6f64 6528 652e 6461  ){t.setNode(e.da
+0015fab0: 7461 2e75 6e69 7175 655f 6964 2c65 2e64  ta.unique_id,e.d
+0015fac0: 6174 612e 6e61 6d65 297d 2929 2c72 2e65  ata.name)})),r.e
+0015fad0: 6163 6828 702e 6772 6170 682e 7072 6973  ach(p.graph.pris
+0015fae0: 7469 6e65 2e65 6467 6573 2c28 6675 6e63  tine.edges,(func
+0015faf0: 7469 6f6e 2865 297b 722e 6561 6368 2865  tion(e){r.each(e
+0015fb00: 2c28 6675 6e63 7469 6f6e 2865 297b 742e  ,(function(e){t.
+0015fb10: 7365 7445 6467 6528 652e 6461 7461 2e73  setEdge(e.data.s
+0015fb20: 6f75 7263 652c 652e 6461 7461 2e74 6172  ource,e.data.tar
+0015fb30: 6765 7429 7d29 297d 2929 2c70 2e67 7261  get)}))})),p.gra
+0015fb40: 7068 2e70 7269 7374 696e 652e 6461 673d  ph.pristine.dag=
+0015fb50: 742c 702e 6772 6170 682e 656c 656d 656e  t,p.graph.elemen
+0015fb60: 7473 3d72 2e66 6c61 7474 656e 2872 2e76  ts=r.flatten(r.v
+0015fb70: 616c 7565 7328 702e 6772 6170 682e 7072  alues(p.graph.pr
+0015fb80: 6973 7469 6e65 2e6e 6f64 6573 292e 636f  istine.nodes).co
+0015fb90: 6e63 6174 2872 2e76 616c 7565 7328 702e  ncat(r.values(p.
+0015fba0: 6772 6170 682e 7072 6973 7469 6e65 2e65  graph.pristine.e
+0015fbb0: 6467 6573 2929 292c 6628 742e 6e6f 6465  dges))),f(t.node
+0015fbc0: 7328 2929 7d29 292c 702e 6869 6465 4772  s())})),p.hideGr
+0015fbd0: 6170 683d 6675 6e63 7469 6f6e 2829 7b70  aph=function(){p
+0015fbe0: 2e6f 7269 656e 7461 7469 6f6e 3d22 7369  .orientation="si
+0015fbf0: 6465 6261 7222 2c70 2e65 7870 616e 6465  debar",p.expande
+0015fc00: 643d 2131 7d2c 702e 7368 6f77 5665 7274  d=!1},p.showVert
+0015fc10: 6963 616c 4772 6170 683d 6675 6e63 7469  icalGraph=functi
+0015fc20: 6f6e 2865 2c74 297b 702e 6f72 6965 6e74  on(e,t){p.orient
+0015fc30: 6174 696f 6e3d 2273 6964 6562 6172 222c  ation="sidebar",
+0015fc40: 7426 2628 702e 6578 7061 6e64 6564 3d21  t&&(p.expanded=!
+0015fc50: 3029 3b76 6172 206e 3d68 2872 2e61 7373  0);var n=h(r.ass
+0015fc60: 6967 6e28 7b7d 2c73 2e6f 7074 696f 6e73  ign({},s.options
+0015fc70: 2c7b 696e 636c 7564 653a 222b 222b 652b  ,{include:"+"+e+
+0015fc80: 222b 222c 6578 636c 7564 653a 2222 2c68  "+",exclude:"",h
+0015fc90: 6f70 733a 317d 292c 2276 6572 7469 6361  ops:1}),"vertica
+0015fca0: 6c22 2c21 3029 3b72 6574 7572 6e20 702e  l",!0);return p.
+0015fcb0: 6772 6170 682e 6c61 796f 7574 3d64 2e74  graph.layout=d.t
+0015fcc0: 6f70 5f64 6f77 6e2c 702e 6772 6170 682e  op_down,p.graph.
+0015fcd0: 6f70 7469 6f6e 733d 752e 7665 7274 6963  options=u.vertic
+0015fce0: 616c 2c6e 7d2c 702e 7368 6f77 4675 6c6c  al,n},p.showFull
+0015fcf0: 4772 6170 683d 6675 6e63 7469 6f6e 2865  Graph=function(e
+0015fd00: 297b 702e 6f72 6965 6e74 6174 696f 6e3d  ){p.orientation=
+0015fd10: 2266 756c 6c73 6372 6565 6e22 2c70 2e65  "fullscreen",p.e
+0015fd20: 7870 616e 6465 643d 2130 3b76 6172 2074  xpanded=!0;var t
+0015fd30: 3d72 2e61 7373 6967 6e28 7b7d 2c73 2e6f  =r.assign({},s.o
+0015fd40: 7074 696f 6e73 293b 653f 2874 2e69 6e63  ptions);e?(t.inc
+0015fd50: 6c75 6465 3d22 2b22 2b65 2b22 2b22 2c74  lude="+"+e+"+",t
+0015fd60: 2e65 7863 6c75 6465 3d22 2229 3a28 742e  .exclude=""):(t.
+0015fd70: 696e 636c 7564 653d 2222 2c74 2e65 7863  include="",t.exc
+0015fd80: 6c75 6465 3d22 2229 3b76 6172 206e 3d68  lude="");var n=h
+0015fd90: 2874 2c22 686f 7269 7a6f 6e74 616c 222c  (t,"horizontal",
+0015fda0: 2130 293b 7265 7475 726e 2070 2e67 7261  !0);return p.gra
+0015fdb0: 7068 2e6c 6179 6f75 743d 642e 6c65 6674  ph.layout=d.left
+0015fdc0: 5f72 6967 6874 2c70 2e67 7261 7068 2e6f  _right,p.graph.o
+0015fdd0: 7074 696f 6e73 3d75 2e68 6f72 697a 6f6e  ptions=u.horizon
+0015fde0: 7461 6c2c 632e 7365 7453 7461 7465 2874  tal,c.setState(t
+0015fdf0: 292c 6e7d 2c70 2e75 7064 6174 6547 7261  ),n},p.updateGra
+0015fe00: 7068 3d66 756e 6374 696f 6e28 6529 7b70  ph=function(e){p
+0015fe10: 2e6f 7269 656e 7461 7469 6f6e 3d22 6675  .orientation="fu
+0015fe20: 6c6c 7363 7265 656e 222c 702e 6578 7061  llscreen",p.expa
+0015fe30: 6e64 6564 3d21 303b 7661 7220 743d 6828  nded=!0;var t=h(
+0015fe40: 652c 2268 6f72 697a 6f6e 7461 6c22 2c21  e,"horizontal",!
+0015fe50: 3129 3b72 6574 7572 6e20 702e 6772 6170  1);return p.grap
+0015fe60: 682e 6c61 796f 7574 3d64 2e6c 6566 745f  h.layout=d.left_
+0015fe70: 7269 6768 742c 702e 6772 6170 682e 6f70  right,p.graph.op
+0015fe80: 7469 6f6e 733d 752e 686f 7269 7a6f 6e74  tions=u.horizont
+0015fe90: 616c 2c63 2e73 6574 5374 6174 6528 6529  al,c.setState(e)
+0015fea0: 2c74 7d2c 702e 6465 7365 6c65 6374 4e6f  ,t},p.deselectNo
+0015feb0: 6465 733d 6675 6e63 7469 6f6e 2829 7b22  des=function(){"
+0015fec0: 6675 6c6c 7363 7265 656e 223d 3d70 2e6f  fullscreen"==p.o
+0015fed0: 7269 656e 7461 7469 6f6e 2626 702e 6772  rientation&&p.gr
+0015fee0: 6170 685f 656c 656d 656e 742e 656c 656d  aph_element.elem
+0015fef0: 656e 7473 2829 2e64 6174 6128 2273 656c  ents().data("sel
+0015ff00: 6563 7465 6422 2c30 297d 2c70 2e73 656c  ected",0)},p.sel
+0015ff10: 6563 744e 6f64 653d 6675 6e63 7469 6f6e  ectNode=function
+0015ff20: 2865 297b 6966 2822 6675 6c6c 7363 7265  (e){if("fullscre
+0015ff30: 656e 223d 3d70 2e6f 7269 656e 7461 7469  en"==p.orientati
+0015ff40: 6f6e 297b 702e 6772 6170 682e 7072 6973  on){p.graph.pris
+0015ff50: 7469 6e65 2e6e 6f64 6573 5b65 5d3b 7661  tine.nodes[e];va
+0015ff60: 7220 743d 702e 6772 6170 682e 7072 6973  r t=p.graph.pris
+0015ff70: 7469 6e65 2e64 6167 2c6e 3d72 2e69 6e64  tine.dag,n=r.ind
+0015ff80: 6578 4279 286f 2e61 6e63 6573 746f 724e  exBy(o.ancestorN
+0015ff90: 6f64 6573 2874 2c65 2929 2c69 3d72 2e69  odes(t,e)),i=r.i
+0015ffa0: 6e64 6578 4279 286f 2e64 6573 6365 6e64  ndexBy(o.descend
+0015ffb0: 656e 744e 6f64 6573 2874 2c65 2929 3b6e  entNodes(t,e));n
+0015ffc0: 5b65 5d3d 652c 695b 655d 3d65 3b76 6172  [e]=e,i[e]=e;var
+0015ffd0: 2061 3d70 2e67 7261 7068 5f65 6c65 6d65   a=p.graph_eleme
+0015ffe0: 6e74 3b72 2e65 6163 6828 702e 6772 6170  nt;r.each(p.grap
+0015fff0: 682e 656c 656d 656e 7473 2c28 6675 6e63  h.elements,(func
+00160000: 7469 6f6e 2874 297b 7661 7220 723d 612e  tion(t){var r=a.
+00160010: 2469 6428 742e 6461 7461 2e69 6429 3b6e  $id(t.data.id);n
 00160020: 5b74 2e64 6174 612e 736f 7572 6365 5d26  [t.data.source]&
-00160030: 2669 5b74 2e64 6174 612e 7461 7267 6574  &i[t.data.target
-00160040: 5d7c 7c74 2e64 6174 612e 756e 6971 7565  ]||t.data.unique
-00160050: 5f69 643d 3d65 3f72 2e64 6174 6128 2273  _id==e?r.data("s
-00160060: 656c 6563 7465 6422 2c31 293a 722e 6461  elected",1):r.da
-00160070: 7461 2822 7365 6c65 6374 6564 222c 3029  ta("selected",0)
-00160080: 7d29 297d 7d2c 702e 6d61 726b 4469 7274  }))}},p.markDirt
-00160090: 793d 6675 6e63 7469 6f6e 2865 297b 702e  y=function(e){p.
-001600a0: 6d61 726b 416c 6c43 6c65 616e 2829 2c72  markAllClean(),r
-001600b0: 2e65 6163 6828 652c 2866 756e 6374 696f  .each(e,(functio
-001600c0: 6e28 6529 7b70 2e67 7261 7068 5f65 6c65  n(e){p.graph_ele
-001600d0: 6d65 6e74 2e24 6964 2865 292e 6164 6443  ment.$id(e).addC
-001600e0: 6c61 7373 2822 6469 7274 7922 297d 2929  lass("dirty")}))
-001600f0: 7d2c 702e 6d61 726b 416c 6c43 6c65 616e  },p.markAllClean
-00160100: 3d66 756e 6374 696f 6e28 297b 702e 6772  =function(){p.gr
-00160110: 6170 685f 656c 656d 656e 7426 2670 2e67  aph_element&&p.g
-00160120: 7261 7068 5f65 6c65 6d65 6e74 2e65 6c65  raph_element.ele
-00160130: 6d65 6e74 7328 292e 7265 6d6f 7665 436c  ments().removeCl
-00160140: 6173 7328 2264 6972 7479 2229 7d2c 707d  ass("dirty")},p}
-00160150: 5d29 7d2c 6675 6e63 7469 6f6e 2865 2c74  ])},function(e,t
-00160160: 2c6e 297b 2275 7365 2073 7472 6963 7422  ,n){"use strict"
-00160170: 3b6e 2e72 2874 292c 6e2e 6428 742c 2269  ;n.r(t),n.d(t,"i
-00160180: 7356 616c 6964 436f 6c6f 7222 2c28 6675  sValidColor",(fu
-00160190: 6e63 7469 6f6e 2829 7b72 6574 7572 6e20  nction(){return 
-001601a0: 697d 2929 3b63 6f6e 7374 2072 3d6e 6577  i}));const r=new
-001601b0: 2053 6574 285b 2261 6c69 6365 626c 7565   Set(["aliceblue
-001601c0: 222c 2261 6e74 6971 7565 7768 6974 6522  ","antiquewhite"
-001601d0: 2c22 6171 7561 222c 2261 7175 616d 6172  ,"aqua","aquamar
-001601e0: 696e 6522 2c22 617a 7572 6522 2c22 6265  ine","azure","be
-001601f0: 6967 6522 2c22 6269 7371 7565 222c 2262  ige","bisque","b
-00160200: 6c61 636b 222c 2262 6c61 6e63 6865 6461  lack","blancheda
-00160210: 6c6d 6f6e 6422 2c22 626c 7565 222c 2262  lmond","blue","b
-00160220: 6c75 6576 696f 6c65 7422 2c22 6272 6f77  lueviolet","brow
-00160230: 6e22 2c22 6275 726c 7977 6f6f 6422 2c22  n","burlywood","
-00160240: 6361 6465 7462 6c75 6522 2c22 6368 6172  cadetblue","char
-00160250: 7472 6575 7365 222c 2263 686f 636f 6c61  treuse","chocola
-00160260: 7465 222c 2263 6f72 616c 222c 2263 6f72  te","coral","cor
-00160270: 6e66 6c6f 7765 7262 6c75 6522 2c22 636f  nflowerblue","co
-00160280: 726e 7369 6c6b 222c 2263 7269 6d73 6f6e  rnsilk","crimson
-00160290: 222c 2263 7961 6e22 2c22 6461 726b 626c  ","cyan","darkbl
-001602a0: 7565 222c 2264 6172 6b63 7961 6e22 2c22  ue","darkcyan","
-001602b0: 6461 726b 676f 6c64 656e 726f 6422 2c22  darkgoldenrod","
-001602c0: 6461 726b 6772 6179 222c 2264 6172 6b67  darkgray","darkg
-001602d0: 7265 656e 222c 2264 6172 6b6b 6861 6b69  reen","darkkhaki
-001602e0: 222c 2264 6172 6b6d 6167 656e 7461 222c  ","darkmagenta",
-001602f0: 2264 6172 6b6f 6c69 7665 6772 6565 6e22  "darkolivegreen"
-00160300: 2c22 6461 726b 6f72 616e 6765 222c 2264  ,"darkorange","d
-00160310: 6172 6b6f 7263 6869 6422 2c22 6461 726b  arkorchid","dark
-00160320: 7265 6422 2c22 6461 726b 7361 6c6d 6f6e  red","darksalmon
-00160330: 222c 2264 6172 6b73 6561 6772 6565 6e22  ","darkseagreen"
-00160340: 2c22 6461 726b 736c 6174 6562 6c75 6522  ,"darkslateblue"
-00160350: 2c22 6461 726b 736c 6174 6567 7261 7922  ,"darkslategray"
-00160360: 2c22 6461 726b 7475 7271 756f 6973 6522  ,"darkturquoise"
-00160370: 2c22 6461 726b 7669 6f6c 6574 222c 2264  ,"darkviolet","d
-00160380: 6565 7070 696e 6b22 2c22 6465 6570 736b  eeppink","deepsk
-00160390: 7962 6c75 6522 2c22 6469 6d67 7261 7922  yblue","dimgray"
-001603a0: 2c22 646f 6467 6572 626c 7565 222c 2266  ,"dodgerblue","f
-001603b0: 6972 6562 7269 636b 222c 2266 6c6f 7261  irebrick","flora
-001603c0: 6c77 6869 7465 222c 2266 6f72 6573 7467  lwhite","forestg
-001603d0: 7265 656e 222c 2266 7563 6873 6961 222c  reen","fuchsia",
-001603e0: 2267 686f 7374 7768 6974 6522 2c22 676f  "ghostwhite","go
-001603f0: 6c64 222c 2267 6f6c 6465 6e72 6f64 222c  ld","goldenrod",
-00160400: 2267 7261 7922 2c22 6772 6565 6e22 2c22  "gray","green","
-00160410: 6772 6565 6e79 656c 6c6f 7722 2c22 686f  greenyellow","ho
-00160420: 6e65 7964 6577 222c 2268 6f74 7069 6e6b  neydew","hotpink
-00160430: 222c 2269 6e64 6961 6e72 6564 222c 2269  ","indianred","i
-00160440: 6e64 6967 6f22 2c22 6976 6f72 7922 2c22  ndigo","ivory","
-00160450: 6b68 616b 6922 2c22 6c61 7665 6e64 6572  khaki","lavender
-00160460: 222c 226c 6176 656e 6465 7262 6c75 7368  ","lavenderblush
-00160470: 222c 226c 6177 6e67 7265 656e 222c 226c  ","lawngreen","l
-00160480: 656d 6f6e 6368 6966 666f 6e22 2c22 6c69  emonchiffon","li
-00160490: 6768 7462 6c75 6522 2c22 6c69 6768 7463  ghtblue","lightc
-001604a0: 6f72 616c 222c 226c 6967 6874 6379 616e  oral","lightcyan
-001604b0: 222c 226c 6967 6874 676f 6c64 656e 726f  ","lightgoldenro
-001604c0: 6479 656c 6c6f 7722 2c22 6c69 6768 7467  dyellow","lightg
-001604d0: 7261 7922 2c22 6c69 6768 7467 7265 656e  ray","lightgreen
-001604e0: 222c 226c 6967 6874 7069 6e6b 222c 226c  ","lightpink","l
-001604f0: 6967 6874 7361 6c6d 6f6e 222c 226c 6967  ightsalmon","lig
-00160500: 6874 7361 6c6d 6f6e 222c 226c 6967 6874  htsalmon","light
-00160510: 7365 6167 7265 656e 222c 226c 6967 6874  seagreen","light
-00160520: 736b 7962 6c75 6522 2c22 6c69 6768 7473  skyblue","lights
-00160530: 6c61 7465 6772 6179 222c 226c 6967 6874  lategray","light
-00160540: 7374 6565 6c62 6c75 6522 2c22 6c69 6768  steelblue","ligh
-00160550: 7479 656c 6c6f 7722 2c22 6c69 6d65 222c  tyellow","lime",
-00160560: 226c 696d 6567 7265 656e 222c 226c 696e  "limegreen","lin
-00160570: 656e 222c 226d 6167 656e 7461 222c 226d  en","magenta","m
-00160580: 6172 6f6f 6e22 2c22 6d65 6469 756d 6171  aroon","mediumaq
-00160590: 7561 6d61 7269 6e65 222c 226d 6564 6975  uamarine","mediu
-001605a0: 6d62 6c75 6522 2c22 6d65 6469 756d 6f72  mblue","mediumor
-001605b0: 6368 6964 222c 226d 6564 6975 6d70 7572  chid","mediumpur
-001605c0: 706c 6522 2c22 6d65 6469 756d 7365 6167  ple","mediumseag
-001605d0: 7265 656e 222c 226d 6564 6975 6d73 6c61  reen","mediumsla
-001605e0: 7465 626c 7565 222c 226d 6564 6975 6d73  teblue","mediums
-001605f0: 6c61 7465 626c 7565 222c 226d 6564 6975  lateblue","mediu
-00160600: 6d73 7072 696e 6767 7265 656e 222c 226d  mspringgreen","m
-00160610: 6564 6975 6d74 7572 7175 6f69 7365 222c  ediumturquoise",
-00160620: 226d 6564 6975 6d76 696f 6c65 7472 6564  "mediumvioletred
-00160630: 222c 226d 6964 6e69 6768 7462 6c75 6522  ","midnightblue"
-00160640: 2c22 6d69 6e74 6372 6561 6d22 2c22 6d69  ,"mintcream","mi
-00160650: 7374 7972 6f73 6522 2c22 6d6f 6363 6173  styrose","moccas
-00160660: 696e 222c 226e 6176 616a 6f77 6869 7465  in","navajowhite
-00160670: 222c 226e 6176 7922 2c22 6f6c 646c 6163  ","navy","oldlac
-00160680: 6522 2c22 6f6c 6976 6522 2c22 6f6c 6976  e","olive","oliv
-00160690: 6564 7261 6222 2c22 6f72 616e 6765 222c  edrab","orange",
-001606a0: 226f 7261 6e67 6572 6564 222c 226f 7263  "orangered","orc
-001606b0: 6869 6422 2c22 7061 6c65 676f 6c64 656e  hid","palegolden
-001606c0: 726f 6422 2c22 7061 6c65 6772 6565 6e22  rod","palegreen"
-001606d0: 2c22 7061 6c65 7475 7271 756f 6973 6522  ,"paleturquoise"
-001606e0: 2c22 7061 6c65 7669 6f6c 6574 7265 6422  ,"palevioletred"
-001606f0: 2c22 7061 7061 7961 7768 6970 222c 2270  ,"papayawhip","p
-00160700: 6561 6368 7075 6666 222c 2270 6572 7522  eachpuff","peru"
-00160710: 2c22 7069 6e6b 222c 2270 6c75 6d22 2c22  ,"pink","plum","
-00160720: 706f 7764 6572 626c 7565 222c 2270 7572  powderblue","pur
-00160730: 706c 6522 2c22 7265 6265 6363 6170 7572  ple","rebeccapur
-00160740: 706c 6522 2c22 7265 6422 2c22 726f 7379  ple","red","rosy
-00160750: 6272 6f77 6e22 2c22 726f 7961 6c62 6c75  brown","royalblu
-00160760: 6522 2c22 7361 6464 6c65 6272 6f77 6e22  e","saddlebrown"
-00160770: 2c22 7361 6c6d 6f6e 222c 2273 616e 6479  ,"salmon","sandy
-00160780: 6272 6f77 6e22 2c22 7365 6167 7265 656e  brown","seagreen
-00160790: 222c 2273 6561 7368 656c 6c22 2c22 7369  ","seashell","si
-001607a0: 656e 6e61 222c 2273 696c 7665 7222 2c22  enna","silver","
-001607b0: 736b 7962 6c75 6522 2c22 736c 6174 6562  skyblue","slateb
-001607c0: 6c75 6522 2c22 736c 6174 6567 7261 7922  lue","slategray"
-001607d0: 2c22 736e 6f77 222c 2273 7072 696e 6767  ,"snow","springg
-001607e0: 7265 656e 222c 2273 7465 656c 626c 7565  reen","steelblue
-001607f0: 222c 2274 616e 222c 2274 6561 6c22 2c22  ","tan","teal","
-00160800: 7468 6973 746c 6522 2c22 746f 6d61 746f  thistle","tomato
-00160810: 222c 2274 7572 7175 6f69 7365 222c 2276  ","turquoise","v
-00160820: 696f 6c65 7422 2c22 7768 6561 7422 2c22  iolet","wheat","
-00160830: 7768 6974 6522 2c22 7768 6974 6573 6d6f  white","whitesmo
-00160840: 6b65 222c 2279 656c 6c6f 7722 2c22 7965  ke","yellow","ye
-00160850: 6c6c 6f77 6772 6565 6e22 5d29 3b66 756e  llowgreen"]);fun
-00160860: 6374 696f 6e20 6928 6529 7b69 6628 2165  ction i(e){if(!e
-00160870: 2972 6574 7572 6e21 313b 636f 6e73 7420  )return!1;const 
-00160880: 743d 652e 7472 696d 2829 2e74 6f4c 6f77  t=e.trim().toLow
-00160890: 6572 4361 7365 2829 3b69 6628 2222 3d3d  erCase();if(""==
-001608a0: 3d74 2972 6574 7572 6e21 313b 636f 6e73  =t)return!1;cons
-001608b0: 7420 6e3d 742e 6d61 7463 6828 2f5e 2328  t n=t.match(/^#(
-001608c0: 5b41 2d46 612d 6630 2d39 5d7b 337d 297b  [A-Fa-f0-9]{3}){
-001608d0: 312c 327d 242f 292c 693d 722e 6861 7328  1,2}$/),i=r.has(
-001608e0: 7429 3b72 6574 7572 6e20 426f 6f6c 6561  t);return Boolea
-001608f0: 6e28 6e29 7c7c 697d 7d2c 6675 6e63 7469  n(n)||i}},functi
-00160900: 6f6e 2865 2c74 2c6e 297b 6e28 3333 293b  on(e,t,n){n(33);
-00160910: 636f 6e73 7420 723d 6e28 3231 292c 693d  const r=n(21),i=
-00160920: 6e28 3437 3229 3b61 6e67 756c 6172 2e6d  n(472);angular.m
-00160930: 6f64 756c 6528 2264 6274 2229 2e66 6163  odule("dbt").fac
-00160940: 746f 7279 2822 7365 6c65 6374 6f72 5365  tory("selectorSe
-00160950: 7276 6963 6522 2c5b 2224 7374 6174 6522  rvice",["$state"
-00160960: 2c66 756e 6374 696f 6e28 6529 7b76 6172  ,function(e){var
-00160970: 2074 3d7b 696e 636c 7564 653a 2222 2c65   t={include:"",e
-00160980: 7863 6c75 6465 3a22 222c 7061 636b 6167  xclude:"",packag
-00160990: 6573 3a5b 5d2c 7461 6773 3a5b 6e75 6c6c  es:[],tags:[null
-001609a0: 5d2c 7265 736f 7572 6365 5f74 7970 6573  ],resource_types
-001609b0: 3a5b 226d 6f64 656c 222c 2273 6565 6422  :["model","seed"
-001609c0: 2c22 736e 6170 7368 6f74 222c 2273 6f75  ,"snapshot","sou
-001609d0: 7263 6522 2c22 7465 7374 222c 2275 6e69  rce","test","uni
-001609e0: 745f 7465 7374 222c 2261 6e61 6c79 7369  t_test","analysi
-001609f0: 7322 2c22 6578 706f 7375 7265 222c 226d  s","exposure","m
-00160a00: 6574 7269 6322 2c22 7365 6d61 6e74 6963  etric","semantic
-00160a10: 5f6d 6f64 656c 225d 2c64 6570 7468 3a31  _model"],depth:1
-00160a20: 7d2c 6e3d 7b76 6965 775f 6e6f 6465 3a6e  },n={view_node:n
-00160a30: 756c 6c2c 7365 6c65 6374 696f 6e3a 7b63  ull,selection:{c
-00160a40: 6c65 616e 3a72 2e63 6c6f 6e65 2874 292c  lean:r.clone(t),
-00160a50: 6469 7274 793a 722e 636c 6f6e 6528 7429  dirty:r.clone(t)
-00160a60: 7d2c 6f70 7469 6f6e 733a 7b70 6163 6b61  },options:{packa
-00160a70: 6765 733a 5b5d 2c74 6167 733a 5b6e 756c  ges:[],tags:[nul
-00160a80: 6c5d 2c72 6573 6f75 7263 655f 7479 7065  l],resource_type
-00160a90: 733a 5b22 6d6f 6465 6c22 2c22 7365 6564  s:["model","seed
-00160aa0: 222c 2273 6e61 7073 686f 7422 2c22 736f  ","snapshot","so
-00160ab0: 7572 6365 222c 2274 6573 7422 2c22 616e  urce","test","an
-00160ac0: 616c 7973 6973 222c 2265 7870 6f73 7572  alysis","exposur
-00160ad0: 6522 2c22 6d65 7472 6963 222c 2273 656d  e","metric","sem
-00160ae0: 616e 7469 635f 6d6f 6465 6c22 2c22 756e  antic_model","un
-00160af0: 6974 5f74 6573 7422 5d7d 2c69 6e69 743a  it_test"]},init:
-00160b00: 6675 6e63 7469 6f6e 2865 297b 722e 6561  function(e){r.ea
-00160b10: 6368 2865 2c28 6675 6e63 7469 6f6e 2865  ch(e,(function(e
-00160b20: 2c72 297b 6e2e 6f70 7469 6f6e 735b 725d  ,r){n.options[r]
-00160b30: 3d65 2c74 5b72 5d3d 652c 6e2e 7365 6c65  =e,t[r]=e,n.sele
-00160b40: 6374 696f 6e2e 636c 6561 6e5b 725d 3d65  ction.clean[r]=e
-00160b50: 2c6e 2e73 656c 6563 7469 6f6e 2e64 6972  ,n.selection.dir
-00160b60: 7479 5b72 5d3d 657d 2929 7d2c 7265 7365  ty[r]=e}))},rese
-00160b70: 7453 656c 6563 7469 6f6e 3a66 756e 6374  tSelection:funct
-00160b80: 696f 6e28 6529 7b76 6172 2069 3d7b 696e  ion(e){var i={in
-00160b90: 636c 7564 653a 6526 2672 2e69 6e63 6c75  clude:e&&r.inclu
-00160ba0: 6465 7328 5b22 6d6f 6465 6c22 2c22 7365  des(["model","se
-00160bb0: 6564 222c 2273 6e61 7073 686f 7422 5d2c  ed","snapshot"],
-00160bc0: 652e 7265 736f 7572 6365 5f74 7970 6529  e.resource_type)
-00160bd0: 3f22 2b22 2b65 2e6e 616d 652b 222b 223a  ?"+"+e.name+"+":
-00160be0: 6526 2622 736f 7572 6365 223d 3d65 2e72  e&&"source"==e.r
-00160bf0: 6573 6f75 7263 655f 7479 7065 3f22 2b73  esource_type?"+s
-00160c00: 6f75 7263 653a 222b 652e 736f 7572 6365  ource:"+e.source
-00160c10: 5f6e 616d 652b 222e 222b 652e 6e61 6d65  _name+"."+e.name
-00160c20: 2b22 2b22 3a65 2626 2265 7870 6f73 7572  +"+":e&&"exposur
-00160c30: 6522 3d3d 652e 7265 736f 7572 6365 5f74  e"==e.resource_t
-00160c40: 7970 653f 222b 6578 706f 7375 7265 3a22  ype?"+exposure:"
-00160c50: 2b65 2e6e 616d 653a 6526 2622 6d65 7472  +e.name:e&&"metr
-00160c60: 6963 223d 3d65 2e72 6573 6f75 7263 655f  ic"==e.resource_
-00160c70: 7479 7065 3f22 2b6d 6574 7269 633a 222b  type?"+metric:"+
-00160c80: 652e 6e61 6d65 3a65 2626 2273 656d 616e  e.name:e&&"seman
-00160c90: 7469 635f 6d6f 6465 6c22 3d3d 652e 7265  tic_model"==e.re
-00160ca0: 736f 7572 6365 5f74 7970 653f 222b 7365  source_type?"+se
-00160cb0: 6d61 6e74 6963 5f6d 6f64 656c 3a22 2b65  mantic_model:"+e
-00160cc0: 2e6e 616d 653a 6526 2672 2e69 6e63 6c75  .name:e&&r.inclu
-00160cd0: 6465 7328 5b22 616e 616c 7973 6973 222c  des(["analysis",
-00160ce0: 2274 6573 7422 2c22 756e 6974 5f74 6573  "test","unit_tes
-00160cf0: 7422 5d2c 652e 7265 736f 7572 6365 5f74  t"],e.resource_t
-00160d00: 7970 6529 3f22 2b22 2b65 2e6e 616d 653a  ype)?"+"+e.name:
-00160d10: 2222 7d2c 6f3d 722e 6173 7369 676e 287b  ""},o=r.assign({
-00160d20: 7d2c 742c 6929 3b6e 2e73 656c 6563 7469  },t,i);n.selecti
-00160d30: 6f6e 2e63 6c65 616e 3d72 2e63 6c6f 6e65  on.clean=r.clone
-00160d40: 286f 292c 6e2e 7365 6c65 6374 696f 6e2e  (o),n.selection.
-00160d50: 6469 7274 793d 722e 636c 6f6e 6528 6f29  dirty=r.clone(o)
-00160d60: 2c6e 2e76 6965 775f 6e6f 6465 3d65 7d2c  ,n.view_node=e},
-00160d70: 6765 7456 6965 774e 6f64 653a 6675 6e63  getViewNode:func
-00160d80: 7469 6f6e 2829 7b72 6574 7572 6e20 6e2e  tion(){return n.
-00160d90: 7669 6577 5f6e 6f64 657d 2c65 7863 6c75  view_node},exclu
-00160da0: 6465 4e6f 6465 3a66 756e 6374 696f 6e28  deNode:function(
-00160db0: 652c 7429 7b76 6172 2072 2c69 3d6e 2e73  e,t){var r,i=n.s
-00160dc0: 656c 6563 7469 6f6e 2e64 6972 7479 2e65  election.dirty.e
-00160dd0: 7863 6c75 6465 2c6f 3d74 2e70 6172 656e  xclude,o=t.paren
-00160de0: 7473 3f22 2b22 3a22 222c 613d 742e 6368  ts?"+":"",a=t.ch
-00160df0: 696c 6472 656e 3f22 2b22 3a22 222c 733d  ildren?"+":"",s=
-00160e00: 692e 6c65 6e67 7468 3e30 3f22 2022 3a22  i.length>0?" ":"
-00160e10: 223b 2273 6f75 7263 6522 3d3d 652e 7265  ";"source"==e.re
-00160e20: 736f 7572 6365 5f74 7970 653f 286f 2b3d  source_type?(o+=
-00160e30: 2273 6f75 7263 653a 222c 723d 652e 736f  "source:",r=e.so
-00160e40: 7572 6365 5f6e 616d 652b 222e 222b 652e  urce_name+"."+e.
-00160e50: 6e61 6d65 293a 5b22 6578 706f 7375 7265  name):["exposure
-00160e60: 222c 226d 6574 7269 6322 2c22 7365 6d61  ","metric","sema
-00160e70: 6e74 6963 5f6d 6f64 656c 225d 2e69 6e64  ntic_model"].ind
-00160e80: 6578 4f66 2865 2e72 6573 6f75 7263 655f  exOf(e.resource_
-00160e90: 7479 7065 293e 2d31 3f28 6f2b 3d65 2e72  type)>-1?(o+=e.r
-00160ea0: 6573 6f75 7263 655f 7479 7065 2b22 3a22  esource_type+":"
-00160eb0: 2c72 3d65 2e6e 616d 6529 3a72 3d65 2e6e  ,r=e.name):r=e.n
-00160ec0: 616d 653b 7661 7220 6c3d 692b 732b 6f2b  ame;var l=i+s+o+
-00160ed0: 722b 613b 7265 7475 726e 206e 2e73 656c  r+a;return n.sel
-00160ee0: 6563 7469 6f6e 2e64 6972 7479 2e65 7863  ection.dirty.exc
-00160ef0: 6c75 6465 3d6c 2c6e 2e75 7064 6174 6553  lude=l,n.updateS
-00160f00: 656c 6563 7469 6f6e 2829 7d2c 7365 6c65  election()},sele
-00160f10: 6374 536f 7572 6365 3a66 756e 6374 696f  ctSource:functio
-00160f20: 6e28 652c 7429 7b76 6172 2072 3d22 736f  n(e,t){var r="so
-00160f30: 7572 6365 3a22 2b65 2b28 742e 6368 696c  urce:"+e+(t.chil
-00160f40: 6472 656e 3f22 2b22 3a22 2229 3b72 6574  dren?"+":"");ret
-00160f50: 7572 6e20 6e2e 7365 6c65 6374 696f 6e2e  urn n.selection.
-00160f60: 6469 7274 792e 696e 636c 7564 653d 722c  dirty.include=r,
-00160f70: 6e2e 7570 6461 7465 5365 6c65 6374 696f  n.updateSelectio
-00160f80: 6e28 297d 2c63 6c65 6172 5669 6577 4e6f  n()},clearViewNo
-00160f90: 6465 3a66 756e 6374 696f 6e28 297b 6e2e  de:function(){n.
-00160fa0: 7669 6577 5f6e 6f64 653d 6e75 6c6c 7d2c  view_node=null},
-00160fb0: 6973 4469 7274 793a 6675 6e63 7469 6f6e  isDirty:function
-00160fc0: 2829 7b72 6574 7572 6e21 722e 6973 4571  (){return!r.isEq
-00160fd0: 7561 6c28 6e2e 7365 6c65 6374 696f 6e2e  ual(n.selection.
-00160fe0: 636c 6561 6e2c 6e2e 7365 6c65 6374 696f  clean,n.selectio
-00160ff0: 6e2e 6469 7274 7929 7d2c 7570 6461 7465  n.dirty)},update
-00161000: 5365 6c65 6374 696f 6e3a 6675 6e63 7469  Selection:functi
-00161010: 6f6e 2829 7b72 6574 7572 6e20 6e2e 7365  on(){return n.se
-00161020: 6c65 6374 696f 6e2e 636c 6561 6e3d 722e  lection.clean=r.
-00161030: 636c 6f6e 6528 6e2e 7365 6c65 6374 696f  clone(n.selectio
-00161040: 6e2e 6469 7274 7929 2c6e 2e73 656c 6563  n.dirty),n.selec
-00161050: 7469 6f6e 2e63 6c65 616e 7d2c 7365 6c65  tion.clean},sele
-00161060: 6374 4e6f 6465 733a 6675 6e63 7469 6f6e  ctNodes:function
-00161070: 2865 2c74 2c6e 297b 7265 7475 726e 2069  (e,t,n){return i
-00161080: 2e73 656c 6563 744e 6f64 6573 2865 2c74  .selectNodes(e,t
-00161090: 2c6e 297d 7d3b 7265 7475 726e 206e 7d5d  ,n)}};return n}]
-001610a0: 297d 2c66 756e 6374 696f 6e28 652c 742c  )},function(e,t,
-001610b0: 6e29 7b63 6f6e 7374 2072 3d6e 2832 3129  n){const r=n(21)
-001610c0: 2c69 3d6e 2834 3733 293b 6675 6e63 7469  ,i=n(473);functi
-001610d0: 6f6e 206f 2865 2c74 297b 7265 7475 726e  on o(e,t){return
-001610e0: 2074 7c7c 2874 3d22 2022 292c 722e 6669   t||(t=" "),r.fi
-001610f0: 6c74 6572 2872 2e75 6e69 7128 652e 7370  lter(r.uniq(e.sp
-00161100: 6c69 7428 7429 292c 2866 756e 6374 696f  lit(t)),(functio
-00161110: 6e28 6529 7b72 6574 7572 6e20 652e 6c65  n(e){return e.le
-00161120: 6e67 7468 3e30 7d29 297d 6675 6e63 7469  ngth>0}))}functi
-00161130: 6f6e 2061 2865 297b 7661 7220 743d 7b72  on a(e){var t={r
-00161140: 6177 3a65 2c73 656c 6563 745f 6174 3a21  aw:e,select_at:!
-00161150: 312c 7365 6c65 6374 5f63 6869 6c64 7265  1,select_childre
-00161160: 6e3a 2131 2c63 6869 6c64 7265 6e5f 6465  n:!1,children_de
-00161170: 7074 683a 6e75 6c6c 2c73 656c 6563 745f  pth:null,select_
-00161180: 7061 7265 6e74 733a 2131 2c70 6172 656e  parents:!1,paren
-00161190: 7473 5f64 6570 7468 3a6e 756c 6c7d 3b63  ts_depth:null};c
-001611a0: 6f6e 7374 206e 3d6e 6577 2052 6567 4578  onst n=new RegEx
-001611b0: 7028 2222 2b2f 5e2f 2e73 6f75 7263 652b  p(""+/^/.source+
-001611c0: 2f28 3f3c 6368 696c 6473 5f70 6172 656e  /(?<childs_paren
-001611d0: 7473 3e28 5c40 2929 3f2f 2e73 6f75 7263  ts>(\@))?/.sourc
-001611e0: 652b 2f28 3f3c 7061 7265 6e74 733e 2828  e+/(?<parents>((
-001611f0: 3f3c 7061 7265 6e74 735f 6465 7074 683e  ?<parents_depth>
-00161200: 285c 642a 2929 5c2b 2929 3f2f 2e73 6f75  (\d*))\+))?/.sou
-00161210: 7263 652b 2f28 283f 3c6d 6574 686f 643e  rce+/((?<method>
-00161220: 285b 5c77 2e5d 2b29 293a 293f 2f2e 736f  ([\w.]+)):)?/.so
-00161230: 7572 6365 2b2f 283f 3c76 616c 7565 3e28  urce+/(?<value>(
-00161240: 2e2a 3f29 292f 2e73 6f75 7263 652b 2f28  .*?))/.source+/(
-00161250: 3f3c 6368 696c 6472 656e 3e28 5c2b 283f  ?<children>(\+(?
-00161260: 3c63 6869 6c64 7265 6e5f 6465 7074 683e  <children_depth>
-00161270: 285c 642a 2929 2929 3f2f 2e73 6f75 7263  (\d*))))?/.sourc
-00161280: 652b 2f24 2f2e 736f 7572 6365 292e 6578  e+/$/.source).ex
-00161290: 6563 2865 292e 6772 6f75 7073 3b74 2e73  ec(e).groups;t.s
-001612a0: 656c 6563 745f 6174 3d22 4022 3d3d 6e2e  elect_at="@"==n.
-001612b0: 6368 696c 6473 5f70 6172 656e 7473 2c74  childs_parents,t
-001612c0: 2e73 656c 6563 745f 7061 7265 6e74 733d  .select_parents=
-001612d0: 2121 6e2e 7061 7265 6e74 732c 742e 7365  !!n.parents,t.se
-001612e0: 6c65 6374 5f63 6869 6c64 7265 6e3d 2121  lect_children=!!
-001612f0: 6e2e 6368 696c 6472 656e 2c6e 2e70 6172  n.children,n.par
-00161300: 656e 7473 5f64 6570 7468 2626 2874 2e70  ents_depth&&(t.p
-00161310: 6172 656e 7473 5f64 6570 7468 3d70 6172  arents_depth=par
-00161320: 7365 496e 7428 6e2e 7061 7265 6e74 735f  seInt(n.parents_
-00161330: 6465 7074 6829 292c 6e2e 6368 696c 6472  depth)),n.childr
-00161340: 656e 5f64 6570 7468 2626 2874 2e63 6869  en_depth&&(t.chi
-00161350: 6c64 7265 6e5f 6465 7074 683d 7061 7273  ldren_depth=pars
-00161360: 6549 6e74 286e 2e63 6869 6c64 7265 6e5f  eInt(n.children_
-00161370: 6465 7074 6829 293b 7661 7220 723d 6e2e  depth));var r=n.
-00161380: 6d65 7468 6f64 2c69 3d6e 2e76 616c 7565  method,i=n.value
-00161390: 3b72 6574 7572 6e20 723f 2d31 213d 722e  ;return r?-1!=r.
-001613a0: 696e 6465 784f 6628 222e 2229 2626 285b  indexOf(".")&&([
-001613b0: 722c 7365 6c65 6374 6f72 5f6d 6f64 6966  r,selector_modif
-001613c0: 6965 725d 3d72 2e73 706c 6974 2822 2e22  ier]=r.split("."
-001613d0: 2c32 292c 693d 7b63 6f6e 6669 673a 7365  ,2),i={config:se
-001613e0: 6c65 6374 6f72 5f6d 6f64 6966 6965 722c  lector_modifier,
-001613f0: 7661 6c75 653a 697d 293a 723d 2269 6d70  value:i}):r="imp
-00161400: 6c69 6369 7422 2c74 2e73 656c 6563 746f  licit",t.selecto
-00161410: 725f 7479 7065 3d72 2c74 2e73 656c 6563  r_type=r,t.selec
-00161420: 746f 725f 7661 6c75 653d 692c 747d 6675  tor_value=i,t}fu
-00161430: 6e63 7469 6f6e 2073 2865 297b 7661 7220  nction s(e){var 
-00161440: 743d 6f28 652c 2220 2229 3b72 6574 7572  t=o(e," ");retur
-00161450: 6e20 722e 6d61 7028 742c 2866 756e 6374  n r.map(t,(funct
-00161460: 696f 6e28 6529 7b76 6172 2074 3d6f 2865  ion(e){var t=o(e
-00161470: 2c22 2c22 293b 7265 7475 726e 2074 2e6c  ,",");return t.l
-00161480: 656e 6774 683e 313f 7b6d 6574 686f 643a  ength>1?{method:
-00161490: 2269 6e74 6572 7365 6374 222c 7365 6c65  "intersect",sele
-001614a0: 6374 6f72 733a 722e 6d61 7028 742c 6129  ctors:r.map(t,a)
-001614b0: 7d3a 7b6d 6574 686f 643a 226e 6f6e 6522  }:{method:"none"
-001614c0: 2c73 656c 6563 746f 7273 3a72 2e6d 6170  ,selectors:r.map
-001614d0: 285b 655d 2c61 297d 7d29 297d 6675 6e63  ([e],a)}}))}func
-001614e0: 7469 6f6e 206c 2865 2c74 297b 7661 7220  tion l(e,t){var 
-001614f0: 6e3d 7328 6529 2c69 3d6e 756c 6c2c 6f3d  n=s(e),i=null,o=
-00161500: 6e75 6c6c 3b72 6574 7572 6e20 722e 6561  null;return r.ea
-00161510: 6368 286e 2c28 6675 6e63 7469 6f6e 2865  ch(n,(function(e
-00161520: 297b 7661 7220 6e3d 2269 6e74 6572 7365  ){var n="interse
-00161530: 6374 223d 3d65 2e6d 6574 686f 643f 722e  ct"==e.method?r.
-00161540: 696e 7465 7273 6563 7469 6f6e 3a72 2e75  intersection:r.u
-00161550: 6e69 6f6e 3b72 2e65 6163 6828 652e 7365  nion;r.each(e.se
-00161560: 6c65 6374 6f72 732c 2866 756e 6374 696f  lectors,(functio
-00161570: 6e28 6529 7b76 6172 2072 3d74 2865 293b  n(e){var r=t(e);
-00161580: 6e75 6c6c 3d3d 3d69 3f28 693d 722e 6d61  null===i?(i=r.ma
-00161590: 7463 6865 642c 6f3d 722e 7365 6c65 6374  tched,o=r.select
-001615a0: 6564 293a 2869 3d6e 2869 2c72 2e6d 6174  ed):(i=n(i,r.mat
-001615b0: 6368 6564 292c 6f3d 6e28 6f2c 722e 7365  ched),o=n(o,r.se
-001615c0: 6c65 6374 6564 2929 7d29 297d 2929 2c7b  lected))}))})),{
-001615d0: 6d61 7463 6865 643a 697c 7c5b 5d2c 7365  matched:i||[],se
-001615e0: 6c65 6374 6564 3a6f 7c7c 5b5d 7d7d 652e  lected:o||[]}}e.
-001615f0: 6578 706f 7274 733d 7b73 706c 6974 5370  exports={splitSp
-00161600: 6563 733a 6f2c 7061 7273 6553 7065 633a  ecs:o,parseSpec:
-00161610: 612c 7061 7273 6553 7065 6373 3a73 2c62  a,parseSpecs:s,b
-00161620: 7569 6c64 5370 6563 3a66 756e 6374 696f  uildSpec:functio
-00161630: 6e28 652c 742c 6e29 7b72 6574 7572 6e7b  n(e,t,n){return{
-00161640: 696e 636c 7564 653a 7328 6529 2c65 7863  include:s(e),exc
-00161650: 6c75 6465 3a73 2874 292c 686f 7073 3a6e  lude:s(t),hops:n
-00161660: 7d7d 2c61 7070 6c79 5370 6563 3a6c 2c73  }},applySpec:l,s
-00161670: 656c 6563 744e 6f64 6573 3a66 756e 6374  electNodes:funct
-00161680: 696f 6e28 652c 742c 6e29 7b6e 2e69 6e63  ion(e,t,n){n.inc
-00161690: 6c75 6465 2c6e 2e65 7863 6c75 6465 3b76  lude,n.exclude;v
-001616a0: 6172 206f 2c61 3d72 2e70 6172 7469 616c  ar o,a=r.partial
-001616b0: 2869 2e67 6574 4e6f 6465 7346 726f 6d53  (i.getNodesFromS
-001616c0: 7065 632c 652c 742c 6e2e 686f 7073 293b  pec,e,t,n.hops);
-001616d0: 722e 7661 6c75 6573 2874 292c 6f3d 303d  r.values(t),o=0=
-001616e0: 3d6e 2e69 6e63 6c75 6465 2e74 7269 6d28  =n.include.trim(
-001616f0: 292e 6c65 6e67 7468 3f7b 7365 6c65 6374  ).length?{select
-00161700: 6564 3a65 2e6e 6f64 6573 2829 2c6d 6174  ed:e.nodes(),mat
-00161710: 6368 6564 3a5b 5d7d 3a6c 286e 2e69 6e63  ched:[]}:l(n.inc
-00161720: 6c75 6465 2c61 293b 7661 7220 733d 6c28  lude,a);var s=l(
-00161730: 6e2e 6578 636c 7564 652c 6129 2c63 3d6f  n.exclude,a),c=o
-00161740: 2e73 656c 6563 7465 642c 753d 6f2e 6d61  .selected,u=o.ma
-00161750: 7463 6865 643b 633d 722e 6469 6666 6572  tched;c=r.differ
-00161760: 656e 6365 2863 2c73 2e73 656c 6563 7465  ence(c,s.selecte
-00161770: 6429 2c75 3d72 2e64 6966 6665 7265 6e63  d),u=r.differenc
-00161780: 6528 752c 732e 6d61 7463 6865 6429 3b76  e(u,s.matched);v
-00161790: 6172 2064 3d5b 5d3b 7265 7475 726e 2072  ar d=[];return r
-001617a0: 2e65 6163 6828 632c 2866 756e 6374 696f  .each(c,(functio
-001617b0: 6e28 6529 7b76 6172 2069 3d74 5b65 5d3b  n(e){var i=t[e];
-001617c0: 692e 6461 7461 2e74 6167 737c 7c28 692e  i.data.tags||(i.
-001617d0: 6461 7461 2e74 6167 733d 5b5d 293b 7661  data.tags=[]);va
-001617e0: 7220 6f3d 722e 696e 636c 7564 6573 286e  r o=r.includes(n
-001617f0: 2e70 6163 6b61 6765 732c 692e 6461 7461  .packages,i.data
-00161800: 2e70 6163 6b61 6765 5f6e 616d 6529 2c61  .package_name),a
-00161810: 3d72 2e69 6e74 6572 7365 6374 696f 6e28  =r.intersection(
-00161820: 6e2e 7461 6773 2c69 2e64 6174 612e 7461  n.tags,i.data.ta
-00161830: 6773 292e 6c65 6e67 7468 3e30 2c73 3d72  gs).length>0,s=r
-00161840: 2e69 6e63 6c75 6465 7328 6e2e 7461 6773  .includes(n.tags
-00161850: 2c6e 756c 6c29 2626 303d 3d69 2e64 6174  ,null)&&0==i.dat
-00161860: 612e 7461 6773 2e6c 656e 6774 682c 6c3d  a.tags.length,l=
-00161870: 722e 696e 636c 7564 6573 286e 2e72 6573  r.includes(n.res
-00161880: 6f75 7263 655f 7479 7065 732c 692e 6461  ource_types,i.da
-00161890: 7461 2e72 6573 6f75 7263 655f 7479 7065  ta.resource_type
-001618a0: 293b 6f26 2628 617c 7c73 2926 266c 7c7c  );o&&(a||s)&&l||
-001618b0: 642e 7075 7368 2869 2e64 6174 612e 756e  d.push(i.data.un
-001618c0: 6971 7565 5f69 6429 7d29 292c 7b73 656c  ique_id)})),{sel
-001618d0: 6563 7465 643a 722e 6469 6666 6572 656e  ected:r.differen
-001618e0: 6365 2863 2c64 292c 6d61 7463 6865 643a  ce(c,d),matched:
-001618f0: 722e 6469 6666 6572 656e 6365 2875 2c64  r.difference(u,d
-00161900: 297d 7d7d 7d2c 6675 6e63 7469 6f6e 2865  )}}}},function(e
-00161910: 2c74 2c6e 297b 636f 6e73 7420 723d 6e28  ,t,n){const r=n(
-00161920: 3231 292c 693d 6e28 3230 3329 3b76 6172  21),i=n(203);var
-00161930: 206f 3d22 6671 6e22 2c61 3d22 7461 6722   o="fqn",a="tag"
-00161940: 2c73 3d22 736f 7572 6365 222c 6c3d 2265  ,s="source",l="e
-00161950: 7870 6f73 7572 6522 2c63 3d22 6d65 7472  xposure",c="metr
-00161960: 6963 222c 753d 2273 656d 616e 7469 635f  ic",u="semantic_
-00161970: 6d6f 6465 6c22 2c64 3d22 6772 6f75 7022  model",d="group"
-00161980: 2c70 3d22 7061 7468 222c 663d 2266 696c  ,p="path",f="fil
-00161990: 6522 2c68 3d22 7061 636b 6167 6522 2c67  e",h="package",g
-001619a0: 3d22 636f 6e66 6967 222c 6d3d 2274 6573  ="config",m="tes
-001619b0: 745f 6e61 6d65 222c 763d 2274 6573 745f  t_name",v="test_
-001619c0: 7479 7065 222c 623d 7b7d 3b66 756e 6374  type",b={};funct
-001619d0: 696f 6e20 7928 652c 742c 6e29 7b76 6172  ion y(e,t,n){var
-001619e0: 2072 3d65 2e73 6c69 6365 282d 3129 5b30   r=e.slice(-1)[0
-001619f0: 5d2c 693d 652e 736c 6963 6528 2d32 2c2d  ],i=e.slice(-2,-
-00161a00: 3129 5b30 5d3b 6966 2874 3d3d 3d72 2972  1)[0];if(t===r)r
-00161a10: 6574 7572 6e21 303b 6966 2876 6572 7369  eturn!0;if(versi
-00161a20: 6f6e 5f6f 7074 696f 6e73 3d5b 692c 692b  on_options=[i,i+
-00161a30: 225f 222b 722c 692b 222e 222b 725d 2c6e  "_"+r,i+"."+r],n
-00161a40: 2626 7665 7273 696f 6e5f 6f70 7469 6f6e  &&version_option
-00161a50: 732e 696e 636c 7564 6573 2874 2929 7265  s.includes(t))re
-00161a60: 7475 726e 2130 3b76 6172 206f 3d65 2e72  turn!0;var o=e.r
-00161a70: 6564 7563 6528 2865 2c74 293d 3e65 2e63  educe((e,t)=>e.c
-00161a80: 6f6e 6361 7428 742e 7370 6c69 7428 222e  oncat(t.split(".
-00161a90: 2229 292c 5b5d 292c 613d 742e 7370 6c69  ")),[]),a=t.spli
-00161aa0: 7428 222e 2229 3b69 6628 6f2e 6c65 6e67  t(".");if(o.leng
-00161ab0: 7468 3c61 2e6c 656e 6774 6829 7265 7475  th<a.length)retu
-00161ac0: 726e 2131 3b66 6f72 2876 6172 2073 3d30  rn!1;for(var s=0
-00161ad0: 3b73 3c61 2e6c 656e 6774 683b 732b 2b29  ;s<a.length;s++)
-00161ae0: 7b76 6172 206c 3d61 5b73 5d3b 6966 2822  {var l=a[s];if("
-00161af0: 2a22 3d3d 6c29 7265 7475 726e 2130 3b69  *"==l)return!0;i
-00161b00: 6628 6f5b 735d 213d 6c29 7265 7475 726e  f(o[s]!=l)return
-00161b10: 2131 7d72 6574 7572 6e21 307d 6675 6e63  !1}return!0}func
-00161b20: 7469 6f6e 2078 2865 2c74 297b 7661 7220  tion x(e,t){var 
-00161b30: 6e3d 5b5d 3b72 6574 7572 6e20 722e 6561  n=[];return r.ea
-00161b40: 6368 2865 2c28 6675 6e63 7469 6f6e 2865  ch(e,(function(e
-00161b50: 297b 7661 7220 693d 652e 6461 7461 2c6f  ){var i=e.data,o
-00161b60: 3d69 2e66 716e 2c61 3d6e 756c 6c21 3d3d  =i.fqn,a=null!==
-00161b70: 692e 7665 7273 696f 6e3b 6966 286f 2626  i.version;if(o&&
-00161b80: 2273 6f75 7263 6522 213d 692e 7265 736f  "source"!=i.reso
-00161b90: 7572 6365 5f74 7970 6526 2622 6578 706f  urce_type&&"expo
-00161ba0: 7375 7265 2221 3d69 2e72 6573 6f75 7263  sure"!=i.resourc
-00161bb0: 655f 7479 7065 2626 226d 6574 7269 6322  e_type&&"metric"
-00161bc0: 213d 692e 7265 736f 7572 6365 5f74 7970  !=i.resource_typ
-00161bd0: 6526 2622 7365 6d61 6e74 6963 5f6d 6f64  e&&"semantic_mod
-00161be0: 656c 2221 3d69 2e72 6573 6f75 7263 655f  el"!=i.resource_
-00161bf0: 7479 7065 297b 7661 7220 733d 722e 7265  type){var s=r.re
-00161c00: 7374 286f 293b 2879 286f 2c74 2c61 297c  st(o);(y(o,t,a)|
-00161c10: 7c79 2873 2c74 2c61 2929 2626 6e2e 7075  |y(s,t,a))&&n.pu
-00161c20: 7368 2869 297d 7d29 292c 722e 756e 6971  sh(i)}})),r.uniq
-00161c30: 286e 297d 6675 6e63 7469 6f6e 2077 2865  (n)}function w(e
-00161c40: 2c74 297b 7661 7220 6e3d 5b5d 2c69 3d74  ,t){var n=[],i=t
-00161c50: 2e73 706c 6974 2822 2f22 293b 7265 7475  .split("/");retu
-00161c60: 726e 2072 2e65 6163 6828 652c 2866 756e  rn r.each(e,(fun
-00161c70: 6374 696f 6e28 6529 7b76 6172 2074 3d28  ction(e){var t=(
-00161c80: 652e 6461 7461 2e6f 7269 6769 6e61 6c5f  e.data.original_
-00161c90: 6669 6c65 5f70 6174 687c 7c22 2229 2e73  file_path||"").s
-00161ca0: 706c 6974 2822 2f22 292c 6f3d 2130 3b72  plit("/"),o=!0;r
-00161cb0: 2e65 6163 6828 692c 2866 756e 6374 696f  .each(i,(functio
-00161cc0: 6e28 652c 6e29 7b22 2a22 3d3d 657c 7c22  n(e,n){"*"==e||"
-00161cd0: 223d 3d65 7c7c 6521 3d74 5b6e 5d26 2628  "==e||e!=t[n]&&(
-00161ce0: 6f3d 2131 297d 2929 2c6f 2626 6e2e 7075  o=!1)})),o&&n.pu
-00161cf0: 7368 2865 2e64 6174 6129 7d29 292c 6e7d  sh(e.data)})),n}
-00161d00: 6675 6e63 7469 6f6e 206b 2865 2c74 297b  function k(e,t){
-00161d10: 7661 7220 6e3d 5b5d 3b72 6574 7572 6e20  var n=[];return 
-00161d20: 722e 6561 6368 2865 2c28 6675 6e63 7469  r.each(e,(functi
-00161d30: 6f6e 2865 297b 7661 7220 693d 652e 6461  on(e){var i=e.da
-00161d40: 7461 2e6f 7269 6769 6e61 6c5f 6669 6c65  ta.original_file
-00161d50: 5f70 6174 682e 7370 6c69 7428 222f 2229  _path.split("/")
-00161d60: 3b72 2e6c 6173 7428 6929 3d3d 7426 266e  ;r.last(i)==t&&n
-00161d70: 2e70 7573 6828 652e 6461 7461 297d 2929  .push(e.data)}))
-00161d80: 2c6e 7d66 756e 6374 696f 6e20 4128 652c  ,n}function A(e,
-00161d90: 7429 7b76 6172 206e 3d5b 5d3b 7265 7475  t){var n=[];retu
-00161da0: 726e 2072 2e65 6163 6828 652c 2866 756e  rn r.each(e,(fun
-00161db0: 6374 696f 6e28 6529 7b76 6172 2069 3d65  ction(e){var i=e
-00161dc0: 2e64 6174 612e 7461 6773 3b72 2e69 6e63  .data.tags;r.inc
-00161dd0: 6c75 6465 7328 692c 7429 2626 6e2e 7075  ludes(i,t)&&n.pu
-00161de0: 7368 2865 2e64 6174 6129 7d29 292c 6e7d  sh(e.data)})),n}
-00161df0: 6675 6e63 7469 6f6e 2045 2865 2c74 297b  function E(e,t){
-00161e00: 7661 7220 6e3d 5b5d 3b72 6574 7572 6e20  var n=[];return 
-00161e10: 722e 6561 6368 2865 2c28 6675 6e63 7469  r.each(e,(functi
-00161e20: 6f6e 2865 297b 652e 6461 7461 2e70 6163  on(e){e.data.pac
-00161e30: 6b61 6765 5f6e 616d 653d 3d74 2626 6e2e  kage_name==t&&n.
-00161e40: 7075 7368 2865 2e64 6174 6129 7d29 292c  push(e.data)})),
-00161e50: 6e7d 6675 6e63 7469 6f6e 2053 2865 2c74  n}function S(e,t
-00161e60: 297b 7661 7220 6e3d 5b5d 3b72 6574 7572  ){var n=[];retur
-00161e70: 6e20 722e 6561 6368 2865 2c28 6675 6e63  n r.each(e,(func
-00161e80: 7469 6f6e 2865 297b 7661 7220 723d 652e  tion(e){var r=e.
-00161e90: 6461 7461 3b72 2e63 6f6e 6669 6726 2672  data;r.config&&r
-00161ea0: 2e63 6f6e 6669 675b 742e 636f 6e66 6967  .config[t.config
-00161eb0: 5d3d 3d74 2e76 616c 7565 2626 6e2e 7075  ]==t.value&&n.pu
-00161ec0: 7368 2872 297d 2929 2c6e 7d66 756e 6374  sh(r)})),n}funct
-00161ed0: 696f 6e20 2428 652c 7429 7b76 6172 206e  ion $(e,t){var n
-00161ee0: 3d5b 5d3b 7265 7475 726e 2072 2e65 6163  =[];return r.eac
-00161ef0: 6828 652c 2866 756e 6374 696f 6e28 6529  h(e,(function(e)
-00161f00: 7b76 6172 2072 3d65 2e64 6174 613b 722e  {var r=e.data;r.
-00161f10: 7465 7374 5f6d 6574 6164 6174 6126 2672  test_metadata&&r
-00161f20: 2e74 6573 745f 6d65 7461 6461 7461 2e6e  .test_metadata.n
-00161f30: 616d 653d 3d74 2626 6e2e 7075 7368 2872  ame==t&&n.push(r
-00161f40: 297d 2929 2c6e 7d66 756e 6374 696f 6e20  )})),n}function 
-00161f50: 4328 652c 7429 7b76 6172 206e 3d5b 5d3b  C(e,t){var n=[];
-00161f60: 7265 7475 726e 2072 2e65 6163 6828 652c  return r.each(e,
-00161f70: 2866 756e 6374 696f 6e28 6529 7b76 6172  (function(e){var
-00161f80: 2072 3d65 2e64 6174 613b 6966 2822 7465   r=e.data;if("te
-00161f90: 7374 2221 3d72 2e72 6573 6f75 7263 655f  st"!=r.resource_
-00161fa0: 7479 7065 2972 6574 7572 6e21 313b 2872  type)return!1;(r
-00161fb0: 2e68 6173 4f77 6e50 726f 7065 7274 7928  .hasOwnProperty(
-00161fc0: 2274 6573 745f 6d65 7461 6461 7461 2229  "test_metadata")
-00161fd0: 2626 5b22 7363 6865 6d61 222c 2267 656e  &&["schema","gen
-00161fe0: 6572 6963 225d 2e69 6e64 6578 4f66 2874  eric"].indexOf(t
-00161ff0: 293e 2d31 7c7c 2172 2e68 6173 4f77 6e50  )>-1||!r.hasOwnP
-00162000: 726f 7065 7274 7928 2274 6573 745f 6d65  roperty("test_me
-00162010: 7461 6461 7461 2229 2626 5b22 6461 7461  tadata")&&["data
-00162020: 222c 2273 696e 6775 6c61 7222 5d2e 696e  ","singular"].in
-00162030: 6465 784f 6628 7429 3e2d 3129 2626 6e2e  dexOf(t)>-1)&&n.
-00162040: 7075 7368 2872 297d 2929 2c6e 7d66 756e  push(r)})),n}fun
-00162050: 6374 696f 6e20 5f28 652c 7429 7b76 6172  ction _(e,t){var
-00162060: 206e 3d5b 5d3b 7265 7475 726e 2072 2e65   n=[];return r.e
-00162070: 6163 6828 652c 2866 756e 6374 696f 6e28  ach(e,(function(
-00162080: 6529 7b76 6172 2072 3d65 2e64 6174 613b  e){var r=e.data;
-00162090: 6966 2822 736f 7572 6365 223d 3d72 2e72  if("source"==r.r
-001620a0: 6573 6f75 7263 655f 7479 7065 297b 7661  esource_type){va
-001620b0: 7220 692c 6f2c 613d 722e 736f 7572 6365  r i,o,a=r.source
-001620c0: 5f6e 616d 652c 733d 722e 6e61 6d65 3b2d  _name,s=r.name;-
-001620d0: 3121 3d74 2e69 6e64 6578 4f66 2822 2e22  1!=t.indexOf("."
-001620e0: 293f 5b69 2c6f 5d3d 742e 7370 6c69 7428  )?[i,o]=t.split(
-001620f0: 222e 222c 3229 3a28 693d 742c 6f3d 6e75  ".",2):(i=t,o=nu
-00162100: 6c6c 292c 2822 2a22 3d3d 697c 7c69 3d3d  ll),("*"==i||i==
-00162110: 6126 2622 2a22 3d3d 3d6f 7c7c 693d 3d61  a&&"*"===o||i==a
-00162120: 2626 6f3d 3d3d 737c 7c69 3d3d 6126 266e  &&o===s||i==a&&n
-00162130: 756c 6c3d 3d3d 6f29 2626 6e2e 7075 7368  ull===o)&&n.push
-00162140: 2865 2e64 6174 6129 7d7d 2929 2c6e 7d62  (e.data)}})),n}b
-00162150: 5b22 696d 706c 6963 6974 225d 3d66 756e  ["implicit"]=fun
-00162160: 6374 696f 6e28 652c 7429 7b76 6172 206e  ction(e,t){var n
-00162170: 3d78 2865 2c74 292c 693d 7728 652c 7429  =x(e,t),i=w(e,t)
-00162180: 2c6f 3d5b 5d3b 742e 746f 4c6f 7765 7243  ,o=[];t.toLowerC
-00162190: 6173 6528 292e 656e 6473 5769 7468 2822  ase().endsWith("
-001621a0: 2e73 716c 2229 2626 286f 3d6b 2865 2c74  .sql")&&(o=k(e,t
-001621b0: 2929 3b76 6172 2061 3d72 2e75 6e69 7128  ));var a=r.uniq(
-001621c0: 5b5d 2e63 6f6e 6361 7428 722e 6d61 7028  [].concat(r.map(
-001621d0: 6e2c 2275 6e69 7175 655f 6964 2229 2c72  n,"unique_id"),r
-001621e0: 2e6d 6170 2869 2c22 756e 6971 7565 5f69  .map(i,"unique_i
-001621f0: 6422 292c 722e 6d61 7028 6f2c 2275 6e69  d"),r.map(o,"uni
-00162200: 7175 655f 6964 2229 2929 3b72 6574 7572  que_id")));retur
-00162210: 6e20 722e 6d61 7028 612c 743d 3e65 5b74  n r.map(a,t=>e[t
-00162220: 5d2e 6461 7461 297d 2c62 5b6f 5d3d 782c  ].data)},b[o]=x,
-00162230: 625b 615d 3d41 2c62 5b73 5d3d 5f2c 625b  b[a]=A,b[s]=_,b[
-00162240: 6c5d 3d66 756e 6374 696f 6e28 652c 7429  l]=function(e,t)
-00162250: 7b76 6172 206e 3d5b 5d3b 7265 7475 726e  {var n=[];return
-00162260: 2072 2e65 6163 6828 652c 2866 756e 6374   r.each(e,(funct
-00162270: 696f 6e28 6529 7b76 6172 2072 3d65 2e64  ion(e){var r=e.d
-00162280: 6174 613b 6966 2822 6578 706f 7375 7265  ata;if("exposure
-00162290: 223d 3d72 2e72 6573 6f75 7263 655f 7479  "==r.resource_ty
-001622a0: 7065 297b 7661 7220 693d 722e 6e61 6d65  pe){var i=r.name
-001622b0: 3b28 222a 223d 3d74 7c7c 743d 3d69 2926  ;("*"==t||t==i)&
-001622c0: 266e 2e70 7573 6828 652e 6461 7461 297d  &n.push(e.data)}
-001622d0: 7d29 292c 6e7d 2c62 5b63 5d3d 6675 6e63  })),n},b[c]=func
-001622e0: 7469 6f6e 2865 2c74 297b 7661 7220 6e3d  tion(e,t){var n=
-001622f0: 5b5d 3b72 6574 7572 6e20 722e 6561 6368  [];return r.each
-00162300: 2865 2c28 6675 6e63 7469 6f6e 2865 297b  (e,(function(e){
-00162310: 7661 7220 723d 652e 6461 7461 3b69 6628  var r=e.data;if(
-00162320: 226d 6574 7269 6322 3d3d 722e 7265 736f  "metric"==r.reso
-00162330: 7572 6365 5f74 7970 6529 7b76 6172 2069  urce_type){var i
-00162340: 3d72 2e6e 616d 653b 2822 2a22 3d3d 747c  =r.name;("*"==t|
-00162350: 7c74 3d3d 6929 2626 6e2e 7075 7368 2865  |t==i)&&n.push(e
-00162360: 2e64 6174 6129 7d7d 2929 2c6e 7d2c 625b  .data)}})),n},b[
-00162370: 755d 3d66 756e 6374 696f 6e28 652c 7429  u]=function(e,t)
-00162380: 7b76 6172 206e 3d5b 5d3b 7265 7475 726e  {var n=[];return
-00162390: 2072 2e65 6163 6828 652c 2866 756e 6374   r.each(e,(funct
-001623a0: 696f 6e28 6529 7b76 6172 2072 3d65 2e64  ion(e){var r=e.d
-001623b0: 6174 613b 6966 2822 7365 6d61 6e74 6963  ata;if("semantic
-001623c0: 5f6d 6f64 656c 223d 3d72 2e72 6573 6f75  _model"==r.resou
-001623d0: 7263 655f 7479 7065 297b 7661 7220 693d  rce_type){var i=
-001623e0: 722e 6e61 6d65 3b28 222a 223d 3d74 7c7c  r.name;("*"==t||
-001623f0: 743d 3d69 2926 266e 2e70 7573 6828 652e  t==i)&&n.push(e.
-00162400: 6461 7461 297d 7d29 292c 6e7d 2c62 5b64  data)}})),n},b[d
-00162410: 5d3d 6675 6e63 7469 6f6e 2865 2c74 297b  ]=function(e,t){
-00162420: 7661 7220 6e3d 5b5d 3b72 6574 7572 6e20  var n=[];return 
-00162430: 722e 6561 6368 2865 2c28 6675 6e63 7469  r.each(e,(functi
-00162440: 6f6e 2865 297b 7661 7220 723d 652e 6461  on(e){var r=e.da
-00162450: 7461 3b72 2e67 726f 7570 3d3d 7426 266e  ta;r.group==t&&n
-00162460: 2e70 7573 6828 7229 7d29 292c 6e7d 2c62  .push(r)})),n},b
-00162470: 5b70 5d3d 772c 625b 665d 3d6b 2c62 5b68  [p]=w,b[f]=k,b[h
-00162480: 5d3d 452c 625b 675d 3d53 2c62 5b6d 5d3d  ]=E,b[g]=S,b[m]=
-00162490: 242c 625b 765d 3d43 2c65 2e65 7870 6f72  $,b[v]=C,e.expor
-001624a0: 7473 3d7b 6973 4651 4e4d 6174 6368 3a79  ts={isFQNMatch:y
-001624b0: 2c67 6574 4e6f 6465 7342 7946 514e 3a78  ,getNodesByFQN:x
-001624c0: 2c67 6574 4e6f 6465 7342 7954 6167 3a41  ,getNodesByTag:A
-001624d0: 2c67 6574 4e6f 6465 7342 7953 6f75 7263  ,getNodesBySourc
-001624e0: 653a 5f2c 6765 744e 6f64 6573 4279 5061  e:_,getNodesByPa
-001624f0: 7468 3a77 2c67 6574 4e6f 6465 7342 7950  th:w,getNodesByP
-00162500: 6163 6b61 6765 3a45 2c67 6574 4e6f 6465  ackage:E,getNode
-00162510: 7342 7943 6f6e 6669 673a 532c 6765 744e  sByConfig:S,getN
-00162520: 6f64 6573 4279 5465 7374 4e61 6d65 3a24  odesByTestName:$
-00162530: 2c67 6574 4e6f 6465 7342 7954 6573 7454  ,getNodesByTestT
-00162540: 7970 653a 432c 6765 744e 6f64 6573 4672  ype:C,getNodesFr
-00162550: 6f6d 5370 6563 3a66 756e 6374 696f 6e28  omSpec:function(
-00162560: 652c 742c 6e2c 6f29 7b63 6f6e 7374 2061  e,t,n,o){const a
-00162570: 3d62 5b6f 2e73 656c 6563 746f 725f 7479  =b[o.selector_ty
-00162580: 7065 5d3b 6966 2821 6129 7265 7475 726e  pe];if(!a)return
-00162590: 7b73 656c 6563 7465 643a 5b5d 2c6d 6174  {selected:[],mat
-001625a0: 6368 6564 3a5b 5d7d 3b76 6172 2073 3d61  ched:[]};var s=a
-001625b0: 2874 2c6f 2e73 656c 6563 746f 725f 7661  (t,o.selector_va
-001625c0: 6c75 6529 2c6c 3d5b 5d2c 633d 5b5d 3b72  lue),l=[],c=[];r
-001625d0: 6574 7572 6e20 722e 6561 6368 2873 2c28  eturn r.each(s,(
-001625e0: 6675 6e63 7469 6f6e 2874 297b 7661 7220  function(t){var 
-001625f0: 613d 742e 756e 6971 7565 5f69 643b 632e  a=t.unique_id;c.
-00162600: 7075 7368 2874 2e75 6e69 7175 655f 6964  push(t.unique_id
-00162610: 293b 7661 7220 733d 5b5d 2c75 3d5b 5d2c  );var s=[],u=[],
-00162620: 643d 5b5d 3b69 6628 6f2e 7365 6c65 6374  d=[];if(o.select
-00162630: 5f61 7426 2628 643d 722e 756e 696f 6e28  _at&&(d=r.union(
-00162640: 692e 7365 6c65 6374 4174 2865 2c61 2929  i.selectAt(e,a))
-00162650: 292c 6f2e 7365 6c65 6374 5f70 6172 656e  ),o.select_paren
-00162660: 7473 297b 7661 7220 703d 6e7c 7c6f 2e70  ts){var p=n||o.p
-00162670: 6172 656e 7473 5f64 6570 7468 3b73 3d69  arents_depth;s=i
-00162680: 2e61 6e63 6573 746f 724e 6f64 6573 2865  .ancestorNodes(e
-00162690: 2c61 2c70 297d 6966 286f 2e73 656c 6563  ,a,p)}if(o.selec
-001626a0: 745f 6368 696c 6472 656e 297b 703d 6e7c  t_children){p=n|
-001626b0: 7c6f 2e63 6869 6c64 7265 6e5f 6465 7074  |o.children_dept
-001626c0: 683b 753d 692e 6465 7363 656e 6465 6e74  h;u=i.descendent
-001626d0: 4e6f 6465 7328 652c 612c 7029 7d6c 3d72  Nodes(e,a,p)}l=r
-001626e0: 2e75 6e69 6f6e 285b 615d 2c6c 2c75 2c73  .union([a],l,u,s
-001626f0: 2c64 297d 2929 2c7b 7365 6c65 6374 6564  ,d)})),{selected
-00162700: 3a6c 2c6d 6174 6368 6564 3a63 7d7d 7d7d  :l,matched:c}}}}
-00162710: 2c66 756e 6374 696f 6e28 652c 742c 6e29  ,function(e,t,n)
-00162720: 7b63 6f6e 7374 2072 3d6e 2839 293b 6e28  {const r=n(9);n(
-00162730: 3437 3529 3b72 2e6d 6f64 756c 6528 2264  475);r.module("d
-00162740: 6274 2229 2e66 6163 746f 7279 2822 7472  bt").factory("tr
-00162750: 6163 6b69 6e67 5365 7276 6963 6522 2c5b  ackingService",[
-00162760: 2224 6c6f 6361 7469 6f6e 222c 2273 656c  "$location","sel
-00162770: 6563 746f 7253 6572 7669 6365 222c 2224  ectorService","$
-00162780: 726f 6f74 5363 6f70 6522 2c66 756e 6374  rootScope",funct
-00162790: 696f 6e28 652c 742c 6e29 7b76 6172 2072  ion(e,t,n){var r
-001627a0: 3d7b 696e 6974 6961 6c69 7a65 643a 2131  ={initialized:!1
-001627b0: 2c73 6e6f 7770 6c6f 773a 6e75 6c6c 2c70  ,snowplow:null,p
-001627c0: 726f 6a65 6374 5f69 643a 6e75 6c6c 2c69  roject_id:null,i
-001627d0: 6e69 743a 6675 6e63 7469 6f6e 2865 297b  nit:function(e){
-001627e0: 722e 696e 6974 6961 6c69 7a65 647c 7c28  r.initialized||(
-001627f0: 722e 696e 6974 6961 6c69 7a65 643d 2130  r.initialized=!0
-00162800: 2c72 2e70 726f 6a65 6374 5f69 643d 652e  ,r.project_id=e.
-00162810: 7072 6f6a 6563 745f 6964 2c21 303d 3d3d  project_id,!0===
-00162820: 652e 7472 6163 6b26 2672 2e74 7572 6e5f  e.track&&r.turn_
-00162830: 6f6e 5f74 7261 636b 696e 6728 2929 7d2c  on_tracking())},
-00162840: 6973 486f 7374 6564 3a66 756e 6374 696f  isHosted:functio
-00162850: 6e28 297b 7265 7475 726e 2068 6f73 7465  n(){return hoste
-00162860: 6467 6574 6462 743d 7769 6e64 6f77 2e6c  dgetdbt=window.l
-00162870: 6f63 6174 696f 6e2e 686f 7374 6e61 6d65  ocation.hostname
-00162880: 2e69 6e64 6578 4f66 2822 2e67 6574 6462  .indexOf(".getdb
-00162890: 742e 636f 6d22 293e 2d31 2c68 6f73 7465  t.com")>-1,hoste
-001628a0: 6464 6274 3d77 696e 646f 772e 6c6f 6361  ddbt=window.loca
-001628b0: 7469 6f6e 2e68 6f73 746e 616d 652e 696e  tion.hostname.in
-001628c0: 6465 784f 6628 222e 6462 742e 636f 6d22  dexOf(".dbt.com"
-001628d0: 293e 2d31 2c68 6f73 7465 6467 6574 6462  )>-1,hostedgetdb
-001628e0: 747c 7c68 6f73 7465 6464 6274 7d2c 7475  t||hosteddbt},tu
-001628f0: 726e 5f6f 6e5f 7472 6163 6b69 6e67 3a66  rn_on_tracking:f
-00162900: 756e 6374 696f 6e28 297b 7661 7220 652c  unction(){var e,
-00162910: 742c 6e2c 692c 6f2c 613b 653d 7769 6e64  t,n,i,o,a;e=wind
-00162920: 6f77 2c74 3d64 6f63 756d 656e 742c 6e3d  ow,t=document,n=
-00162930: 2273 6372 6970 7422 2c65 5b69 3d22 736e  "script",e[i="sn
-00162940: 6f77 706c 6f77 225d 7c7c 2865 2e47 6c6f  owplow"]||(e.Glo
-00162950: 6261 6c53 6e6f 7770 6c6f 774e 616d 6573  balSnowplowNames
-00162960: 7061 6365 3d65 2e47 6c6f 6261 6c53 6e6f  pace=e.GlobalSno
-00162970: 7770 6c6f 774e 616d 6573 7061 6365 7c7c  wplowNamespace||
-00162980: 5b5d 2c65 2e47 6c6f 6261 6c53 6e6f 7770  [],e.GlobalSnowp
-00162990: 6c6f 774e 616d 6573 7061 6365 2e70 7573  lowNamespace.pus
-001629a0: 6828 6929 2c65 5b69 5d3d 6675 6e63 7469  h(i),e[i]=functi
-001629b0: 6f6e 2829 7b28 655b 695d 2e71 3d65 5b69  on(){(e[i].q=e[i
-001629c0: 5d2e 717c 7c5b 5d29 2e70 7573 6828 6172  ].q||[]).push(ar
-001629d0: 6775 6d65 6e74 7329 7d2c 655b 695d 2e71  guments)},e[i].q
-001629e0: 3d65 5b69 5d2e 717c 7c5b 5d2c 6f3d 742e  =e[i].q||[],o=t.
-001629f0: 6372 6561 7465 456c 656d 656e 7428 6e29  createElement(n)
-00162a00: 2c61 3d74 2e67 6574 456c 656d 656e 7473  ,a=t.getElements
-00162a10: 4279 5461 674e 616d 6528 6e29 5b30 5d2c  ByTagName(n)[0],
-00162a20: 6f2e 6173 796e 633d 312c 6f2e 7372 633d  o.async=1,o.src=
-00162a30: 222f 2f64 3166 6338 7776 387a 6167 3563  "//d1fc8wv8zag5c
-00162a40: 612e 636c 6f75 6466 726f 6e74 2e6e 6574  a.cloudfront.net
-00162a50: 2f32 2e39 2e30 2f73 702e 6a73 222c 612e  /2.9.0/sp.js",a.
-00162a60: 7061 7265 6e74 4e6f 6465 2e69 6e73 6572  parentNode.inser
-00162a70: 7442 6566 6f72 6528 6f2c 6129 293b 7661  tBefore(o,a));va
-00162a80: 7220 733d 7b61 7070 4964 3a22 6462 742d  r s={appId:"dbt-
-00162a90: 646f 6373 222c 666f 7263 6553 6563 7572  docs",forceSecur
-00162aa0: 6554 7261 636b 6572 3a21 302c 7265 7370  eTracker:!0,resp
-00162ab0: 6563 7444 6f4e 6f74 5472 6163 6b3a 2130  ectDoNotTrack:!0
-00162ac0: 2c75 7365 7246 696e 6765 7270 7269 6e74  ,userFingerprint
-00162ad0: 3a21 312c 636f 6e74 6578 7473 3a7b 7765  :!1,contexts:{we
-00162ae0: 6250 6167 653a 2130 7d7d 3b72 2e69 7348  bPage:!0}};r.isH
-00162af0: 6f73 7465 6428 2926 2628 7769 6e64 6f77  osted()&&(window
-00162b00: 2e6c 6f63 6174 696f 6e2e 686f 7374 6e61  .location.hostna
-00162b10: 6d65 2e69 6e64 6578 4f66 2822 2e67 6574  me.indexOf(".get
-00162b20: 6462 742e 636f 6d22 293e 2d31 3f73 2e63  dbt.com")>-1?s.c
-00162b30: 6f6f 6b69 6544 6f6d 6169 6e3d 222e 6765  ookieDomain=".ge
-00162b40: 7464 6274 2e63 6f6d 223a 732e 636f 6f6b  tdbt.com":s.cook
-00162b50: 6965 446f 6d61 696e 3d22 2e64 6274 2e63  ieDomain=".dbt.c
-00162b60: 6f6d 2229 2c72 2e73 6e6f 7770 6c6f 773d  om"),r.snowplow=
-00162b70: 7769 6e64 6f77 2e73 6e6f 7770 6c6f 772c  window.snowplow,
-00162b80: 722e 736e 6f77 706c 6f77 2822 6e65 7754  r.snowplow("newT
-00162b90: 7261 636b 6572 222c 2273 7022 2c22 6669  racker","sp","fi
-00162ba0: 7368 746f 776e 616e 616c 7974 6963 732e  shtownanalytics.
-00162bb0: 7369 6e74 6572 2d63 6f6c 6c65 6374 2e63  sinter-collect.c
-00162bc0: 6f6d 222c 7329 2c72 2e73 6e6f 7770 6c6f  om",s),r.snowplo
-00162bd0: 7728 2265 6e61 626c 6541 6374 6976 6974  w("enableActivit
-00162be0: 7954 7261 636b 696e 6722 2c33 302c 3330  yTracking",30,30
-00162bf0: 292c 722e 7472 6163 6b5f 7061 6765 7669  ),r.track_pagevi
-00162c00: 6577 2829 7d2c 6675 7a7a 5572 6c73 3a66  ew()},fuzzUrls:f
-00162c10: 756e 6374 696f 6e28 297b 722e 6973 486f  unction(){r.isHo
-00162c20: 7374 6564 2829 7c7c 2872 2e73 6e6f 7770  sted()||(r.snowp
-00162c30: 6c6f 7728 2273 6574 4375 7374 6f6d 5572  low("setCustomUr
-00162c40: 6c22 2c22 6874 7470 733a 2f2f 6675 7a7a  l","https://fuzz
-00162c50: 6564 2e67 6574 6462 742e 636f 6d2f 2229  ed.getdbt.com/")
-00162c60: 2c72 2e73 6e6f 7770 6c6f 7728 2273 6574  ,r.snowplow("set
-00162c70: 5265 6665 7272 6572 5572 6c22 2c22 6874  ReferrerUrl","ht
-00162c80: 7470 733a 2f2f 6675 7a7a 6564 2e67 6574  tps://fuzzed.get
-00162c90: 6462 742e 636f 6d2f 2229 297d 2c67 6574  dbt.com/"))},get
-00162ca0: 436f 6e74 6578 743a 6675 6e63 7469 6f6e  Context:function
-00162cb0: 2829 7b72 6574 7572 6e5b 7b73 6368 656d  (){return[{schem
-00162cc0: 613a 2269 676c 753a 636f 6d2e 6462 742f  a:"iglu:com.dbt/
-00162cd0: 6462 745f 646f 6373 2f6a 736f 6e73 6368  dbt_docs/jsonsch
-00162ce0: 656d 612f 312d 302d 3022 2c64 6174 613a  ema/1-0-0",data:
-00162cf0: 7b69 735f 636c 6f75 645f 686f 7374 6564  {is_cloud_hosted
-00162d00: 3a72 2e69 7348 6f73 7465 6428 292c 636f  :r.isHosted(),co
-00162d10: 7265 5f70 726f 6a65 6374 5f69 643a 722e  re_project_id:r.
-00162d20: 7072 6f6a 6563 745f 6964 7d7d 5d7d 2c74  project_id}}]},t
-00162d30: 7261 636b 5f70 6167 6576 6965 773a 6675  rack_pageview:fu
-00162d40: 6e63 7469 6f6e 2829 7b69 6628 722e 736e  nction(){if(r.sn
-00162d50: 6f77 706c 6f77 297b 722e 6675 7a7a 5572  owplow){r.fuzzUr
-00162d60: 6c73 2829 3b72 2e73 6e6f 7770 6c6f 7728  ls();r.snowplow(
-00162d70: 2274 7261 636b 5061 6765 5669 6577 222c  "trackPageView",
-00162d80: 6e75 6c6c 2c72 2e67 6574 436f 6e74 6578  null,r.getContex
-00162d90: 7428 2929 7d7d 2c74 7261 636b 5f65 7665  t())}},track_eve
-00162da0: 6e74 3a66 756e 6374 696f 6e28 652c 742c  nt:function(e,t,
-00162db0: 6e2c 6929 7b72 2e73 6e6f 7770 6c6f 7726  n,i){r.snowplow&
-00162dc0: 2628 722e 6675 7a7a 5572 6c73 2829 2c72  &(r.fuzzUrls(),r
-00162dd0: 2e73 6e6f 7770 6c6f 7728 2274 7261 636b  .snowplow("track
-00162de0: 5374 7275 6374 4576 656e 7422 2c22 6462  StructEvent","db
-00162df0: 742d 646f 6373 222c 652c 742c 6e2c 692c  t-docs",e,t,n,i,
-00162e00: 722e 6765 7443 6f6e 7465 7874 2829 2929  r.getContext()))
-00162e10: 7d2c 7472 6163 6b5f 6772 6170 685f 696e  },track_graph_in
-00162e20: 7465 7261 6374 696f 6e3a 6675 6e63 7469  teraction:functi
-00162e30: 6f6e 2865 2c74 297b 722e 736e 6f77 706c  on(e,t){r.snowpl
-00162e40: 6f77 2626 2872 2e66 757a 7a55 726c 7328  ow&&(r.fuzzUrls(
-00162e50: 292c 722e 7472 6163 6b5f 6576 656e 7428  ),r.track_event(
-00162e60: 2267 7261 7068 222c 2269 6e74 6572 6163  "graph","interac
-00162e70: 7422 2c65 2c74 2929 7d7d 3b72 6574 7572  t",e,t))}};retur
-00162e80: 6e20 727d 5d29 7d2c 6675 6e63 7469 6f6e  n r}])},function
-00162e90: 2865 2c74 2c6e 297b 7661 7220 722c 692c  (e,t,n){var r,i,
-00162ea0: 6f2c 612c 733b 723d 6e28 3437 3629 2c69  o,a,s;r=n(476),i
-00162eb0: 3d6e 2832 3034 292e 7574 6638 2c6f 3d6e  =n(204).utf8,o=n
-00162ec0: 2834 3737 292c 613d 6e28 3230 3429 2e62  (477),a=n(204).b
-00162ed0: 696e 2c28 733d 6675 6e63 7469 6f6e 2865  in,(s=function(e
-00162ee0: 2c74 297b 652e 636f 6e73 7472 7563 746f  ,t){e.constructo
-00162ef0: 723d 3d53 7472 696e 673f 653d 7426 2622  r==String?e=t&&"
-00162f00: 6269 6e61 7279 223d 3d3d 742e 656e 636f  binary"===t.enco
-00162f10: 6469 6e67 3f61 2e73 7472 696e 6754 6f42  ding?a.stringToB
-00162f20: 7974 6573 2865 293a 692e 7374 7269 6e67  ytes(e):i.string
-00162f30: 546f 4279 7465 7328 6529 3a6f 2865 293f  ToBytes(e):o(e)?
-00162f40: 653d 4172 7261 792e 7072 6f74 6f74 7970  e=Array.prototyp
-00162f50: 652e 736c 6963 652e 6361 6c6c 2865 2c30  e.slice.call(e,0
-00162f60: 293a 4172 7261 792e 6973 4172 7261 7928  ):Array.isArray(
-00162f70: 6529 7c7c 652e 636f 6e73 7472 7563 746f  e)||e.constructo
-00162f80: 723d 3d3d 5569 6e74 3841 7272 6179 7c7c  r===Uint8Array||
-00162f90: 2865 3d65 2e74 6f53 7472 696e 6728 2929  (e=e.toString())
-00162fa0: 3b66 6f72 2876 6172 206e 3d72 2e62 7974  ;for(var n=r.byt
-00162fb0: 6573 546f 576f 7264 7328 6529 2c6c 3d38  esToWords(e),l=8
-00162fc0: 2a65 2e6c 656e 6774 682c 633d 3137 3332  *e.length,c=1732
-00162fd0: 3538 3431 3933 2c75 3d2d 3237 3137 3333  584193,u=-271733
-00162fe0: 3837 392c 643d 2d31 3733 3235 3834 3139  879,d=-173258419
-00162ff0: 342c 703d 3237 3137 3333 3837 382c 663d  4,p=271733878,f=
-00163000: 303b 663c 6e2e 6c65 6e67 7468 3b66 2b2b  0;f<n.length;f++
-00163010: 296e 5b66 5d3d 3136 3731 3139 3335 2628  )n[f]=16711935&(
-00163020: 6e5b 665d 3c3c 387c 6e5b 665d 3e3e 3e32  n[f]<<8|n[f]>>>2
-00163030: 3429 7c34 3237 3832 3535 3336 3026 286e  4)|4278255360&(n
-00163040: 5b66 5d3c 3c32 347c 6e5b 665d 3e3e 3e38  [f]<<24|n[f]>>>8
-00163050: 293b 6e5b 6c3e 3e3e 355d 7c3d 3132 383c  );n[l>>>5]|=128<
-00163060: 3c6c 2533 322c 6e5b 3134 2b28 6c2b 3634  <l%32,n[14+(l+64
-00163070: 3e3e 3e39 3c3c 3429 5d3d 6c3b 7661 7220  >>>9<<4)]=l;var 
-00163080: 683d 732e 5f66 662c 673d 732e 5f67 672c  h=s._ff,g=s._gg,
-00163090: 6d3d 732e 5f68 682c 763d 732e 5f69 693b  m=s._hh,v=s._ii;
-001630a0: 666f 7228 663d 303b 663c 6e2e 6c65 6e67  for(f=0;f<n.leng
-001630b0: 7468 3b66 2b3d 3136 297b 7661 7220 623d  th;f+=16){var b=
-001630c0: 632c 793d 752c 783d 642c 773d 703b 633d  c,y=u,x=d,w=p;c=
-001630d0: 6828 632c 752c 642c 702c 6e5b 662b 305d  h(c,u,d,p,n[f+0]
-001630e0: 2c37 2c2d 3638 3038 3736 3933 3629 2c70  ,7,-680876936),p
-001630f0: 3d68 2870 2c63 2c75 2c64 2c6e 5b66 2b31  =h(p,c,u,d,n[f+1
-00163100: 5d2c 3132 2c2d 3338 3935 3634 3538 3629  ],12,-389564586)
-00163110: 2c64 3d68 2864 2c70 2c63 2c75 2c6e 5b66  ,d=h(d,p,c,u,n[f
-00163120: 2b32 5d2c 3137 2c36 3036 3130 3538 3139  +2],17,606105819
-00163130: 292c 753d 6828 752c 642c 702c 632c 6e5b  ),u=h(u,d,p,c,n[
-00163140: 662b 335d 2c32 322c 2d31 3034 3435 3235  f+3],22,-1044525
-00163150: 3333 3029 2c63 3d68 2863 2c75 2c64 2c70  330),c=h(c,u,d,p
-00163160: 2c6e 5b66 2b34 5d2c 372c 2d31 3736 3431  ,n[f+4],7,-17641
-00163170: 3838 3937 292c 703d 6828 702c 632c 752c  8897),p=h(p,c,u,
-00163180: 642c 6e5b 662b 355d 2c31 322c 3132 3030  d,n[f+5],12,1200
-00163190: 3038 3034 3236 292c 643d 6828 642c 702c  080426),d=h(d,p,
-001631a0: 632c 752c 6e5b 662b 365d 2c31 372c 2d31  c,u,n[f+6],17,-1
-001631b0: 3437 3332 3331 3334 3129 2c75 3d68 2875  473231341),u=h(u
-001631c0: 2c64 2c70 2c63 2c6e 5b66 2b37 5d2c 3232  ,d,p,c,n[f+7],22
-001631d0: 2c2d 3435 3730 3539 3833 292c 633d 6828  ,-45705983),c=h(
-001631e0: 632c 752c 642c 702c 6e5b 662b 385d 2c37  c,u,d,p,n[f+8],7
-001631f0: 2c31 3737 3030 3335 3431 3629 2c70 3d68  ,1770035416),p=h
-00163200: 2870 2c63 2c75 2c64 2c6e 5b66 2b39 5d2c  (p,c,u,d,n[f+9],
-00163210: 3132 2c2d 3139 3538 3431 3434 3137 292c  12,-1958414417),
-00163220: 643d 6828 642c 702c 632c 752c 6e5b 662b  d=h(d,p,c,u,n[f+
-00163230: 3130 5d2c 3137 2c2d 3432 3036 3329 2c75  10],17,-42063),u
-00163240: 3d68 2875 2c64 2c70 2c63 2c6e 5b66 2b31  =h(u,d,p,c,n[f+1
-00163250: 315d 2c32 322c 2d31 3939 3034 3034 3136  1],22,-199040416
-00163260: 3229 2c63 3d68 2863 2c75 2c64 2c70 2c6e  2),c=h(c,u,d,p,n
-00163270: 5b66 2b31 325d 2c37 2c31 3830 3436 3033  [f+12],7,1804603
-00163280: 3638 3229 2c70 3d68 2870 2c63 2c75 2c64  682),p=h(p,c,u,d
-00163290: 2c6e 5b66 2b31 335d 2c31 322c 2d34 3033  ,n[f+13],12,-403
-001632a0: 3431 3130 3129 2c64 3d68 2864 2c70 2c63  41101),d=h(d,p,c
-001632b0: 2c75 2c6e 5b66 2b31 345d 2c31 372c 2d31  ,u,n[f+14],17,-1
-001632c0: 3530 3230 3032 3239 3029 2c63 3d67 2863  502002290),c=g(c
-001632d0: 2c75 3d68 2875 2c64 2c70 2c63 2c6e 5b66  ,u=h(u,d,p,c,n[f
-001632e0: 2b31 355d 2c32 322c 3132 3336 3533 3533  +15],22,12365353
-001632f0: 3239 292c 642c 702c 6e5b 662b 315d 2c35  29),d,p,n[f+1],5
-00163300: 2c2d 3136 3537 3936 3531 3029 2c70 3d67  ,-165796510),p=g
-00163310: 2870 2c63 2c75 2c64 2c6e 5b66 2b36 5d2c  (p,c,u,d,n[f+6],
-00163320: 392c 2d31 3036 3935 3031 3633 3229 2c64  9,-1069501632),d
-00163330: 3d67 2864 2c70 2c63 2c75 2c6e 5b66 2b31  =g(d,p,c,u,n[f+1
-00163340: 315d 2c31 342c 3634 3337 3137 3731 3329  1],14,643717713)
-00163350: 2c75 3d67 2875 2c64 2c70 2c63 2c6e 5b66  ,u=g(u,d,p,c,n[f
-00163360: 2b30 5d2c 3230 2c2d 3337 3338 3937 3330  +0],20,-37389730
-00163370: 3229 2c63 3d67 2863 2c75 2c64 2c70 2c6e  2),c=g(c,u,d,p,n
-00163380: 5b66 2b35 5d2c 352c 2d37 3031 3535 3836  [f+5],5,-7015586
-00163390: 3931 292c 703d 6728 702c 632c 752c 642c  91),p=g(p,c,u,d,
-001633a0: 6e5b 662b 3130 5d2c 392c 3338 3031 3630  n[f+10],9,380160
-001633b0: 3833 292c 643d 6728 642c 702c 632c 752c  83),d=g(d,p,c,u,
-001633c0: 6e5b 662b 3135 5d2c 3134 2c2d 3636 3034  n[f+15],14,-6604
-001633d0: 3738 3333 3529 2c75 3d67 2875 2c64 2c70  78335),u=g(u,d,p
-001633e0: 2c63 2c6e 5b66 2b34 5d2c 3230 2c2d 3430  ,c,n[f+4],20,-40
-001633f0: 3535 3337 3834 3829 2c63 3d67 2863 2c75  5537848),c=g(c,u
-00163400: 2c64 2c70 2c6e 5b66 2b39 5d2c 352c 3536  ,d,p,n[f+9],5,56
-00163410: 3834 3436 3433 3829 2c70 3d67 2870 2c63  8446438),p=g(p,c
-00163420: 2c75 2c64 2c6e 5b66 2b31 345d 2c39 2c2d  ,u,d,n[f+14],9,-
-00163430: 3130 3139 3830 3336 3930 292c 643d 6728  1019803690),d=g(
-00163440: 642c 702c 632c 752c 6e5b 662b 335d 2c31  d,p,c,u,n[f+3],1
-00163450: 342c 2d31 3837 3336 3339 3631 292c 753d  4,-187363961),u=
-00163460: 6728 752c 642c 702c 632c 6e5b 662b 385d  g(u,d,p,c,n[f+8]
-00163470: 2c32 302c 3131 3633 3533 3135 3031 292c  ,20,1163531501),
-00163480: 633d 6728 632c 752c 642c 702c 6e5b 662b  c=g(c,u,d,p,n[f+
-00163490: 3133 5d2c 352c 2d31 3434 3436 3831 3436  13],5,-144468146
-001634a0: 3729 2c70 3d67 2870 2c63 2c75 2c64 2c6e  7),p=g(p,c,u,d,n
-001634b0: 5b66 2b32 5d2c 392c 2d35 3134 3033 3738  [f+2],9,-5140378
-001634c0: 3429 2c64 3d67 2864 2c70 2c63 2c75 2c6e  4),d=g(d,p,c,u,n
-001634d0: 5b66 2b37 5d2c 3134 2c31 3733 3533 3238  [f+7],14,1735328
-001634e0: 3437 3329 2c63 3d6d 2863 2c75 3d67 2875  473),c=m(c,u=g(u
-001634f0: 2c64 2c70 2c63 2c6e 5b66 2b31 325d 2c32  ,d,p,c,n[f+12],2
-00163500: 302c 2d31 3932 3636 3037 3733 3429 2c64  0,-1926607734),d
-00163510: 2c70 2c6e 5b66 2b35 5d2c 342c 2d33 3738  ,p,n[f+5],4,-378
-00163520: 3535 3829 2c70 3d6d 2870 2c63 2c75 2c64  558),p=m(p,c,u,d
-00163530: 2c6e 5b66 2b38 5d2c 3131 2c2d 3230 3232  ,n[f+8],11,-2022
-00163540: 3537 3434 3633 292c 643d 6d28 642c 702c  574463),d=m(d,p,
-00163550: 632c 752c 6e5b 662b 3131 5d2c 3136 2c31  c,u,n[f+11],16,1
-00163560: 3833 3930 3330 3536 3229 2c75 3d6d 2875  839030562),u=m(u
-00163570: 2c64 2c70 2c63 2c6e 5b66 2b31 345d 2c32  ,d,p,c,n[f+14],2
-00163580: 332c 2d33 3533 3039 3535 3629 2c63 3d6d  3,-35309556),c=m
-00163590: 2863 2c75 2c64 2c70 2c6e 5b66 2b31 5d2c  (c,u,d,p,n[f+1],
-001635a0: 342c 2d31 3533 3039 3932 3036 3029 2c70  4,-1530992060),p
-001635b0: 3d6d 2870 2c63 2c75 2c64 2c6e 5b66 2b34  =m(p,c,u,d,n[f+4
-001635c0: 5d2c 3131 2c31 3237 3238 3933 3335 3329  ],11,1272893353)
-001635d0: 2c64 3d6d 2864 2c70 2c63 2c75 2c6e 5b66  ,d=m(d,p,c,u,n[f
-001635e0: 2b37 5d2c 3136 2c2d 3135 3534 3937 3633  +7],16,-15549763
-001635f0: 3229 2c75 3d6d 2875 2c64 2c70 2c63 2c6e  2),u=m(u,d,p,c,n
-00163600: 5b66 2b31 305d 2c32 332c 2d31 3039 3437  [f+10],23,-10947
-00163610: 3330 3634 3029 2c63 3d6d 2863 2c75 2c64  30640),c=m(c,u,d
-00163620: 2c70 2c6e 5b66 2b31 335d 2c34 2c36 3831  ,p,n[f+13],4,681
-00163630: 3237 3931 3734 292c 703d 6d28 702c 632c  279174),p=m(p,c,
-00163640: 752c 642c 6e5b 662b 305d 2c31 312c 2d33  u,d,n[f+0],11,-3
-00163650: 3538 3533 3732 3232 292c 643d 6d28 642c  58537222),d=m(d,
-00163660: 702c 632c 752c 6e5b 662b 335d 2c31 362c  p,c,u,n[f+3],16,
-00163670: 2d37 3232 3532 3139 3739 292c 753d 6d28  -722521979),u=m(
-00163680: 752c 642c 702c 632c 6e5b 662b 365d 2c32  u,d,p,c,n[f+6],2
-00163690: 332c 3736 3032 3931 3839 292c 633d 6d28  3,76029189),c=m(
-001636a0: 632c 752c 642c 702c 6e5b 662b 395d 2c34  c,u,d,p,n[f+9],4
-001636b0: 2c2d 3634 3033 3634 3438 3729 2c70 3d6d  ,-640364487),p=m
-001636c0: 2870 2c63 2c75 2c64 2c6e 5b66 2b31 325d  (p,c,u,d,n[f+12]
-001636d0: 2c31 312c 2d34 3231 3831 3538 3335 292c  ,11,-421815835),
-001636e0: 643d 6d28 642c 702c 632c 752c 6e5b 662b  d=m(d,p,c,u,n[f+
-001636f0: 3135 5d2c 3136 2c35 3330 3734 3235 3230  15],16,530742520
-00163700: 292c 633d 7628 632c 753d 6d28 752c 642c  ),c=v(c,u=m(u,d,
-00163710: 702c 632c 6e5b 662b 325d 2c32 332c 2d39  p,c,n[f+2],23,-9
-00163720: 3935 3333 3836 3531 292c 642c 702c 6e5b  95338651),d,p,n[
-00163730: 662b 305d 2c36 2c2d 3139 3836 3330 3834  f+0],6,-19863084
-00163740: 3429 2c70 3d76 2870 2c63 2c75 2c64 2c6e  4),p=v(p,c,u,d,n
-00163750: 5b66 2b37 5d2c 3130 2c31 3132 3638 3931  [f+7],10,1126891
-00163760: 3431 3529 2c64 3d76 2864 2c70 2c63 2c75  415),d=v(d,p,c,u
-00163770: 2c6e 5b66 2b31 345d 2c31 352c 2d31 3431  ,n[f+14],15,-141
-00163780: 3633 3534 3930 3529 2c75 3d76 2875 2c64  6354905),u=v(u,d
-00163790: 2c70 2c63 2c6e 5b66 2b35 5d2c 3231 2c2d  ,p,c,n[f+5],21,-
-001637a0: 3537 3433 3430 3535 292c 633d 7628 632c  57434055),c=v(c,
-001637b0: 752c 642c 702c 6e5b 662b 3132 5d2c 362c  u,d,p,n[f+12],6,
-001637c0: 3137 3030 3438 3535 3731 292c 703d 7628  1700485571),p=v(
-001637d0: 702c 632c 752c 642c 6e5b 662b 335d 2c31  p,c,u,d,n[f+3],1
-001637e0: 302c 2d31 3839 3439 3836 3630 3629 2c64  0,-1894986606),d
-001637f0: 3d76 2864 2c70 2c63 2c75 2c6e 5b66 2b31  =v(d,p,c,u,n[f+1
-00163800: 305d 2c31 352c 2d31 3035 3135 3233 292c  0],15,-1051523),
-00163810: 753d 7628 752c 642c 702c 632c 6e5b 662b  u=v(u,d,p,c,n[f+
-00163820: 315d 2c32 312c 2d32 3035 3439 3232 3739  1],21,-205492279
-00163830: 3929 2c63 3d76 2863 2c75 2c64 2c70 2c6e  9),c=v(c,u,d,p,n
-00163840: 5b66 2b38 5d2c 362c 3138 3733 3331 3333  [f+8],6,18733133
-00163850: 3539 292c 703d 7628 702c 632c 752c 642c  59),p=v(p,c,u,d,
-00163860: 6e5b 662b 3135 5d2c 3130 2c2d 3330 3631  n[f+15],10,-3061
-00163870: 3137 3434 292c 643d 7628 642c 702c 632c  1744),d=v(d,p,c,
-00163880: 752c 6e5b 662b 365d 2c31 352c 2d31 3536  u,n[f+6],15,-156
-00163890: 3031 3938 3338 3029 2c75 3d76 2875 2c64  0198380),u=v(u,d
-001638a0: 2c70 2c63 2c6e 5b66 2b31 335d 2c32 312c  ,p,c,n[f+13],21,
-001638b0: 3133 3039 3135 3136 3439 292c 633d 7628  1309151649),c=v(
-001638c0: 632c 752c 642c 702c 6e5b 662b 345d 2c36  c,u,d,p,n[f+4],6
-001638d0: 2c2d 3134 3535 3233 3037 3029 2c70 3d76  ,-145523070),p=v
-001638e0: 2870 2c63 2c75 2c64 2c6e 5b66 2b31 315d  (p,c,u,d,n[f+11]
-001638f0: 2c31 302c 2d31 3132 3032 3130 3337 3929  ,10,-1120210379)
-00163900: 2c64 3d76 2864 2c70 2c63 2c75 2c6e 5b66  ,d=v(d,p,c,u,n[f
-00163910: 2b32 5d2c 3135 2c37 3138 3738 3732 3539  +2],15,718787259
-00163920: 292c 753d 7628 752c 642c 702c 632c 6e5b  ),u=v(u,d,p,c,n[
-00163930: 662b 395d 2c32 312c 2d33 3433 3438 3535  f+9],21,-3434855
-00163940: 3531 292c 633d 632b 623e 3e3e 302c 753d  51),c=c+b>>>0,u=
-00163950: 752b 793e 3e3e 302c 643d 642b 783e 3e3e  u+y>>>0,d=d+x>>>
-00163960: 302c 703d 702b 773e 3e3e 307d 7265 7475  0,p=p+w>>>0}retu
-00163970: 726e 2072 2e65 6e64 6961 6e28 5b63 2c75  rn r.endian([c,u
-00163980: 2c64 2c70 5d29 7d29 2e5f 6666 3d66 756e  ,d,p])})._ff=fun
-00163990: 6374 696f 6e28 652c 742c 6e2c 722c 692c  ction(e,t,n,r,i,
-001639a0: 6f2c 6129 7b76 6172 2073 3d65 2b28 7426  o,a){var s=e+(t&
-001639b0: 6e7c 7e74 2672 292b 2869 3e3e 3e30 292b  n|~t&r)+(i>>>0)+
-001639c0: 613b 7265 7475 726e 2873 3c3c 6f7c 733e  a;return(s<<o|s>
-001639d0: 3e3e 3332 2d6f 292b 747d 2c73 2e5f 6767  >>32-o)+t},s._gg
-001639e0: 3d66 756e 6374 696f 6e28 652c 742c 6e2c  =function(e,t,n,
-001639f0: 722c 692c 6f2c 6129 7b76 6172 2073 3d65  r,i,o,a){var s=e
-00163a00: 2b28 7426 727c 6e26 7e72 292b 2869 3e3e  +(t&r|n&~r)+(i>>
-00163a10: 3e30 292b 613b 7265 7475 726e 2873 3c3c  >0)+a;return(s<<
-00163a20: 6f7c 733e 3e3e 3332 2d6f 292b 747d 2c73  o|s>>>32-o)+t},s
-00163a30: 2e5f 6868 3d66 756e 6374 696f 6e28 652c  ._hh=function(e,
-00163a40: 742c 6e2c 722c 692c 6f2c 6129 7b76 6172  t,n,r,i,o,a){var
-00163a50: 2073 3d65 2b28 745e 6e5e 7229 2b28 693e   s=e+(t^n^r)+(i>
-00163a60: 3e3e 3029 2b61 3b72 6574 7572 6e28 733c  >>0)+a;return(s<
-00163a70: 3c6f 7c73 3e3e 3e33 322d 6f29 2b74 7d2c  <o|s>>>32-o)+t},
-00163a80: 732e 5f69 693d 6675 6e63 7469 6f6e 2865  s._ii=function(e
-00163a90: 2c74 2c6e 2c72 2c69 2c6f 2c61 297b 7661  ,t,n,r,i,o,a){va
-00163aa0: 7220 733d 652b 286e 5e28 747c 7e72 2929  r s=e+(n^(t|~r))
-00163ab0: 2b28 693e 3e3e 3029 2b61 3b72 6574 7572  +(i>>>0)+a;retur
-00163ac0: 6e28 733c 3c6f 7c73 3e3e 3e33 322d 6f29  n(s<<o|s>>>32-o)
-00163ad0: 2b74 7d2c 732e 5f62 6c6f 636b 7369 7a65  +t},s._blocksize
-00163ae0: 3d31 362c 732e 5f64 6967 6573 7473 697a  =16,s._digestsiz
-00163af0: 653d 3136 2c65 2e65 7870 6f72 7473 3d66  e=16,e.exports=f
-00163b00: 756e 6374 696f 6e28 652c 7429 7b69 6628  unction(e,t){if(
-00163b10: 6e75 6c6c 3d3d 6529 7468 726f 7720 6e65  null==e)throw ne
-00163b20: 7720 4572 726f 7228 2249 6c6c 6567 616c  w Error("Illegal
-00163b30: 2061 7267 756d 656e 7420 222b 6529 3b76   argument "+e);v
-00163b40: 6172 206e 3d72 2e77 6f72 6473 546f 4279  ar n=r.wordsToBy
-00163b50: 7465 7328 7328 652c 7429 293b 7265 7475  tes(s(e,t));retu
-00163b60: 726e 2074 2626 742e 6173 4279 7465 733f  rn t&&t.asBytes?
-00163b70: 6e3a 7426 2674 2e61 7353 7472 696e 673f  n:t&&t.asString?
-00163b80: 612e 6279 7465 7354 6f53 7472 696e 6728  a.bytesToString(
-00163b90: 6e29 3a72 2e62 7974 6573 546f 4865 7828  n):r.bytesToHex(
-00163ba0: 6e29 7d7d 2c66 756e 6374 696f 6e28 652c  n)}},function(e,
-00163bb0: 7429 7b76 6172 206e 2c72 3b6e 3d22 4142  t){var n,r;n="AB
-00163bc0: 4344 4546 4748 494a 4b4c 4d4e 4f50 5152  CDEFGHIJKLMNOPQR
-00163bd0: 5354 5556 5758 595a 6162 6364 6566 6768  STUVWXYZabcdefgh
-00163be0: 696a 6b6c 6d6e 6f70 7172 7374 7576 7778  ijklmnopqrstuvwx
-00163bf0: 797a 3031 3233 3435 3637 3839 2b2f 222c  yz0123456789+/",
-00163c00: 723d 7b72 6f74 6c3a 6675 6e63 7469 6f6e  r={rotl:function
-00163c10: 2865 2c74 297b 7265 7475 726e 2065 3c3c  (e,t){return e<<
-00163c20: 747c 653e 3e3e 3332 2d74 7d2c 726f 7472  t|e>>>32-t},rotr
-00163c30: 3a66 756e 6374 696f 6e28 652c 7429 7b72  :function(e,t){r
-00163c40: 6574 7572 6e20 653c 3c33 322d 747c 653e  eturn e<<32-t|e>
-00163c50: 3e3e 747d 2c65 6e64 6961 6e3a 6675 6e63  >>t},endian:func
-00163c60: 7469 6f6e 2865 297b 6966 2865 2e63 6f6e  tion(e){if(e.con
-00163c70: 7374 7275 6374 6f72 3d3d 4e75 6d62 6572  structor==Number
-00163c80: 2972 6574 7572 6e20 3136 3731 3139 3335  )return 16711935
-00163c90: 2672 2e72 6f74 6c28 652c 3829 7c34 3237  &r.rotl(e,8)|427
-00163ca0: 3832 3535 3336 3026 722e 726f 746c 2865  8255360&r.rotl(e
-00163cb0: 2c32 3429 3b66 6f72 2876 6172 2074 3d30  ,24);for(var t=0
-00163cc0: 3b74 3c65 2e6c 656e 6774 683b 742b 2b29  ;t<e.length;t++)
-00163cd0: 655b 745d 3d72 2e65 6e64 6961 6e28 655b  e[t]=r.endian(e[
-00163ce0: 745d 293b 7265 7475 726e 2065 7d2c 7261  t]);return e},ra
-00163cf0: 6e64 6f6d 4279 7465 733a 6675 6e63 7469  ndomBytes:functi
-00163d00: 6f6e 2865 297b 666f 7228 7661 7220 743d  on(e){for(var t=
-00163d10: 5b5d 3b65 3e30 3b65 2d2d 2974 2e70 7573  [];e>0;e--)t.pus
-00163d20: 6828 4d61 7468 2e66 6c6f 6f72 2832 3536  h(Math.floor(256
-00163d30: 2a4d 6174 682e 7261 6e64 6f6d 2829 2929  *Math.random()))
-00163d40: 3b72 6574 7572 6e20 747d 2c62 7974 6573  ;return t},bytes
-00163d50: 546f 576f 7264 733a 6675 6e63 7469 6f6e  ToWords:function
-00163d60: 2865 297b 666f 7228 7661 7220 743d 5b5d  (e){for(var t=[]
-00163d70: 2c6e 3d30 2c72 3d30 3b6e 3c65 2e6c 656e  ,n=0,r=0;n<e.len
-00163d80: 6774 683b 6e2b 2b2c 722b 3d38 2974 5b72  gth;n++,r+=8)t[r
-00163d90: 3e3e 3e35 5d7c 3d65 5b6e 5d3c 3c32 342d  >>>5]|=e[n]<<24-
-00163da0: 7225 3332 3b72 6574 7572 6e20 747d 2c77  r%32;return t},w
-00163db0: 6f72 6473 546f 4279 7465 733a 6675 6e63  ordsToBytes:func
-00163dc0: 7469 6f6e 2865 297b 666f 7228 7661 7220  tion(e){for(var 
-00163dd0: 743d 5b5d 2c6e 3d30 3b6e 3c33 322a 652e  t=[],n=0;n<32*e.
-00163de0: 6c65 6e67 7468 3b6e 2b3d 3829 742e 7075  length;n+=8)t.pu
-00163df0: 7368 2865 5b6e 3e3e 3e35 5d3e 3e3e 3234  sh(e[n>>>5]>>>24
-00163e00: 2d6e 2533 3226 3235 3529 3b72 6574 7572  -n%32&255);retur
-00163e10: 6e20 747d 2c62 7974 6573 546f 4865 783a  n t},bytesToHex:
-00163e20: 6675 6e63 7469 6f6e 2865 297b 666f 7228  function(e){for(
-00163e30: 7661 7220 743d 5b5d 2c6e 3d30 3b6e 3c65  var t=[],n=0;n<e
-00163e40: 2e6c 656e 6774 683b 6e2b 2b29 742e 7075  .length;n++)t.pu
-00163e50: 7368 2828 655b 6e5d 3e3e 3e34 292e 746f  sh((e[n]>>>4).to
-00163e60: 5374 7269 6e67 2831 3629 292c 742e 7075  String(16)),t.pu
-00163e70: 7368 2828 3135 2665 5b6e 5d29 2e74 6f53  sh((15&e[n]).toS
-00163e80: 7472 696e 6728 3136 2929 3b72 6574 7572  tring(16));retur
-00163e90: 6e20 742e 6a6f 696e 2822 2229 7d2c 6865  n t.join("")},he
-00163ea0: 7854 6f42 7974 6573 3a66 756e 6374 696f  xToBytes:functio
-00163eb0: 6e28 6529 7b66 6f72 2876 6172 2074 3d5b  n(e){for(var t=[
-00163ec0: 5d2c 6e3d 303b 6e3c 652e 6c65 6e67 7468  ],n=0;n<e.length
-00163ed0: 3b6e 2b3d 3229 742e 7075 7368 2870 6172  ;n+=2)t.push(par
-00163ee0: 7365 496e 7428 652e 7375 6273 7472 286e  seInt(e.substr(n
-00163ef0: 2c32 292c 3136 2929 3b72 6574 7572 6e20  ,2),16));return 
-00163f00: 747d 2c62 7974 6573 546f 4261 7365 3634  t},bytesToBase64
-00163f10: 3a66 756e 6374 696f 6e28 6529 7b66 6f72  :function(e){for
-00163f20: 2876 6172 2074 3d5b 5d2c 723d 303b 723c  (var t=[],r=0;r<
-00163f30: 652e 6c65 6e67 7468 3b72 2b3d 3329 666f  e.length;r+=3)fo
-00163f40: 7228 7661 7220 693d 655b 725d 3c3c 3136  r(var i=e[r]<<16
-00163f50: 7c65 5b72 2b31 5d3c 3c38 7c65 5b72 2b32  |e[r+1]<<8|e[r+2
-00163f60: 5d2c 6f3d 303b 6f3c 343b 6f2b 2b29 382a  ],o=0;o<4;o++)8*
-00163f70: 722b 362a 6f3c 3d38 2a65 2e6c 656e 6774  r+6*o<=8*e.lengt
-00163f80: 683f 742e 7075 7368 286e 2e63 6861 7241  h?t.push(n.charA
-00163f90: 7428 693e 3e3e 362a 2833 2d6f 2926 3633  t(i>>>6*(3-o)&63
-00163fa0: 2929 3a74 2e70 7573 6828 223d 2229 3b72  )):t.push("=");r
-00163fb0: 6574 7572 6e20 742e 6a6f 696e 2822 2229  eturn t.join("")
-00163fc0: 7d2c 6261 7365 3634 546f 4279 7465 733a  },base64ToBytes:
-00163fd0: 6675 6e63 7469 6f6e 2865 297b 653d 652e  function(e){e=e.
-00163fe0: 7265 706c 6163 6528 2f5b 5e41 2d5a 302d  replace(/[^A-Z0-
-00163ff0: 392b 5c2f 5d2f 6769 2c22 2229 3b66 6f72  9+\/]/gi,"");for
-00164000: 2876 6172 2074 3d5b 5d2c 723d 302c 693d  (var t=[],r=0,i=
-00164010: 303b 723c 652e 6c65 6e67 7468 3b69 3d2b  0;r<e.length;i=+
-00164020: 2b72 2534 2930 213d 6926 2674 2e70 7573  +r%4)0!=i&&t.pus
-00164030: 6828 286e 2e69 6e64 6578 4f66 2865 2e63  h((n.indexOf(e.c
-00164040: 6861 7241 7428 722d 3129 2926 4d61 7468  harAt(r-1))&Math
-00164050: 2e70 6f77 2832 2c2d 322a 692b 3829 2d31  .pow(2,-2*i+8)-1
-00164060: 293c 3c32 2a69 7c6e 2e69 6e64 6578 4f66  )<<2*i|n.indexOf
-00164070: 2865 2e63 6861 7241 7428 7229 293e 3e3e  (e.charAt(r))>>>
-00164080: 362d 322a 6929 3b72 6574 7572 6e20 747d  6-2*i);return t}
-00164090: 7d2c 652e 6578 706f 7274 733d 727d 2c66  },e.exports=r},f
-001640a0: 756e 6374 696f 6e28 652c 7429 7b66 756e  unction(e,t){fun
-001640b0: 6374 696f 6e20 6e28 6529 7b72 6574 7572  ction n(e){retur
-001640c0: 6e21 2165 2e63 6f6e 7374 7275 6374 6f72  n!!e.constructor
-001640d0: 2626 2266 756e 6374 696f 6e22 3d3d 7479  &&"function"==ty
-001640e0: 7065 6f66 2065 2e63 6f6e 7374 7275 6374  peof e.construct
-001640f0: 6f72 2e69 7342 7566 6665 7226 2665 2e63  or.isBuffer&&e.c
-00164100: 6f6e 7374 7275 6374 6f72 2e69 7342 7566  onstructor.isBuf
-00164110: 6665 7228 6529 7d0a 2f2a 210a 202a 2044  fer(e)}./*!. * D
-00164120: 6574 6572 6d69 6e65 2069 6620 616e 206f  etermine if an o
-00164130: 626a 6563 7420 6973 2061 2042 7566 6665  bject is a Buffe
-00164140: 720a 202a 0a20 2a20 4061 7574 686f 7220  r. *. * @author 
-00164150: 2020 4665 726f 7373 2041 626f 756b 6861    Feross Aboukha
-00164160: 6469 6a65 6820 3c68 7474 7073 3a2f 2f66  dijeh <https://f
-00164170: 6572 6f73 732e 6f72 673e 0a20 2a20 406c  eross.org>. * @l
-00164180: 6963 656e 7365 2020 4d49 540a 202a 2f0a  icense  MIT. */.
-00164190: 652e 6578 706f 7274 733d 6675 6e63 7469  e.exports=functi
-001641a0: 6f6e 2865 297b 7265 7475 726e 206e 756c  on(e){return nul
-001641b0: 6c21 3d65 2626 286e 2865 297c 7c66 756e  l!=e&&(n(e)||fun
-001641c0: 6374 696f 6e28 6529 7b72 6574 7572 6e22  ction(e){return"
-001641d0: 6675 6e63 7469 6f6e 223d 3d74 7970 656f  function"==typeo
-001641e0: 6620 652e 7265 6164 466c 6f61 744c 4526  f e.readFloatLE&
-001641f0: 2622 6675 6e63 7469 6f6e 223d 3d74 7970  &"function"==typ
-00164200: 656f 6620 652e 736c 6963 6526 266e 2865  eof e.slice&&n(e
-00164210: 2e73 6c69 6365 2830 2c30 2929 7d28 6529  .slice(0,0))}(e)
-00164220: 7c7c 2121 652e 5f69 7342 7566 6665 7229  ||!!e._isBuffer)
-00164230: 7d7d 2c66 756e 6374 696f 6e28 652c 742c  }},function(e,t,
-00164240: 6e29 7b6e 2839 292e 6d6f 6475 6c65 2822  n){n(9).module("
-00164250: 6462 7422 292e 6661 6374 6f72 7928 226c  dbt").factory("l
-00164260: 6f63 6174 696f 6e53 6572 7669 6365 222c  ocationService",
-00164270: 5b22 2473 7461 7465 222c 6675 6e63 7469  ["$state",functi
-00164280: 6f6e 2865 297b 7661 7220 743d 7b7d 3b72  on(e){var t={};r
-00164290: 6574 7572 6e20 742e 7061 7273 6553 7461  eturn t.parseSta
-001642a0: 7465 3d66 756e 6374 696f 6e28 6529 7b72  te=function(e){r
-001642b0: 6574 7572 6e20 6675 6e63 7469 6f6e 2865  eturn function(e
-001642c0: 297b 7265 7475 726e 7b73 656c 6563 7465  ){return{selecte
-001642d0: 643a 7b69 6e63 6c75 6465 3a65 2e67 5f69  d:{include:e.g_i
-001642e0: 7c7c 2222 2c65 7863 6c75 6465 3a65 2e67  ||"",exclude:e.g
-001642f0: 5f65 7c7c 2222 7d2c 7368 6f77 5f67 7261  _e||""},show_gra
-00164300: 7068 3a21 2165 2e67 5f76 7d7d 2865 297d  ph:!!e.g_v}}(e)}
-00164310: 2c74 2e73 6574 5374 6174 653d 6675 6e63  ,t.setState=func
-00164320: 7469 6f6e 2874 297b 7661 7220 6e3d 6675  tion(t){var n=fu
-00164330: 6e63 7469 6f6e 2865 297b 7661 7220 743d  nction(e){var t=
-00164340: 7b67 5f76 3a31 7d3b 7265 7475 726e 2074  {g_v:1};return t
-00164350: 2e67 5f69 3d65 2e69 6e63 6c75 6465 2c74  .g_i=e.include,t
-00164360: 2e67 5f65 3d65 2e65 7863 6c75 6465 2c74  .g_e=e.exclude,t
-00164370: 7d28 7429 2c72 3d65 2e63 7572 7265 6e74  }(t),r=e.current
-00164380: 2e6e 616d 653b 652e 676f 2872 2c6e 297d  .name;e.go(r,n)}
-00164390: 2c74 2e63 6c65 6172 5374 6174 653d 6675  ,t.clearState=fu
-001643a0: 6e63 7469 6f6e 2829 7b76 6172 2074 3d65  nction(){var t=e
-001643b0: 2e63 7572 7265 6e74 2e6e 616d 653b 652e  .current.name;e.
-001643c0: 676f 2874 2c7b 675f 693a 6e75 6c6c 2c67  go(t,{g_i:null,g
-001643d0: 5f65 3a6e 756c 6c2c 675f 763a 6e75 6c6c  _e:null,g_v:null
-001643e0: 7d29 7d2c 747d 5d29 7d2c 6675 6e63 7469  })},t}])},functi
-001643f0: 6f6e 2865 2c74 2c6e 297b 2275 7365 2073  on(e,t,n){"use s
-00164400: 7472 6963 7422 3b63 6f6e 7374 2072 3d6e  trict";const r=n
-00164410: 2839 292c 693d 6e28 3230 3229 3b72 2e6d  (9),i=n(202);r.m
-00164420: 6f64 756c 6528 2264 6274 2229 2e63 6f6e  odule("dbt").con
-00164430: 7472 6f6c 6c65 7228 224f 7665 7276 6965  troller("Overvie
-00164440: 7743 7472 6c22 2c5b 2224 7363 6f70 6522  wCtrl",["$scope"
-00164450: 2c22 2473 7461 7465 222c 2270 726f 6a65  ,"$state","proje
-00164460: 6374 222c 6675 6e63 7469 6f6e 2865 2c74  ct",function(e,t
-00164470: 2c6e 297b 652e 6f76 6572 7669 6577 5f6d  ,n){e.overview_m
-00164480: 643d 2228 6c6f 6164 696e 6729 222c 6e2e  d="(loading)",n.
-00164490: 7265 6164 7928 2866 756e 6374 696f 6e28  ready((function(
-001644a0: 6e29 7b6c 6574 2072 3d74 2e70 6172 616d  n){let r=t.param
-001644b0: 732e 7072 6f6a 6563 745f 6e61 6d65 3f74  s.project_name?t
-001644c0: 2e70 6172 616d 732e 7072 6f6a 6563 745f  .params.project_
-001644d0: 6e61 6d65 3a6e 756c 6c3b 7661 7220 6f3d  name:null;var o=
-001644e0: 6e2e 646f 6373 5b22 646f 632e 6462 742e  n.docs["doc.dbt.
-001644f0: 5f5f 6f76 6572 7669 6577 5f5f 225d 2c61  __overview__"],a
-00164500: 3d69 2e66 696c 7465 7228 6e2e 646f 6373  =i.filter(n.docs
-00164510: 2c7b 6e61 6d65 3a22 5f5f 6f76 6572 7669  ,{name:"__overvi
-00164520: 6577 5f5f 227d 293b 6966 2869 2e65 6163  ew__"});if(i.eac
-00164530: 6828 612c 2866 756e 6374 696f 6e28 6529  h(a,(function(e)
-00164540: 7b22 6462 7422 213d 652e 7061 636b 6167  {"dbt"!=e.packag
-00164550: 655f 6e61 6d65 2626 286f 3d65 297d 2929  e_name&&(o=e)}))
-00164560: 2c6e 756c 6c21 3d3d 7229 7b6f 3d6e 2e64  ,null!==r){o=n.d
-00164570: 6f63 735b 6064 6f63 2e24 7b72 7d2e 5f5f  ocs[`doc.${r}.__
-00164580: 247b 727d 5f5f 605d 7c7c 6f3b 6c65 7420  ${r}__`]||o;let 
-00164590: 653d 692e 6669 6c74 6572 286e 2e64 6f63  e=i.filter(n.doc
-001645a0: 732c 7b6e 616d 653a 605f 5f24 7b72 7d5f  s,{name:`__${r}_
-001645b0: 5f60 7d29 3b69 2e65 6163 6828 652c 653d  _`});i.each(e,e=
-001645c0: 3e7b 652e 7061 636b 6167 655f 6e61 6d65  >{e.package_name
-001645d0: 213d 3d72 2626 286f 3d65 297d 297d 652e  !==r&&(o=e)})}e.
-001645e0: 6f76 6572 7669 6577 5f6d 643d 6f2e 626c  overview_md=o.bl
-001645f0: 6f63 6b5f 636f 6e74 656e 7473 7d29 297d  ock_contents}))}
-00164600: 5d29 7d2c 6675 6e63 7469 6f6e 2865 2c74  ])},function(e,t
-00164610: 2c6e 297b 2275 7365 2073 7472 6963 7422  ,n){"use strict"
-00164620: 3b6e 2839 292e 6d6f 6475 6c65 2822 6462  ;n(9).module("db
-00164630: 7422 292e 636f 6e74 726f 6c6c 6572 2822  t").controller("
-00164640: 536f 7572 6365 4c69 7374 4374 726c 222c  SourceListCtrl",
-00164650: 5b22 2473 636f 7065 222c 2224 7374 6174  ["$scope","$stat
-00164660: 6522 2c22 7072 6f6a 6563 7422 2c66 756e  e","project",fun
-00164670: 6374 696f 6e28 652c 742c 6e29 7b65 2e73  ction(e,t,n){e.s
-00164680: 6f75 7263 653d 742e 7061 7261 6d73 2e73  ource=t.params.s
-00164690: 6f75 7263 652c 652e 6d6f 6465 6c3d 7b7d  ource,e.model={}
-001646a0: 2c65 2e65 7874 7261 5f74 6162 6c65 5f66  ,e.extra_table_f
-001646b0: 6965 6c64 733d 5b5d 2c65 2e68 6173 5f6d  ields=[],e.has_m
-001646c0: 6f72 655f 696e 666f 3d66 756e 6374 696f  ore_info=functio
-001646d0: 6e28 6529 7b72 6574 7572 6e28 652e 6465  n(e){return(e.de
-001646e0: 7363 7269 7074 696f 6e7c 7c22 2229 2e6c  scription||"").l
-001646f0: 656e 6774 687d 2c65 2e74 6f67 676c 655f  ength},e.toggle_
-00164700: 736f 7572 6365 5f65 7870 616e 6465 643d  source_expanded=
-00164710: 6675 6e63 7469 6f6e 2874 297b 652e 6861  function(t){e.ha
-00164720: 735f 6d6f 7265 5f69 6e66 6f28 7429 2626  s_more_info(t)&&
-00164730: 2874 2e65 7870 616e 6465 643d 2174 2e65  (t.expanded=!t.e
-00164740: 7870 616e 6465 6429 7d2c 6e2e 7265 6164  xpanded)},n.read
-00164750: 7928 2866 756e 6374 696f 6e28 7429 7b76  y((function(t){v
-00164760: 6172 206e 3d5f 2e66 696c 7465 7228 742e  ar n=_.filter(t.
-00164770: 6e6f 6465 732c 2866 756e 6374 696f 6e28  nodes,(function(
-00164780: 7429 7b72 6574 7572 6e20 742e 736f 7572  t){return t.sour
-00164790: 6365 5f6e 616d 653d 3d65 2e73 6f75 7263  ce_name==e.sourc
-001647a0: 657d 2929 3b69 6628 3021 3d6e 2e6c 656e  e}));if(0!=n.len
-001647b0: 6774 6829 7b6e 2e73 6f72 7428 2865 2c74  gth){n.sort((e,t
-001647c0: 293d 3e65 2e6e 616d 652e 6c6f 6361 6c65  )=>e.name.locale
-001647d0: 436f 6d70 6172 6528 742e 6e61 6d65 2929  Compare(t.name))
-001647e0: 3b76 6172 2072 3d6e 5b30 5d3b 652e 6d6f  ;var r=n[0];e.mo
-001647f0: 6465 6c3d 7b6e 616d 653a 652e 736f 7572  del={name:e.sour
-00164800: 6365 2c73 6f75 7263 655f 6465 7363 7269  ce,source_descri
-00164810: 7074 696f 6e3a 722e 736f 7572 6365 5f64  ption:r.source_d
-00164820: 6573 6372 6970 7469 6f6e 2c73 6f75 7263  escription,sourc
-00164830: 6573 3a6e 7d3b 7661 7220 693d 5f2e 756e  es:n};var i=_.un
-00164840: 6971 285f 2e6d 6170 286e 2c22 6d65 7461  iq(_.map(n,"meta
-00164850: 6461 7461 2e6f 776e 6572 2229 292c 6f3d  data.owner")),o=
+00160030: 266e 5b74 2e64 6174 612e 7461 7267 6574  &n[t.data.target
+00160040: 5d7c 7c69 5b74 2e64 6174 612e 736f 7572  ]||i[t.data.sour
+00160050: 6365 5d26 2669 5b74 2e64 6174 612e 7461  ce]&&i[t.data.ta
+00160060: 7267 6574 5d7c 7c74 2e64 6174 612e 756e  rget]||t.data.un
+00160070: 6971 7565 5f69 643d 3d65 3f72 2e64 6174  ique_id==e?r.dat
+00160080: 6128 2273 656c 6563 7465 6422 2c31 293a  a("selected",1):
+00160090: 722e 6461 7461 2822 7365 6c65 6374 6564  r.data("selected
+001600a0: 222c 3029 7d29 297d 7d2c 702e 6d61 726b  ",0)}))}},p.mark
+001600b0: 4469 7274 793d 6675 6e63 7469 6f6e 2865  Dirty=function(e
+001600c0: 297b 702e 6d61 726b 416c 6c43 6c65 616e  ){p.markAllClean
+001600d0: 2829 2c72 2e65 6163 6828 652c 2866 756e  (),r.each(e,(fun
+001600e0: 6374 696f 6e28 6529 7b70 2e67 7261 7068  ction(e){p.graph
+001600f0: 5f65 6c65 6d65 6e74 2e24 6964 2865 292e  _element.$id(e).
+00160100: 6164 6443 6c61 7373 2822 6469 7274 7922  addClass("dirty"
+00160110: 297d 2929 7d2c 702e 6d61 726b 416c 6c43  )}))},p.markAllC
+00160120: 6c65 616e 3d66 756e 6374 696f 6e28 297b  lean=function(){
+00160130: 702e 6772 6170 685f 656c 656d 656e 7426  p.graph_element&
+00160140: 2670 2e67 7261 7068 5f65 6c65 6d65 6e74  &p.graph_element
+00160150: 2e65 6c65 6d65 6e74 7328 292e 7265 6d6f  .elements().remo
+00160160: 7665 436c 6173 7328 2264 6972 7479 2229  veClass("dirty")
+00160170: 7d2c 707d 5d29 7d2c 6675 6e63 7469 6f6e  },p}])},function
+00160180: 2865 2c74 2c6e 297b 2275 7365 2073 7472  (e,t,n){"use str
+00160190: 6963 7422 3b6e 2e72 2874 292c 6e2e 6428  ict";n.r(t),n.d(
+001601a0: 742c 2269 7356 616c 6964 436f 6c6f 7222  t,"isValidColor"
+001601b0: 2c28 6675 6e63 7469 6f6e 2829 7b72 6574  ,(function(){ret
+001601c0: 7572 6e20 697d 2929 3b63 6f6e 7374 2072  urn i}));const r
+001601d0: 3d6e 6577 2053 6574 285b 2261 6c69 6365  =new Set(["alice
+001601e0: 626c 7565 222c 2261 6e74 6971 7565 7768  blue","antiquewh
+001601f0: 6974 6522 2c22 6171 7561 222c 2261 7175  ite","aqua","aqu
+00160200: 616d 6172 696e 6522 2c22 617a 7572 6522  amarine","azure"
+00160210: 2c22 6265 6967 6522 2c22 6269 7371 7565  ,"beige","bisque
+00160220: 222c 2262 6c61 636b 222c 2262 6c61 6e63  ","black","blanc
+00160230: 6865 6461 6c6d 6f6e 6422 2c22 626c 7565  hedalmond","blue
+00160240: 222c 2262 6c75 6576 696f 6c65 7422 2c22  ","blueviolet","
+00160250: 6272 6f77 6e22 2c22 6275 726c 7977 6f6f  brown","burlywoo
+00160260: 6422 2c22 6361 6465 7462 6c75 6522 2c22  d","cadetblue","
+00160270: 6368 6172 7472 6575 7365 222c 2263 686f  chartreuse","cho
+00160280: 636f 6c61 7465 222c 2263 6f72 616c 222c  colate","coral",
+00160290: 2263 6f72 6e66 6c6f 7765 7262 6c75 6522  "cornflowerblue"
+001602a0: 2c22 636f 726e 7369 6c6b 222c 2263 7269  ,"cornsilk","cri
+001602b0: 6d73 6f6e 222c 2263 7961 6e22 2c22 6461  mson","cyan","da
+001602c0: 726b 626c 7565 222c 2264 6172 6b63 7961  rkblue","darkcya
+001602d0: 6e22 2c22 6461 726b 676f 6c64 656e 726f  n","darkgoldenro
+001602e0: 6422 2c22 6461 726b 6772 6179 222c 2264  d","darkgray","d
+001602f0: 6172 6b67 7265 656e 222c 2264 6172 6b6b  arkgreen","darkk
+00160300: 6861 6b69 222c 2264 6172 6b6d 6167 656e  haki","darkmagen
+00160310: 7461 222c 2264 6172 6b6f 6c69 7665 6772  ta","darkolivegr
+00160320: 6565 6e22 2c22 6461 726b 6f72 616e 6765  een","darkorange
+00160330: 222c 2264 6172 6b6f 7263 6869 6422 2c22  ","darkorchid","
+00160340: 6461 726b 7265 6422 2c22 6461 726b 7361  darkred","darksa
+00160350: 6c6d 6f6e 222c 2264 6172 6b73 6561 6772  lmon","darkseagr
+00160360: 6565 6e22 2c22 6461 726b 736c 6174 6562  een","darkslateb
+00160370: 6c75 6522 2c22 6461 726b 736c 6174 6567  lue","darkslateg
+00160380: 7261 7922 2c22 6461 726b 7475 7271 756f  ray","darkturquo
+00160390: 6973 6522 2c22 6461 726b 7669 6f6c 6574  ise","darkviolet
+001603a0: 222c 2264 6565 7070 696e 6b22 2c22 6465  ","deeppink","de
+001603b0: 6570 736b 7962 6c75 6522 2c22 6469 6d67  epskyblue","dimg
+001603c0: 7261 7922 2c22 646f 6467 6572 626c 7565  ray","dodgerblue
+001603d0: 222c 2266 6972 6562 7269 636b 222c 2266  ","firebrick","f
+001603e0: 6c6f 7261 6c77 6869 7465 222c 2266 6f72  loralwhite","for
+001603f0: 6573 7467 7265 656e 222c 2266 7563 6873  estgreen","fuchs
+00160400: 6961 222c 2267 686f 7374 7768 6974 6522  ia","ghostwhite"
+00160410: 2c22 676f 6c64 222c 2267 6f6c 6465 6e72  ,"gold","goldenr
+00160420: 6f64 222c 2267 7261 7922 2c22 6772 6565  od","gray","gree
+00160430: 6e22 2c22 6772 6565 6e79 656c 6c6f 7722  n","greenyellow"
+00160440: 2c22 686f 6e65 7964 6577 222c 2268 6f74  ,"honeydew","hot
+00160450: 7069 6e6b 222c 2269 6e64 6961 6e72 6564  pink","indianred
+00160460: 222c 2269 6e64 6967 6f22 2c22 6976 6f72  ","indigo","ivor
+00160470: 7922 2c22 6b68 616b 6922 2c22 6c61 7665  y","khaki","lave
+00160480: 6e64 6572 222c 226c 6176 656e 6465 7262  nder","lavenderb
+00160490: 6c75 7368 222c 226c 6177 6e67 7265 656e  lush","lawngreen
+001604a0: 222c 226c 656d 6f6e 6368 6966 666f 6e22  ","lemonchiffon"
+001604b0: 2c22 6c69 6768 7462 6c75 6522 2c22 6c69  ,"lightblue","li
+001604c0: 6768 7463 6f72 616c 222c 226c 6967 6874  ghtcoral","light
+001604d0: 6379 616e 222c 226c 6967 6874 676f 6c64  cyan","lightgold
+001604e0: 656e 726f 6479 656c 6c6f 7722 2c22 6c69  enrodyellow","li
+001604f0: 6768 7467 7261 7922 2c22 6c69 6768 7467  ghtgray","lightg
+00160500: 7265 656e 222c 226c 6967 6874 7069 6e6b  reen","lightpink
+00160510: 222c 226c 6967 6874 7361 6c6d 6f6e 222c  ","lightsalmon",
+00160520: 226c 6967 6874 7361 6c6d 6f6e 222c 226c  "lightsalmon","l
+00160530: 6967 6874 7365 6167 7265 656e 222c 226c  ightseagreen","l
+00160540: 6967 6874 736b 7962 6c75 6522 2c22 6c69  ightskyblue","li
+00160550: 6768 7473 6c61 7465 6772 6179 222c 226c  ghtslategray","l
+00160560: 6967 6874 7374 6565 6c62 6c75 6522 2c22  ightsteelblue","
+00160570: 6c69 6768 7479 656c 6c6f 7722 2c22 6c69  lightyellow","li
+00160580: 6d65 222c 226c 696d 6567 7265 656e 222c  me","limegreen",
+00160590: 226c 696e 656e 222c 226d 6167 656e 7461  "linen","magenta
+001605a0: 222c 226d 6172 6f6f 6e22 2c22 6d65 6469  ","maroon","medi
+001605b0: 756d 6171 7561 6d61 7269 6e65 222c 226d  umaquamarine","m
+001605c0: 6564 6975 6d62 6c75 6522 2c22 6d65 6469  ediumblue","medi
+001605d0: 756d 6f72 6368 6964 222c 226d 6564 6975  umorchid","mediu
+001605e0: 6d70 7572 706c 6522 2c22 6d65 6469 756d  mpurple","medium
+001605f0: 7365 6167 7265 656e 222c 226d 6564 6975  seagreen","mediu
+00160600: 6d73 6c61 7465 626c 7565 222c 226d 6564  mslateblue","med
+00160610: 6975 6d73 6c61 7465 626c 7565 222c 226d  iumslateblue","m
+00160620: 6564 6975 6d73 7072 696e 6767 7265 656e  ediumspringgreen
+00160630: 222c 226d 6564 6975 6d74 7572 7175 6f69  ","mediumturquoi
+00160640: 7365 222c 226d 6564 6975 6d76 696f 6c65  se","mediumviole
+00160650: 7472 6564 222c 226d 6964 6e69 6768 7462  tred","midnightb
+00160660: 6c75 6522 2c22 6d69 6e74 6372 6561 6d22  lue","mintcream"
+00160670: 2c22 6d69 7374 7972 6f73 6522 2c22 6d6f  ,"mistyrose","mo
+00160680: 6363 6173 696e 222c 226e 6176 616a 6f77  ccasin","navajow
+00160690: 6869 7465 222c 226e 6176 7922 2c22 6f6c  hite","navy","ol
+001606a0: 646c 6163 6522 2c22 6f6c 6976 6522 2c22  dlace","olive","
+001606b0: 6f6c 6976 6564 7261 6222 2c22 6f72 616e  olivedrab","oran
+001606c0: 6765 222c 226f 7261 6e67 6572 6564 222c  ge","orangered",
+001606d0: 226f 7263 6869 6422 2c22 7061 6c65 676f  "orchid","palego
+001606e0: 6c64 656e 726f 6422 2c22 7061 6c65 6772  ldenrod","palegr
+001606f0: 6565 6e22 2c22 7061 6c65 7475 7271 756f  een","paleturquo
+00160700: 6973 6522 2c22 7061 6c65 7669 6f6c 6574  ise","paleviolet
+00160710: 7265 6422 2c22 7061 7061 7961 7768 6970  red","papayawhip
+00160720: 222c 2270 6561 6368 7075 6666 222c 2270  ","peachpuff","p
+00160730: 6572 7522 2c22 7069 6e6b 222c 2270 6c75  eru","pink","plu
+00160740: 6d22 2c22 706f 7764 6572 626c 7565 222c  m","powderblue",
+00160750: 2270 7572 706c 6522 2c22 7265 6265 6363  "purple","rebecc
+00160760: 6170 7572 706c 6522 2c22 7265 6422 2c22  apurple","red","
+00160770: 726f 7379 6272 6f77 6e22 2c22 726f 7961  rosybrown","roya
+00160780: 6c62 6c75 6522 2c22 7361 6464 6c65 6272  lblue","saddlebr
+00160790: 6f77 6e22 2c22 7361 6c6d 6f6e 222c 2273  own","salmon","s
+001607a0: 616e 6479 6272 6f77 6e22 2c22 7365 6167  andybrown","seag
+001607b0: 7265 656e 222c 2273 6561 7368 656c 6c22  reen","seashell"
+001607c0: 2c22 7369 656e 6e61 222c 2273 696c 7665  ,"sienna","silve
+001607d0: 7222 2c22 736b 7962 6c75 6522 2c22 736c  r","skyblue","sl
+001607e0: 6174 6562 6c75 6522 2c22 736c 6174 6567  ateblue","slateg
+001607f0: 7261 7922 2c22 736e 6f77 222c 2273 7072  ray","snow","spr
+00160800: 696e 6767 7265 656e 222c 2273 7465 656c  inggreen","steel
+00160810: 626c 7565 222c 2274 616e 222c 2274 6561  blue","tan","tea
+00160820: 6c22 2c22 7468 6973 746c 6522 2c22 746f  l","thistle","to
+00160830: 6d61 746f 222c 2274 7572 7175 6f69 7365  mato","turquoise
+00160840: 222c 2276 696f 6c65 7422 2c22 7768 6561  ","violet","whea
+00160850: 7422 2c22 7768 6974 6522 2c22 7768 6974  t","white","whit
+00160860: 6573 6d6f 6b65 222c 2279 656c 6c6f 7722  esmoke","yellow"
+00160870: 2c22 7965 6c6c 6f77 6772 6565 6e22 5d29  ,"yellowgreen"])
+00160880: 3b66 756e 6374 696f 6e20 6928 6529 7b69  ;function i(e){i
+00160890: 6628 2165 2972 6574 7572 6e21 313b 636f  f(!e)return!1;co
+001608a0: 6e73 7420 743d 652e 7472 696d 2829 2e74  nst t=e.trim().t
+001608b0: 6f4c 6f77 6572 4361 7365 2829 3b69 6628  oLowerCase();if(
+001608c0: 2222 3d3d 3d74 2972 6574 7572 6e21 313b  ""===t)return!1;
+001608d0: 636f 6e73 7420 6e3d 742e 6d61 7463 6828  const n=t.match(
+001608e0: 2f5e 2328 5b41 2d46 612d 6630 2d39 5d7b  /^#([A-Fa-f0-9]{
+001608f0: 337d 297b 312c 327d 242f 292c 693d 722e  3}){1,2}$/),i=r.
+00160900: 6861 7328 7429 3b72 6574 7572 6e20 426f  has(t);return Bo
+00160910: 6f6c 6561 6e28 6e29 7c7c 697d 7d2c 6675  olean(n)||i}},fu
+00160920: 6e63 7469 6f6e 2865 2c74 2c6e 297b 6e28  nction(e,t,n){n(
+00160930: 3333 293b 636f 6e73 7420 723d 6e28 3231  33);const r=n(21
+00160940: 292c 693d 6e28 3437 3229 3b61 6e67 756c  ),i=n(472);angul
+00160950: 6172 2e6d 6f64 756c 6528 2264 6274 2229  ar.module("dbt")
+00160960: 2e66 6163 746f 7279 2822 7365 6c65 6374  .factory("select
+00160970: 6f72 5365 7276 6963 6522 2c5b 2224 7374  orService",["$st
+00160980: 6174 6522 2c66 756e 6374 696f 6e28 6529  ate",function(e)
+00160990: 7b76 6172 2074 3d7b 696e 636c 7564 653a  {var t={include:
+001609a0: 2222 2c65 7863 6c75 6465 3a22 222c 7061  "",exclude:"",pa
+001609b0: 636b 6167 6573 3a5b 5d2c 7461 6773 3a5b  ckages:[],tags:[
+001609c0: 6e75 6c6c 5d2c 7265 736f 7572 6365 5f74  null],resource_t
+001609d0: 7970 6573 3a5b 226d 6f64 656c 222c 2273  ypes:["model","s
+001609e0: 6565 6422 2c22 736e 6170 7368 6f74 222c  eed","snapshot",
+001609f0: 2273 6f75 7263 6522 2c22 7465 7374 222c  "source","test",
+00160a00: 2275 6e69 745f 7465 7374 222c 2261 6e61  "unit_test","ana
+00160a10: 6c79 7369 7322 2c22 6578 706f 7375 7265  lysis","exposure
+00160a20: 222c 226d 6574 7269 6322 2c22 7365 6d61  ","metric","sema
+00160a30: 6e74 6963 5f6d 6f64 656c 225d 2c64 6570  ntic_model"],dep
+00160a40: 7468 3a31 7d2c 6e3d 7b76 6965 775f 6e6f  th:1},n={view_no
+00160a50: 6465 3a6e 756c 6c2c 7365 6c65 6374 696f  de:null,selectio
+00160a60: 6e3a 7b63 6c65 616e 3a72 2e63 6c6f 6e65  n:{clean:r.clone
+00160a70: 2874 292c 6469 7274 793a 722e 636c 6f6e  (t),dirty:r.clon
+00160a80: 6528 7429 7d2c 6f70 7469 6f6e 733a 7b70  e(t)},options:{p
+00160a90: 6163 6b61 6765 733a 5b5d 2c74 6167 733a  ackages:[],tags:
+00160aa0: 5b6e 756c 6c5d 2c72 6573 6f75 7263 655f  [null],resource_
+00160ab0: 7479 7065 733a 5b22 6d6f 6465 6c22 2c22  types:["model","
+00160ac0: 7365 6564 222c 2273 6e61 7073 686f 7422  seed","snapshot"
+00160ad0: 2c22 736f 7572 6365 222c 2274 6573 7422  ,"source","test"
+00160ae0: 2c22 616e 616c 7973 6973 222c 2265 7870  ,"analysis","exp
+00160af0: 6f73 7572 6522 2c22 6d65 7472 6963 222c  osure","metric",
+00160b00: 2273 656d 616e 7469 635f 6d6f 6465 6c22  "semantic_model"
+00160b10: 2c22 756e 6974 5f74 6573 7422 5d7d 2c69  ,"unit_test"]},i
+00160b20: 6e69 743a 6675 6e63 7469 6f6e 2865 297b  nit:function(e){
+00160b30: 722e 6561 6368 2865 2c28 6675 6e63 7469  r.each(e,(functi
+00160b40: 6f6e 2865 2c72 297b 6e2e 6f70 7469 6f6e  on(e,r){n.option
+00160b50: 735b 725d 3d65 2c74 5b72 5d3d 652c 6e2e  s[r]=e,t[r]=e,n.
+00160b60: 7365 6c65 6374 696f 6e2e 636c 6561 6e5b  selection.clean[
+00160b70: 725d 3d65 2c6e 2e73 656c 6563 7469 6f6e  r]=e,n.selection
+00160b80: 2e64 6972 7479 5b72 5d3d 657d 2929 7d2c  .dirty[r]=e}))},
+00160b90: 7265 7365 7453 656c 6563 7469 6f6e 3a66  resetSelection:f
+00160ba0: 756e 6374 696f 6e28 6529 7b76 6172 2069  unction(e){var i
+00160bb0: 3d7b 696e 636c 7564 653a 6526 2672 2e69  ={include:e&&r.i
+00160bc0: 6e63 6c75 6465 7328 5b22 6d6f 6465 6c22  ncludes(["model"
+00160bd0: 2c22 7365 6564 222c 2273 6e61 7073 686f  ,"seed","snapsho
+00160be0: 7422 5d2c 652e 7265 736f 7572 6365 5f74  t"],e.resource_t
+00160bf0: 7970 6529 3f22 2b22 2b65 2e6e 616d 652b  ype)?"+"+e.name+
+00160c00: 222b 223a 6526 2622 736f 7572 6365 223d  "+":e&&"source"=
+00160c10: 3d65 2e72 6573 6f75 7263 655f 7479 7065  =e.resource_type
+00160c20: 3f22 2b73 6f75 7263 653a 222b 652e 736f  ?"+source:"+e.so
+00160c30: 7572 6365 5f6e 616d 652b 222e 222b 652e  urce_name+"."+e.
+00160c40: 6e61 6d65 2b22 2b22 3a65 2626 2265 7870  name+"+":e&&"exp
+00160c50: 6f73 7572 6522 3d3d 652e 7265 736f 7572  osure"==e.resour
+00160c60: 6365 5f74 7970 653f 222b 6578 706f 7375  ce_type?"+exposu
+00160c70: 7265 3a22 2b65 2e6e 616d 653a 6526 2622  re:"+e.name:e&&"
+00160c80: 6d65 7472 6963 223d 3d65 2e72 6573 6f75  metric"==e.resou
+00160c90: 7263 655f 7479 7065 3f22 2b6d 6574 7269  rce_type?"+metri
+00160ca0: 633a 222b 652e 6e61 6d65 3a65 2626 2273  c:"+e.name:e&&"s
+00160cb0: 656d 616e 7469 635f 6d6f 6465 6c22 3d3d  emantic_model"==
+00160cc0: 652e 7265 736f 7572 6365 5f74 7970 653f  e.resource_type?
+00160cd0: 222b 7365 6d61 6e74 6963 5f6d 6f64 656c  "+semantic_model
+00160ce0: 3a22 2b65 2e6e 616d 653a 6526 2672 2e69  :"+e.name:e&&r.i
+00160cf0: 6e63 6c75 6465 7328 5b22 616e 616c 7973  ncludes(["analys
+00160d00: 6973 222c 2274 6573 7422 2c22 756e 6974  is","test","unit
+00160d10: 5f74 6573 7422 5d2c 652e 7265 736f 7572  _test"],e.resour
+00160d20: 6365 5f74 7970 6529 3f22 2b22 2b65 2e6e  ce_type)?"+"+e.n
+00160d30: 616d 653a 2222 7d2c 6f3d 722e 6173 7369  ame:""},o=r.assi
+00160d40: 676e 287b 7d2c 742c 6929 3b6e 2e73 656c  gn({},t,i);n.sel
+00160d50: 6563 7469 6f6e 2e63 6c65 616e 3d72 2e63  ection.clean=r.c
+00160d60: 6c6f 6e65 286f 292c 6e2e 7365 6c65 6374  lone(o),n.select
+00160d70: 696f 6e2e 6469 7274 793d 722e 636c 6f6e  ion.dirty=r.clon
+00160d80: 6528 6f29 2c6e 2e76 6965 775f 6e6f 6465  e(o),n.view_node
+00160d90: 3d65 7d2c 6765 7456 6965 774e 6f64 653a  =e},getViewNode:
+00160da0: 6675 6e63 7469 6f6e 2829 7b72 6574 7572  function(){retur
+00160db0: 6e20 6e2e 7669 6577 5f6e 6f64 657d 2c65  n n.view_node},e
+00160dc0: 7863 6c75 6465 4e6f 6465 3a66 756e 6374  xcludeNode:funct
+00160dd0: 696f 6e28 652c 7429 7b76 6172 2072 2c69  ion(e,t){var r,i
+00160de0: 3d6e 2e73 656c 6563 7469 6f6e 2e64 6972  =n.selection.dir
+00160df0: 7479 2e65 7863 6c75 6465 2c6f 3d74 2e70  ty.exclude,o=t.p
+00160e00: 6172 656e 7473 3f22 2b22 3a22 222c 613d  arents?"+":"",a=
+00160e10: 742e 6368 696c 6472 656e 3f22 2b22 3a22  t.children?"+":"
+00160e20: 222c 733d 692e 6c65 6e67 7468 3e30 3f22  ",s=i.length>0?"
+00160e30: 2022 3a22 223b 2273 6f75 7263 6522 3d3d   ":"";"source"==
+00160e40: 652e 7265 736f 7572 6365 5f74 7970 653f  e.resource_type?
+00160e50: 286f 2b3d 2273 6f75 7263 653a 222c 723d  (o+="source:",r=
+00160e60: 652e 736f 7572 6365 5f6e 616d 652b 222e  e.source_name+".
+00160e70: 222b 652e 6e61 6d65 293a 5b22 6578 706f  "+e.name):["expo
+00160e80: 7375 7265 222c 226d 6574 7269 6322 2c22  sure","metric","
+00160e90: 7365 6d61 6e74 6963 5f6d 6f64 656c 225d  semantic_model"]
+00160ea0: 2e69 6e64 6578 4f66 2865 2e72 6573 6f75  .indexOf(e.resou
+00160eb0: 7263 655f 7479 7065 293e 2d31 3f28 6f2b  rce_type)>-1?(o+
+00160ec0: 3d65 2e72 6573 6f75 7263 655f 7479 7065  =e.resource_type
+00160ed0: 2b22 3a22 2c72 3d65 2e6e 616d 6529 3a72  +":",r=e.name):r
+00160ee0: 3d65 2e6e 616d 653b 7661 7220 6c3d 692b  =e.name;var l=i+
+00160ef0: 732b 6f2b 722b 613b 7265 7475 726e 206e  s+o+r+a;return n
+00160f00: 2e73 656c 6563 7469 6f6e 2e64 6972 7479  .selection.dirty
+00160f10: 2e65 7863 6c75 6465 3d6c 2c6e 2e75 7064  .exclude=l,n.upd
+00160f20: 6174 6553 656c 6563 7469 6f6e 2829 7d2c  ateSelection()},
+00160f30: 7365 6c65 6374 536f 7572 6365 3a66 756e  selectSource:fun
+00160f40: 6374 696f 6e28 652c 7429 7b76 6172 2072  ction(e,t){var r
+00160f50: 3d22 736f 7572 6365 3a22 2b65 2b28 742e  ="source:"+e+(t.
+00160f60: 6368 696c 6472 656e 3f22 2b22 3a22 2229  children?"+":"")
+00160f70: 3b72 6574 7572 6e20 6e2e 7365 6c65 6374  ;return n.select
+00160f80: 696f 6e2e 6469 7274 792e 696e 636c 7564  ion.dirty.includ
+00160f90: 653d 722c 6e2e 7570 6461 7465 5365 6c65  e=r,n.updateSele
+00160fa0: 6374 696f 6e28 297d 2c63 6c65 6172 5669  ction()},clearVi
+00160fb0: 6577 4e6f 6465 3a66 756e 6374 696f 6e28  ewNode:function(
+00160fc0: 297b 6e2e 7669 6577 5f6e 6f64 653d 6e75  ){n.view_node=nu
+00160fd0: 6c6c 7d2c 6973 4469 7274 793a 6675 6e63  ll},isDirty:func
+00160fe0: 7469 6f6e 2829 7b72 6574 7572 6e21 722e  tion(){return!r.
+00160ff0: 6973 4571 7561 6c28 6e2e 7365 6c65 6374  isEqual(n.select
+00161000: 696f 6e2e 636c 6561 6e2c 6e2e 7365 6c65  ion.clean,n.sele
+00161010: 6374 696f 6e2e 6469 7274 7929 7d2c 7570  ction.dirty)},up
+00161020: 6461 7465 5365 6c65 6374 696f 6e3a 6675  dateSelection:fu
+00161030: 6e63 7469 6f6e 2829 7b72 6574 7572 6e20  nction(){return 
+00161040: 6e2e 7365 6c65 6374 696f 6e2e 636c 6561  n.selection.clea
+00161050: 6e3d 722e 636c 6f6e 6528 6e2e 7365 6c65  n=r.clone(n.sele
+00161060: 6374 696f 6e2e 6469 7274 7929 2c6e 2e73  ction.dirty),n.s
+00161070: 656c 6563 7469 6f6e 2e63 6c65 616e 7d2c  election.clean},
+00161080: 7365 6c65 6374 4e6f 6465 733a 6675 6e63  selectNodes:func
+00161090: 7469 6f6e 2865 2c74 2c6e 297b 7265 7475  tion(e,t,n){retu
+001610a0: 726e 2069 2e73 656c 6563 744e 6f64 6573  rn i.selectNodes
+001610b0: 2865 2c74 2c6e 297d 7d3b 7265 7475 726e  (e,t,n)}};return
+001610c0: 206e 7d5d 297d 2c66 756e 6374 696f 6e28   n}])},function(
+001610d0: 652c 742c 6e29 7b63 6f6e 7374 2072 3d6e  e,t,n){const r=n
+001610e0: 2832 3129 2c69 3d6e 2834 3733 293b 6675  (21),i=n(473);fu
+001610f0: 6e63 7469 6f6e 206f 2865 2c74 297b 7265  nction o(e,t){re
+00161100: 7475 726e 2074 7c7c 2874 3d22 2022 292c  turn t||(t=" "),
+00161110: 722e 6669 6c74 6572 2872 2e75 6e69 7128  r.filter(r.uniq(
+00161120: 652e 7370 6c69 7428 7429 292c 2866 756e  e.split(t)),(fun
+00161130: 6374 696f 6e28 6529 7b72 6574 7572 6e20  ction(e){return 
+00161140: 652e 6c65 6e67 7468 3e30 7d29 297d 6675  e.length>0}))}fu
+00161150: 6e63 7469 6f6e 2061 2865 297b 7661 7220  nction a(e){var 
+00161160: 743d 7b72 6177 3a65 2c73 656c 6563 745f  t={raw:e,select_
+00161170: 6174 3a21 312c 7365 6c65 6374 5f63 6869  at:!1,select_chi
+00161180: 6c64 7265 6e3a 2131 2c63 6869 6c64 7265  ldren:!1,childre
+00161190: 6e5f 6465 7074 683a 6e75 6c6c 2c73 656c  n_depth:null,sel
+001611a0: 6563 745f 7061 7265 6e74 733a 2131 2c70  ect_parents:!1,p
+001611b0: 6172 656e 7473 5f64 6570 7468 3a6e 756c  arents_depth:nul
+001611c0: 6c7d 3b63 6f6e 7374 206e 3d6e 6577 2052  l};const n=new R
+001611d0: 6567 4578 7028 2222 2b2f 5e2f 2e73 6f75  egExp(""+/^/.sou
+001611e0: 7263 652b 2f28 3f3c 6368 696c 6473 5f70  rce+/(?<childs_p
+001611f0: 6172 656e 7473 3e28 5c40 2929 3f2f 2e73  arents>(\@))?/.s
+00161200: 6f75 7263 652b 2f28 3f3c 7061 7265 6e74  ource+/(?<parent
+00161210: 733e 2828 3f3c 7061 7265 6e74 735f 6465  s>((?<parents_de
+00161220: 7074 683e 285c 642a 2929 5c2b 2929 3f2f  pth>(\d*))\+))?/
+00161230: 2e73 6f75 7263 652b 2f28 283f 3c6d 6574  .source+/((?<met
+00161240: 686f 643e 285b 5c77 2e5d 2b29 293a 293f  hod>([\w.]+)):)?
+00161250: 2f2e 736f 7572 6365 2b2f 283f 3c76 616c  /.source+/(?<val
+00161260: 7565 3e28 2e2a 3f29 292f 2e73 6f75 7263  ue>(.*?))/.sourc
+00161270: 652b 2f28 3f3c 6368 696c 6472 656e 3e28  e+/(?<children>(
+00161280: 5c2b 283f 3c63 6869 6c64 7265 6e5f 6465  \+(?<children_de
+00161290: 7074 683e 285c 642a 2929 2929 3f2f 2e73  pth>(\d*))))?/.s
+001612a0: 6f75 7263 652b 2f24 2f2e 736f 7572 6365  ource+/$/.source
+001612b0: 292e 6578 6563 2865 292e 6772 6f75 7073  ).exec(e).groups
+001612c0: 3b74 2e73 656c 6563 745f 6174 3d22 4022  ;t.select_at="@"
+001612d0: 3d3d 6e2e 6368 696c 6473 5f70 6172 656e  ==n.childs_paren
+001612e0: 7473 2c74 2e73 656c 6563 745f 7061 7265  ts,t.select_pare
+001612f0: 6e74 733d 2121 6e2e 7061 7265 6e74 732c  nts=!!n.parents,
+00161300: 742e 7365 6c65 6374 5f63 6869 6c64 7265  t.select_childre
+00161310: 6e3d 2121 6e2e 6368 696c 6472 656e 2c6e  n=!!n.children,n
+00161320: 2e70 6172 656e 7473 5f64 6570 7468 2626  .parents_depth&&
+00161330: 2874 2e70 6172 656e 7473 5f64 6570 7468  (t.parents_depth
+00161340: 3d70 6172 7365 496e 7428 6e2e 7061 7265  =parseInt(n.pare
+00161350: 6e74 735f 6465 7074 6829 292c 6e2e 6368  nts_depth)),n.ch
+00161360: 696c 6472 656e 5f64 6570 7468 2626 2874  ildren_depth&&(t
+00161370: 2e63 6869 6c64 7265 6e5f 6465 7074 683d  .children_depth=
+00161380: 7061 7273 6549 6e74 286e 2e63 6869 6c64  parseInt(n.child
+00161390: 7265 6e5f 6465 7074 6829 293b 7661 7220  ren_depth));var 
+001613a0: 723d 6e2e 6d65 7468 6f64 2c69 3d6e 2e76  r=n.method,i=n.v
+001613b0: 616c 7565 3b72 6574 7572 6e20 723f 2d31  alue;return r?-1
+001613c0: 213d 722e 696e 6465 784f 6628 222e 2229  !=r.indexOf(".")
+001613d0: 2626 285b 722c 7365 6c65 6374 6f72 5f6d  &&([r,selector_m
+001613e0: 6f64 6966 6965 725d 3d72 2e73 706c 6974  odifier]=r.split
+001613f0: 2822 2e22 2c32 292c 693d 7b63 6f6e 6669  (".",2),i={confi
+00161400: 673a 7365 6c65 6374 6f72 5f6d 6f64 6966  g:selector_modif
+00161410: 6965 722c 7661 6c75 653a 697d 293a 723d  ier,value:i}):r=
+00161420: 2269 6d70 6c69 6369 7422 2c74 2e73 656c  "implicit",t.sel
+00161430: 6563 746f 725f 7479 7065 3d72 2c74 2e73  ector_type=r,t.s
+00161440: 656c 6563 746f 725f 7661 6c75 653d 692c  elector_value=i,
+00161450: 747d 6675 6e63 7469 6f6e 2073 2865 297b  t}function s(e){
+00161460: 7661 7220 743d 6f28 652c 2220 2229 3b72  var t=o(e," ");r
+00161470: 6574 7572 6e20 722e 6d61 7028 742c 2866  eturn r.map(t,(f
+00161480: 756e 6374 696f 6e28 6529 7b76 6172 2074  unction(e){var t
+00161490: 3d6f 2865 2c22 2c22 293b 7265 7475 726e  =o(e,",");return
+001614a0: 2074 2e6c 656e 6774 683e 313f 7b6d 6574   t.length>1?{met
+001614b0: 686f 643a 2269 6e74 6572 7365 6374 222c  hod:"intersect",
+001614c0: 7365 6c65 6374 6f72 733a 722e 6d61 7028  selectors:r.map(
+001614d0: 742c 6129 7d3a 7b6d 6574 686f 643a 226e  t,a)}:{method:"n
+001614e0: 6f6e 6522 2c73 656c 6563 746f 7273 3a72  one",selectors:r
+001614f0: 2e6d 6170 285b 655d 2c61 297d 7d29 297d  .map([e],a)}}))}
+00161500: 6675 6e63 7469 6f6e 206c 2865 2c74 297b  function l(e,t){
+00161510: 7661 7220 6e3d 7328 6529 2c69 3d6e 756c  var n=s(e),i=nul
+00161520: 6c2c 6f3d 6e75 6c6c 3b72 6574 7572 6e20  l,o=null;return 
+00161530: 722e 6561 6368 286e 2c28 6675 6e63 7469  r.each(n,(functi
+00161540: 6f6e 2865 297b 7661 7220 6e3d 2269 6e74  on(e){var n="int
+00161550: 6572 7365 6374 223d 3d65 2e6d 6574 686f  ersect"==e.metho
+00161560: 643f 722e 696e 7465 7273 6563 7469 6f6e  d?r.intersection
+00161570: 3a72 2e75 6e69 6f6e 3b72 2e65 6163 6828  :r.union;r.each(
+00161580: 652e 7365 6c65 6374 6f72 732c 2866 756e  e.selectors,(fun
+00161590: 6374 696f 6e28 6529 7b76 6172 2072 3d74  ction(e){var r=t
+001615a0: 2865 293b 6e75 6c6c 3d3d 3d69 3f28 693d  (e);null===i?(i=
+001615b0: 722e 6d61 7463 6865 642c 6f3d 722e 7365  r.matched,o=r.se
+001615c0: 6c65 6374 6564 293a 2869 3d6e 2869 2c72  lected):(i=n(i,r
+001615d0: 2e6d 6174 6368 6564 292c 6f3d 6e28 6f2c  .matched),o=n(o,
+001615e0: 722e 7365 6c65 6374 6564 2929 7d29 297d  r.selected))}))}
+001615f0: 2929 2c7b 6d61 7463 6865 643a 697c 7c5b  )),{matched:i||[
+00161600: 5d2c 7365 6c65 6374 6564 3a6f 7c7c 5b5d  ],selected:o||[]
+00161610: 7d7d 652e 6578 706f 7274 733d 7b73 706c  }}e.exports={spl
+00161620: 6974 5370 6563 733a 6f2c 7061 7273 6553  itSpecs:o,parseS
+00161630: 7065 633a 612c 7061 7273 6553 7065 6373  pec:a,parseSpecs
+00161640: 3a73 2c62 7569 6c64 5370 6563 3a66 756e  :s,buildSpec:fun
+00161650: 6374 696f 6e28 652c 742c 6e29 7b72 6574  ction(e,t,n){ret
+00161660: 7572 6e7b 696e 636c 7564 653a 7328 6529  urn{include:s(e)
+00161670: 2c65 7863 6c75 6465 3a73 2874 292c 686f  ,exclude:s(t),ho
+00161680: 7073 3a6e 7d7d 2c61 7070 6c79 5370 6563  ps:n}},applySpec
+00161690: 3a6c 2c73 656c 6563 744e 6f64 6573 3a66  :l,selectNodes:f
+001616a0: 756e 6374 696f 6e28 652c 742c 6e29 7b6e  unction(e,t,n){n
+001616b0: 2e69 6e63 6c75 6465 2c6e 2e65 7863 6c75  .include,n.exclu
+001616c0: 6465 3b76 6172 206f 2c61 3d72 2e70 6172  de;var o,a=r.par
+001616d0: 7469 616c 2869 2e67 6574 4e6f 6465 7346  tial(i.getNodesF
+001616e0: 726f 6d53 7065 632c 652c 742c 6e2e 686f  romSpec,e,t,n.ho
+001616f0: 7073 293b 722e 7661 6c75 6573 2874 292c  ps);r.values(t),
+00161700: 6f3d 303d 3d6e 2e69 6e63 6c75 6465 2e74  o=0==n.include.t
+00161710: 7269 6d28 292e 6c65 6e67 7468 3f7b 7365  rim().length?{se
+00161720: 6c65 6374 6564 3a65 2e6e 6f64 6573 2829  lected:e.nodes()
+00161730: 2c6d 6174 6368 6564 3a5b 5d7d 3a6c 286e  ,matched:[]}:l(n
+00161740: 2e69 6e63 6c75 6465 2c61 293b 7661 7220  .include,a);var 
+00161750: 733d 6c28 6e2e 6578 636c 7564 652c 6129  s=l(n.exclude,a)
+00161760: 2c63 3d6f 2e73 656c 6563 7465 642c 753d  ,c=o.selected,u=
+00161770: 6f2e 6d61 7463 6865 643b 633d 722e 6469  o.matched;c=r.di
+00161780: 6666 6572 656e 6365 2863 2c73 2e73 656c  fference(c,s.sel
+00161790: 6563 7465 6429 2c75 3d72 2e64 6966 6665  ected),u=r.diffe
+001617a0: 7265 6e63 6528 752c 732e 6d61 7463 6865  rence(u,s.matche
+001617b0: 6429 3b76 6172 2064 3d5b 5d3b 7265 7475  d);var d=[];retu
+001617c0: 726e 2072 2e65 6163 6828 632c 2866 756e  rn r.each(c,(fun
+001617d0: 6374 696f 6e28 6529 7b76 6172 2069 3d74  ction(e){var i=t
+001617e0: 5b65 5d3b 692e 6461 7461 2e74 6167 737c  [e];i.data.tags|
+001617f0: 7c28 692e 6461 7461 2e74 6167 733d 5b5d  |(i.data.tags=[]
+00161800: 293b 7661 7220 6f3d 722e 696e 636c 7564  );var o=r.includ
+00161810: 6573 286e 2e70 6163 6b61 6765 732c 692e  es(n.packages,i.
+00161820: 6461 7461 2e70 6163 6b61 6765 5f6e 616d  data.package_nam
+00161830: 6529 2c61 3d72 2e69 6e74 6572 7365 6374  e),a=r.intersect
+00161840: 696f 6e28 6e2e 7461 6773 2c69 2e64 6174  ion(n.tags,i.dat
+00161850: 612e 7461 6773 292e 6c65 6e67 7468 3e30  a.tags).length>0
+00161860: 2c73 3d72 2e69 6e63 6c75 6465 7328 6e2e  ,s=r.includes(n.
+00161870: 7461 6773 2c6e 756c 6c29 2626 303d 3d69  tags,null)&&0==i
+00161880: 2e64 6174 612e 7461 6773 2e6c 656e 6774  .data.tags.lengt
+00161890: 682c 6c3d 722e 696e 636c 7564 6573 286e  h,l=r.includes(n
+001618a0: 2e72 6573 6f75 7263 655f 7479 7065 732c  .resource_types,
+001618b0: 692e 6461 7461 2e72 6573 6f75 7263 655f  i.data.resource_
+001618c0: 7479 7065 293b 6f26 2628 617c 7c73 2926  type);o&&(a||s)&
+001618d0: 266c 7c7c 642e 7075 7368 2869 2e64 6174  &l||d.push(i.dat
+001618e0: 612e 756e 6971 7565 5f69 6429 7d29 292c  a.unique_id)})),
+001618f0: 7b73 656c 6563 7465 643a 722e 6469 6666  {selected:r.diff
+00161900: 6572 656e 6365 2863 2c64 292c 6d61 7463  erence(c,d),matc
+00161910: 6865 643a 722e 6469 6666 6572 656e 6365  hed:r.difference
+00161920: 2875 2c64 297d 7d7d 7d2c 6675 6e63 7469  (u,d)}}}},functi
+00161930: 6f6e 2865 2c74 2c6e 297b 636f 6e73 7420  on(e,t,n){const 
+00161940: 723d 6e28 3231 292c 693d 6e28 3230 3329  r=n(21),i=n(203)
+00161950: 3b76 6172 206f 3d22 6671 6e22 2c61 3d22  ;var o="fqn",a="
+00161960: 7461 6722 2c73 3d22 736f 7572 6365 222c  tag",s="source",
+00161970: 6c3d 2265 7870 6f73 7572 6522 2c63 3d22  l="exposure",c="
+00161980: 6d65 7472 6963 222c 753d 2273 656d 616e  metric",u="seman
+00161990: 7469 635f 6d6f 6465 6c22 2c64 3d22 6772  tic_model",d="gr
+001619a0: 6f75 7022 2c70 3d22 7061 7468 222c 663d  oup",p="path",f=
+001619b0: 2266 696c 6522 2c68 3d22 7061 636b 6167  "file",h="packag
+001619c0: 6522 2c67 3d22 636f 6e66 6967 222c 6d3d  e",g="config",m=
+001619d0: 2274 6573 745f 6e61 6d65 222c 763d 2274  "test_name",v="t
+001619e0: 6573 745f 7479 7065 222c 623d 7b7d 3b66  est_type",b={};f
+001619f0: 756e 6374 696f 6e20 7928 652c 742c 6e29  unction y(e,t,n)
+00161a00: 7b76 6172 2072 3d65 2e73 6c69 6365 282d  {var r=e.slice(-
+00161a10: 3129 5b30 5d2c 693d 652e 736c 6963 6528  1)[0],i=e.slice(
+00161a20: 2d32 2c2d 3129 5b30 5d3b 6966 2874 3d3d  -2,-1)[0];if(t==
+00161a30: 3d72 2972 6574 7572 6e21 303b 6966 2876  =r)return!0;if(v
+00161a40: 6572 7369 6f6e 5f6f 7074 696f 6e73 3d5b  ersion_options=[
+00161a50: 692c 692b 225f 222b 722c 692b 222e 222b  i,i+"_"+r,i+"."+
+00161a60: 725d 2c6e 2626 7665 7273 696f 6e5f 6f70  r],n&&version_op
+00161a70: 7469 6f6e 732e 696e 636c 7564 6573 2874  tions.includes(t
+00161a80: 2929 7265 7475 726e 2130 3b76 6172 206f  ))return!0;var o
+00161a90: 3d65 2e72 6564 7563 6528 2865 2c74 293d  =e.reduce((e,t)=
+00161aa0: 3e65 2e63 6f6e 6361 7428 742e 7370 6c69  >e.concat(t.spli
+00161ab0: 7428 222e 2229 292c 5b5d 292c 613d 742e  t(".")),[]),a=t.
+00161ac0: 7370 6c69 7428 222e 2229 3b69 6628 6f2e  split(".");if(o.
+00161ad0: 6c65 6e67 7468 3c61 2e6c 656e 6774 6829  length<a.length)
+00161ae0: 7265 7475 726e 2131 3b66 6f72 2876 6172  return!1;for(var
+00161af0: 2073 3d30 3b73 3c61 2e6c 656e 6774 683b   s=0;s<a.length;
+00161b00: 732b 2b29 7b76 6172 206c 3d61 5b73 5d3b  s++){var l=a[s];
+00161b10: 6966 2822 2a22 3d3d 6c29 7265 7475 726e  if("*"==l)return
+00161b20: 2130 3b69 6628 6f5b 735d 213d 6c29 7265  !0;if(o[s]!=l)re
+00161b30: 7475 726e 2131 7d72 6574 7572 6e21 307d  turn!1}return!0}
+00161b40: 6675 6e63 7469 6f6e 2078 2865 2c74 297b  function x(e,t){
+00161b50: 7661 7220 6e3d 5b5d 3b72 6574 7572 6e20  var n=[];return 
+00161b60: 722e 6561 6368 2865 2c28 6675 6e63 7469  r.each(e,(functi
+00161b70: 6f6e 2865 297b 7661 7220 693d 652e 6461  on(e){var i=e.da
+00161b80: 7461 2c6f 3d69 2e66 716e 2c61 3d6e 756c  ta,o=i.fqn,a=nul
+00161b90: 6c21 3d3d 692e 7665 7273 696f 6e3b 6966  l!==i.version;if
+00161ba0: 286f 2626 2273 6f75 7263 6522 213d 692e  (o&&"source"!=i.
+00161bb0: 7265 736f 7572 6365 5f74 7970 6526 2622  resource_type&&"
+00161bc0: 6578 706f 7375 7265 2221 3d69 2e72 6573  exposure"!=i.res
+00161bd0: 6f75 7263 655f 7479 7065 2626 226d 6574  ource_type&&"met
+00161be0: 7269 6322 213d 692e 7265 736f 7572 6365  ric"!=i.resource
+00161bf0: 5f74 7970 6526 2622 7365 6d61 6e74 6963  _type&&"semantic
+00161c00: 5f6d 6f64 656c 2221 3d69 2e72 6573 6f75  _model"!=i.resou
+00161c10: 7263 655f 7479 7065 297b 7661 7220 733d  rce_type){var s=
+00161c20: 722e 7265 7374 286f 293b 2879 286f 2c74  r.rest(o);(y(o,t
+00161c30: 2c61 297c 7c79 2873 2c74 2c61 2929 2626  ,a)||y(s,t,a))&&
+00161c40: 6e2e 7075 7368 2869 297d 7d29 292c 722e  n.push(i)}})),r.
+00161c50: 756e 6971 286e 297d 6675 6e63 7469 6f6e  uniq(n)}function
+00161c60: 2077 2865 2c74 297b 7661 7220 6e3d 5b5d   w(e,t){var n=[]
+00161c70: 2c69 3d74 2e73 706c 6974 2822 2f22 293b  ,i=t.split("/");
+00161c80: 7265 7475 726e 2072 2e65 6163 6828 652c  return r.each(e,
+00161c90: 2866 756e 6374 696f 6e28 6529 7b76 6172  (function(e){var
+00161ca0: 2074 3d28 652e 6461 7461 2e6f 7269 6769   t=(e.data.origi
+00161cb0: 6e61 6c5f 6669 6c65 5f70 6174 687c 7c22  nal_file_path||"
+00161cc0: 2229 2e73 706c 6974 2822 2f22 292c 6f3d  ").split("/"),o=
+00161cd0: 2130 3b72 2e65 6163 6828 692c 2866 756e  !0;r.each(i,(fun
+00161ce0: 6374 696f 6e28 652c 6e29 7b22 2a22 3d3d  ction(e,n){"*"==
+00161cf0: 657c 7c22 223d 3d65 7c7c 6521 3d74 5b6e  e||""==e||e!=t[n
+00161d00: 5d26 2628 6f3d 2131 297d 2929 2c6f 2626  ]&&(o=!1)})),o&&
+00161d10: 6e2e 7075 7368 2865 2e64 6174 6129 7d29  n.push(e.data)})
+00161d20: 292c 6e7d 6675 6e63 7469 6f6e 206b 2865  ),n}function k(e
+00161d30: 2c74 297b 7661 7220 6e3d 5b5d 3b72 6574  ,t){var n=[];ret
+00161d40: 7572 6e20 722e 6561 6368 2865 2c28 6675  urn r.each(e,(fu
+00161d50: 6e63 7469 6f6e 2865 297b 7661 7220 693d  nction(e){var i=
+00161d60: 652e 6461 7461 2e6f 7269 6769 6e61 6c5f  e.data.original_
+00161d70: 6669 6c65 5f70 6174 682e 7370 6c69 7428  file_path.split(
+00161d80: 222f 2229 3b72 2e6c 6173 7428 6929 3d3d  "/");r.last(i)==
+00161d90: 7426 266e 2e70 7573 6828 652e 6461 7461  t&&n.push(e.data
+00161da0: 297d 2929 2c6e 7d66 756e 6374 696f 6e20  )})),n}function 
+00161db0: 4128 652c 7429 7b76 6172 206e 3d5b 5d3b  A(e,t){var n=[];
+00161dc0: 7265 7475 726e 2072 2e65 6163 6828 652c  return r.each(e,
+00161dd0: 2866 756e 6374 696f 6e28 6529 7b76 6172  (function(e){var
+00161de0: 2069 3d65 2e64 6174 612e 7461 6773 3b72   i=e.data.tags;r
+00161df0: 2e69 6e63 6c75 6465 7328 692c 7429 2626  .includes(i,t)&&
+00161e00: 6e2e 7075 7368 2865 2e64 6174 6129 7d29  n.push(e.data)})
+00161e10: 292c 6e7d 6675 6e63 7469 6f6e 2045 2865  ),n}function E(e
+00161e20: 2c74 297b 7661 7220 6e3d 5b5d 3b72 6574  ,t){var n=[];ret
+00161e30: 7572 6e20 722e 6561 6368 2865 2c28 6675  urn r.each(e,(fu
+00161e40: 6e63 7469 6f6e 2865 297b 652e 6461 7461  nction(e){e.data
+00161e50: 2e70 6163 6b61 6765 5f6e 616d 653d 3d74  .package_name==t
+00161e60: 2626 6e2e 7075 7368 2865 2e64 6174 6129  &&n.push(e.data)
+00161e70: 7d29 292c 6e7d 6675 6e63 7469 6f6e 2053  })),n}function S
+00161e80: 2865 2c74 297b 7661 7220 6e3d 5b5d 3b72  (e,t){var n=[];r
+00161e90: 6574 7572 6e20 722e 6561 6368 2865 2c28  eturn r.each(e,(
+00161ea0: 6675 6e63 7469 6f6e 2865 297b 7661 7220  function(e){var 
+00161eb0: 723d 652e 6461 7461 3b72 2e63 6f6e 6669  r=e.data;r.confi
+00161ec0: 6726 2672 2e63 6f6e 6669 675b 742e 636f  g&&r.config[t.co
+00161ed0: 6e66 6967 5d3d 3d74 2e76 616c 7565 2626  nfig]==t.value&&
+00161ee0: 6e2e 7075 7368 2872 297d 2929 2c6e 7d66  n.push(r)})),n}f
+00161ef0: 756e 6374 696f 6e20 2428 652c 7429 7b76  unction $(e,t){v
+00161f00: 6172 206e 3d5b 5d3b 7265 7475 726e 2072  ar n=[];return r
+00161f10: 2e65 6163 6828 652c 2866 756e 6374 696f  .each(e,(functio
+00161f20: 6e28 6529 7b76 6172 2072 3d65 2e64 6174  n(e){var r=e.dat
+00161f30: 613b 722e 7465 7374 5f6d 6574 6164 6174  a;r.test_metadat
+00161f40: 6126 2672 2e74 6573 745f 6d65 7461 6461  a&&r.test_metada
+00161f50: 7461 2e6e 616d 653d 3d74 2626 6e2e 7075  ta.name==t&&n.pu
+00161f60: 7368 2872 297d 2929 2c6e 7d66 756e 6374  sh(r)})),n}funct
+00161f70: 696f 6e20 4328 652c 7429 7b76 6172 206e  ion C(e,t){var n
+00161f80: 3d5b 5d3b 7265 7475 726e 2072 2e65 6163  =[];return r.eac
+00161f90: 6828 652c 2866 756e 6374 696f 6e28 6529  h(e,(function(e)
+00161fa0: 7b76 6172 2072 3d65 2e64 6174 613b 6966  {var r=e.data;if
+00161fb0: 2822 7465 7374 2221 3d72 2e72 6573 6f75  ("test"!=r.resou
+00161fc0: 7263 655f 7479 7065 2972 6574 7572 6e21  rce_type)return!
+00161fd0: 313b 2872 2e68 6173 4f77 6e50 726f 7065  1;(r.hasOwnPrope
+00161fe0: 7274 7928 2274 6573 745f 6d65 7461 6461  rty("test_metada
+00161ff0: 7461 2229 2626 5b22 7363 6865 6d61 222c  ta")&&["schema",
+00162000: 2267 656e 6572 6963 225d 2e69 6e64 6578  "generic"].index
+00162010: 4f66 2874 293e 2d31 7c7c 2172 2e68 6173  Of(t)>-1||!r.has
+00162020: 4f77 6e50 726f 7065 7274 7928 2274 6573  OwnProperty("tes
+00162030: 745f 6d65 7461 6461 7461 2229 2626 5b22  t_metadata")&&["
+00162040: 6461 7461 222c 2273 696e 6775 6c61 7222  data","singular"
+00162050: 5d2e 696e 6465 784f 6628 7429 3e2d 3129  ].indexOf(t)>-1)
+00162060: 2626 6e2e 7075 7368 2872 297d 2929 2c6e  &&n.push(r)})),n
+00162070: 7d66 756e 6374 696f 6e20 5f28 652c 7429  }function _(e,t)
+00162080: 7b76 6172 206e 3d5b 5d3b 7265 7475 726e  {var n=[];return
+00162090: 2072 2e65 6163 6828 652c 2866 756e 6374   r.each(e,(funct
+001620a0: 696f 6e28 6529 7b76 6172 2072 3d65 2e64  ion(e){var r=e.d
+001620b0: 6174 613b 6966 2822 736f 7572 6365 223d  ata;if("source"=
+001620c0: 3d72 2e72 6573 6f75 7263 655f 7479 7065  =r.resource_type
+001620d0: 297b 7661 7220 692c 6f2c 613d 722e 736f  ){var i,o,a=r.so
+001620e0: 7572 6365 5f6e 616d 652c 733d 722e 6e61  urce_name,s=r.na
+001620f0: 6d65 3b2d 3121 3d74 2e69 6e64 6578 4f66  me;-1!=t.indexOf
+00162100: 2822 2e22 293f 5b69 2c6f 5d3d 742e 7370  (".")?[i,o]=t.sp
+00162110: 6c69 7428 222e 222c 3229 3a28 693d 742c  lit(".",2):(i=t,
+00162120: 6f3d 6e75 6c6c 292c 2822 2a22 3d3d 697c  o=null),("*"==i|
+00162130: 7c69 3d3d 6126 2622 2a22 3d3d 3d6f 7c7c  |i==a&&"*"===o||
+00162140: 693d 3d61 2626 6f3d 3d3d 737c 7c69 3d3d  i==a&&o===s||i==
+00162150: 6126 266e 756c 6c3d 3d3d 6f29 2626 6e2e  a&&null===o)&&n.
+00162160: 7075 7368 2865 2e64 6174 6129 7d7d 2929  push(e.data)}}))
+00162170: 2c6e 7d62 5b22 696d 706c 6963 6974 225d  ,n}b["implicit"]
+00162180: 3d66 756e 6374 696f 6e28 652c 7429 7b76  =function(e,t){v
+00162190: 6172 206e 3d78 2865 2c74 292c 693d 7728  ar n=x(e,t),i=w(
+001621a0: 652c 7429 2c6f 3d5b 5d3b 742e 746f 4c6f  e,t),o=[];t.toLo
+001621b0: 7765 7243 6173 6528 292e 656e 6473 5769  werCase().endsWi
+001621c0: 7468 2822 2e73 716c 2229 2626 286f 3d6b  th(".sql")&&(o=k
+001621d0: 2865 2c74 2929 3b76 6172 2061 3d72 2e75  (e,t));var a=r.u
+001621e0: 6e69 7128 5b5d 2e63 6f6e 6361 7428 722e  niq([].concat(r.
+001621f0: 6d61 7028 6e2c 2275 6e69 7175 655f 6964  map(n,"unique_id
+00162200: 2229 2c72 2e6d 6170 2869 2c22 756e 6971  "),r.map(i,"uniq
+00162210: 7565 5f69 6422 292c 722e 6d61 7028 6f2c  ue_id"),r.map(o,
+00162220: 2275 6e69 7175 655f 6964 2229 2929 3b72  "unique_id")));r
+00162230: 6574 7572 6e20 722e 6d61 7028 612c 743d  eturn r.map(a,t=
+00162240: 3e65 5b74 5d2e 6461 7461 297d 2c62 5b6f  >e[t].data)},b[o
+00162250: 5d3d 782c 625b 615d 3d41 2c62 5b73 5d3d  ]=x,b[a]=A,b[s]=
+00162260: 5f2c 625b 6c5d 3d66 756e 6374 696f 6e28  _,b[l]=function(
+00162270: 652c 7429 7b76 6172 206e 3d5b 5d3b 7265  e,t){var n=[];re
+00162280: 7475 726e 2072 2e65 6163 6828 652c 2866  turn r.each(e,(f
+00162290: 756e 6374 696f 6e28 6529 7b76 6172 2072  unction(e){var r
+001622a0: 3d65 2e64 6174 613b 6966 2822 6578 706f  =e.data;if("expo
+001622b0: 7375 7265 223d 3d72 2e72 6573 6f75 7263  sure"==r.resourc
+001622c0: 655f 7479 7065 297b 7661 7220 693d 722e  e_type){var i=r.
+001622d0: 6e61 6d65 3b28 222a 223d 3d74 7c7c 743d  name;("*"==t||t=
+001622e0: 3d69 2926 266e 2e70 7573 6828 652e 6461  =i)&&n.push(e.da
+001622f0: 7461 297d 7d29 292c 6e7d 2c62 5b63 5d3d  ta)}})),n},b[c]=
+00162300: 6675 6e63 7469 6f6e 2865 2c74 297b 7661  function(e,t){va
+00162310: 7220 6e3d 5b5d 3b72 6574 7572 6e20 722e  r n=[];return r.
+00162320: 6561 6368 2865 2c28 6675 6e63 7469 6f6e  each(e,(function
+00162330: 2865 297b 7661 7220 723d 652e 6461 7461  (e){var r=e.data
+00162340: 3b69 6628 226d 6574 7269 6322 3d3d 722e  ;if("metric"==r.
+00162350: 7265 736f 7572 6365 5f74 7970 6529 7b76  resource_type){v
+00162360: 6172 2069 3d72 2e6e 616d 653b 2822 2a22  ar i=r.name;("*"
+00162370: 3d3d 747c 7c74 3d3d 6929 2626 6e2e 7075  ==t||t==i)&&n.pu
+00162380: 7368 2865 2e64 6174 6129 7d7d 2929 2c6e  sh(e.data)}})),n
+00162390: 7d2c 625b 755d 3d66 756e 6374 696f 6e28  },b[u]=function(
+001623a0: 652c 7429 7b76 6172 206e 3d5b 5d3b 7265  e,t){var n=[];re
+001623b0: 7475 726e 2072 2e65 6163 6828 652c 2866  turn r.each(e,(f
+001623c0: 756e 6374 696f 6e28 6529 7b76 6172 2072  unction(e){var r
+001623d0: 3d65 2e64 6174 613b 6966 2822 7365 6d61  =e.data;if("sema
+001623e0: 6e74 6963 5f6d 6f64 656c 223d 3d72 2e72  ntic_model"==r.r
+001623f0: 6573 6f75 7263 655f 7479 7065 297b 7661  esource_type){va
+00162400: 7220 693d 722e 6e61 6d65 3b28 222a 223d  r i=r.name;("*"=
+00162410: 3d74 7c7c 743d 3d69 2926 266e 2e70 7573  =t||t==i)&&n.pus
+00162420: 6828 652e 6461 7461 297d 7d29 292c 6e7d  h(e.data)}})),n}
+00162430: 2c62 5b64 5d3d 6675 6e63 7469 6f6e 2865  ,b[d]=function(e
+00162440: 2c74 297b 7661 7220 6e3d 5b5d 3b72 6574  ,t){var n=[];ret
+00162450: 7572 6e20 722e 6561 6368 2865 2c28 6675  urn r.each(e,(fu
+00162460: 6e63 7469 6f6e 2865 297b 7661 7220 723d  nction(e){var r=
+00162470: 652e 6461 7461 3b72 2e67 726f 7570 3d3d  e.data;r.group==
+00162480: 7426 266e 2e70 7573 6828 7229 7d29 292c  t&&n.push(r)})),
+00162490: 6e7d 2c62 5b70 5d3d 772c 625b 665d 3d6b  n},b[p]=w,b[f]=k
+001624a0: 2c62 5b68 5d3d 452c 625b 675d 3d53 2c62  ,b[h]=E,b[g]=S,b
+001624b0: 5b6d 5d3d 242c 625b 765d 3d43 2c65 2e65  [m]=$,b[v]=C,e.e
+001624c0: 7870 6f72 7473 3d7b 6973 4651 4e4d 6174  xports={isFQNMat
+001624d0: 6368 3a79 2c67 6574 4e6f 6465 7342 7946  ch:y,getNodesByF
+001624e0: 514e 3a78 2c67 6574 4e6f 6465 7342 7954  QN:x,getNodesByT
+001624f0: 6167 3a41 2c67 6574 4e6f 6465 7342 7953  ag:A,getNodesByS
+00162500: 6f75 7263 653a 5f2c 6765 744e 6f64 6573  ource:_,getNodes
+00162510: 4279 5061 7468 3a77 2c67 6574 4e6f 6465  ByPath:w,getNode
+00162520: 7342 7950 6163 6b61 6765 3a45 2c67 6574  sByPackage:E,get
+00162530: 4e6f 6465 7342 7943 6f6e 6669 673a 532c  NodesByConfig:S,
+00162540: 6765 744e 6f64 6573 4279 5465 7374 4e61  getNodesByTestNa
+00162550: 6d65 3a24 2c67 6574 4e6f 6465 7342 7954  me:$,getNodesByT
+00162560: 6573 7454 7970 653a 432c 6765 744e 6f64  estType:C,getNod
+00162570: 6573 4672 6f6d 5370 6563 3a66 756e 6374  esFromSpec:funct
+00162580: 696f 6e28 652c 742c 6e2c 6f29 7b63 6f6e  ion(e,t,n,o){con
+00162590: 7374 2061 3d62 5b6f 2e73 656c 6563 746f  st a=b[o.selecto
+001625a0: 725f 7479 7065 5d3b 6966 2821 6129 7265  r_type];if(!a)re
+001625b0: 7475 726e 7b73 656c 6563 7465 643a 5b5d  turn{selected:[]
+001625c0: 2c6d 6174 6368 6564 3a5b 5d7d 3b76 6172  ,matched:[]};var
+001625d0: 2073 3d61 2874 2c6f 2e73 656c 6563 746f   s=a(t,o.selecto
+001625e0: 725f 7661 6c75 6529 2c6c 3d5b 5d2c 633d  r_value),l=[],c=
+001625f0: 5b5d 3b72 6574 7572 6e20 722e 6561 6368  [];return r.each
+00162600: 2873 2c28 6675 6e63 7469 6f6e 2874 297b  (s,(function(t){
+00162610: 7661 7220 613d 742e 756e 6971 7565 5f69  var a=t.unique_i
+00162620: 643b 632e 7075 7368 2874 2e75 6e69 7175  d;c.push(t.uniqu
+00162630: 655f 6964 293b 7661 7220 733d 5b5d 2c75  e_id);var s=[],u
+00162640: 3d5b 5d2c 643d 5b5d 3b69 6628 6f2e 7365  =[],d=[];if(o.se
+00162650: 6c65 6374 5f61 7426 2628 643d 722e 756e  lect_at&&(d=r.un
+00162660: 696f 6e28 692e 7365 6c65 6374 4174 2865  ion(i.selectAt(e
+00162670: 2c61 2929 292c 6f2e 7365 6c65 6374 5f70  ,a))),o.select_p
+00162680: 6172 656e 7473 297b 7661 7220 703d 6e7c  arents){var p=n|
+00162690: 7c6f 2e70 6172 656e 7473 5f64 6570 7468  |o.parents_depth
+001626a0: 3b73 3d69 2e61 6e63 6573 746f 724e 6f64  ;s=i.ancestorNod
+001626b0: 6573 2865 2c61 2c70 297d 6966 286f 2e73  es(e,a,p)}if(o.s
+001626c0: 656c 6563 745f 6368 696c 6472 656e 297b  elect_children){
+001626d0: 703d 6e7c 7c6f 2e63 6869 6c64 7265 6e5f  p=n||o.children_
+001626e0: 6465 7074 683b 753d 692e 6465 7363 656e  depth;u=i.descen
+001626f0: 6465 6e74 4e6f 6465 7328 652c 612c 7029  dentNodes(e,a,p)
+00162700: 7d6c 3d72 2e75 6e69 6f6e 285b 615d 2c6c  }l=r.union([a],l
+00162710: 2c75 2c73 2c64 297d 2929 2c7b 7365 6c65  ,u,s,d)})),{sele
+00162720: 6374 6564 3a6c 2c6d 6174 6368 6564 3a63  cted:l,matched:c
+00162730: 7d7d 7d7d 2c66 756e 6374 696f 6e28 652c  }}}},function(e,
+00162740: 742c 6e29 7b63 6f6e 7374 2072 3d6e 2839  t,n){const r=n(9
+00162750: 293b 6e28 3437 3529 3b72 2e6d 6f64 756c  );n(475);r.modul
+00162760: 6528 2264 6274 2229 2e66 6163 746f 7279  e("dbt").factory
+00162770: 2822 7472 6163 6b69 6e67 5365 7276 6963  ("trackingServic
+00162780: 6522 2c5b 2224 6c6f 6361 7469 6f6e 222c  e",["$location",
+00162790: 2273 656c 6563 746f 7253 6572 7669 6365  "selectorService
+001627a0: 222c 2224 726f 6f74 5363 6f70 6522 2c66  ","$rootScope",f
+001627b0: 756e 6374 696f 6e28 652c 742c 6e29 7b76  unction(e,t,n){v
+001627c0: 6172 2072 3d7b 696e 6974 6961 6c69 7a65  ar r={initialize
+001627d0: 643a 2131 2c73 6e6f 7770 6c6f 773a 6e75  d:!1,snowplow:nu
+001627e0: 6c6c 2c70 726f 6a65 6374 5f69 643a 6e75  ll,project_id:nu
+001627f0: 6c6c 2c69 6e69 743a 6675 6e63 7469 6f6e  ll,init:function
+00162800: 2865 297b 722e 696e 6974 6961 6c69 7a65  (e){r.initialize
+00162810: 647c 7c28 722e 696e 6974 6961 6c69 7a65  d||(r.initialize
+00162820: 643d 2130 2c72 2e70 726f 6a65 6374 5f69  d=!0,r.project_i
+00162830: 643d 652e 7072 6f6a 6563 745f 6964 2c21  d=e.project_id,!
+00162840: 303d 3d3d 652e 7472 6163 6b26 2672 2e74  0===e.track&&r.t
+00162850: 7572 6e5f 6f6e 5f74 7261 636b 696e 6728  urn_on_tracking(
+00162860: 2929 7d2c 6973 486f 7374 6564 3a66 756e  ))},isHosted:fun
+00162870: 6374 696f 6e28 297b 7265 7475 726e 2068  ction(){return h
+00162880: 6f73 7465 6467 6574 6462 743d 7769 6e64  ostedgetdbt=wind
+00162890: 6f77 2e6c 6f63 6174 696f 6e2e 686f 7374  ow.location.host
+001628a0: 6e61 6d65 2e69 6e64 6578 4f66 2822 2e67  name.indexOf(".g
+001628b0: 6574 6462 742e 636f 6d22 293e 2d31 2c68  etdbt.com")>-1,h
+001628c0: 6f73 7465 6464 6274 3d77 696e 646f 772e  osteddbt=window.
+001628d0: 6c6f 6361 7469 6f6e 2e68 6f73 746e 616d  location.hostnam
+001628e0: 652e 696e 6465 784f 6628 222e 6462 742e  e.indexOf(".dbt.
+001628f0: 636f 6d22 293e 2d31 2c68 6f73 7465 6467  com")>-1,hostedg
+00162900: 6574 6462 747c 7c68 6f73 7465 6464 6274  etdbt||hosteddbt
+00162910: 7d2c 7475 726e 5f6f 6e5f 7472 6163 6b69  },turn_on_tracki
+00162920: 6e67 3a66 756e 6374 696f 6e28 297b 7661  ng:function(){va
+00162930: 7220 652c 742c 6e2c 692c 6f2c 613b 653d  r e,t,n,i,o,a;e=
+00162940: 7769 6e64 6f77 2c74 3d64 6f63 756d 656e  window,t=documen
+00162950: 742c 6e3d 2273 6372 6970 7422 2c65 5b69  t,n="script",e[i
+00162960: 3d22 736e 6f77 706c 6f77 225d 7c7c 2865  ="snowplow"]||(e
+00162970: 2e47 6c6f 6261 6c53 6e6f 7770 6c6f 774e  .GlobalSnowplowN
+00162980: 616d 6573 7061 6365 3d65 2e47 6c6f 6261  amespace=e.Globa
+00162990: 6c53 6e6f 7770 6c6f 774e 616d 6573 7061  lSnowplowNamespa
+001629a0: 6365 7c7c 5b5d 2c65 2e47 6c6f 6261 6c53  ce||[],e.GlobalS
+001629b0: 6e6f 7770 6c6f 774e 616d 6573 7061 6365  nowplowNamespace
+001629c0: 2e70 7573 6828 6929 2c65 5b69 5d3d 6675  .push(i),e[i]=fu
+001629d0: 6e63 7469 6f6e 2829 7b28 655b 695d 2e71  nction(){(e[i].q
+001629e0: 3d65 5b69 5d2e 717c 7c5b 5d29 2e70 7573  =e[i].q||[]).pus
+001629f0: 6828 6172 6775 6d65 6e74 7329 7d2c 655b  h(arguments)},e[
+00162a00: 695d 2e71 3d65 5b69 5d2e 717c 7c5b 5d2c  i].q=e[i].q||[],
+00162a10: 6f3d 742e 6372 6561 7465 456c 656d 656e  o=t.createElemen
+00162a20: 7428 6e29 2c61 3d74 2e67 6574 456c 656d  t(n),a=t.getElem
+00162a30: 656e 7473 4279 5461 674e 616d 6528 6e29  entsByTagName(n)
+00162a40: 5b30 5d2c 6f2e 6173 796e 633d 312c 6f2e  [0],o.async=1,o.
+00162a50: 7372 633d 222f 2f64 3166 6338 7776 387a  src="//d1fc8wv8z
+00162a60: 6167 3563 612e 636c 6f75 6466 726f 6e74  ag5ca.cloudfront
+00162a70: 2e6e 6574 2f32 2e39 2e30 2f73 702e 6a73  .net/2.9.0/sp.js
+00162a80: 222c 612e 7061 7265 6e74 4e6f 6465 2e69  ",a.parentNode.i
+00162a90: 6e73 6572 7442 6566 6f72 6528 6f2c 6129  nsertBefore(o,a)
+00162aa0: 293b 7661 7220 733d 7b61 7070 4964 3a22  );var s={appId:"
+00162ab0: 6462 742d 646f 6373 222c 666f 7263 6553  dbt-docs",forceS
+00162ac0: 6563 7572 6554 7261 636b 6572 3a21 302c  ecureTracker:!0,
+00162ad0: 7265 7370 6563 7444 6f4e 6f74 5472 6163  respectDoNotTrac
+00162ae0: 6b3a 2130 2c75 7365 7246 696e 6765 7270  k:!0,userFingerp
+00162af0: 7269 6e74 3a21 312c 636f 6e74 6578 7473  rint:!1,contexts
+00162b00: 3a7b 7765 6250 6167 653a 2130 7d7d 3b72  :{webPage:!0}};r
+00162b10: 2e69 7348 6f73 7465 6428 2926 2628 7769  .isHosted()&&(wi
+00162b20: 6e64 6f77 2e6c 6f63 6174 696f 6e2e 686f  ndow.location.ho
+00162b30: 7374 6e61 6d65 2e69 6e64 6578 4f66 2822  stname.indexOf("
+00162b40: 2e67 6574 6462 742e 636f 6d22 293e 2d31  .getdbt.com")>-1
+00162b50: 3f73 2e63 6f6f 6b69 6544 6f6d 6169 6e3d  ?s.cookieDomain=
+00162b60: 222e 6765 7464 6274 2e63 6f6d 223a 732e  ".getdbt.com":s.
+00162b70: 636f 6f6b 6965 446f 6d61 696e 3d22 2e64  cookieDomain=".d
+00162b80: 6274 2e63 6f6d 2229 2c72 2e73 6e6f 7770  bt.com"),r.snowp
+00162b90: 6c6f 773d 7769 6e64 6f77 2e73 6e6f 7770  low=window.snowp
+00162ba0: 6c6f 772c 722e 736e 6f77 706c 6f77 2822  low,r.snowplow("
+00162bb0: 6e65 7754 7261 636b 6572 222c 2273 7022  newTracker","sp"
+00162bc0: 2c22 6669 7368 746f 776e 616e 616c 7974  ,"fishtownanalyt
+00162bd0: 6963 732e 7369 6e74 6572 2d63 6f6c 6c65  ics.sinter-colle
+00162be0: 6374 2e63 6f6d 222c 7329 2c72 2e73 6e6f  ct.com",s),r.sno
+00162bf0: 7770 6c6f 7728 2265 6e61 626c 6541 6374  wplow("enableAct
+00162c00: 6976 6974 7954 7261 636b 696e 6722 2c33  ivityTracking",3
+00162c10: 302c 3330 292c 722e 7472 6163 6b5f 7061  0,30),r.track_pa
+00162c20: 6765 7669 6577 2829 7d2c 6675 7a7a 5572  geview()},fuzzUr
+00162c30: 6c73 3a66 756e 6374 696f 6e28 297b 722e  ls:function(){r.
+00162c40: 6973 486f 7374 6564 2829 7c7c 2872 2e73  isHosted()||(r.s
+00162c50: 6e6f 7770 6c6f 7728 2273 6574 4375 7374  nowplow("setCust
+00162c60: 6f6d 5572 6c22 2c22 6874 7470 733a 2f2f  omUrl","https://
+00162c70: 6675 7a7a 6564 2e67 6574 6462 742e 636f  fuzzed.getdbt.co
+00162c80: 6d2f 2229 2c72 2e73 6e6f 7770 6c6f 7728  m/"),r.snowplow(
+00162c90: 2273 6574 5265 6665 7272 6572 5572 6c22  "setReferrerUrl"
+00162ca0: 2c22 6874 7470 733a 2f2f 6675 7a7a 6564  ,"https://fuzzed
+00162cb0: 2e67 6574 6462 742e 636f 6d2f 2229 297d  .getdbt.com/"))}
+00162cc0: 2c67 6574 436f 6e74 6578 743a 6675 6e63  ,getContext:func
+00162cd0: 7469 6f6e 2829 7b72 6574 7572 6e5b 7b73  tion(){return[{s
+00162ce0: 6368 656d 613a 2269 676c 753a 636f 6d2e  chema:"iglu:com.
+00162cf0: 6462 742f 6462 745f 646f 6373 2f6a 736f  dbt/dbt_docs/jso
+00162d00: 6e73 6368 656d 612f 312d 302d 3022 2c64  nschema/1-0-0",d
+00162d10: 6174 613a 7b69 735f 636c 6f75 645f 686f  ata:{is_cloud_ho
+00162d20: 7374 6564 3a72 2e69 7348 6f73 7465 6428  sted:r.isHosted(
+00162d30: 292c 636f 7265 5f70 726f 6a65 6374 5f69  ),core_project_i
+00162d40: 643a 722e 7072 6f6a 6563 745f 6964 7d7d  d:r.project_id}}
+00162d50: 5d7d 2c74 7261 636b 5f70 6167 6576 6965  ]},track_pagevie
+00162d60: 773a 6675 6e63 7469 6f6e 2829 7b69 6628  w:function(){if(
+00162d70: 722e 736e 6f77 706c 6f77 297b 722e 6675  r.snowplow){r.fu
+00162d80: 7a7a 5572 6c73 2829 3b72 2e73 6e6f 7770  zzUrls();r.snowp
+00162d90: 6c6f 7728 2274 7261 636b 5061 6765 5669  low("trackPageVi
+00162da0: 6577 222c 6e75 6c6c 2c72 2e67 6574 436f  ew",null,r.getCo
+00162db0: 6e74 6578 7428 2929 7d7d 2c74 7261 636b  ntext())}},track
+00162dc0: 5f65 7665 6e74 3a66 756e 6374 696f 6e28  _event:function(
+00162dd0: 652c 742c 6e2c 6929 7b72 2e73 6e6f 7770  e,t,n,i){r.snowp
+00162de0: 6c6f 7726 2628 722e 6675 7a7a 5572 6c73  low&&(r.fuzzUrls
+00162df0: 2829 2c72 2e73 6e6f 7770 6c6f 7728 2274  (),r.snowplow("t
+00162e00: 7261 636b 5374 7275 6374 4576 656e 7422  rackStructEvent"
+00162e10: 2c22 6462 742d 646f 6373 222c 652c 742c  ,"dbt-docs",e,t,
+00162e20: 6e2c 692c 722e 6765 7443 6f6e 7465 7874  n,i,r.getContext
+00162e30: 2829 2929 7d2c 7472 6163 6b5f 6772 6170  ()))},track_grap
+00162e40: 685f 696e 7465 7261 6374 696f 6e3a 6675  h_interaction:fu
+00162e50: 6e63 7469 6f6e 2865 2c74 297b 722e 736e  nction(e,t){r.sn
+00162e60: 6f77 706c 6f77 2626 2872 2e66 757a 7a55  owplow&&(r.fuzzU
+00162e70: 726c 7328 292c 722e 7472 6163 6b5f 6576  rls(),r.track_ev
+00162e80: 656e 7428 2267 7261 7068 222c 2269 6e74  ent("graph","int
+00162e90: 6572 6163 7422 2c65 2c74 2929 7d7d 3b72  eract",e,t))}};r
+00162ea0: 6574 7572 6e20 727d 5d29 7d2c 6675 6e63  eturn r}])},func
+00162eb0: 7469 6f6e 2865 2c74 2c6e 297b 7661 7220  tion(e,t,n){var 
+00162ec0: 722c 692c 6f2c 612c 733b 723d 6e28 3437  r,i,o,a,s;r=n(47
+00162ed0: 3629 2c69 3d6e 2832 3034 292e 7574 6638  6),i=n(204).utf8
+00162ee0: 2c6f 3d6e 2834 3737 292c 613d 6e28 3230  ,o=n(477),a=n(20
+00162ef0: 3429 2e62 696e 2c28 733d 6675 6e63 7469  4).bin,(s=functi
+00162f00: 6f6e 2865 2c74 297b 652e 636f 6e73 7472  on(e,t){e.constr
+00162f10: 7563 746f 723d 3d53 7472 696e 673f 653d  uctor==String?e=
+00162f20: 7426 2622 6269 6e61 7279 223d 3d3d 742e  t&&"binary"===t.
+00162f30: 656e 636f 6469 6e67 3f61 2e73 7472 696e  encoding?a.strin
+00162f40: 6754 6f42 7974 6573 2865 293a 692e 7374  gToBytes(e):i.st
+00162f50: 7269 6e67 546f 4279 7465 7328 6529 3a6f  ringToBytes(e):o
+00162f60: 2865 293f 653d 4172 7261 792e 7072 6f74  (e)?e=Array.prot
+00162f70: 6f74 7970 652e 736c 6963 652e 6361 6c6c  otype.slice.call
+00162f80: 2865 2c30 293a 4172 7261 792e 6973 4172  (e,0):Array.isAr
+00162f90: 7261 7928 6529 7c7c 652e 636f 6e73 7472  ray(e)||e.constr
+00162fa0: 7563 746f 723d 3d3d 5569 6e74 3841 7272  uctor===Uint8Arr
+00162fb0: 6179 7c7c 2865 3d65 2e74 6f53 7472 696e  ay||(e=e.toStrin
+00162fc0: 6728 2929 3b66 6f72 2876 6172 206e 3d72  g());for(var n=r
+00162fd0: 2e62 7974 6573 546f 576f 7264 7328 6529  .bytesToWords(e)
+00162fe0: 2c6c 3d38 2a65 2e6c 656e 6774 682c 633d  ,l=8*e.length,c=
+00162ff0: 3137 3332 3538 3431 3933 2c75 3d2d 3237  1732584193,u=-27
+00163000: 3137 3333 3837 392c 643d 2d31 3733 3235  1733879,d=-17325
+00163010: 3834 3139 342c 703d 3237 3137 3333 3837  84194,p=27173387
+00163020: 382c 663d 303b 663c 6e2e 6c65 6e67 7468  8,f=0;f<n.length
+00163030: 3b66 2b2b 296e 5b66 5d3d 3136 3731 3139  ;f++)n[f]=167119
+00163040: 3335 2628 6e5b 665d 3c3c 387c 6e5b 665d  35&(n[f]<<8|n[f]
+00163050: 3e3e 3e32 3429 7c34 3237 3832 3535 3336  >>>24)|427825536
+00163060: 3026 286e 5b66 5d3c 3c32 347c 6e5b 665d  0&(n[f]<<24|n[f]
+00163070: 3e3e 3e38 293b 6e5b 6c3e 3e3e 355d 7c3d  >>>8);n[l>>>5]|=
+00163080: 3132 383c 3c6c 2533 322c 6e5b 3134 2b28  128<<l%32,n[14+(
+00163090: 6c2b 3634 3e3e 3e39 3c3c 3429 5d3d 6c3b  l+64>>>9<<4)]=l;
+001630a0: 7661 7220 683d 732e 5f66 662c 673d 732e  var h=s._ff,g=s.
+001630b0: 5f67 672c 6d3d 732e 5f68 682c 763d 732e  _gg,m=s._hh,v=s.
+001630c0: 5f69 693b 666f 7228 663d 303b 663c 6e2e  _ii;for(f=0;f<n.
+001630d0: 6c65 6e67 7468 3b66 2b3d 3136 297b 7661  length;f+=16){va
+001630e0: 7220 623d 632c 793d 752c 783d 642c 773d  r b=c,y=u,x=d,w=
+001630f0: 703b 633d 6828 632c 752c 642c 702c 6e5b  p;c=h(c,u,d,p,n[
+00163100: 662b 305d 2c37 2c2d 3638 3038 3736 3933  f+0],7,-68087693
+00163110: 3629 2c70 3d68 2870 2c63 2c75 2c64 2c6e  6),p=h(p,c,u,d,n
+00163120: 5b66 2b31 5d2c 3132 2c2d 3338 3935 3634  [f+1],12,-389564
+00163130: 3538 3629 2c64 3d68 2864 2c70 2c63 2c75  586),d=h(d,p,c,u
+00163140: 2c6e 5b66 2b32 5d2c 3137 2c36 3036 3130  ,n[f+2],17,60610
+00163150: 3538 3139 292c 753d 6828 752c 642c 702c  5819),u=h(u,d,p,
+00163160: 632c 6e5b 662b 335d 2c32 322c 2d31 3034  c,n[f+3],22,-104
+00163170: 3435 3235 3333 3029 2c63 3d68 2863 2c75  4525330),c=h(c,u
+00163180: 2c64 2c70 2c6e 5b66 2b34 5d2c 372c 2d31  ,d,p,n[f+4],7,-1
+00163190: 3736 3431 3838 3937 292c 703d 6828 702c  76418897),p=h(p,
+001631a0: 632c 752c 642c 6e5b 662b 355d 2c31 322c  c,u,d,n[f+5],12,
+001631b0: 3132 3030 3038 3034 3236 292c 643d 6828  1200080426),d=h(
+001631c0: 642c 702c 632c 752c 6e5b 662b 365d 2c31  d,p,c,u,n[f+6],1
+001631d0: 372c 2d31 3437 3332 3331 3334 3129 2c75  7,-1473231341),u
+001631e0: 3d68 2875 2c64 2c70 2c63 2c6e 5b66 2b37  =h(u,d,p,c,n[f+7
+001631f0: 5d2c 3232 2c2d 3435 3730 3539 3833 292c  ],22,-45705983),
+00163200: 633d 6828 632c 752c 642c 702c 6e5b 662b  c=h(c,u,d,p,n[f+
+00163210: 385d 2c37 2c31 3737 3030 3335 3431 3629  8],7,1770035416)
+00163220: 2c70 3d68 2870 2c63 2c75 2c64 2c6e 5b66  ,p=h(p,c,u,d,n[f
+00163230: 2b39 5d2c 3132 2c2d 3139 3538 3431 3434  +9],12,-19584144
+00163240: 3137 292c 643d 6828 642c 702c 632c 752c  17),d=h(d,p,c,u,
+00163250: 6e5b 662b 3130 5d2c 3137 2c2d 3432 3036  n[f+10],17,-4206
+00163260: 3329 2c75 3d68 2875 2c64 2c70 2c63 2c6e  3),u=h(u,d,p,c,n
+00163270: 5b66 2b31 315d 2c32 322c 2d31 3939 3034  [f+11],22,-19904
+00163280: 3034 3136 3229 2c63 3d68 2863 2c75 2c64  04162),c=h(c,u,d
+00163290: 2c70 2c6e 5b66 2b31 325d 2c37 2c31 3830  ,p,n[f+12],7,180
+001632a0: 3436 3033 3638 3229 2c70 3d68 2870 2c63  4603682),p=h(p,c
+001632b0: 2c75 2c64 2c6e 5b66 2b31 335d 2c31 322c  ,u,d,n[f+13],12,
+001632c0: 2d34 3033 3431 3130 3129 2c64 3d68 2864  -40341101),d=h(d
+001632d0: 2c70 2c63 2c75 2c6e 5b66 2b31 345d 2c31  ,p,c,u,n[f+14],1
+001632e0: 372c 2d31 3530 3230 3032 3239 3029 2c63  7,-1502002290),c
+001632f0: 3d67 2863 2c75 3d68 2875 2c64 2c70 2c63  =g(c,u=h(u,d,p,c
+00163300: 2c6e 5b66 2b31 355d 2c32 322c 3132 3336  ,n[f+15],22,1236
+00163310: 3533 3533 3239 292c 642c 702c 6e5b 662b  535329),d,p,n[f+
+00163320: 315d 2c35 2c2d 3136 3537 3936 3531 3029  1],5,-165796510)
+00163330: 2c70 3d67 2870 2c63 2c75 2c64 2c6e 5b66  ,p=g(p,c,u,d,n[f
+00163340: 2b36 5d2c 392c 2d31 3036 3935 3031 3633  +6],9,-106950163
+00163350: 3229 2c64 3d67 2864 2c70 2c63 2c75 2c6e  2),d=g(d,p,c,u,n
+00163360: 5b66 2b31 315d 2c31 342c 3634 3337 3137  [f+11],14,643717
+00163370: 3731 3329 2c75 3d67 2875 2c64 2c70 2c63  713),u=g(u,d,p,c
+00163380: 2c6e 5b66 2b30 5d2c 3230 2c2d 3337 3338  ,n[f+0],20,-3738
+00163390: 3937 3330 3229 2c63 3d67 2863 2c75 2c64  97302),c=g(c,u,d
+001633a0: 2c70 2c6e 5b66 2b35 5d2c 352c 2d37 3031  ,p,n[f+5],5,-701
+001633b0: 3535 3836 3931 292c 703d 6728 702c 632c  558691),p=g(p,c,
+001633c0: 752c 642c 6e5b 662b 3130 5d2c 392c 3338  u,d,n[f+10],9,38
+001633d0: 3031 3630 3833 292c 643d 6728 642c 702c  016083),d=g(d,p,
+001633e0: 632c 752c 6e5b 662b 3135 5d2c 3134 2c2d  c,u,n[f+15],14,-
+001633f0: 3636 3034 3738 3333 3529 2c75 3d67 2875  660478335),u=g(u
+00163400: 2c64 2c70 2c63 2c6e 5b66 2b34 5d2c 3230  ,d,p,c,n[f+4],20
+00163410: 2c2d 3430 3535 3337 3834 3829 2c63 3d67  ,-405537848),c=g
+00163420: 2863 2c75 2c64 2c70 2c6e 5b66 2b39 5d2c  (c,u,d,p,n[f+9],
+00163430: 352c 3536 3834 3436 3433 3829 2c70 3d67  5,568446438),p=g
+00163440: 2870 2c63 2c75 2c64 2c6e 5b66 2b31 345d  (p,c,u,d,n[f+14]
+00163450: 2c39 2c2d 3130 3139 3830 3336 3930 292c  ,9,-1019803690),
+00163460: 643d 6728 642c 702c 632c 752c 6e5b 662b  d=g(d,p,c,u,n[f+
+00163470: 335d 2c31 342c 2d31 3837 3336 3339 3631  3],14,-187363961
+00163480: 292c 753d 6728 752c 642c 702c 632c 6e5b  ),u=g(u,d,p,c,n[
+00163490: 662b 385d 2c32 302c 3131 3633 3533 3135  f+8],20,11635315
+001634a0: 3031 292c 633d 6728 632c 752c 642c 702c  01),c=g(c,u,d,p,
+001634b0: 6e5b 662b 3133 5d2c 352c 2d31 3434 3436  n[f+13],5,-14446
+001634c0: 3831 3436 3729 2c70 3d67 2870 2c63 2c75  81467),p=g(p,c,u
+001634d0: 2c64 2c6e 5b66 2b32 5d2c 392c 2d35 3134  ,d,n[f+2],9,-514
+001634e0: 3033 3738 3429 2c64 3d67 2864 2c70 2c63  03784),d=g(d,p,c
+001634f0: 2c75 2c6e 5b66 2b37 5d2c 3134 2c31 3733  ,u,n[f+7],14,173
+00163500: 3533 3238 3437 3329 2c63 3d6d 2863 2c75  5328473),c=m(c,u
+00163510: 3d67 2875 2c64 2c70 2c63 2c6e 5b66 2b31  =g(u,d,p,c,n[f+1
+00163520: 325d 2c32 302c 2d31 3932 3636 3037 3733  2],20,-192660773
+00163530: 3429 2c64 2c70 2c6e 5b66 2b35 5d2c 342c  4),d,p,n[f+5],4,
+00163540: 2d33 3738 3535 3829 2c70 3d6d 2870 2c63  -378558),p=m(p,c
+00163550: 2c75 2c64 2c6e 5b66 2b38 5d2c 3131 2c2d  ,u,d,n[f+8],11,-
+00163560: 3230 3232 3537 3434 3633 292c 643d 6d28  2022574463),d=m(
+00163570: 642c 702c 632c 752c 6e5b 662b 3131 5d2c  d,p,c,u,n[f+11],
+00163580: 3136 2c31 3833 3930 3330 3536 3229 2c75  16,1839030562),u
+00163590: 3d6d 2875 2c64 2c70 2c63 2c6e 5b66 2b31  =m(u,d,p,c,n[f+1
+001635a0: 345d 2c32 332c 2d33 3533 3039 3535 3629  4],23,-35309556)
+001635b0: 2c63 3d6d 2863 2c75 2c64 2c70 2c6e 5b66  ,c=m(c,u,d,p,n[f
+001635c0: 2b31 5d2c 342c 2d31 3533 3039 3932 3036  +1],4,-153099206
+001635d0: 3029 2c70 3d6d 2870 2c63 2c75 2c64 2c6e  0),p=m(p,c,u,d,n
+001635e0: 5b66 2b34 5d2c 3131 2c31 3237 3238 3933  [f+4],11,1272893
+001635f0: 3335 3329 2c64 3d6d 2864 2c70 2c63 2c75  353),d=m(d,p,c,u
+00163600: 2c6e 5b66 2b37 5d2c 3136 2c2d 3135 3534  ,n[f+7],16,-1554
+00163610: 3937 3633 3229 2c75 3d6d 2875 2c64 2c70  97632),u=m(u,d,p
+00163620: 2c63 2c6e 5b66 2b31 305d 2c32 332c 2d31  ,c,n[f+10],23,-1
+00163630: 3039 3437 3330 3634 3029 2c63 3d6d 2863  094730640),c=m(c
+00163640: 2c75 2c64 2c70 2c6e 5b66 2b31 335d 2c34  ,u,d,p,n[f+13],4
+00163650: 2c36 3831 3237 3931 3734 292c 703d 6d28  ,681279174),p=m(
+00163660: 702c 632c 752c 642c 6e5b 662b 305d 2c31  p,c,u,d,n[f+0],1
+00163670: 312c 2d33 3538 3533 3732 3232 292c 643d  1,-358537222),d=
+00163680: 6d28 642c 702c 632c 752c 6e5b 662b 335d  m(d,p,c,u,n[f+3]
+00163690: 2c31 362c 2d37 3232 3532 3139 3739 292c  ,16,-722521979),
+001636a0: 753d 6d28 752c 642c 702c 632c 6e5b 662b  u=m(u,d,p,c,n[f+
+001636b0: 365d 2c32 332c 3736 3032 3931 3839 292c  6],23,76029189),
+001636c0: 633d 6d28 632c 752c 642c 702c 6e5b 662b  c=m(c,u,d,p,n[f+
+001636d0: 395d 2c34 2c2d 3634 3033 3634 3438 3729  9],4,-640364487)
+001636e0: 2c70 3d6d 2870 2c63 2c75 2c64 2c6e 5b66  ,p=m(p,c,u,d,n[f
+001636f0: 2b31 325d 2c31 312c 2d34 3231 3831 3538  +12],11,-4218158
+00163700: 3335 292c 643d 6d28 642c 702c 632c 752c  35),d=m(d,p,c,u,
+00163710: 6e5b 662b 3135 5d2c 3136 2c35 3330 3734  n[f+15],16,53074
+00163720: 3235 3230 292c 633d 7628 632c 753d 6d28  2520),c=v(c,u=m(
+00163730: 752c 642c 702c 632c 6e5b 662b 325d 2c32  u,d,p,c,n[f+2],2
+00163740: 332c 2d39 3935 3333 3836 3531 292c 642c  3,-995338651),d,
+00163750: 702c 6e5b 662b 305d 2c36 2c2d 3139 3836  p,n[f+0],6,-1986
+00163760: 3330 3834 3429 2c70 3d76 2870 2c63 2c75  30844),p=v(p,c,u
+00163770: 2c64 2c6e 5b66 2b37 5d2c 3130 2c31 3132  ,d,n[f+7],10,112
+00163780: 3638 3931 3431 3529 2c64 3d76 2864 2c70  6891415),d=v(d,p
+00163790: 2c63 2c75 2c6e 5b66 2b31 345d 2c31 352c  ,c,u,n[f+14],15,
+001637a0: 2d31 3431 3633 3534 3930 3529 2c75 3d76  -1416354905),u=v
+001637b0: 2875 2c64 2c70 2c63 2c6e 5b66 2b35 5d2c  (u,d,p,c,n[f+5],
+001637c0: 3231 2c2d 3537 3433 3430 3535 292c 633d  21,-57434055),c=
+001637d0: 7628 632c 752c 642c 702c 6e5b 662b 3132  v(c,u,d,p,n[f+12
+001637e0: 5d2c 362c 3137 3030 3438 3535 3731 292c  ],6,1700485571),
+001637f0: 703d 7628 702c 632c 752c 642c 6e5b 662b  p=v(p,c,u,d,n[f+
+00163800: 335d 2c31 302c 2d31 3839 3439 3836 3630  3],10,-189498660
+00163810: 3629 2c64 3d76 2864 2c70 2c63 2c75 2c6e  6),d=v(d,p,c,u,n
+00163820: 5b66 2b31 305d 2c31 352c 2d31 3035 3135  [f+10],15,-10515
+00163830: 3233 292c 753d 7628 752c 642c 702c 632c  23),u=v(u,d,p,c,
+00163840: 6e5b 662b 315d 2c32 312c 2d32 3035 3439  n[f+1],21,-20549
+00163850: 3232 3739 3929 2c63 3d76 2863 2c75 2c64  22799),c=v(c,u,d
+00163860: 2c70 2c6e 5b66 2b38 5d2c 362c 3138 3733  ,p,n[f+8],6,1873
+00163870: 3331 3333 3539 292c 703d 7628 702c 632c  313359),p=v(p,c,
+00163880: 752c 642c 6e5b 662b 3135 5d2c 3130 2c2d  u,d,n[f+15],10,-
+00163890: 3330 3631 3137 3434 292c 643d 7628 642c  30611744),d=v(d,
+001638a0: 702c 632c 752c 6e5b 662b 365d 2c31 352c  p,c,u,n[f+6],15,
+001638b0: 2d31 3536 3031 3938 3338 3029 2c75 3d76  -1560198380),u=v
+001638c0: 2875 2c64 2c70 2c63 2c6e 5b66 2b31 335d  (u,d,p,c,n[f+13]
+001638d0: 2c32 312c 3133 3039 3135 3136 3439 292c  ,21,1309151649),
+001638e0: 633d 7628 632c 752c 642c 702c 6e5b 662b  c=v(c,u,d,p,n[f+
+001638f0: 345d 2c36 2c2d 3134 3535 3233 3037 3029  4],6,-145523070)
+00163900: 2c70 3d76 2870 2c63 2c75 2c64 2c6e 5b66  ,p=v(p,c,u,d,n[f
+00163910: 2b31 315d 2c31 302c 2d31 3132 3032 3130  +11],10,-1120210
+00163920: 3337 3929 2c64 3d76 2864 2c70 2c63 2c75  379),d=v(d,p,c,u
+00163930: 2c6e 5b66 2b32 5d2c 3135 2c37 3138 3738  ,n[f+2],15,71878
+00163940: 3732 3539 292c 753d 7628 752c 642c 702c  7259),u=v(u,d,p,
+00163950: 632c 6e5b 662b 395d 2c32 312c 2d33 3433  c,n[f+9],21,-343
+00163960: 3438 3535 3531 292c 633d 632b 623e 3e3e  485551),c=c+b>>>
+00163970: 302c 753d 752b 793e 3e3e 302c 643d 642b  0,u=u+y>>>0,d=d+
+00163980: 783e 3e3e 302c 703d 702b 773e 3e3e 307d  x>>>0,p=p+w>>>0}
+00163990: 7265 7475 726e 2072 2e65 6e64 6961 6e28  return r.endian(
+001639a0: 5b63 2c75 2c64 2c70 5d29 7d29 2e5f 6666  [c,u,d,p])})._ff
+001639b0: 3d66 756e 6374 696f 6e28 652c 742c 6e2c  =function(e,t,n,
+001639c0: 722c 692c 6f2c 6129 7b76 6172 2073 3d65  r,i,o,a){var s=e
+001639d0: 2b28 7426 6e7c 7e74 2672 292b 2869 3e3e  +(t&n|~t&r)+(i>>
+001639e0: 3e30 292b 613b 7265 7475 726e 2873 3c3c  >0)+a;return(s<<
+001639f0: 6f7c 733e 3e3e 3332 2d6f 292b 747d 2c73  o|s>>>32-o)+t},s
+00163a00: 2e5f 6767 3d66 756e 6374 696f 6e28 652c  ._gg=function(e,
+00163a10: 742c 6e2c 722c 692c 6f2c 6129 7b76 6172  t,n,r,i,o,a){var
+00163a20: 2073 3d65 2b28 7426 727c 6e26 7e72 292b   s=e+(t&r|n&~r)+
+00163a30: 2869 3e3e 3e30 292b 613b 7265 7475 726e  (i>>>0)+a;return
+00163a40: 2873 3c3c 6f7c 733e 3e3e 3332 2d6f 292b  (s<<o|s>>>32-o)+
+00163a50: 747d 2c73 2e5f 6868 3d66 756e 6374 696f  t},s._hh=functio
+00163a60: 6e28 652c 742c 6e2c 722c 692c 6f2c 6129  n(e,t,n,r,i,o,a)
+00163a70: 7b76 6172 2073 3d65 2b28 745e 6e5e 7229  {var s=e+(t^n^r)
+00163a80: 2b28 693e 3e3e 3029 2b61 3b72 6574 7572  +(i>>>0)+a;retur
+00163a90: 6e28 733c 3c6f 7c73 3e3e 3e33 322d 6f29  n(s<<o|s>>>32-o)
+00163aa0: 2b74 7d2c 732e 5f69 693d 6675 6e63 7469  +t},s._ii=functi
+00163ab0: 6f6e 2865 2c74 2c6e 2c72 2c69 2c6f 2c61  on(e,t,n,r,i,o,a
+00163ac0: 297b 7661 7220 733d 652b 286e 5e28 747c  ){var s=e+(n^(t|
+00163ad0: 7e72 2929 2b28 693e 3e3e 3029 2b61 3b72  ~r))+(i>>>0)+a;r
+00163ae0: 6574 7572 6e28 733c 3c6f 7c73 3e3e 3e33  eturn(s<<o|s>>>3
+00163af0: 322d 6f29 2b74 7d2c 732e 5f62 6c6f 636b  2-o)+t},s._block
+00163b00: 7369 7a65 3d31 362c 732e 5f64 6967 6573  size=16,s._diges
+00163b10: 7473 697a 653d 3136 2c65 2e65 7870 6f72  tsize=16,e.expor
+00163b20: 7473 3d66 756e 6374 696f 6e28 652c 7429  ts=function(e,t)
+00163b30: 7b69 6628 6e75 6c6c 3d3d 6529 7468 726f  {if(null==e)thro
+00163b40: 7720 6e65 7720 4572 726f 7228 2249 6c6c  w new Error("Ill
+00163b50: 6567 616c 2061 7267 756d 656e 7420 222b  egal argument "+
+00163b60: 6529 3b76 6172 206e 3d72 2e77 6f72 6473  e);var n=r.words
+00163b70: 546f 4279 7465 7328 7328 652c 7429 293b  ToBytes(s(e,t));
+00163b80: 7265 7475 726e 2074 2626 742e 6173 4279  return t&&t.asBy
+00163b90: 7465 733f 6e3a 7426 2674 2e61 7353 7472  tes?n:t&&t.asStr
+00163ba0: 696e 673f 612e 6279 7465 7354 6f53 7472  ing?a.bytesToStr
+00163bb0: 696e 6728 6e29 3a72 2e62 7974 6573 546f  ing(n):r.bytesTo
+00163bc0: 4865 7828 6e29 7d7d 2c66 756e 6374 696f  Hex(n)}},functio
+00163bd0: 6e28 652c 7429 7b76 6172 206e 2c72 3b6e  n(e,t){var n,r;n
+00163be0: 3d22 4142 4344 4546 4748 494a 4b4c 4d4e  ="ABCDEFGHIJKLMN
+00163bf0: 4f50 5152 5354 5556 5758 595a 6162 6364  OPQRSTUVWXYZabcd
+00163c00: 6566 6768 696a 6b6c 6d6e 6f70 7172 7374  efghijklmnopqrst
+00163c10: 7576 7778 797a 3031 3233 3435 3637 3839  uvwxyz0123456789
+00163c20: 2b2f 222c 723d 7b72 6f74 6c3a 6675 6e63  +/",r={rotl:func
+00163c30: 7469 6f6e 2865 2c74 297b 7265 7475 726e  tion(e,t){return
+00163c40: 2065 3c3c 747c 653e 3e3e 3332 2d74 7d2c   e<<t|e>>>32-t},
+00163c50: 726f 7472 3a66 756e 6374 696f 6e28 652c  rotr:function(e,
+00163c60: 7429 7b72 6574 7572 6e20 653c 3c33 322d  t){return e<<32-
+00163c70: 747c 653e 3e3e 747d 2c65 6e64 6961 6e3a  t|e>>>t},endian:
+00163c80: 6675 6e63 7469 6f6e 2865 297b 6966 2865  function(e){if(e
+00163c90: 2e63 6f6e 7374 7275 6374 6f72 3d3d 4e75  .constructor==Nu
+00163ca0: 6d62 6572 2972 6574 7572 6e20 3136 3731  mber)return 1671
+00163cb0: 3139 3335 2672 2e72 6f74 6c28 652c 3829  1935&r.rotl(e,8)
+00163cc0: 7c34 3237 3832 3535 3336 3026 722e 726f  |4278255360&r.ro
+00163cd0: 746c 2865 2c32 3429 3b66 6f72 2876 6172  tl(e,24);for(var
+00163ce0: 2074 3d30 3b74 3c65 2e6c 656e 6774 683b   t=0;t<e.length;
+00163cf0: 742b 2b29 655b 745d 3d72 2e65 6e64 6961  t++)e[t]=r.endia
+00163d00: 6e28 655b 745d 293b 7265 7475 726e 2065  n(e[t]);return e
+00163d10: 7d2c 7261 6e64 6f6d 4279 7465 733a 6675  },randomBytes:fu
+00163d20: 6e63 7469 6f6e 2865 297b 666f 7228 7661  nction(e){for(va
+00163d30: 7220 743d 5b5d 3b65 3e30 3b65 2d2d 2974  r t=[];e>0;e--)t
+00163d40: 2e70 7573 6828 4d61 7468 2e66 6c6f 6f72  .push(Math.floor
+00163d50: 2832 3536 2a4d 6174 682e 7261 6e64 6f6d  (256*Math.random
+00163d60: 2829 2929 3b72 6574 7572 6e20 747d 2c62  ()));return t},b
+00163d70: 7974 6573 546f 576f 7264 733a 6675 6e63  ytesToWords:func
+00163d80: 7469 6f6e 2865 297b 666f 7228 7661 7220  tion(e){for(var 
+00163d90: 743d 5b5d 2c6e 3d30 2c72 3d30 3b6e 3c65  t=[],n=0,r=0;n<e
+00163da0: 2e6c 656e 6774 683b 6e2b 2b2c 722b 3d38  .length;n++,r+=8
+00163db0: 2974 5b72 3e3e 3e35 5d7c 3d65 5b6e 5d3c  )t[r>>>5]|=e[n]<
+00163dc0: 3c32 342d 7225 3332 3b72 6574 7572 6e20  <24-r%32;return 
+00163dd0: 747d 2c77 6f72 6473 546f 4279 7465 733a  t},wordsToBytes:
+00163de0: 6675 6e63 7469 6f6e 2865 297b 666f 7228  function(e){for(
+00163df0: 7661 7220 743d 5b5d 2c6e 3d30 3b6e 3c33  var t=[],n=0;n<3
+00163e00: 322a 652e 6c65 6e67 7468 3b6e 2b3d 3829  2*e.length;n+=8)
+00163e10: 742e 7075 7368 2865 5b6e 3e3e 3e35 5d3e  t.push(e[n>>>5]>
+00163e20: 3e3e 3234 2d6e 2533 3226 3235 3529 3b72  >>24-n%32&255);r
+00163e30: 6574 7572 6e20 747d 2c62 7974 6573 546f  eturn t},bytesTo
+00163e40: 4865 783a 6675 6e63 7469 6f6e 2865 297b  Hex:function(e){
+00163e50: 666f 7228 7661 7220 743d 5b5d 2c6e 3d30  for(var t=[],n=0
+00163e60: 3b6e 3c65 2e6c 656e 6774 683b 6e2b 2b29  ;n<e.length;n++)
+00163e70: 742e 7075 7368 2828 655b 6e5d 3e3e 3e34  t.push((e[n]>>>4
+00163e80: 292e 746f 5374 7269 6e67 2831 3629 292c  ).toString(16)),
+00163e90: 742e 7075 7368 2828 3135 2665 5b6e 5d29  t.push((15&e[n])
+00163ea0: 2e74 6f53 7472 696e 6728 3136 2929 3b72  .toString(16));r
+00163eb0: 6574 7572 6e20 742e 6a6f 696e 2822 2229  eturn t.join("")
+00163ec0: 7d2c 6865 7854 6f42 7974 6573 3a66 756e  },hexToBytes:fun
+00163ed0: 6374 696f 6e28 6529 7b66 6f72 2876 6172  ction(e){for(var
+00163ee0: 2074 3d5b 5d2c 6e3d 303b 6e3c 652e 6c65   t=[],n=0;n<e.le
+00163ef0: 6e67 7468 3b6e 2b3d 3229 742e 7075 7368  ngth;n+=2)t.push
+00163f00: 2870 6172 7365 496e 7428 652e 7375 6273  (parseInt(e.subs
+00163f10: 7472 286e 2c32 292c 3136 2929 3b72 6574  tr(n,2),16));ret
+00163f20: 7572 6e20 747d 2c62 7974 6573 546f 4261  urn t},bytesToBa
+00163f30: 7365 3634 3a66 756e 6374 696f 6e28 6529  se64:function(e)
+00163f40: 7b66 6f72 2876 6172 2074 3d5b 5d2c 723d  {for(var t=[],r=
+00163f50: 303b 723c 652e 6c65 6e67 7468 3b72 2b3d  0;r<e.length;r+=
+00163f60: 3329 666f 7228 7661 7220 693d 655b 725d  3)for(var i=e[r]
+00163f70: 3c3c 3136 7c65 5b72 2b31 5d3c 3c38 7c65  <<16|e[r+1]<<8|e
+00163f80: 5b72 2b32 5d2c 6f3d 303b 6f3c 343b 6f2b  [r+2],o=0;o<4;o+
+00163f90: 2b29 382a 722b 362a 6f3c 3d38 2a65 2e6c  +)8*r+6*o<=8*e.l
+00163fa0: 656e 6774 683f 742e 7075 7368 286e 2e63  ength?t.push(n.c
+00163fb0: 6861 7241 7428 693e 3e3e 362a 2833 2d6f  harAt(i>>>6*(3-o
+00163fc0: 2926 3633 2929 3a74 2e70 7573 6828 223d  )&63)):t.push("=
+00163fd0: 2229 3b72 6574 7572 6e20 742e 6a6f 696e  ");return t.join
+00163fe0: 2822 2229 7d2c 6261 7365 3634 546f 4279  ("")},base64ToBy
+00163ff0: 7465 733a 6675 6e63 7469 6f6e 2865 297b  tes:function(e){
+00164000: 653d 652e 7265 706c 6163 6528 2f5b 5e41  e=e.replace(/[^A
+00164010: 2d5a 302d 392b 5c2f 5d2f 6769 2c22 2229  -Z0-9+\/]/gi,"")
+00164020: 3b66 6f72 2876 6172 2074 3d5b 5d2c 723d  ;for(var t=[],r=
+00164030: 302c 693d 303b 723c 652e 6c65 6e67 7468  0,i=0;r<e.length
+00164040: 3b69 3d2b 2b72 2534 2930 213d 6926 2674  ;i=++r%4)0!=i&&t
+00164050: 2e70 7573 6828 286e 2e69 6e64 6578 4f66  .push((n.indexOf
+00164060: 2865 2e63 6861 7241 7428 722d 3129 2926  (e.charAt(r-1))&
+00164070: 4d61 7468 2e70 6f77 2832 2c2d 322a 692b  Math.pow(2,-2*i+
+00164080: 3829 2d31 293c 3c32 2a69 7c6e 2e69 6e64  8)-1)<<2*i|n.ind
+00164090: 6578 4f66 2865 2e63 6861 7241 7428 7229  exOf(e.charAt(r)
+001640a0: 293e 3e3e 362d 322a 6929 3b72 6574 7572  )>>>6-2*i);retur
+001640b0: 6e20 747d 7d2c 652e 6578 706f 7274 733d  n t}},e.exports=
+001640c0: 727d 2c66 756e 6374 696f 6e28 652c 7429  r},function(e,t)
+001640d0: 7b66 756e 6374 696f 6e20 6e28 6529 7b72  {function n(e){r
+001640e0: 6574 7572 6e21 2165 2e63 6f6e 7374 7275  eturn!!e.constru
+001640f0: 6374 6f72 2626 2266 756e 6374 696f 6e22  ctor&&"function"
+00164100: 3d3d 7479 7065 6f66 2065 2e63 6f6e 7374  ==typeof e.const
+00164110: 7275 6374 6f72 2e69 7342 7566 6665 7226  ructor.isBuffer&
+00164120: 2665 2e63 6f6e 7374 7275 6374 6f72 2e69  &e.constructor.i
+00164130: 7342 7566 6665 7228 6529 7d0a 2f2a 210a  sBuffer(e)}./*!.
+00164140: 202a 2044 6574 6572 6d69 6e65 2069 6620   * Determine if 
+00164150: 616e 206f 626a 6563 7420 6973 2061 2042  an object is a B
+00164160: 7566 6665 720a 202a 0a20 2a20 4061 7574  uffer. *. * @aut
+00164170: 686f 7220 2020 4665 726f 7373 2041 626f  hor   Feross Abo
+00164180: 756b 6861 6469 6a65 6820 3c68 7474 7073  ukhadijeh <https
+00164190: 3a2f 2f66 6572 6f73 732e 6f72 673e 0a20  ://feross.org>. 
+001641a0: 2a20 406c 6963 656e 7365 2020 4d49 540a  * @license  MIT.
+001641b0: 202a 2f0a 652e 6578 706f 7274 733d 6675   */.e.exports=fu
+001641c0: 6e63 7469 6f6e 2865 297b 7265 7475 726e  nction(e){return
+001641d0: 206e 756c 6c21 3d65 2626 286e 2865 297c   null!=e&&(n(e)|
+001641e0: 7c66 756e 6374 696f 6e28 6529 7b72 6574  |function(e){ret
+001641f0: 7572 6e22 6675 6e63 7469 6f6e 223d 3d74  urn"function"==t
+00164200: 7970 656f 6620 652e 7265 6164 466c 6f61  ypeof e.readFloa
+00164210: 744c 4526 2622 6675 6e63 7469 6f6e 223d  tLE&&"function"=
+00164220: 3d74 7970 656f 6620 652e 736c 6963 6526  =typeof e.slice&
+00164230: 266e 2865 2e73 6c69 6365 2830 2c30 2929  &n(e.slice(0,0))
+00164240: 7d28 6529 7c7c 2121 652e 5f69 7342 7566  }(e)||!!e._isBuf
+00164250: 6665 7229 7d7d 2c66 756e 6374 696f 6e28  fer)}},function(
+00164260: 652c 742c 6e29 7b6e 2839 292e 6d6f 6475  e,t,n){n(9).modu
+00164270: 6c65 2822 6462 7422 292e 6661 6374 6f72  le("dbt").factor
+00164280: 7928 226c 6f63 6174 696f 6e53 6572 7669  y("locationServi
+00164290: 6365 222c 5b22 2473 7461 7465 222c 6675  ce",["$state",fu
+001642a0: 6e63 7469 6f6e 2865 297b 7661 7220 743d  nction(e){var t=
+001642b0: 7b7d 3b72 6574 7572 6e20 742e 7061 7273  {};return t.pars
+001642c0: 6553 7461 7465 3d66 756e 6374 696f 6e28  eState=function(
+001642d0: 6529 7b72 6574 7572 6e20 6675 6e63 7469  e){return functi
+001642e0: 6f6e 2865 297b 7265 7475 726e 7b73 656c  on(e){return{sel
+001642f0: 6563 7465 643a 7b69 6e63 6c75 6465 3a65  ected:{include:e
+00164300: 2e67 5f69 7c7c 2222 2c65 7863 6c75 6465  .g_i||"",exclude
+00164310: 3a65 2e67 5f65 7c7c 2222 7d2c 7368 6f77  :e.g_e||""},show
+00164320: 5f67 7261 7068 3a21 2165 2e67 5f76 7d7d  _graph:!!e.g_v}}
+00164330: 2865 297d 2c74 2e73 6574 5374 6174 653d  (e)},t.setState=
+00164340: 6675 6e63 7469 6f6e 2874 297b 7661 7220  function(t){var 
+00164350: 6e3d 6675 6e63 7469 6f6e 2865 297b 7661  n=function(e){va
+00164360: 7220 743d 7b67 5f76 3a31 7d3b 7265 7475  r t={g_v:1};retu
+00164370: 726e 2074 2e67 5f69 3d65 2e69 6e63 6c75  rn t.g_i=e.inclu
+00164380: 6465 2c74 2e67 5f65 3d65 2e65 7863 6c75  de,t.g_e=e.exclu
+00164390: 6465 2c74 7d28 7429 2c72 3d65 2e63 7572  de,t}(t),r=e.cur
+001643a0: 7265 6e74 2e6e 616d 653b 652e 676f 2872  rent.name;e.go(r
+001643b0: 2c6e 297d 2c74 2e63 6c65 6172 5374 6174  ,n)},t.clearStat
+001643c0: 653d 6675 6e63 7469 6f6e 2829 7b76 6172  e=function(){var
+001643d0: 2074 3d65 2e63 7572 7265 6e74 2e6e 616d   t=e.current.nam
+001643e0: 653b 652e 676f 2874 2c7b 675f 693a 6e75  e;e.go(t,{g_i:nu
+001643f0: 6c6c 2c67 5f65 3a6e 756c 6c2c 675f 763a  ll,g_e:null,g_v:
+00164400: 6e75 6c6c 7d29 7d2c 747d 5d29 7d2c 6675  null})},t}])},fu
+00164410: 6e63 7469 6f6e 2865 2c74 2c6e 297b 2275  nction(e,t,n){"u
+00164420: 7365 2073 7472 6963 7422 3b63 6f6e 7374  se strict";const
+00164430: 2072 3d6e 2839 292c 693d 6e28 3230 3229   r=n(9),i=n(202)
+00164440: 3b72 2e6d 6f64 756c 6528 2264 6274 2229  ;r.module("dbt")
+00164450: 2e63 6f6e 7472 6f6c 6c65 7228 224f 7665  .controller("Ove
+00164460: 7276 6965 7743 7472 6c22 2c5b 2224 7363  rviewCtrl",["$sc
+00164470: 6f70 6522 2c22 2473 7461 7465 222c 2270  ope","$state","p
+00164480: 726f 6a65 6374 222c 6675 6e63 7469 6f6e  roject",function
+00164490: 2865 2c74 2c6e 297b 652e 6f76 6572 7669  (e,t,n){e.overvi
+001644a0: 6577 5f6d 643d 2228 6c6f 6164 696e 6729  ew_md="(loading)
+001644b0: 222c 6e2e 7265 6164 7928 2866 756e 6374  ",n.ready((funct
+001644c0: 696f 6e28 6e29 7b6c 6574 2072 3d74 2e70  ion(n){let r=t.p
+001644d0: 6172 616d 732e 7072 6f6a 6563 745f 6e61  arams.project_na
+001644e0: 6d65 3f74 2e70 6172 616d 732e 7072 6f6a  me?t.params.proj
+001644f0: 6563 745f 6e61 6d65 3a6e 756c 6c3b 7661  ect_name:null;va
+00164500: 7220 6f3d 6e2e 646f 6373 5b22 646f 632e  r o=n.docs["doc.
+00164510: 6462 742e 5f5f 6f76 6572 7669 6577 5f5f  dbt.__overview__
+00164520: 225d 2c61 3d69 2e66 696c 7465 7228 6e2e  "],a=i.filter(n.
+00164530: 646f 6373 2c7b 6e61 6d65 3a22 5f5f 6f76  docs,{name:"__ov
+00164540: 6572 7669 6577 5f5f 227d 293b 6966 2869  erview__"});if(i
+00164550: 2e65 6163 6828 612c 2866 756e 6374 696f  .each(a,(functio
+00164560: 6e28 6529 7b22 6462 7422 213d 652e 7061  n(e){"dbt"!=e.pa
+00164570: 636b 6167 655f 6e61 6d65 2626 286f 3d65  ckage_name&&(o=e
+00164580: 297d 2929 2c6e 756c 6c21 3d3d 7229 7b6f  )})),null!==r){o
+00164590: 3d6e 2e64 6f63 735b 6064 6f63 2e24 7b72  =n.docs[`doc.${r
+001645a0: 7d2e 5f5f 247b 727d 5f5f 605d 7c7c 6f3b  }.__${r}__`]||o;
+001645b0: 6c65 7420 653d 692e 6669 6c74 6572 286e  let e=i.filter(n
+001645c0: 2e64 6f63 732c 7b6e 616d 653a 605f 5f24  .docs,{name:`__$
+001645d0: 7b72 7d5f 5f60 7d29 3b69 2e65 6163 6828  {r}__`});i.each(
+001645e0: 652c 653d 3e7b 652e 7061 636b 6167 655f  e,e=>{e.package_
+001645f0: 6e61 6d65 213d 3d72 2626 286f 3d65 297d  name!==r&&(o=e)}
+00164600: 297d 652e 6f76 6572 7669 6577 5f6d 643d  )}e.overview_md=
+00164610: 6f2e 626c 6f63 6b5f 636f 6e74 656e 7473  o.block_contents
+00164620: 7d29 297d 5d29 7d2c 6675 6e63 7469 6f6e  }))}])},function
+00164630: 2865 2c74 2c6e 297b 2275 7365 2073 7472  (e,t,n){"use str
+00164640: 6963 7422 3b6e 2839 292e 6d6f 6475 6c65  ict";n(9).module
+00164650: 2822 6462 7422 292e 636f 6e74 726f 6c6c  ("dbt").controll
+00164660: 6572 2822 536f 7572 6365 4c69 7374 4374  er("SourceListCt
+00164670: 726c 222c 5b22 2473 636f 7065 222c 2224  rl",["$scope","$
+00164680: 7374 6174 6522 2c22 7072 6f6a 6563 7422  state","project"
+00164690: 2c66 756e 6374 696f 6e28 652c 742c 6e29  ,function(e,t,n)
+001646a0: 7b65 2e73 6f75 7263 653d 742e 7061 7261  {e.source=t.para
+001646b0: 6d73 2e73 6f75 7263 652c 652e 6d6f 6465  ms.source,e.mode
+001646c0: 6c3d 7b7d 2c65 2e65 7874 7261 5f74 6162  l={},e.extra_tab
+001646d0: 6c65 5f66 6965 6c64 733d 5b5d 2c65 2e68  le_fields=[],e.h
+001646e0: 6173 5f6d 6f72 655f 696e 666f 3d66 756e  as_more_info=fun
+001646f0: 6374 696f 6e28 6529 7b72 6574 7572 6e28  ction(e){return(
+00164700: 652e 6465 7363 7269 7074 696f 6e7c 7c22  e.description||"
+00164710: 2229 2e6c 656e 6774 687d 2c65 2e74 6f67  ").length},e.tog
+00164720: 676c 655f 736f 7572 6365 5f65 7870 616e  gle_source_expan
+00164730: 6465 643d 6675 6e63 7469 6f6e 2874 297b  ded=function(t){
+00164740: 652e 6861 735f 6d6f 7265 5f69 6e66 6f28  e.has_more_info(
+00164750: 7429 2626 2874 2e65 7870 616e 6465 643d  t)&&(t.expanded=
+00164760: 2174 2e65 7870 616e 6465 6429 7d2c 6e2e  !t.expanded)},n.
+00164770: 7265 6164 7928 2866 756e 6374 696f 6e28  ready((function(
+00164780: 7429 7b76 6172 206e 3d5f 2e66 696c 7465  t){var n=_.filte
+00164790: 7228 742e 6e6f 6465 732c 2866 756e 6374  r(t.nodes,(funct
+001647a0: 696f 6e28 7429 7b72 6574 7572 6e20 742e  ion(t){return t.
+001647b0: 736f 7572 6365 5f6e 616d 653d 3d65 2e73  source_name==e.s
+001647c0: 6f75 7263 657d 2929 3b69 6628 3021 3d6e  ource}));if(0!=n
+001647d0: 2e6c 656e 6774 6829 7b6e 2e73 6f72 7428  .length){n.sort(
+001647e0: 2865 2c74 293d 3e65 2e6e 616d 652e 6c6f  (e,t)=>e.name.lo
+001647f0: 6361 6c65 436f 6d70 6172 6528 742e 6e61  caleCompare(t.na
+00164800: 6d65 2929 3b76 6172 2072 3d6e 5b30 5d3b  me));var r=n[0];
+00164810: 652e 6d6f 6465 6c3d 7b6e 616d 653a 652e  e.model={name:e.
+00164820: 736f 7572 6365 2c73 6f75 7263 655f 6465  source,source_de
+00164830: 7363 7269 7074 696f 6e3a 722e 736f 7572  scription:r.sour
+00164840: 6365 5f64 6573 6372 6970 7469 6f6e 2c73  ce_description,s
+00164850: 6f75 7263 6573 3a6e 7d3b 7661 7220 693d  ources:n};var i=
 00164860: 5f2e 756e 6971 285f 2e6d 6170 286e 2c22  _.uniq(_.map(n,"
-00164870: 6461 7461 6261 7365 2229 292c 613d 5f2e  database")),a=_.
-00164880: 756e 6971 285f 2e6d 6170 286e 2c22 7363  uniq(_.map(n,"sc
-00164890: 6865 6d61 2229 293b 652e 6578 7472 615f  hema"));e.extra_
-001648a0: 7461 626c 655f 6669 656c 6473 3d5b 7b6e  table_fields=[{n
-001648b0: 616d 653a 224c 6f61 6465 7222 2c76 616c  ame:"Loader",val
-001648c0: 7565 3a72 2e6c 6f61 6465 727d 2c7b 6e61  ue:r.loader},{na
-001648d0: 6d65 3a31 3d3d 692e 6c65 6e67 7468 3f22  me:1==i.length?"
-001648e0: 4f77 6e65 7222 3a22 4f77 6e65 7273 222c  Owner":"Owners",
-001648f0: 7661 6c75 653a 692e 6a6f 696e 2822 2c20  value:i.join(", 
-00164900: 2229 7d2c 7b6e 616d 653a 313d 3d6f 2e6c  ")},{name:1==o.l
-00164910: 656e 6774 683f 2244 6174 6162 6173 6522  ength?"Database"
-00164920: 3a22 4461 7461 6261 7365 7322 2c76 616c  :"Databases",val
-00164930: 7565 3a6f 2e6a 6f69 6e28 222c 2022 297d  ue:o.join(", ")}
-00164940: 2c7b 6e61 6d65 3a31 3d3d 612e 6c65 6e67  ,{name:1==a.leng
-00164950: 7468 3f22 5363 6865 6d61 223a 2253 6368  th?"Schema":"Sch
-00164960: 656d 6173 222c 7661 6c75 653a 612e 6a6f  emas",value:a.jo
-00164970: 696e 2822 2c20 2229 7d2c 7b6e 616d 653a  in(", ")},{name:
-00164980: 2254 6162 6c65 7322 2c76 616c 7565 3a6e  "Tables",value:n
-00164990: 2e6c 656e 6774 687d 5d7d 7d29 297d 5d29  .length}]}}))}])
-001649a0: 7d2c 6675 6e63 7469 6f6e 2865 2c74 2c6e  },function(e,t,n
-001649b0: 297b 636f 6e73 7420 723d 6e28 3929 2c69  ){const r=n(9),i
-001649c0: 3d7b 6d61 696e 3a6e 2834 3832 292c 6f76  ={main:n(482),ov
-001649d0: 6572 7669 6577 3a6e 2834 3833 292c 6772  erview:n(483),gr
-001649e0: 6170 683a 6e28 3438 3429 2c73 6f75 7263  aph:n(484),sourc
-001649f0: 653a 6e28 3230 3529 2c73 6f75 7263 655f  e:n(205),source_
-00164a00: 6c69 7374 3a6e 2834 3835 292c 6d6f 6465  list:n(485),mode
-00164a10: 6c3a 6e28 3438 3629 2c73 6f75 7263 653a  l:n(486),source:
-00164a20: 6e28 3230 3529 2c73 6e61 7073 686f 743a  n(205),snapshot:
-00164a30: 6e28 3438 3729 2c73 6565 643a 6e28 3438  n(487),seed:n(48
-00164a40: 3829 2c75 6e69 745f 7465 7374 3a6e 2834  8),unit_test:n(4
-00164a50: 3839 292c 7465 7374 3a6e 2834 3930 292c  89),test:n(490),
-00164a60: 616e 616c 7973 6973 3a6e 2834 3931 292c  analysis:n(491),
-00164a70: 6d61 6372 6f3a 6e28 3439 3229 2c65 7870  macro:n(492),exp
-00164a80: 6f73 7572 653a 6e28 3439 3329 2c6d 6574  osure:n(493),met
-00164a90: 7269 633a 6e28 3439 3429 2c73 656d 616e  ric:n(494),seman
-00164aa0: 7469 635f 6d6f 6465 6c3a 6e28 3439 3529  tic_model:n(495)
-00164ab0: 2c6f 7065 7261 7469 6f6e 3a6e 2834 3936  ,operation:n(496
-00164ac0: 297d 3b72 2e6d 6f64 756c 6528 2264 6274  )};r.module("dbt
-00164ad0: 2229 2e63 6f6e 6669 6728 5b22 2473 7461  ").config(["$sta
-00164ae0: 7465 5072 6f76 6964 6572 222c 2224 7572  teProvider","$ur
-00164af0: 6c52 6f75 7465 7250 726f 7669 6465 7222  lRouterProvider"
-00164b00: 2c66 756e 6374 696f 6e28 652c 7429 7b76  ,function(e,t){v
-00164b10: 6172 206e 3d22 675f 7626 675f 6926 675f  ar n="g_v&g_i&g_
-00164b20: 6526 675f 7026 675f 6e22 3b74 2e6f 7468  e&g_p&g_n";t.oth
-00164b30: 6572 7769 7365 2822 2f6f 7665 7276 6965  erwise("/overvie
-00164b40: 7722 292c 652e 7374 6174 6528 2264 6274  w"),e.state("dbt
-00164b50: 222c 7b75 726c 3a22 2f22 2c61 6273 7472  ",{url:"/",abstr
-00164b60: 6163 743a 2130 2c63 6f6e 7472 6f6c 6c65  act:!0,controlle
-00164b70: 723a 224d 6169 6e43 6f6e 7472 6f6c 6c65  r:"MainControlle
-00164b80: 7222 2c74 656d 706c 6174 6555 726c 3a69  r",templateUrl:i
-00164b90: 2e6d 6169 6e7d 292e 7374 6174 6528 2264  .main}).state("d
-00164ba0: 6274 2e6f 7665 7276 6965 7722 2c7b 7572  bt.overview",{ur
-00164bb0: 6c3a 226f 7665 7276 6965 773f 222b 6e2c  l:"overview?"+n,
-00164bc0: 636f 6e74 726f 6c6c 6572 3a22 4f76 6572  controller:"Over
-00164bd0: 7669 6577 4374 726c 222c 7465 6d70 6c61  viewCtrl",templa
-00164be0: 7465 5572 6c3a 692e 6f76 6572 7669 6577  teUrl:i.overview
-00164bf0: 7d29 2e73 7461 7465 2822 6462 742e 7072  }).state("dbt.pr
-00164c00: 6f6a 6563 745f 6f76 6572 7669 6577 222c  oject_overview",
-00164c10: 7b75 726c 3a22 6f76 6572 7669 6577 2f3a  {url:"overview/:
-00164c20: 7072 6f6a 6563 745f 6e61 6d65 3f22 2b6e  project_name?"+n
-00164c30: 2c63 6f6e 7472 6f6c 6c65 723a 224f 7665  ,controller:"Ove
-00164c40: 7276 6965 7743 7472 6c22 2c74 656d 706c  rviewCtrl",templ
-00164c50: 6174 6555 726c 3a69 2e6f 7665 7276 6965  ateUrl:i.overvie
-00164c60: 772c 7061 7261 6d73 3a7b 7072 6f6a 6563  w,params:{projec
-00164c70: 745f 6e61 6d65 3a7b 7479 7065 3a22 7374  t_name:{type:"st
-00164c80: 7269 6e67 227d 7d7d 292e 7374 6174 6528  ring"}}}).state(
-00164c90: 2264 6274 2e67 7261 7068 222c 7b75 726c  "dbt.graph",{url
-00164ca0: 3a22 6772 6170 6822 2c63 6f6e 7472 6f6c  :"graph",control
-00164cb0: 6c65 723a 2247 7261 7068 4374 726c 222c  ler:"GraphCtrl",
-00164cc0: 7465 6d70 6c61 7465 5572 6c3a 692e 6772  templateUrl:i.gr
-00164cd0: 6170 687d 292e 7374 6174 6528 2264 6274  aph}).state("dbt
-00164ce0: 2e6d 6f64 656c 222c 7b75 726c 3a22 6d6f  .model",{url:"mo
-00164cf0: 6465 6c2f 3a75 6e69 7175 655f 6964 3f73  del/:unique_id?s
-00164d00: 6563 7469 6f6e 2622 2b6e 2c63 6f6e 7472  ection&"+n,contr
-00164d10: 6f6c 6c65 723a 224d 6f64 656c 4374 726c  oller:"ModelCtrl
-00164d20: 222c 7465 6d70 6c61 7465 5572 6c3a 692e  ",templateUrl:i.
-00164d30: 6d6f 6465 6c2c 7061 7261 6d73 3a7b 756e  model,params:{un
-00164d40: 6971 7565 5f69 643a 7b74 7970 653a 2273  ique_id:{type:"s
-00164d50: 7472 696e 6722 7d7d 7d29 2e73 7461 7465  tring"}}}).state
-00164d60: 2822 6462 742e 7365 6564 222c 7b75 726c  ("dbt.seed",{url
-00164d70: 3a22 7365 6564 2f3a 756e 6971 7565 5f69  :"seed/:unique_i
-00164d80: 643f 7365 6374 696f 6e26 222b 6e2c 636f  d?section&"+n,co
-00164d90: 6e74 726f 6c6c 6572 3a22 5365 6564 4374  ntroller:"SeedCt
-00164da0: 726c 222c 7465 6d70 6c61 7465 5572 6c3a  rl",templateUrl:
-00164db0: 692e 7365 6564 2c70 6172 616d 733a 7b75  i.seed,params:{u
-00164dc0: 6e69 7175 655f 6964 3a7b 7479 7065 3a22  nique_id:{type:"
-00164dd0: 7374 7269 6e67 227d 7d7d 292e 7374 6174  string"}}}).stat
-00164de0: 6528 2264 6274 2e73 6e61 7073 686f 7422  e("dbt.snapshot"
-00164df0: 2c7b 7572 6c3a 2273 6e61 7073 686f 742f  ,{url:"snapshot/
-00164e00: 3a75 6e69 7175 655f 6964 3f73 6563 7469  :unique_id?secti
-00164e10: 6f6e 2622 2b6e 2c63 6f6e 7472 6f6c 6c65  on&"+n,controlle
-00164e20: 723a 2253 6e61 7073 686f 7443 7472 6c22  r:"SnapshotCtrl"
-00164e30: 2c74 656d 706c 6174 6555 726c 3a69 2e73  ,templateUrl:i.s
-00164e40: 6e61 7073 686f 742c 7061 7261 6d73 3a7b  napshot,params:{
-00164e50: 756e 6971 7565 5f69 643a 7b74 7970 653a  unique_id:{type:
-00164e60: 2273 7472 696e 6722 7d7d 7d29 2e73 7461  "string"}}}).sta
-00164e70: 7465 2822 6462 742e 756e 6974 5f74 6573  te("dbt.unit_tes
-00164e80: 7422 2c7b 7572 6c3a 2275 6e69 745f 7465  t",{url:"unit_te
-00164e90: 7374 2f3a 756e 6971 7565 5f69 643f 7365  st/:unique_id?se
-00164ea0: 6374 696f 6e26 222b 6e2c 636f 6e74 726f  ction&"+n,contro
-00164eb0: 6c6c 6572 3a22 5465 7374 4374 726c 222c  ller:"TestCtrl",
-00164ec0: 7465 6d70 6c61 7465 5572 6c3a 692e 756e  templateUrl:i.un
-00164ed0: 6974 5f74 6573 742c 7061 7261 6d73 3a7b  it_test,params:{
-00164ee0: 756e 6971 7565 5f69 643a 7b74 7970 653a  unique_id:{type:
-00164ef0: 2273 7472 696e 6722 7d7d 7d29 2e73 7461  "string"}}}).sta
-00164f00: 7465 2822 6462 742e 7465 7374 222c 7b75  te("dbt.test",{u
-00164f10: 726c 3a22 7465 7374 2f3a 756e 6971 7565  rl:"test/:unique
-00164f20: 5f69 643f 7365 6374 696f 6e26 222b 6e2c  _id?section&"+n,
-00164f30: 636f 6e74 726f 6c6c 6572 3a22 5465 7374  controller:"Test
-00164f40: 4374 726c 222c 7465 6d70 6c61 7465 5572  Ctrl",templateUr
-00164f50: 6c3a 692e 7465 7374 2c70 6172 616d 733a  l:i.test,params:
-00164f60: 7b75 6e69 7175 655f 6964 3a7b 7479 7065  {unique_id:{type
-00164f70: 3a22 7374 7269 6e67 227d 7d7d 292e 7374  :"string"}}}).st
-00164f80: 6174 6528 2264 6274 2e61 6e61 6c79 7369  ate("dbt.analysi
-00164f90: 7322 2c7b 7572 6c3a 2261 6e61 6c79 7369  s",{url:"analysi
-00164fa0: 732f 3a75 6e69 7175 655f 6964 3f73 6563  s/:unique_id?sec
-00164fb0: 7469 6f6e 2622 2b6e 2c63 6f6e 7472 6f6c  tion&"+n,control
-00164fc0: 6c65 723a 2241 6e61 6c79 7369 7343 7472  ler:"AnalysisCtr
-00164fd0: 6c22 2c74 656d 706c 6174 6555 726c 3a69  l",templateUrl:i
-00164fe0: 2e61 6e61 6c79 7369 732c 7061 7261 6d73  .analysis,params
-00164ff0: 3a7b 756e 6971 7565 5f69 643a 7b74 7970  :{unique_id:{typ
-00165000: 653a 2273 7472 696e 6722 7d7d 7d29 2e73  e:"string"}}}).s
-00165010: 7461 7465 2822 6462 742e 736f 7572 6365  tate("dbt.source
-00165020: 222c 7b75 726c 3a22 736f 7572 6365 2f3a  ",{url:"source/:
-00165030: 756e 6971 7565 5f69 643f 7365 6374 696f  unique_id?sectio
-00165040: 6e26 222b 6e2c 636f 6e74 726f 6c6c 6572  n&"+n,controller
-00165050: 3a22 536f 7572 6365 4374 726c 222c 7465  :"SourceCtrl",te
-00165060: 6d70 6c61 7465 5572 6c3a 692e 736f 7572  mplateUrl:i.sour
-00165070: 6365 2c70 6172 616d 733a 7b75 6e69 7175  ce,params:{uniqu
-00165080: 655f 6964 3a7b 7479 7065 3a22 7374 7269  e_id:{type:"stri
-00165090: 6e67 227d 7d7d 292e 7374 6174 6528 2264  ng"}}}).state("d
-001650a0: 6274 2e73 6f75 7263 655f 6c69 7374 222c  bt.source_list",
-001650b0: 7b75 726c 3a22 736f 7572 6365 5f6c 6973  {url:"source_lis
-001650c0: 742f 3a73 6f75 7263 653f 7365 6374 696f  t/:source?sectio
-001650d0: 6e26 222b 6e2c 636f 6e74 726f 6c6c 6572  n&"+n,controller
-001650e0: 3a22 536f 7572 6365 4c69 7374 4374 726c  :"SourceListCtrl
-001650f0: 222c 7465 6d70 6c61 7465 5572 6c3a 692e  ",templateUrl:i.
-00165100: 736f 7572 6365 5f6c 6973 742c 7061 7261  source_list,para
-00165110: 6d73 3a7b 736f 7572 6365 3a7b 7479 7065  ms:{source:{type
-00165120: 3a22 7374 7269 6e67 227d 7d7d 292e 7374  :"string"}}}).st
-00165130: 6174 6528 2264 6274 2e6d 6163 726f 222c  ate("dbt.macro",
-00165140: 7b75 726c 3a22 6d61 6372 6f2f 3a75 6e69  {url:"macro/:uni
-00165150: 7175 655f 6964 3f73 6563 7469 6f6e 222c  que_id?section",
-00165160: 636f 6e74 726f 6c6c 6572 3a22 4d61 6372  controller:"Macr
-00165170: 6f43 7472 6c22 2c74 656d 706c 6174 6555  oCtrl",templateU
-00165180: 726c 3a69 2e6d 6163 726f 2c70 6172 616d  rl:i.macro,param
-00165190: 733a 7b75 6e69 7175 655f 6964 3a7b 7479  s:{unique_id:{ty
-001651a0: 7065 3a22 7374 7269 6e67 227d 7d7d 292e  pe:"string"}}}).
-001651b0: 7374 6174 6528 2264 6274 2e65 7870 6f73  state("dbt.expos
-001651c0: 7572 6522 2c7b 7572 6c3a 2265 7870 6f73  ure",{url:"expos
-001651d0: 7572 652f 3a75 6e69 7175 655f 6964 3f73  ure/:unique_id?s
-001651e0: 6563 7469 6f6e 2622 2b6e 2c63 6f6e 7472  ection&"+n,contr
-001651f0: 6f6c 6c65 723a 2245 7870 6f73 7572 6543  oller:"ExposureC
-00165200: 7472 6c22 2c74 656d 706c 6174 6555 726c  trl",templateUrl
-00165210: 3a69 2e65 7870 6f73 7572 652c 7061 7261  :i.exposure,para
-00165220: 6d73 3a7b 756e 6971 7565 5f69 643a 7b74  ms:{unique_id:{t
-00165230: 7970 653a 2273 7472 696e 6722 7d7d 7d29  ype:"string"}}})
-00165240: 2e73 7461 7465 2822 6462 742e 6d65 7472  .state("dbt.metr
-00165250: 6963 222c 7b75 726c 3a22 6d65 7472 6963  ic",{url:"metric
-00165260: 2f3a 756e 6971 7565 5f69 643f 7365 6374  /:unique_id?sect
-00165270: 696f 6e26 222b 6e2c 636f 6e74 726f 6c6c  ion&"+n,controll
-00165280: 6572 3a22 4d65 7472 6963 4374 726c 222c  er:"MetricCtrl",
-00165290: 7465 6d70 6c61 7465 5572 6c3a 692e 6d65  templateUrl:i.me
-001652a0: 7472 6963 2c70 6172 616d 733a 7b75 6e69  tric,params:{uni
-001652b0: 7175 655f 6964 3a7b 7479 7065 3a22 7374  que_id:{type:"st
-001652c0: 7269 6e67 227d 7d7d 292e 7374 6174 6528  ring"}}}).state(
-001652d0: 2264 6274 2e73 656d 616e 7469 635f 6d6f  "dbt.semantic_mo
-001652e0: 6465 6c22 2c7b 7572 6c3a 2273 656d 616e  del",{url:"seman
-001652f0: 7469 635f 6d6f 6465 6c2f 3a75 6e69 7175  tic_model/:uniqu
-00165300: 655f 6964 3f73 6563 7469 6f6e 2622 2b6e  e_id?section&"+n
-00165310: 2c63 6f6e 7472 6f6c 6c65 723a 2253 656d  ,controller:"Sem
-00165320: 616e 7469 634d 6f64 656c 4374 726c 222c  anticModelCtrl",
-00165330: 7465 6d70 6c61 7465 5572 6c3a 692e 7365  templateUrl:i.se
-00165340: 6d61 6e74 6963 5f6d 6f64 656c 2c70 6172  mantic_model,par
-00165350: 616d 733a 7b75 6e69 7175 655f 6964 3a7b  ams:{unique_id:{
-00165360: 7479 7065 3a22 7374 7269 6e67 227d 7d7d  type:"string"}}}
-00165370: 292e 7374 6174 6528 2264 6274 2e6f 7065  ).state("dbt.ope
-00165380: 7261 7469 6f6e 222c 7b75 726c 3a22 6f70  ration",{url:"op
-00165390: 6572 6174 696f 6e2f 3a75 6e69 7175 655f  eration/:unique_
-001653a0: 6964 3f73 6563 7469 6f6e 2622 2b6e 2c63  id?section&"+n,c
-001653b0: 6f6e 7472 6f6c 6c65 723a 224f 7065 7261  ontroller:"Opera
-001653c0: 7469 6f6e 4374 726c 222c 7465 6d70 6c61  tionCtrl",templa
-001653d0: 7465 5572 6c3a 692e 6f70 6572 6174 696f  teUrl:i.operatio
-001653e0: 6e2c 7061 7261 6d73 3a7b 756e 6971 7565  n,params:{unique
-001653f0: 5f69 643a 7b74 7970 653a 2273 7472 696e  _id:{type:"strin
-00165400: 6722 7d7d 7d29 7d5d 297d 2c66 756e 6374  g"}}})}])},funct
-00165410: 696f 6e28 652c 7429 7b76 6172 206e 3d22  ion(e,t){var n="
-00165420: 2f6d 6169 6e2f 6d61 696e 2e68 746d 6c22  /main/main.html"
-00165430: 3b77 696e 646f 772e 616e 6775 6c61 722e  ;window.angular.
-00165440: 6d6f 6475 6c65 2822 6e67 2229 2e72 756e  module("ng").run
-00165450: 285b 2224 7465 6d70 6c61 7465 4361 6368  (["$templateCach
-00165460: 6522 2c66 756e 6374 696f 6e28 6529 7b65  e",function(e){e
-00165470: 2e70 7574 286e 2c27 3c73 7479 6c65 3e5c  .put(n,'<style>\
-00165480: 6e2e 6e6f 2d78 2d6f 7665 7266 6c6f 7720  n.no-x-overflow 
-00165490: 7b5c 6e20 2020 206f 7665 7266 6c6f 772d  {\n    overflow-
-001654a0: 783a 2068 6964 6465 6e3b 5c6e 7d5c 6e5c  x: hidden;\n}\n\
-001654b0: 6e2e 6c6f 676f 207b 5c6e 2020 2020 7769  n.logo {\n    wi
-001654c0: 6474 683a 2031 3430 7078 3b5c 6e20 2020  dth: 140px;\n   
-001654d0: 2068 6569 6768 743a 2034 3670 7820 3b5c   height: 46px ;\
-001654e0: 6e7d 5c6e 3c2f 7374 796c 653e 5c6e 5c6e  n}\n</style>\n\n
-001654f0: 3c64 6976 3e5c 6e20 2020 203c 6772 6170  <div>\n    <grap
-00165500: 682d 6c61 756e 6368 6572 3e3c 2f67 7261  h-launcher></gra
-00165510: 7068 2d6c 6175 6e63 6865 723e 5c6e 5c6e  ph-launcher>\n\n
-00165520: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00165530: 6170 7020 6170 702d 726f 7722 3e5c 6e20  app app-row">\n 
-00165540: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00165550: 733d 2261 7070 2d6d 656e 7520 6170 702d  s="app-menu app-
-00165560: 636f 6c75 6d6e 223e 5c6e 2020 2020 2020  column">\n      
-00165570: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00165580: 3d22 6170 702d 6f76 6572 6c61 7922 2064  ="app-overlay" d
-00165590: 6174 612d 746f 6767 6c65 3d22 2e61 7070  ata-toggle=".app
-001655a0: 2d6d 656e 7522 3e3c 2f64 6976 3e5c 6e20  -menu"></div>\n 
-001655b0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-001655c0: 636c 6173 733d 2261 7070 2d68 6561 6465  class="app-heade
-001655d0: 7220 6170 702d 6e61 7662 6172 2061 7070  r app-navbar app
-001655e0: 2d73 6861 646f 7720 6170 702d 7061 6422  -shadow app-pad"
-001655f0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-00165600: 2020 203c 6469 7620 636c 6173 733d 2261     <div class="a
-00165610: 7070 2d72 6f77 2061 7070 2d6d 6964 646c  pp-row app-middl
-00165620: 6522 3e5c 6e20 2020 2020 2020 2020 2020  e">\n           
-00165630: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00165640: 6173 733d 2261 7070 2d62 6f64 7922 3e5c  ass="app-body">\
-00165650: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00165660: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00165670: 6173 733d 226c 6f67 6f22 3e5c 6e20 2020  ass="logo">\n   
-00165680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00165690: 2020 2020 2020 2020 203c 6120 7569 2d73           <a ui-s
-001656a0: 7265 663d 2264 6274 2e6f 7665 7276 6965  ref="dbt.overvie
-001656b0: 7728 2922 3e5c 6e20 2020 2020 2020 2020  w()">\n         
-001656c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001656d0: 2020 2020 2020 203c 696d 6720 7374 796c         <img styl
-001656e0: 653d 2277 6964 7468 3a20 3130 3070 783b  e="width: 100px;
-001656f0: 2068 6569 6768 743a 2034 3070 7822 2063   height: 40px" c
-00165700: 6c61 7373 3d22 6c6f 676f 2220 6e67 2d73  lass="logo" ng-s
-00165710: 7263 3d22 7b7b 206c 6f67 6f20 7d7d 2220  rc="{{ logo }}" 
-00165720: 2f3e 5c6e 2020 2020 2020 2020 2020 2020  />\n            
-00165730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00165740: 3c2f 613e 5c6e 2020 2020 2020 2020 2020  </a>\n          
-00165750: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00165760: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
-00165770: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00165780: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00165790: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
-001657a0: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
-001657b0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-001657c0: 6c61 7373 3d22 6170 702d 626f 6479 223e  lass="app-body">
-001657d0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-001657e0: 2020 3c64 6976 2063 6c61 7373 3d22 6170    <div class="ap
-001657f0: 702d 7363 726f 6c6c 2061 7070 2d70 6164  p-scroll app-pad
-00165800: 2061 7070 2d66 6c75 7368 2d72 6967 6874   app-flush-right
-00165810: 206e 6f2d 782d 6f76 6572 666c 6f77 223e   no-x-overflow">
-00165820: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00165830: 2020 2020 2020 3c6d 6f64 656c 2d74 7265        <model-tre
-00165840: 6520 7472 6565 3d22 7472 6565 223e 3c2f  e tree="tree"></
-00165850: 6d6f 6465 6c2d 7472 6565 3e5c 6e20 2020  model-tree>\n   
-00165860: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00165870: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
-00165880: 203c 2f64 6976 3e5c 6e20 2020 2020 2020   </div>\n       
+00164870: 6d65 7461 6461 7461 2e6f 776e 6572 2229  metadata.owner")
+00164880: 292c 6f3d 5f2e 756e 6971 285f 2e6d 6170  ),o=_.uniq(_.map
+00164890: 286e 2c22 6461 7461 6261 7365 2229 292c  (n,"database")),
+001648a0: 613d 5f2e 756e 6971 285f 2e6d 6170 286e  a=_.uniq(_.map(n
+001648b0: 2c22 7363 6865 6d61 2229 293b 652e 6578  ,"schema"));e.ex
+001648c0: 7472 615f 7461 626c 655f 6669 656c 6473  tra_table_fields
+001648d0: 3d5b 7b6e 616d 653a 224c 6f61 6465 7222  =[{name:"Loader"
+001648e0: 2c76 616c 7565 3a72 2e6c 6f61 6465 727d  ,value:r.loader}
+001648f0: 2c7b 6e61 6d65 3a31 3d3d 692e 6c65 6e67  ,{name:1==i.leng
+00164900: 7468 3f22 4f77 6e65 7222 3a22 4f77 6e65  th?"Owner":"Owne
+00164910: 7273 222c 7661 6c75 653a 692e 6a6f 696e  rs",value:i.join
+00164920: 2822 2c20 2229 7d2c 7b6e 616d 653a 313d  (", ")},{name:1=
+00164930: 3d6f 2e6c 656e 6774 683f 2244 6174 6162  =o.length?"Datab
+00164940: 6173 6522 3a22 4461 7461 6261 7365 7322  ase":"Databases"
+00164950: 2c76 616c 7565 3a6f 2e6a 6f69 6e28 222c  ,value:o.join(",
+00164960: 2022 297d 2c7b 6e61 6d65 3a31 3d3d 612e   ")},{name:1==a.
+00164970: 6c65 6e67 7468 3f22 5363 6865 6d61 223a  length?"Schema":
+00164980: 2253 6368 656d 6173 222c 7661 6c75 653a  "Schemas",value:
+00164990: 612e 6a6f 696e 2822 2c20 2229 7d2c 7b6e  a.join(", ")},{n
+001649a0: 616d 653a 2254 6162 6c65 7322 2c76 616c  ame:"Tables",val
+001649b0: 7565 3a6e 2e6c 656e 6774 687d 5d7d 7d29  ue:n.length}]}})
+001649c0: 297d 5d29 7d2c 6675 6e63 7469 6f6e 2865  )}])},function(e
+001649d0: 2c74 2c6e 297b 636f 6e73 7420 723d 6e28  ,t,n){const r=n(
+001649e0: 3929 2c69 3d7b 6d61 696e 3a6e 2834 3832  9),i={main:n(482
+001649f0: 292c 6f76 6572 7669 6577 3a6e 2834 3833  ),overview:n(483
+00164a00: 292c 6772 6170 683a 6e28 3438 3429 2c73  ),graph:n(484),s
+00164a10: 6f75 7263 653a 6e28 3230 3529 2c73 6f75  ource:n(205),sou
+00164a20: 7263 655f 6c69 7374 3a6e 2834 3835 292c  rce_list:n(485),
+00164a30: 6d6f 6465 6c3a 6e28 3438 3629 2c73 6f75  model:n(486),sou
+00164a40: 7263 653a 6e28 3230 3529 2c73 6e61 7073  rce:n(205),snaps
+00164a50: 686f 743a 6e28 3438 3729 2c73 6565 643a  hot:n(487),seed:
+00164a60: 6e28 3438 3829 2c75 6e69 745f 7465 7374  n(488),unit_test
+00164a70: 3a6e 2834 3839 292c 7465 7374 3a6e 2834  :n(489),test:n(4
+00164a80: 3930 292c 616e 616c 7973 6973 3a6e 2834  90),analysis:n(4
+00164a90: 3931 292c 6d61 6372 6f3a 6e28 3439 3229  91),macro:n(492)
+00164aa0: 2c65 7870 6f73 7572 653a 6e28 3439 3329  ,exposure:n(493)
+00164ab0: 2c6d 6574 7269 633a 6e28 3439 3429 2c73  ,metric:n(494),s
+00164ac0: 656d 616e 7469 635f 6d6f 6465 6c3a 6e28  emantic_model:n(
+00164ad0: 3439 3529 2c6f 7065 7261 7469 6f6e 3a6e  495),operation:n
+00164ae0: 2834 3936 297d 3b72 2e6d 6f64 756c 6528  (496)};r.module(
+00164af0: 2264 6274 2229 2e63 6f6e 6669 6728 5b22  "dbt").config(["
+00164b00: 2473 7461 7465 5072 6f76 6964 6572 222c  $stateProvider",
+00164b10: 2224 7572 6c52 6f75 7465 7250 726f 7669  "$urlRouterProvi
+00164b20: 6465 7222 2c66 756e 6374 696f 6e28 652c  der",function(e,
+00164b30: 7429 7b76 6172 206e 3d22 675f 7626 675f  t){var n="g_v&g_
+00164b40: 6926 675f 6526 675f 7026 675f 6e22 3b74  i&g_e&g_p&g_n";t
+00164b50: 2e6f 7468 6572 7769 7365 2822 2f6f 7665  .otherwise("/ove
+00164b60: 7276 6965 7722 292c 652e 7374 6174 6528  rview"),e.state(
+00164b70: 2264 6274 222c 7b75 726c 3a22 2f22 2c61  "dbt",{url:"/",a
+00164b80: 6273 7472 6163 743a 2130 2c63 6f6e 7472  bstract:!0,contr
+00164b90: 6f6c 6c65 723a 224d 6169 6e43 6f6e 7472  oller:"MainContr
+00164ba0: 6f6c 6c65 7222 2c74 656d 706c 6174 6555  oller",templateU
+00164bb0: 726c 3a69 2e6d 6169 6e7d 292e 7374 6174  rl:i.main}).stat
+00164bc0: 6528 2264 6274 2e6f 7665 7276 6965 7722  e("dbt.overview"
+00164bd0: 2c7b 7572 6c3a 226f 7665 7276 6965 773f  ,{url:"overview?
+00164be0: 222b 6e2c 636f 6e74 726f 6c6c 6572 3a22  "+n,controller:"
+00164bf0: 4f76 6572 7669 6577 4374 726c 222c 7465  OverviewCtrl",te
+00164c00: 6d70 6c61 7465 5572 6c3a 692e 6f76 6572  mplateUrl:i.over
+00164c10: 7669 6577 7d29 2e73 7461 7465 2822 6462  view}).state("db
+00164c20: 742e 7072 6f6a 6563 745f 6f76 6572 7669  t.project_overvi
+00164c30: 6577 222c 7b75 726c 3a22 6f76 6572 7669  ew",{url:"overvi
+00164c40: 6577 2f3a 7072 6f6a 6563 745f 6e61 6d65  ew/:project_name
+00164c50: 3f22 2b6e 2c63 6f6e 7472 6f6c 6c65 723a  ?"+n,controller:
+00164c60: 224f 7665 7276 6965 7743 7472 6c22 2c74  "OverviewCtrl",t
+00164c70: 656d 706c 6174 6555 726c 3a69 2e6f 7665  emplateUrl:i.ove
+00164c80: 7276 6965 772c 7061 7261 6d73 3a7b 7072  rview,params:{pr
+00164c90: 6f6a 6563 745f 6e61 6d65 3a7b 7479 7065  oject_name:{type
+00164ca0: 3a22 7374 7269 6e67 227d 7d7d 292e 7374  :"string"}}}).st
+00164cb0: 6174 6528 2264 6274 2e67 7261 7068 222c  ate("dbt.graph",
+00164cc0: 7b75 726c 3a22 6772 6170 6822 2c63 6f6e  {url:"graph",con
+00164cd0: 7472 6f6c 6c65 723a 2247 7261 7068 4374  troller:"GraphCt
+00164ce0: 726c 222c 7465 6d70 6c61 7465 5572 6c3a  rl",templateUrl:
+00164cf0: 692e 6772 6170 687d 292e 7374 6174 6528  i.graph}).state(
+00164d00: 2264 6274 2e6d 6f64 656c 222c 7b75 726c  "dbt.model",{url
+00164d10: 3a22 6d6f 6465 6c2f 3a75 6e69 7175 655f  :"model/:unique_
+00164d20: 6964 3f73 6563 7469 6f6e 2622 2b6e 2c63  id?section&"+n,c
+00164d30: 6f6e 7472 6f6c 6c65 723a 224d 6f64 656c  ontroller:"Model
+00164d40: 4374 726c 222c 7465 6d70 6c61 7465 5572  Ctrl",templateUr
+00164d50: 6c3a 692e 6d6f 6465 6c2c 7061 7261 6d73  l:i.model,params
+00164d60: 3a7b 756e 6971 7565 5f69 643a 7b74 7970  :{unique_id:{typ
+00164d70: 653a 2273 7472 696e 6722 7d7d 7d29 2e73  e:"string"}}}).s
+00164d80: 7461 7465 2822 6462 742e 7365 6564 222c  tate("dbt.seed",
+00164d90: 7b75 726c 3a22 7365 6564 2f3a 756e 6971  {url:"seed/:uniq
+00164da0: 7565 5f69 643f 7365 6374 696f 6e26 222b  ue_id?section&"+
+00164db0: 6e2c 636f 6e74 726f 6c6c 6572 3a22 5365  n,controller:"Se
+00164dc0: 6564 4374 726c 222c 7465 6d70 6c61 7465  edCtrl",template
+00164dd0: 5572 6c3a 692e 7365 6564 2c70 6172 616d  Url:i.seed,param
+00164de0: 733a 7b75 6e69 7175 655f 6964 3a7b 7479  s:{unique_id:{ty
+00164df0: 7065 3a22 7374 7269 6e67 227d 7d7d 292e  pe:"string"}}}).
+00164e00: 7374 6174 6528 2264 6274 2e73 6e61 7073  state("dbt.snaps
+00164e10: 686f 7422 2c7b 7572 6c3a 2273 6e61 7073  hot",{url:"snaps
+00164e20: 686f 742f 3a75 6e69 7175 655f 6964 3f73  hot/:unique_id?s
+00164e30: 6563 7469 6f6e 2622 2b6e 2c63 6f6e 7472  ection&"+n,contr
+00164e40: 6f6c 6c65 723a 2253 6e61 7073 686f 7443  oller:"SnapshotC
+00164e50: 7472 6c22 2c74 656d 706c 6174 6555 726c  trl",templateUrl
+00164e60: 3a69 2e73 6e61 7073 686f 742c 7061 7261  :i.snapshot,para
+00164e70: 6d73 3a7b 756e 6971 7565 5f69 643a 7b74  ms:{unique_id:{t
+00164e80: 7970 653a 2273 7472 696e 6722 7d7d 7d29  ype:"string"}}})
+00164e90: 2e73 7461 7465 2822 6462 742e 756e 6974  .state("dbt.unit
+00164ea0: 5f74 6573 7422 2c7b 7572 6c3a 2275 6e69  _test",{url:"uni
+00164eb0: 745f 7465 7374 2f3a 756e 6971 7565 5f69  t_test/:unique_i
+00164ec0: 643f 7365 6374 696f 6e26 222b 6e2c 636f  d?section&"+n,co
+00164ed0: 6e74 726f 6c6c 6572 3a22 5465 7374 4374  ntroller:"TestCt
+00164ee0: 726c 222c 7465 6d70 6c61 7465 5572 6c3a  rl",templateUrl:
+00164ef0: 692e 756e 6974 5f74 6573 742c 7061 7261  i.unit_test,para
+00164f00: 6d73 3a7b 756e 6971 7565 5f69 643a 7b74  ms:{unique_id:{t
+00164f10: 7970 653a 2273 7472 696e 6722 7d7d 7d29  ype:"string"}}})
+00164f20: 2e73 7461 7465 2822 6462 742e 7465 7374  .state("dbt.test
+00164f30: 222c 7b75 726c 3a22 7465 7374 2f3a 756e  ",{url:"test/:un
+00164f40: 6971 7565 5f69 643f 7365 6374 696f 6e26  ique_id?section&
+00164f50: 222b 6e2c 636f 6e74 726f 6c6c 6572 3a22  "+n,controller:"
+00164f60: 5465 7374 4374 726c 222c 7465 6d70 6c61  TestCtrl",templa
+00164f70: 7465 5572 6c3a 692e 7465 7374 2c70 6172  teUrl:i.test,par
+00164f80: 616d 733a 7b75 6e69 7175 655f 6964 3a7b  ams:{unique_id:{
+00164f90: 7479 7065 3a22 7374 7269 6e67 227d 7d7d  type:"string"}}}
+00164fa0: 292e 7374 6174 6528 2264 6274 2e61 6e61  ).state("dbt.ana
+00164fb0: 6c79 7369 7322 2c7b 7572 6c3a 2261 6e61  lysis",{url:"ana
+00164fc0: 6c79 7369 732f 3a75 6e69 7175 655f 6964  lysis/:unique_id
+00164fd0: 3f73 6563 7469 6f6e 2622 2b6e 2c63 6f6e  ?section&"+n,con
+00164fe0: 7472 6f6c 6c65 723a 2241 6e61 6c79 7369  troller:"Analysi
+00164ff0: 7343 7472 6c22 2c74 656d 706c 6174 6555  sCtrl",templateU
+00165000: 726c 3a69 2e61 6e61 6c79 7369 732c 7061  rl:i.analysis,pa
+00165010: 7261 6d73 3a7b 756e 6971 7565 5f69 643a  rams:{unique_id:
+00165020: 7b74 7970 653a 2273 7472 696e 6722 7d7d  {type:"string"}}
+00165030: 7d29 2e73 7461 7465 2822 6462 742e 736f  }).state("dbt.so
+00165040: 7572 6365 222c 7b75 726c 3a22 736f 7572  urce",{url:"sour
+00165050: 6365 2f3a 756e 6971 7565 5f69 643f 7365  ce/:unique_id?se
+00165060: 6374 696f 6e26 222b 6e2c 636f 6e74 726f  ction&"+n,contro
+00165070: 6c6c 6572 3a22 536f 7572 6365 4374 726c  ller:"SourceCtrl
+00165080: 222c 7465 6d70 6c61 7465 5572 6c3a 692e  ",templateUrl:i.
+00165090: 736f 7572 6365 2c70 6172 616d 733a 7b75  source,params:{u
+001650a0: 6e69 7175 655f 6964 3a7b 7479 7065 3a22  nique_id:{type:"
+001650b0: 7374 7269 6e67 227d 7d7d 292e 7374 6174  string"}}}).stat
+001650c0: 6528 2264 6274 2e73 6f75 7263 655f 6c69  e("dbt.source_li
+001650d0: 7374 222c 7b75 726c 3a22 736f 7572 6365  st",{url:"source
+001650e0: 5f6c 6973 742f 3a73 6f75 7263 653f 7365  _list/:source?se
+001650f0: 6374 696f 6e26 222b 6e2c 636f 6e74 726f  ction&"+n,contro
+00165100: 6c6c 6572 3a22 536f 7572 6365 4c69 7374  ller:"SourceList
+00165110: 4374 726c 222c 7465 6d70 6c61 7465 5572  Ctrl",templateUr
+00165120: 6c3a 692e 736f 7572 6365 5f6c 6973 742c  l:i.source_list,
+00165130: 7061 7261 6d73 3a7b 736f 7572 6365 3a7b  params:{source:{
+00165140: 7479 7065 3a22 7374 7269 6e67 227d 7d7d  type:"string"}}}
+00165150: 292e 7374 6174 6528 2264 6274 2e6d 6163  ).state("dbt.mac
+00165160: 726f 222c 7b75 726c 3a22 6d61 6372 6f2f  ro",{url:"macro/
+00165170: 3a75 6e69 7175 655f 6964 3f73 6563 7469  :unique_id?secti
+00165180: 6f6e 222c 636f 6e74 726f 6c6c 6572 3a22  on",controller:"
+00165190: 4d61 6372 6f43 7472 6c22 2c74 656d 706c  MacroCtrl",templ
+001651a0: 6174 6555 726c 3a69 2e6d 6163 726f 2c70  ateUrl:i.macro,p
+001651b0: 6172 616d 733a 7b75 6e69 7175 655f 6964  arams:{unique_id
+001651c0: 3a7b 7479 7065 3a22 7374 7269 6e67 227d  :{type:"string"}
+001651d0: 7d7d 292e 7374 6174 6528 2264 6274 2e65  }}).state("dbt.e
+001651e0: 7870 6f73 7572 6522 2c7b 7572 6c3a 2265  xposure",{url:"e
+001651f0: 7870 6f73 7572 652f 3a75 6e69 7175 655f  xposure/:unique_
+00165200: 6964 3f73 6563 7469 6f6e 2622 2b6e 2c63  id?section&"+n,c
+00165210: 6f6e 7472 6f6c 6c65 723a 2245 7870 6f73  ontroller:"Expos
+00165220: 7572 6543 7472 6c22 2c74 656d 706c 6174  ureCtrl",templat
+00165230: 6555 726c 3a69 2e65 7870 6f73 7572 652c  eUrl:i.exposure,
+00165240: 7061 7261 6d73 3a7b 756e 6971 7565 5f69  params:{unique_i
+00165250: 643a 7b74 7970 653a 2273 7472 696e 6722  d:{type:"string"
+00165260: 7d7d 7d29 2e73 7461 7465 2822 6462 742e  }}}).state("dbt.
+00165270: 6d65 7472 6963 222c 7b75 726c 3a22 6d65  metric",{url:"me
+00165280: 7472 6963 2f3a 756e 6971 7565 5f69 643f  tric/:unique_id?
+00165290: 7365 6374 696f 6e26 222b 6e2c 636f 6e74  section&"+n,cont
+001652a0: 726f 6c6c 6572 3a22 4d65 7472 6963 4374  roller:"MetricCt
+001652b0: 726c 222c 7465 6d70 6c61 7465 5572 6c3a  rl",templateUrl:
+001652c0: 692e 6d65 7472 6963 2c70 6172 616d 733a  i.metric,params:
+001652d0: 7b75 6e69 7175 655f 6964 3a7b 7479 7065  {unique_id:{type
+001652e0: 3a22 7374 7269 6e67 227d 7d7d 292e 7374  :"string"}}}).st
+001652f0: 6174 6528 2264 6274 2e73 656d 616e 7469  ate("dbt.semanti
+00165300: 635f 6d6f 6465 6c22 2c7b 7572 6c3a 2273  c_model",{url:"s
+00165310: 656d 616e 7469 635f 6d6f 6465 6c2f 3a75  emantic_model/:u
+00165320: 6e69 7175 655f 6964 3f73 6563 7469 6f6e  nique_id?section
+00165330: 2622 2b6e 2c63 6f6e 7472 6f6c 6c65 723a  &"+n,controller:
+00165340: 2253 656d 616e 7469 634d 6f64 656c 4374  "SemanticModelCt
+00165350: 726c 222c 7465 6d70 6c61 7465 5572 6c3a  rl",templateUrl:
+00165360: 692e 7365 6d61 6e74 6963 5f6d 6f64 656c  i.semantic_model
+00165370: 2c70 6172 616d 733a 7b75 6e69 7175 655f  ,params:{unique_
+00165380: 6964 3a7b 7479 7065 3a22 7374 7269 6e67  id:{type:"string
+00165390: 227d 7d7d 292e 7374 6174 6528 2264 6274  "}}}).state("dbt
+001653a0: 2e6f 7065 7261 7469 6f6e 222c 7b75 726c  .operation",{url
+001653b0: 3a22 6f70 6572 6174 696f 6e2f 3a75 6e69  :"operation/:uni
+001653c0: 7175 655f 6964 3f73 6563 7469 6f6e 2622  que_id?section&"
+001653d0: 2b6e 2c63 6f6e 7472 6f6c 6c65 723a 224f  +n,controller:"O
+001653e0: 7065 7261 7469 6f6e 4374 726c 222c 7465  perationCtrl",te
+001653f0: 6d70 6c61 7465 5572 6c3a 692e 6f70 6572  mplateUrl:i.oper
+00165400: 6174 696f 6e2c 7061 7261 6d73 3a7b 756e  ation,params:{un
+00165410: 6971 7565 5f69 643a 7b74 7970 653a 2273  ique_id:{type:"s
+00165420: 7472 696e 6722 7d7d 7d29 7d5d 297d 2c66  tring"}}})}])},f
+00165430: 756e 6374 696f 6e28 652c 7429 7b76 6172  unction(e,t){var
+00165440: 206e 3d22 2f6d 6169 6e2f 6d61 696e 2e68   n="/main/main.h
+00165450: 746d 6c22 3b77 696e 646f 772e 616e 6775  tml";window.angu
+00165460: 6c61 722e 6d6f 6475 6c65 2822 6e67 2229  lar.module("ng")
+00165470: 2e72 756e 285b 2224 7465 6d70 6c61 7465  .run(["$template
+00165480: 4361 6368 6522 2c66 756e 6374 696f 6e28  Cache",function(
+00165490: 6529 7b65 2e70 7574 286e 2c27 3c73 7479  e){e.put(n,'<sty
+001654a0: 6c65 3e5c 6e2e 6e6f 2d78 2d6f 7665 7266  le>\n.no-x-overf
+001654b0: 6c6f 7720 7b5c 6e20 2020 206f 7665 7266  low {\n    overf
+001654c0: 6c6f 772d 783a 2068 6964 6465 6e3b 5c6e  low-x: hidden;\n
+001654d0: 7d5c 6e5c 6e2e 6c6f 676f 207b 5c6e 2020  }\n\n.logo {\n  
+001654e0: 2020 7769 6474 683a 2031 3430 7078 3b5c    width: 140px;\
+001654f0: 6e20 2020 2068 6569 6768 743a 2034 3670  n    height: 46p
+00165500: 7820 3b5c 6e7d 5c6e 3c2f 7374 796c 653e  x ;\n}\n</style>
+00165510: 5c6e 5c6e 3c64 6976 3e5c 6e20 2020 203c  \n\n<div>\n    <
+00165520: 6772 6170 682d 6c61 756e 6368 6572 3e3c  graph-launcher><
+00165530: 2f67 7261 7068 2d6c 6175 6e63 6865 723e  /graph-launcher>
+00165540: 5c6e 5c6e 2020 2020 3c64 6976 2063 6c61  \n\n    <div cla
+00165550: 7373 3d22 6170 7020 6170 702d 726f 7722  ss="app app-row"
+00165560: 3e5c 6e20 2020 2020 2020 203c 6469 7620  >\n        <div 
+00165570: 636c 6173 733d 2261 7070 2d6d 656e 7520  class="app-menu 
+00165580: 6170 702d 636f 6c75 6d6e 223e 5c6e 2020  app-column">\n  
+00165590: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+001655a0: 6c61 7373 3d22 6170 702d 6f76 6572 6c61  lass="app-overla
+001655b0: 7922 2064 6174 612d 746f 6767 6c65 3d22  y" data-toggle="
+001655c0: 2e61 7070 2d6d 656e 7522 3e3c 2f64 6976  .app-menu"></div
+001655d0: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
+001655e0: 6469 7620 636c 6173 733d 2261 7070 2d68  div class="app-h
+001655f0: 6561 6465 7220 6170 702d 6e61 7662 6172  eader app-navbar
+00165600: 2061 7070 2d73 6861 646f 7720 6170 702d   app-shadow app-
+00165610: 7061 6422 3e5c 6e20 2020 2020 2020 2020  pad">\n         
+00165620: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00165630: 733d 2261 7070 2d72 6f77 2061 7070 2d6d  s="app-row app-m
+00165640: 6964 646c 6522 3e5c 6e20 2020 2020 2020  iddle">\n       
+00165650: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00165660: 7620 636c 6173 733d 2261 7070 2d62 6f64  v class="app-bod
+00165670: 7922 3e5c 6e20 2020 2020 2020 2020 2020  y">\n           
+00165680: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00165690: 7620 636c 6173 733d 226c 6f67 6f22 3e5c  v class="logo">\
+001656a0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+001656b0: 2020 2020 2020 2020 2020 2020 203c 6120               <a 
+001656c0: 7569 2d73 7265 663d 2264 6274 2e6f 7665  ui-sref="dbt.ove
+001656d0: 7276 6965 7728 2922 3e5c 6e20 2020 2020  rview()">\n     
+001656e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001656f0: 2020 2020 2020 2020 2020 203c 696d 6720             <img 
+00165700: 7374 796c 653d 2277 6964 7468 3a20 3130  style="width: 10
+00165710: 3070 783b 2068 6569 6768 743a 2034 3070  0px; height: 40p
+00165720: 7822 2063 6c61 7373 3d22 6c6f 676f 2220  x" class="logo" 
+00165730: 6e67 2d73 7263 3d22 7b7b 206c 6f67 6f20  ng-src="{{ logo 
+00165740: 7d7d 2220 2f3e 5c6e 2020 2020 2020 2020  }}" />\n        
+00165750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00165760: 2020 2020 3c2f 613e 5c6e 2020 2020 2020      </a>\n      
+00165770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00165780: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
+00165790: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+001657a0: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
+001657b0: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
+001657c0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+001657d0: 5c6e 2020 2020 2020 2020 2020 2020 3c64  \n            <d
+001657e0: 6976 2063 6c61 7373 3d22 6170 702d 626f  iv class="app-bo
+001657f0: 6479 223e 5c6e 2020 2020 2020 2020 2020  dy">\n          
+00165800: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00165810: 3d22 6170 702d 7363 726f 6c6c 2061 7070  ="app-scroll app
+00165820: 2d70 6164 2061 7070 2d66 6c75 7368 2d72  -pad app-flush-r
+00165830: 6967 6874 206e 6f2d 782d 6f76 6572 666c  ight no-x-overfl
+00165840: 6f77 223e 5c6e 2020 2020 2020 2020 2020  ow">\n          
+00165850: 2020 2020 2020 2020 2020 3c6d 6f64 656c            <model
+00165860: 2d74 7265 6520 7472 6565 3d22 7472 6565  -tree tree="tree
+00165870: 223e 3c2f 6d6f 6465 6c2d 7472 6565 3e5c  "></model-tree>\
+00165880: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
 00165890: 203c 2f64 6976 3e5c 6e20 2020 2020 2020   </div>\n       
-001658a0: 203c 6469 7620 636c 6173 733d 2261 7070   <div class="app
-001658b0: 2d63 6f6e 7465 6e74 2061 7070 2d63 6f6c  -content app-col
-001658c0: 756d 6e22 3e5c 6e20 2020 2020 2020 2020  umn">\n         
-001658d0: 2020 203c 6469 7620 636c 6173 733d 2261     <div class="a
-001658e0: 7070 2d68 6561 6465 7220 6170 702d 6e61  pp-header app-na
-001658f0: 7662 6172 2061 7070 2d73 6861 646f 7722  vbar app-shadow"
-00165900: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-00165910: 2020 203c 6469 7620 636c 6173 733d 2261     <div class="a
-00165920: 7070 2d66 7261 6d65 2061 7070 2d70 6164  pp-frame app-pad
-00165930: 2061 7070 2d72 6f77 2061 7070 2d6d 6964   app-row app-mid
-00165940: 646c 6522 3e5c 6e20 2020 2020 2020 2020  dle">\n         
-00165950: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00165960: 696e 7075 745c 6e20 2020 2020 2020 2020  input\n         
+001658a0: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
+001658b0: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
+001658c0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+001658d0: 2261 7070 2d63 6f6e 7465 6e74 2061 7070  "app-content app
+001658e0: 2d63 6f6c 756d 6e22 3e5c 6e20 2020 2020  -column">\n     
+001658f0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00165900: 733d 2261 7070 2d68 6561 6465 7220 6170  s="app-header ap
+00165910: 702d 6e61 7662 6172 2061 7070 2d73 6861  p-navbar app-sha
+00165920: 646f 7722 3e5c 6e20 2020 2020 2020 2020  dow">\n         
+00165930: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+00165940: 733d 2261 7070 2d66 7261 6d65 2061 7070  s="app-frame app
+00165950: 2d70 6164 2061 7070 2d72 6f77 2061 7070  -pad app-row app
+00165960: 2d6d 6964 646c 6522 3e5c 6e20 2020 2020  -middle">\n     
 00165970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00165980: 2020 2069 643d 2273 6561 7263 6822 5c6e     id="search"\n
+00165980: 2020 203c 696e 7075 745c 6e20 2020 2020     <input\n     
 00165990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001659a0: 2020 2020 2020 2020 2020 2020 6e67 2d6d              ng-m
-001659b0: 6f64 656c 3d22 7365 6172 6368 2e71 7565  odel="search.que
-001659c0: 7279 225c 6e20 2020 2020 2020 2020 2020  ry"\n           
-001659d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001659e0: 206e 672d 666f 6375 733d 226f 6e53 6561   ng-focus="onSea
-001659f0: 7263 6846 6f63 7573 2824 6576 656e 742c  rchFocus($event,
-00165a00: 2074 7275 6529 225c 6e20 2020 2020 2020   true)"\n       
-00165a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00165a20: 2020 2020 206e 672d 6b65 7964 6f77 6e3d       ng-keydown=
-00165a30: 226f 6e53 6561 7263 684b 6579 7072 6573  "onSearchKeypres
-00165a40: 7328 2465 7665 6e74 2922 5c6e 2020 2020  s($event)"\n    
-00165a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00165a60: 2020 2020 2020 2020 7479 7065 3d22 7465          type="te
-00165a70: 7874 225c 6e20 2020 2020 2020 2020 2020  xt"\n           
-00165a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00165a90: 2063 6c61 7373 3d22 666f 726d 2d63 6f6e   class="form-con
-00165aa0: 7472 6f6c 225c 6e20 2020 2020 2020 2020  trol"\n         
-00165ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00165ac0: 2020 2070 6c61 6365 686f 6c64 6572 3d22     placeholder="
-00165ad0: 5365 6172 6368 2066 6f72 206d 6f64 656c  Search for model
-00165ae0: 732e 2e2e 2220 2f3e 5c6e 2020 2020 2020  s..." />\n      
-00165af0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00165b00: 6976 2063 6c61 7373 3d22 6170 702d 626f  iv class="app-bo
-00165b10: 6479 223e 5c6e 2020 2020 2020 2020 2020  dy">\n          
-00165b20: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00165b30: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00165b40: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00165b50: 3d22 6170 702d 666f 6f74 6572 2061 7070  ="app-footer app
-00165b60: 2d69 636e 2220 6e67 2d73 686f 773d 2273  -icn" ng-show="s
-00165b70: 6561 7263 682e 6973 5f66 6f63 7573 6564  earch.is_focused
-00165b80: 2220 6e67 2d63 6c69 636b 3d22 636c 6561  " ng-click="clea
-00165b90: 7253 6561 7263 6828 2922 3e5c 6e20 2020  rSearch()">\n   
-00165ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00165bb0: 2020 2020 203c 7376 6720 636c 6173 733d       <svg class=
-00165bc0: 2269 636e 2069 636e 2d6d 6422 3e3c 7573  "icn icn-md"><us
-00165bd0: 6520 786c 696e 6b3a 6872 6566 3d22 2369  e xlink:href="#i
-00165be0: 636e 2d63 6c6f 7365 223e 3c2f 7573 653e  cn-close"></use>
-00165bf0: 3c2f 7376 673e 5c6e 2020 2020 2020 2020  </svg>\n        
-00165c00: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00165c10: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
-00165c20: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
-00165c30: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
-00165c40: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00165c50: 2063 6c61 7373 3d5c 2761 7070 2d62 6f64   class=\'app-bod
-00165c60: 795c 2720 6e67 2d73 686f 773d 5c27 2173  y\' ng-show=\'!s
-00165c70: 6561 7263 682e 6973 5f66 6f63 7573 6564  earch.is_focused
-00165c80: 5c27 2075 692d 7669 6577 3e3c 2f64 6976  \' ui-view></div
-00165c90: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
-00165ca0: 6469 7620 636c 6173 733d 2261 7070 2d62  div class="app-b
-00165cb0: 6f64 7922 206e 672d 7368 6f77 3d22 7365  ody" ng-show="se
-00165cc0: 6172 6368 2e69 735f 666f 6375 7365 6422  arch.is_focused"
-00165cd0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-00165ce0: 2020 203c 646f 6373 2d73 6561 7263 6820     <docs-search 
-00165cf0: 7175 6572 793d 2273 6561 7263 682e 7175  query="search.qu
-00165d00: 6572 7922 2072 6573 756c 7473 3d22 7365  ery" results="se
-00165d10: 6172 6368 2e72 6573 756c 7473 2220 6f6e  arch.results" on
-00165d20: 2d73 656c 6563 743d 2263 6c65 6172 5365  -select="clearSe
-00165d30: 6172 6368 2829 223e 3c2f 646f 6373 2d73  arch()"></docs-s
-00165d40: 6561 7263 683e 5c6e 2020 2020 2020 2020  earch>\n        
-00165d50: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
-00165d60: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
-00165d70: 3c2f 6469 763e 5c6e 3c2f 6469 763e 5c6e  </div>\n</div>\n
-00165d80: 2729 7d5d 292c 652e 6578 706f 7274 733d  ')}]),e.exports=
-00165d90: 6e7d 2c66 756e 6374 696f 6e28 652c 7429  n},function(e,t)
-00165da0: 7b76 6172 206e 3d22 2f6f 7665 7276 6965  {var n="/overvie
-00165db0: 772f 6f76 6572 7669 6577 2e68 746d 6c22  w/overview.html"
-00165dc0: 3b77 696e 646f 772e 616e 6775 6c61 722e  ;window.angular.
-00165dd0: 6d6f 6475 6c65 2822 6e67 2229 2e72 756e  module("ng").run
-00165de0: 285b 2224 7465 6d70 6c61 7465 4361 6368  (["$templateCach
-00165df0: 6522 2c66 756e 6374 696f 6e28 6529 7b65  e",function(e){e
-00165e00: 2e70 7574 286e 2c27 3c64 6976 2063 6c61  .put(n,'<div cla
-00165e10: 7373 3d22 6170 702d 6465 7461 696c 7320  ss="app-details 
-00165e20: 6170 702d 7363 726f 6c6c 2061 7070 2d70  app-scroll app-p
-00165e30: 6164 223e 5c6e 2020 2020 3c61 7070 2d73  ad">\n    <app-s
-00165e40: 6372 6f6c 6c20 6469 7620 636c 6173 733d  croll div class=
-00165e50: 2261 7070 2d66 7261 6d65 2061 7070 2d70  "app-frame app-p
-00165e60: 6164 223e 5c6e 2020 2020 2020 2020 3c64  ad">\n        <d
-00165e70: 6976 2063 6c61 7373 3d22 7061 6e65 6c20  iv class="panel 
-00165e80: 7061 6e65 6c2d 6465 6661 756c 7422 3e5c  panel-default">\
-00165e90: 6e20 2020 2020 2020 2020 2020 203c 6469  n            <di
-00165ea0: 7620 636c 6173 733d 2270 616e 656c 2d62  v class="panel-b
-00165eb0: 6f64 7922 3e5c 6e20 2020 2020 2020 2020  ody">\n         
-00165ec0: 2020 2020 2020 203c 7020 6d61 726b 6564         <p marked
-00165ed0: 3d5c 276f 7665 7276 6965 775f 6d64 5c27  =\'overview_md\'
-00165ee0: 3e3c 2f70 3e5c 6e20 2020 2020 2020 2020  ></p>\n         
-00165ef0: 2020 203c 2f64 6976 3e5c 6e20 2020 2020     </div>\n     
-00165f00: 2020 203c 2f64 6976 3e5c 6e20 2020 203c     </div>\n    <
-00165f10: 2f64 6976 3e5c 6e3c 2f64 6976 3e5c 6e27  /div>\n</div>\n'
-00165f20: 297d 5d29 2c65 2e65 7870 6f72 7473 3d6e  )}]),e.exports=n
-00165f30: 7d2c 6675 6e63 7469 6f6e 2865 2c74 297b  },function(e,t){
-00165f40: 7661 7220 6e3d 222f 6772 6170 682f 6772  var n="/graph/gr
-00165f50: 6170 682e 6874 6d6c 223b 7769 6e64 6f77  aph.html";window
-00165f60: 2e61 6e67 756c 6172 2e6d 6f64 756c 6528  .angular.module(
-00165f70: 226e 6722 292e 7275 6e28 5b22 2474 656d  "ng").run(["$tem
-00165f80: 706c 6174 6543 6163 6865 222c 6675 6e63  plateCache",func
-00165f90: 7469 6f6e 2865 297b 652e 7075 7428 6e2c  tion(e){e.put(n,
-00165fa0: 273c 6469 7620 6e67 2d63 6f6e 7472 6f6c  '<div ng-control
-00165fb0: 6c65 723d 2247 7261 7068 4374 726c 2220  ler="GraphCtrl" 
-00165fc0: 6964 3d5c 2767 7261 7068 2d63 6f6e 7461  id=\'graph-conta
-00165fd0: 696e 6572 5c27 2073 7479 6c65 3d22 7769  iner\' style="wi
-00165fe0: 6474 683a 2031 3030 2522 3e5c 6e20 2020  dth: 100%">\n   
-00165ff0: 203c 6469 7620 636c 6173 733d 5c27 726f   <div class=\'ro
-00166000: 7720 7669 7a2d 636f 6e74 6169 6e65 725c  w viz-container\
-00166010: 2720 7374 796c 653d 226d 6172 6769 6e3a  ' style="margin:
-00166020: 2030 223e 5c6e 2020 2020 2020 2020 3c64   0">\n        <d
-00166030: 6976 2063 6c61 7373 3d5c 2763 6f6c 2d6d  iv class=\'col-m
-00166040: 642d 3132 5c27 3e5c 6e20 2020 2020 2020  d-12\'>\n       
-00166050: 2020 2020 2020 3c64 6976 2067 7261 7068        <div graph
-00166060: 2d76 697a 5c6e 2020 2020 2020 2020 2020  -viz\n          
-00166070: 2020 2020 2020 2020 2020 2020 2020 7669                vi
-00166080: 7a2d 6f70 7469 6f6e 733d 2267 7261 7068  z-options="graph
-00166090: 2e6f 7074 696f 6e73 225c 6e20 2020 2020  .options"\n     
-001660a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001660b0: 2020 2076 697a 2d65 6c65 6d65 6e74 733d     viz-elements=
-001660c0: 2267 7261 7068 2e65 6c65 6d65 6e74 7322  "graph.elements"
-001660d0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-001660e0: 2020 2020 2020 2020 2020 7669 7a2d 7374            viz-st
-001660f0: 796c 653d 2267 7261 7068 2e73 7479 6c65  yle="graph.style
-00166100: 225c 6e20 2020 2020 2020 2020 2020 2020  "\n             
-00166110: 2020 2020 2020 2020 2020 2076 697a 2d6c             viz-l
-00166120: 6179 6f75 743d 2267 7261 7068 2e6c 6179  ayout="graph.lay
-00166130: 6f75 7422 5c6e 2020 2020 2020 2020 2020  out"\n          
-00166140: 2020 2020 2020 2020 2020 2020 2020 7669                vi
-00166150: 7a2d 7265 6164 793d 2267 7261 7068 2e72  z-ready="graph.r
-00166160: 6561 6479 225c 6e20 2020 2020 2020 2020  eady"\n         
-00166170: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00166180: 697a 2d73 697a 653d 227b 6865 6967 6874  iz-size="{height
-00166190: 3a20 5c27 3830 3070 785c 272c 2077 6964  : \'800px\', wid
-001661a0: 7468 3a20 5c27 3130 3025 5c27 7d22 3e3c  th: \'100%\'}"><
-001661b0: 2f64 6976 3e5c 6e20 2020 2020 2020 203c  /div>\n        <
-001661c0: 2f64 6976 3e5c 6e20 2020 203c 2f64 6976  /div>\n    </div
-001661d0: 3e5c 6e3c 2f64 6976 3e5c 6e27 297d 5d29  >\n</div>\n')}])
-001661e0: 2c65 2e65 7870 6f72 7473 3d6e 7d2c 6675  ,e.exports=n},fu
-001661f0: 6e63 7469 6f6e 2865 2c74 297b 7661 7220  nction(e,t){var 
-00166200: 6e3d 222f 736f 7572 6365 732f 736f 7572  n="/sources/sour
-00166210: 6365 5f6c 6973 742e 6874 6d6c 223b 7769  ce_list.html";wi
-00166220: 6e64 6f77 2e61 6e67 756c 6172 2e6d 6f64  ndow.angular.mod
-00166230: 756c 6528 226e 6722 292e 7275 6e28 5b22  ule("ng").run(["
-00166240: 2474 656d 706c 6174 6543 6163 6865 222c  $templateCache",
-00166250: 6675 6e63 7469 6f6e 2865 297b 652e 7075  function(e){e.pu
-00166260: 7428 6e2c 273c 7374 796c 653e 5c6e 2f2a  t(n,'<style>\n/*
-00166270: 2054 4f44 4f20 2a2f 5c6e 2e73 6563 7469   TODO */\n.secti
-00166280: 6f6e 2d74 6172 6765 7420 7b5c 6e20 2020  on-target {\n   
-00166290: 2074 6f70 3a20 2d38 656d 3b5c 6e7d 5c6e   top: -8em;\n}\n
-001662a0: 5c6e 2e6e 6f66 6c65 7820 7b5c 6e20 2020  \n.noflex {\n   
-001662b0: 2066 6c65 783a 2030 2030 2031 3630 7078   flex: 0 0 160px
-001662c0: 2021 696d 706f 7274 616e 743b 5c6e 7d5c   !important;\n}\
-001662d0: 6e5c 6e2e 6869 6768 6c69 6768 7420 7b5c  n\n.highlight {\
-001662e0: 6e20 2020 2063 6f6c 6f72 3a20 2332 3432  n    color: #242
-001662f0: 3932 653b 5c6e 2020 2020 6261 636b 6772  92e;\n    backgr
-00166300: 6f75 6e64 2d63 6f6c 6f72 3a20 7768 6974  ound-color: whit
-00166310: 653b 5c6e 7d5c 6e5c 6e3c 2f73 7479 6c65  e;\n}\n\n</style
-00166320: 3e5c 6e5c 6e3c 6469 7620 636c 6173 733d  >\n\n<div class=
-00166330: 5c27 6170 702d 7363 726f 6c6c 5c27 3e5c  \'app-scroll\'>\
-00166340: 6e20 2020 203c 6469 7620 636c 6173 733d  n    <div class=
-00166350: 2261 7070 2d6c 696e 6b73 2061 7070 2d73  "app-links app-s
-00166360: 7469 636b 7922 3e5c 6e20 2020 2020 2020  ticky">\n       
-00166370: 203c 6469 7620 636c 6173 733d 2261 7070   <div class="app
-00166380: 2d74 6974 6c65 223e 5c6e 2020 2020 2020  -title">\n      
-00166390: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-001663a0: 3d22 6170 702d 6672 616d 6520 6170 702d  ="app-frame app-
-001663b0: 7061 6420 6170 702d 666c 7573 682d 626f  pad app-flush-bo
-001663c0: 7474 6f6d 223e 5c6e 2020 2020 2020 2020  ttom">\n        
-001663d0: 2020 2020 2020 2020 3c68 313e 5c6e 2020          <h1>\n  
-001663e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001663f0: 2020 3c73 7061 6e20 636c 6173 733d 2262    <span class="b
-00166400: 7265 616b 223e 7b7b 2073 6f75 7263 6520  reak">{{ source 
-00166410: 7d7d 3c2f 7370 616e 3e5c 6e20 2020 2020  }}</span>\n     
-00166420: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00166430: 736d 616c 6c3e 736f 7572 6365 3c2f 736d  small>source</sm
-00166440: 616c 6c3e 5c6e 2020 2020 2020 2020 2020  all>\n          
-00166450: 2020 2020 2020 3c2f 6831 3e5c 6e20 2020        </h1>\n   
-00166460: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-00166470: 6e20 2020 2020 2020 203c 2f64 6976 3e5c  n        </div>\
-00166480: 6e20 2020 2020 2020 203c 6469 7620 636c  n        <div cl
-00166490: 6173 733d 2261 7070 2d66 7261 6d65 2061  ass="app-frame a
-001664a0: 7070 2d70 6164 2d68 223e 5c6e 2020 2020  pp-pad-h">\n    
-001664b0: 2020 2020 2020 2020 3c75 6c20 636c 6173          <ul clas
-001664c0: 733d 226e 6176 206e 6176 2d74 6162 7322  s="nav nav-tabs"
-001664d0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-001664e0: 2020 203c 6c69 2075 692d 7372 6566 2d61     <li ui-sref-a
-001664f0: 6374 6976 653d 5c27 6163 7469 7665 5c27  ctive=\'active\'
-00166500: 3e3c 6120 7569 2d73 7265 663d 2264 6274  ><a ui-sref="dbt
-00166510: 2e73 6f75 7263 655f 6c69 7374 287b 5c27  .source_list({\'
-00166520: 235c 273a 205c 2764 6574 6169 6c73 5c27  #\': \'details\'
-00166530: 7d29 223e 4465 7461 696c 733c 2f61 3e3c  })">Details</a><
-00166540: 2f6c 693e 5c6e 2020 2020 2020 2020 2020  /li>\n          
-00166550: 2020 2020 2020 3c6c 6920 7569 2d73 7265        <li ui-sre
-00166560: 662d 6163 7469 7665 3d5c 2761 6374 6976  f-active=\'activ
-00166570: 655c 273e 3c61 2075 692d 7372 6566 3d22  e\'><a ui-sref="
-00166580: 6462 742e 736f 7572 6365 5f6c 6973 7428  dbt.source_list(
-00166590: 7b5c 2723 5c27 3a20 5c27 6465 7363 7269  {\'#\': \'descri
-001665a0: 7074 696f 6e5c 277d 2922 3e44 6573 6372  ption\'})">Descr
-001665b0: 6970 7469 6f6e 3c2f 613e 3c2f 6c69 3e5c  iption</a></li>\
-001665c0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-001665d0: 203c 6c69 2075 692d 7372 6566 2d61 6374   <li ui-sref-act
-001665e0: 6976 653d 5c27 6163 7469 7665 5c27 3e3c  ive=\'active\'><
-001665f0: 6120 7569 2d73 7265 663d 2264 6274 2e73  a ui-sref="dbt.s
-00166600: 6f75 7263 655f 6c69 7374 287b 5c27 235c  ource_list({\'#\
-00166610: 273a 205c 2773 6f75 7263 6573 5c27 7d29  ': \'sources\'})
-00166620: 223e 536f 7572 6365 733c 2f61 3e3c 2f6c  ">Sources</a></l
-00166630: 693e 5c6e 2020 2020 2020 2020 2020 2020  i>\n            
-00166640: 3c2f 756c 3e5c 6e20 2020 2020 2020 203c  </ul>\n        <
-00166650: 2f64 6976 3e5c 6e20 2020 203c 2f64 6976  /div>\n    </div
-00166660: 3e5c 6e20 2020 203c 6469 7620 636c 6173  >\n    <div clas
-00166670: 733d 2261 7070 2d64 6574 6169 6c73 223e  s="app-details">
-00166680: 5c6e 2020 2020 2020 2020 3c64 6976 2063  \n        <div c
-00166690: 6c61 7373 3d22 6170 702d 6672 616d 6520  lass="app-frame 
-001666a0: 6170 702d 7061 6422 3e5c 6e20 2020 2020  app-pad">\n     
-001666b0: 2020 2020 2020 203c 7365 6374 696f 6e20         <section 
-001666c0: 636c 6173 733d 2273 6563 7469 6f6e 223e  class="section">
-001666d0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-001666e0: 2020 3c64 6976 2063 6c61 7373 3d22 7365    <div class="se
-001666f0: 6374 696f 6e2d 7461 7267 6574 2220 6964  ction-target" id
-00166700: 3d22 6465 7461 696c 7322 3e3c 2f64 6976  ="details"></div
-00166710: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-00166720: 2020 203c 7461 626c 652d 6465 7461 696c     <table-detail
-00166730: 7320 6d6f 6465 6c3d 226d 6f64 656c 2220  s model="model" 
-00166740: 6578 7472 6173 3d22 6578 7472 615f 7461  extras="extra_ta
-00166750: 626c 655f 6669 656c 6473 222f 3e5c 6e20  ble_fields"/>\n 
-00166760: 2020 2020 2020 2020 2020 203c 2f73 6563             </sec
-00166770: 7469 6f6e 3e5c 6e5c 6e20 2020 2020 2020  tion>\n\n       
-00166780: 2020 2020 203c 7365 6374 696f 6e20 636c       <section cl
-00166790: 6173 733d 2273 6563 7469 6f6e 223e 5c6e  ass="section">\n
-001667a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001667b0: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
-001667c0: 696f 6e2d 7461 7267 6574 2220 6964 3d22  ion-target" id="
-001667d0: 6465 7363 7269 7074 696f 6e22 3e3c 2f64  description"></d
-001667e0: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
-001667f0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00166800: 2273 6563 7469 6f6e 2d63 6f6e 7465 6e74  "section-content
-00166810: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
-00166820: 2020 2020 2020 2020 3c68 363e 4465 7363          <h6>Desc
-00166830: 7269 7074 696f 6e3c 2f68 363e 5c6e 2020  ription</h6>\n  
-00166840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166850: 2020 3c64 6976 2063 6c61 7373 3d22 7061    <div class="pa
-00166860: 6e65 6c22 3e5c 6e20 2020 2020 2020 2020  nel">\n         
-00166870: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00166880: 6469 7620 636c 6173 733d 2270 616e 656c  div class="panel
-00166890: 2d62 6f64 7922 3e5c 6e20 2020 2020 2020  -body">\n       
-001668a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001668b0: 2020 2020 203c 6469 7620 6e67 2d69 663d       <div ng-if=
-001668c0: 226d 6f64 656c 2e73 6f75 7263 655f 6465  "model.source_de
-001668d0: 7363 7269 7074 696f 6e22 2063 6c61 7373  scription" class
-001668e0: 3d22 6d6f 6465 6c2d 6d61 726b 646f 776e  ="model-markdown
-001668f0: 2220 6d61 726b 6564 3d22 6d6f 6465 6c2e  " marked="model.
-00166900: 736f 7572 6365 5f64 6573 6372 6970 7469  source_descripti
-00166910: 6f6e 223e 3c2f 6469 763e 5c6e 2020 2020  on"></div>\n    
-00166920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166930: 2020 2020 2020 2020 3c64 6976 206e 672d          <div ng-
-00166940: 6966 3d22 216d 6f64 656c 2e73 6f75 7263  if="!model.sourc
-00166950: 655f 6465 7363 7269 7074 696f 6e22 3e54  e_description">T
-00166960: 6869 7320 7b7b 206d 6f64 656c 2e72 6573  his {{ model.res
-00166970: 6f75 7263 655f 7479 7065 207d 7d20 6973  ource_type }} is
-00166980: 206e 6f74 2063 7572 7265 6e74 6c79 2064   not currently d
-00166990: 6f63 756d 656e 7465 643c 2f64 6976 3e5c  ocumented</div>\
-001669a0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-001669b0: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-001669c0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-001669d0: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
-001669e0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-001669f0: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
-00166a00: 203c 2f73 6563 7469 6f6e 3e5c 6e5c 6e5c   </section>\n\n\
-00166a10: 6e20 2020 2020 2020 2020 2020 203c 7365  n            <se
-00166a20: 6374 696f 6e20 636c 6173 733d 2273 6563  ction class="sec
-00166a30: 7469 6f6e 223e 5c6e 2020 2020 2020 2020  tion">\n        
-00166a40: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00166a50: 7373 3d22 7365 6374 696f 6e2d 7461 7267  ss="section-targ
-00166a60: 6574 2220 6964 3d22 736f 7572 6365 7322  et" id="sources"
-00166a70: 3e3c 2f64 6976 3e5c 6e20 2020 2020 2020  ></div>\n       
-00166a80: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00166a90: 6173 733d 2273 6563 7469 6f6e 2d63 6f6e  ass="section-con
-00166aa0: 7465 6e74 223e 5c6e 2020 2020 2020 2020  tent">\n        
-00166ab0: 2020 2020 2020 2020 2020 2020 3c68 363e              <h6>
-00166ac0: 536f 7572 6365 2054 6162 6c65 733c 2f68  Source Tables</h
-00166ad0: 363e 5c6e 2020 2020 2020 2020 2020 2020  6>\n            
-00166ae0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00166af0: 7373 3d22 7061 6e65 6c22 3e5c 6e20 2020  ss="panel">\n   
-00166b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166b10: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00166b20: 2270 616e 656c 2d62 6f64 7922 3e5c 6e20  "panel-body">\n 
-00166b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166b40: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00166b50: 636c 6173 733d 2274 6162 6c65 2d72 6573  class="table-res
-00166b60: 706f 6e73 6976 6522 2073 7479 6c65 3d22  ponsive" style="
-00166b70: 6d61 782d 6865 6967 6874 3a20 3830 3070  max-height: 800p
-00166b80: 783b 206f 7665 7266 6c6f 772d 793a 2073  x; overflow-y: s
-00166b90: 6372 6f6c 6c3b 2220 6e67 2d69 663d 2221  croll;" ng-if="!
-00166ba0: 5f2e 6973 456d 7074 7928 6d6f 6465 6c2e  _.isEmpty(model.
-00166bb0: 736f 7572 6365 7329 223e 5c6e 2020 2020  sources)">\n    
-00166bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166bd0: 2020 2020 2020 2020 2020 2020 3c74 6162              <tab
-00166be0: 6c65 2063 6c61 7373 3d22 7461 626c 6520  le class="table 
-00166bf0: 7461 626c 652d 626f 7264 6572 6c65 7373  table-borderless
-00166c00: 2074 6162 6c65 2d68 6f76 6572 223e 5c6e   table-hover">\n
-00166c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166c30: 2020 2020 3c74 6865 6164 3e5c 6e20 2020      <thead>\n   
+001659a0: 2020 2020 2020 2069 643d 2273 6561 7263         id="searc
+001659b0: 6822 5c6e 2020 2020 2020 2020 2020 2020  h"\n            
+001659c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001659d0: 6e67 2d6d 6f64 656c 3d22 7365 6172 6368  ng-model="search
+001659e0: 2e71 7565 7279 225c 6e20 2020 2020 2020  .query"\n       
+001659f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00165a00: 2020 2020 206e 672d 666f 6375 733d 226f       ng-focus="o
+00165a10: 6e53 6561 7263 6846 6f63 7573 2824 6576  nSearchFocus($ev
+00165a20: 656e 742c 2074 7275 6529 225c 6e20 2020  ent, true)"\n   
+00165a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00165a40: 2020 2020 2020 2020 206e 672d 6b65 7964           ng-keyd
+00165a50: 6f77 6e3d 226f 6e53 6561 7263 684b 6579  own="onSearchKey
+00165a60: 7072 6573 7328 2465 7665 6e74 2922 5c6e  press($event)"\n
+00165a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00165a80: 2020 2020 2020 2020 2020 2020 7479 7065              type
+00165a90: 3d22 7465 7874 225c 6e20 2020 2020 2020  ="text"\n       
+00165aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00165ab0: 2020 2020 2063 6c61 7373 3d22 666f 726d       class="form
+00165ac0: 2d63 6f6e 7472 6f6c 225c 6e20 2020 2020  -control"\n     
+00165ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00165ae0: 2020 2020 2020 2070 6c61 6365 686f 6c64         placehold
+00165af0: 6572 3d22 5365 6172 6368 2066 6f72 206d  er="Search for m
+00165b00: 6f64 656c 732e 2e2e 2220 2f3e 5c6e 2020  odels..." />\n  
+00165b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00165b20: 2020 3c64 6976 2063 6c61 7373 3d22 6170    <div class="ap
+00165b30: 702d 626f 6479 223e 5c6e 2020 2020 2020  p-body">\n      
+00165b40: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00165b50: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
+00165b60: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00165b70: 6c61 7373 3d22 6170 702d 666f 6f74 6572  lass="app-footer
+00165b80: 2061 7070 2d69 636e 2220 6e67 2d73 686f   app-icn" ng-sho
+00165b90: 773d 2273 6561 7263 682e 6973 5f66 6f63  w="search.is_foc
+00165ba0: 7573 6564 2220 6e67 2d63 6c69 636b 3d22  used" ng-click="
+00165bb0: 636c 6561 7253 6561 7263 6828 2922 3e5c  clearSearch()">\
+00165bc0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00165bd0: 2020 2020 2020 2020 203c 7376 6720 636c           <svg cl
+00165be0: 6173 733d 2269 636e 2069 636e 2d6d 6422  ass="icn icn-md"
+00165bf0: 3e3c 7573 6520 786c 696e 6b3a 6872 6566  ><use xlink:href
+00165c00: 3d22 2369 636e 2d63 6c6f 7365 223e 3c2f  ="#icn-close"></
+00165c10: 7573 653e 3c2f 7376 673e 5c6e 2020 2020  use></svg>\n    
+00165c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00165c30: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
+00165c40: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
+00165c50: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00165c60: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
+00165c70: 3c64 6976 2063 6c61 7373 3d5c 2761 7070  <div class=\'app
+00165c80: 2d62 6f64 795c 2720 6e67 2d73 686f 773d  -body\' ng-show=
+00165c90: 5c27 2173 6561 7263 682e 6973 5f66 6f63  \'!search.is_foc
+00165ca0: 7573 6564 5c27 2075 692d 7669 6577 3e3c  used\' ui-view><
+00165cb0: 2f64 6976 3e5c 6e20 2020 2020 2020 2020  /div>\n         
+00165cc0: 2020 203c 6469 7620 636c 6173 733d 2261     <div class="a
+00165cd0: 7070 2d62 6f64 7922 206e 672d 7368 6f77  pp-body" ng-show
+00165ce0: 3d22 7365 6172 6368 2e69 735f 666f 6375  ="search.is_focu
+00165cf0: 7365 6422 3e5c 6e20 2020 2020 2020 2020  sed">\n         
+00165d00: 2020 2020 2020 203c 646f 6373 2d73 6561         <docs-sea
+00165d10: 7263 6820 7175 6572 793d 2273 6561 7263  rch query="searc
+00165d20: 682e 7175 6572 7922 2072 6573 756c 7473  h.query" results
+00165d30: 3d22 7365 6172 6368 2e72 6573 756c 7473  ="search.results
+00165d40: 2220 6f6e 2d73 656c 6563 743d 2263 6c65  " on-select="cle
+00165d50: 6172 5365 6172 6368 2829 223e 3c2f 646f  arSearch()"></do
+00165d60: 6373 2d73 6561 7263 683e 5c6e 2020 2020  cs-search>\n    
+00165d70: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
+00165d80: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
+00165d90: 2020 2020 3c2f 6469 763e 5c6e 3c2f 6469      </div>\n</di
+00165da0: 763e 5c6e 2729 7d5d 292c 652e 6578 706f  v>\n')}]),e.expo
+00165db0: 7274 733d 6e7d 2c66 756e 6374 696f 6e28  rts=n},function(
+00165dc0: 652c 7429 7b76 6172 206e 3d22 2f6f 7665  e,t){var n="/ove
+00165dd0: 7276 6965 772f 6f76 6572 7669 6577 2e68  rview/overview.h
+00165de0: 746d 6c22 3b77 696e 646f 772e 616e 6775  tml";window.angu
+00165df0: 6c61 722e 6d6f 6475 6c65 2822 6e67 2229  lar.module("ng")
+00165e00: 2e72 756e 285b 2224 7465 6d70 6c61 7465  .run(["$template
+00165e10: 4361 6368 6522 2c66 756e 6374 696f 6e28  Cache",function(
+00165e20: 6529 7b65 2e70 7574 286e 2c27 3c64 6976  e){e.put(n,'<div
+00165e30: 2063 6c61 7373 3d22 6170 702d 6465 7461   class="app-deta
+00165e40: 696c 7320 6170 702d 7363 726f 6c6c 2061  ils app-scroll a
+00165e50: 7070 2d70 6164 223e 5c6e 2020 2020 3c61  pp-pad">\n    <a
+00165e60: 7070 2d73 6372 6f6c 6c20 6469 7620 636c  pp-scroll div cl
+00165e70: 6173 733d 2261 7070 2d66 7261 6d65 2061  ass="app-frame a
+00165e80: 7070 2d70 6164 223e 5c6e 2020 2020 2020  pp-pad">\n      
+00165e90: 2020 3c64 6976 2063 6c61 7373 3d22 7061    <div class="pa
+00165ea0: 6e65 6c20 7061 6e65 6c2d 6465 6661 756c  nel panel-defaul
+00165eb0: 7422 3e5c 6e20 2020 2020 2020 2020 2020  t">\n           
+00165ec0: 203c 6469 7620 636c 6173 733d 2270 616e   <div class="pan
+00165ed0: 656c 2d62 6f64 7922 3e5c 6e20 2020 2020  el-body">\n     
+00165ee0: 2020 2020 2020 2020 2020 203c 7020 6d61             <p ma
+00165ef0: 726b 6564 3d5c 276f 7665 7276 6965 775f  rked=\'overview_
+00165f00: 6d64 5c27 3e3c 2f70 3e5c 6e20 2020 2020  md\'></p>\n     
+00165f10: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
+00165f20: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
+00165f30: 2020 203c 2f64 6976 3e5c 6e3c 2f64 6976     </div>\n</div
+00165f40: 3e5c 6e27 297d 5d29 2c65 2e65 7870 6f72  >\n')}]),e.expor
+00165f50: 7473 3d6e 7d2c 6675 6e63 7469 6f6e 2865  ts=n},function(e
+00165f60: 2c74 297b 7661 7220 6e3d 222f 6772 6170  ,t){var n="/grap
+00165f70: 682f 6772 6170 682e 6874 6d6c 223b 7769  h/graph.html";wi
+00165f80: 6e64 6f77 2e61 6e67 756c 6172 2e6d 6f64  ndow.angular.mod
+00165f90: 756c 6528 226e 6722 292e 7275 6e28 5b22  ule("ng").run(["
+00165fa0: 2474 656d 706c 6174 6543 6163 6865 222c  $templateCache",
+00165fb0: 6675 6e63 7469 6f6e 2865 297b 652e 7075  function(e){e.pu
+00165fc0: 7428 6e2c 273c 6469 7620 6e67 2d63 6f6e  t(n,'<div ng-con
+00165fd0: 7472 6f6c 6c65 723d 2247 7261 7068 4374  troller="GraphCt
+00165fe0: 726c 2220 6964 3d5c 2767 7261 7068 2d63  rl" id=\'graph-c
+00165ff0: 6f6e 7461 696e 6572 5c27 2073 7479 6c65  ontainer\' style
+00166000: 3d22 7769 6474 683a 2031 3030 2522 3e5c  ="width: 100%">\
+00166010: 6e20 2020 203c 6469 7620 636c 6173 733d  n    <div class=
+00166020: 5c27 726f 7720 7669 7a2d 636f 6e74 6169  \'row viz-contai
+00166030: 6e65 725c 2720 7374 796c 653d 226d 6172  ner\' style="mar
+00166040: 6769 6e3a 2030 223e 5c6e 2020 2020 2020  gin: 0">\n      
+00166050: 2020 3c64 6976 2063 6c61 7373 3d5c 2763    <div class=\'c
+00166060: 6f6c 2d6d 642d 3132 5c27 3e5c 6e20 2020  ol-md-12\'>\n   
+00166070: 2020 2020 2020 2020 2020 3c64 6976 2067            <div g
+00166080: 7261 7068 2d76 697a 5c6e 2020 2020 2020  raph-viz\n      
+00166090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001660a0: 2020 7669 7a2d 6f70 7469 6f6e 733d 2267    viz-options="g
+001660b0: 7261 7068 2e6f 7074 696f 6e73 225c 6e20  raph.options"\n 
+001660c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001660d0: 2020 2020 2020 2076 697a 2d65 6c65 6d65         viz-eleme
+001660e0: 6e74 733d 2267 7261 7068 2e65 6c65 6d65  nts="graph.eleme
+001660f0: 6e74 7322 5c6e 2020 2020 2020 2020 2020  nts"\n          
+00166100: 2020 2020 2020 2020 2020 2020 2020 7669                vi
+00166110: 7a2d 7374 796c 653d 2267 7261 7068 2e73  z-style="graph.s
+00166120: 7479 6c65 225c 6e20 2020 2020 2020 2020  tyle"\n         
+00166130: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00166140: 697a 2d6c 6179 6f75 743d 2267 7261 7068  iz-layout="graph
+00166150: 2e6c 6179 6f75 7422 5c6e 2020 2020 2020  .layout"\n      
+00166160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166170: 2020 7669 7a2d 7265 6164 793d 2267 7261    viz-ready="gra
+00166180: 7068 2e72 6561 6479 225c 6e20 2020 2020  ph.ready"\n     
+00166190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001661a0: 2020 2076 697a 2d73 697a 653d 227b 6865     viz-size="{he
+001661b0: 6967 6874 3a20 5c27 3830 3070 785c 272c  ight: \'800px\',
+001661c0: 2077 6964 7468 3a20 5c27 3130 3025 5c27   width: \'100%\'
+001661d0: 7d22 3e3c 2f64 6976 3e5c 6e20 2020 2020  }"></div>\n     
+001661e0: 2020 203c 2f64 6976 3e5c 6e20 2020 203c     </div>\n    <
+001661f0: 2f64 6976 3e5c 6e3c 2f64 6976 3e5c 6e27  /div>\n</div>\n'
+00166200: 297d 5d29 2c65 2e65 7870 6f72 7473 3d6e  )}]),e.exports=n
+00166210: 7d2c 6675 6e63 7469 6f6e 2865 2c74 297b  },function(e,t){
+00166220: 7661 7220 6e3d 222f 736f 7572 6365 732f  var n="/sources/
+00166230: 736f 7572 6365 5f6c 6973 742e 6874 6d6c  source_list.html
+00166240: 223b 7769 6e64 6f77 2e61 6e67 756c 6172  ";window.angular
+00166250: 2e6d 6f64 756c 6528 226e 6722 292e 7275  .module("ng").ru
+00166260: 6e28 5b22 2474 656d 706c 6174 6543 6163  n(["$templateCac
+00166270: 6865 222c 6675 6e63 7469 6f6e 2865 297b  he",function(e){
+00166280: 652e 7075 7428 6e2c 273c 7374 796c 653e  e.put(n,'<style>
+00166290: 5c6e 2f2a 2054 4f44 4f20 2a2f 5c6e 2e73  \n/* TODO */\n.s
+001662a0: 6563 7469 6f6e 2d74 6172 6765 7420 7b5c  ection-target {\
+001662b0: 6e20 2020 2074 6f70 3a20 2d38 656d 3b5c  n    top: -8em;\
+001662c0: 6e7d 5c6e 5c6e 2e6e 6f66 6c65 7820 7b5c  n}\n\n.noflex {\
+001662d0: 6e20 2020 2066 6c65 783a 2030 2030 2031  n    flex: 0 0 1
+001662e0: 3630 7078 2021 696d 706f 7274 616e 743b  60px !important;
+001662f0: 5c6e 7d5c 6e5c 6e2e 6869 6768 6c69 6768  \n}\n\n.highligh
+00166300: 7420 7b5c 6e20 2020 2063 6f6c 6f72 3a20  t {\n    color: 
+00166310: 2332 3432 3932 653b 5c6e 2020 2020 6261  #24292e;\n    ba
+00166320: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a20  ckground-color: 
+00166330: 7768 6974 653b 5c6e 7d5c 6e5c 6e3c 2f73  white;\n}\n\n</s
+00166340: 7479 6c65 3e5c 6e5c 6e3c 6469 7620 636c  tyle>\n\n<div cl
+00166350: 6173 733d 5c27 6170 702d 7363 726f 6c6c  ass=\'app-scroll
+00166360: 5c27 3e5c 6e20 2020 203c 6469 7620 636c  \'>\n    <div cl
+00166370: 6173 733d 2261 7070 2d6c 696e 6b73 2061  ass="app-links a
+00166380: 7070 2d73 7469 636b 7922 3e5c 6e20 2020  pp-sticky">\n   
+00166390: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+001663a0: 2261 7070 2d74 6974 6c65 223e 5c6e 2020  "app-title">\n  
+001663b0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+001663c0: 6c61 7373 3d22 6170 702d 6672 616d 6520  lass="app-frame 
+001663d0: 6170 702d 7061 6420 6170 702d 666c 7573  app-pad app-flus
+001663e0: 682d 626f 7474 6f6d 223e 5c6e 2020 2020  h-bottom">\n    
+001663f0: 2020 2020 2020 2020 2020 2020 3c68 313e              <h1>
+00166400: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00166410: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
+00166420: 733d 2262 7265 616b 223e 7b7b 2073 6f75  s="break">{{ sou
+00166430: 7263 6520 7d7d 3c2f 7370 616e 3e5c 6e20  rce }}</span>\n 
+00166440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166450: 2020 203c 736d 616c 6c3e 736f 7572 6365     <small>source
+00166460: 3c2f 736d 616c 6c3e 5c6e 2020 2020 2020  </small>\n      
+00166470: 2020 2020 2020 2020 2020 3c2f 6831 3e5c            </h1>\
+00166480: 6e20 2020 2020 2020 2020 2020 203c 2f64  n            </d
+00166490: 6976 3e5c 6e20 2020 2020 2020 203c 2f64  iv>\n        </d
+001664a0: 6976 3e5c 6e20 2020 2020 2020 203c 6469  iv>\n        <di
+001664b0: 7620 636c 6173 733d 2261 7070 2d66 7261  v class="app-fra
+001664c0: 6d65 2061 7070 2d70 6164 2d68 223e 5c6e  me app-pad-h">\n
+001664d0: 2020 2020 2020 2020 2020 2020 3c75 6c20              <ul 
+001664e0: 636c 6173 733d 226e 6176 206e 6176 2d74  class="nav nav-t
+001664f0: 6162 7322 3e5c 6e20 2020 2020 2020 2020  abs">\n         
+00166500: 2020 2020 2020 203c 6c69 2075 692d 7372         <li ui-sr
+00166510: 6566 2d61 6374 6976 653d 5c27 6163 7469  ef-active=\'acti
+00166520: 7665 5c27 3e3c 6120 7569 2d73 7265 663d  ve\'><a ui-sref=
+00166530: 2264 6274 2e73 6f75 7263 655f 6c69 7374  "dbt.source_list
+00166540: 287b 5c27 235c 273a 205c 2764 6574 6169  ({\'#\': \'detai
+00166550: 6c73 5c27 7d29 223e 4465 7461 696c 733c  ls\'})">Details<
+00166560: 2f61 3e3c 2f6c 693e 5c6e 2020 2020 2020  /a></li>\n      
+00166570: 2020 2020 2020 2020 2020 3c6c 6920 7569            <li ui
+00166580: 2d73 7265 662d 6163 7469 7665 3d5c 2761  -sref-active=\'a
+00166590: 6374 6976 655c 273e 3c61 2075 692d 7372  ctive\'><a ui-sr
+001665a0: 6566 3d22 6462 742e 736f 7572 6365 5f6c  ef="dbt.source_l
+001665b0: 6973 7428 7b5c 2723 5c27 3a20 5c27 6465  ist({\'#\': \'de
+001665c0: 7363 7269 7074 696f 6e5c 277d 2922 3e44  scription\'})">D
+001665d0: 6573 6372 6970 7469 6f6e 3c2f 613e 3c2f  escription</a></
+001665e0: 6c69 3e5c 6e20 2020 2020 2020 2020 2020  li>\n           
+001665f0: 2020 2020 203c 6c69 2075 692d 7372 6566       <li ui-sref
+00166600: 2d61 6374 6976 653d 5c27 6163 7469 7665  -active=\'active
+00166610: 5c27 3e3c 6120 7569 2d73 7265 663d 2264  \'><a ui-sref="d
+00166620: 6274 2e73 6f75 7263 655f 6c69 7374 287b  bt.source_list({
+00166630: 5c27 235c 273a 205c 2773 6f75 7263 6573  \'#\': \'sources
+00166640: 5c27 7d29 223e 536f 7572 6365 733c 2f61  \'})">Sources</a
+00166650: 3e3c 2f6c 693e 5c6e 2020 2020 2020 2020  ></li>\n        
+00166660: 2020 2020 3c2f 756c 3e5c 6e20 2020 2020      </ul>\n     
+00166670: 2020 203c 2f64 6976 3e5c 6e20 2020 203c     </div>\n    <
+00166680: 2f64 6976 3e5c 6e20 2020 203c 6469 7620  /div>\n    <div 
+00166690: 636c 6173 733d 2261 7070 2d64 6574 6169  class="app-detai
+001666a0: 6c73 223e 5c6e 2020 2020 2020 2020 3c64  ls">\n        <d
+001666b0: 6976 2063 6c61 7373 3d22 6170 702d 6672  iv class="app-fr
+001666c0: 616d 6520 6170 702d 7061 6422 3e5c 6e20  ame app-pad">\n 
+001666d0: 2020 2020 2020 2020 2020 203c 7365 6374             <sect
+001666e0: 696f 6e20 636c 6173 733d 2273 6563 7469  ion class="secti
+001666f0: 6f6e 223e 5c6e 2020 2020 2020 2020 2020  on">\n          
+00166700: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00166710: 3d22 7365 6374 696f 6e2d 7461 7267 6574  ="section-target
+00166720: 2220 6964 3d22 6465 7461 696c 7322 3e3c  " id="details"><
+00166730: 2f64 6976 3e5c 6e20 2020 2020 2020 2020  /div>\n         
+00166740: 2020 2020 2020 203c 7461 626c 652d 6465         <table-de
+00166750: 7461 696c 7320 6d6f 6465 6c3d 226d 6f64  tails model="mod
+00166760: 656c 2220 6578 7472 6173 3d22 6578 7472  el" extras="extr
+00166770: 615f 7461 626c 655f 6669 656c 6473 222f  a_table_fields"/
+00166780: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
+00166790: 2f73 6563 7469 6f6e 3e5c 6e5c 6e20 2020  /section>\n\n   
+001667a0: 2020 2020 2020 2020 203c 7365 6374 696f           <sectio
+001667b0: 6e20 636c 6173 733d 2273 6563 7469 6f6e  n class="section
+001667c0: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
+001667d0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+001667e0: 7365 6374 696f 6e2d 7461 7267 6574 2220  section-target" 
+001667f0: 6964 3d22 6465 7363 7269 7074 696f 6e22  id="description"
+00166800: 3e3c 2f64 6976 3e5c 6e20 2020 2020 2020  ></div>\n       
+00166810: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00166820: 6173 733d 2273 6563 7469 6f6e 2d63 6f6e  ass="section-con
+00166830: 7465 6e74 223e 5c6e 2020 2020 2020 2020  tent">\n        
+00166840: 2020 2020 2020 2020 2020 2020 3c68 363e              <h6>
+00166850: 4465 7363 7269 7074 696f 6e3c 2f68 363e  Description</h6>
+00166860: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00166870: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00166880: 3d22 7061 6e65 6c22 3e5c 6e20 2020 2020  ="panel">\n     
+00166890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001668a0: 2020 203c 6469 7620 636c 6173 733d 2270     <div class="p
+001668b0: 616e 656c 2d62 6f64 7922 3e5c 6e20 2020  anel-body">\n   
+001668c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001668d0: 2020 2020 2020 2020 203c 6469 7620 6e67           <div ng
+001668e0: 2d69 663d 226d 6f64 656c 2e73 6f75 7263  -if="model.sourc
+001668f0: 655f 6465 7363 7269 7074 696f 6e22 2063  e_description" c
+00166900: 6c61 7373 3d22 6d6f 6465 6c2d 6d61 726b  lass="model-mark
+00166910: 646f 776e 2220 6d61 726b 6564 3d22 6d6f  down" marked="mo
+00166920: 6465 6c2e 736f 7572 6365 5f64 6573 6372  del.source_descr
+00166930: 6970 7469 6f6e 223e 3c2f 6469 763e 5c6e  iption"></div>\n
+00166940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166950: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00166960: 206e 672d 6966 3d22 216d 6f64 656c 2e73   ng-if="!model.s
+00166970: 6f75 7263 655f 6465 7363 7269 7074 696f  ource_descriptio
+00166980: 6e22 3e54 6869 7320 7b7b 206d 6f64 656c  n">This {{ model
+00166990: 2e72 6573 6f75 7263 655f 7479 7065 207d  .resource_type }
+001669a0: 7d20 6973 206e 6f74 2063 7572 7265 6e74  } is not current
+001669b0: 6c79 2064 6f63 756d 656e 7465 643c 2f64  ly documented</d
+001669c0: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
+001669d0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+001669e0: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
+001669f0: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
+00166a00: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00166a10: 203c 2f64 6976 3e5c 6e20 2020 2020 2020   </div>\n       
+00166a20: 2020 2020 203c 2f73 6563 7469 6f6e 3e5c       </section>\
+00166a30: 6e5c 6e5c 6e20 2020 2020 2020 2020 2020  n\n\n           
+00166a40: 203c 7365 6374 696f 6e20 636c 6173 733d   <section class=
+00166a50: 2273 6563 7469 6f6e 223e 5c6e 2020 2020  "section">\n    
+00166a60: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00166a70: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
+00166a80: 7461 7267 6574 2220 6964 3d22 736f 7572  target" id="sour
+00166a90: 6365 7322 3e3c 2f64 6976 3e5c 6e20 2020  ces"></div>\n   
+00166aa0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00166ab0: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
+00166ac0: 2d63 6f6e 7465 6e74 223e 5c6e 2020 2020  -content">\n    
+00166ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166ae0: 3c68 363e 536f 7572 6365 2054 6162 6c65  <h6>Source Table
+00166af0: 733c 2f68 363e 5c6e 2020 2020 2020 2020  s</h6>\n        
+00166b00: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00166b10: 2063 6c61 7373 3d22 7061 6e65 6c22 3e5c   class="panel">\
+00166b20: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00166b30: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00166b40: 6173 733d 2270 616e 656c 2d62 6f64 7922  ass="panel-body"
+00166b50: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+00166b60: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00166b70: 6469 7620 636c 6173 733d 2274 6162 6c65  div class="table
+00166b80: 2d72 6573 706f 6e73 6976 6522 2073 7479  -responsive" sty
+00166b90: 6c65 3d22 6d61 782d 6865 6967 6874 3a20  le="max-height: 
+00166ba0: 3830 3070 783b 206f 7665 7266 6c6f 772d  800px; overflow-
+00166bb0: 793a 2073 6372 6f6c 6c3b 2220 6e67 2d69  y: scroll;" ng-i
+00166bc0: 663d 2221 5f2e 6973 456d 7074 7928 6d6f  f="!_.isEmpty(mo
+00166bd0: 6465 6c2e 736f 7572 6365 7329 223e 5c6e  del.sources)">\n
+00166be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166c00: 3c74 6162 6c65 2063 6c61 7373 3d22 7461  <table class="ta
+00166c10: 626c 6520 7461 626c 652d 626f 7264 6572  ble table-border
+00166c20: 6c65 7373 2074 6162 6c65 2d68 6f76 6572  less table-hover
+00166c30: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
 00166c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166c60: 2020 2020 203c 7472 3e5c 6e20 2020 2020       <tr>\n     
+00166c50: 2020 2020 2020 2020 3c74 6865 6164 3e5c          <thead>\
+00166c60: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
 00166c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166c90: 2020 2020 2020 203c 7468 2073 7479 6c65         <th style
-00166ca0: 3d22 6261 636b 6772 6f75 6e64 2d63 6f6c  ="background-col
-00166cb0: 6f72 3a20 7768 6974 653b 2070 6f73 6974  or: white; posit
-00166cc0: 696f 6e3a 2073 7469 636b 793b 2074 6f70  ion: sticky; top
-00166cd0: 3a20 303b 207a 2d69 6e64 6578 3a20 313b  : 0; z-index: 1;
-00166ce0: 223e 536f 7572 6365 3c2f 7468 3e5c 6e20  ">Source</th>\n 
-00166cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166d10: 2020 2020 2020 2020 2020 203c 7468 2073             <th s
-00166d20: 7479 6c65 3d22 6261 636b 6772 6f75 6e64  tyle="background
-00166d30: 2d63 6f6c 6f72 3a20 7768 6974 653b 2070  -color: white; p
-00166d40: 6f73 6974 696f 6e3a 2073 7469 636b 793b  osition: sticky;
-00166d50: 2074 6f70 3a20 303b 207a 2d69 6e64 6578   top: 0; z-index
-00166d60: 3a20 313b 223e 5461 626c 653c 2f74 683e  : 1;">Table</th>
-00166d70: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00166d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166d90: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
-00166da0: 6820 7374 796c 653d 2262 6163 6b67 726f  h style="backgro
-00166db0: 756e 642d 636f 6c6f 723a 2077 6869 7465  und-color: white
-00166dc0: 3b20 706f 7369 7469 6f6e 3a20 7374 6963  ; position: stic
-00166dd0: 6b79 3b20 746f 703a 2030 3b20 7a2d 696e  ky; top: 0; z-in
-00166de0: 6465 783a 2031 3b22 3e44 6573 6372 6970  dex: 1;">Descrip
-00166df0: 7469 6f6e 3c2f 7468 3e5c 6e20 2020 2020  tion</th>\n     
-00166e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166e20: 2020 2020 2020 203c 7468 2073 7479 6c65         <th style
-00166e30: 3d22 6261 636b 6772 6f75 6e64 2d63 6f6c  ="background-col
-00166e40: 6f72 3a20 7768 6974 653b 2070 6f73 6974  or: white; posit
-00166e50: 696f 6e3a 2073 7469 636b 793b 2074 6f70  ion: sticky; top
-00166e60: 3a20 303b 207a 2d69 6e64 6578 3a20 313b  : 0; z-index: 1;
-00166e70: 223e 4c69 6e6b 3c2f 7468 3e5c 6e20 2020  ">Link</th>\n   
-00166e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166ea0: 2020 2020 2020 2020 203c 7468 2073 7479           <th sty
-00166eb0: 6c65 3d22 7769 6474 683a 2031 7078 3b20  le="width: 1px; 
-00166ec0: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-00166ed0: 3a20 7768 6974 653b 2070 6f73 6974 696f  : white; positio
-00166ee0: 6e3a 2073 7469 636b 793b 2074 6f70 3a20  n: sticky; top: 
-00166ef0: 303b 207a 2d69 6e64 6578 3a20 313b 2220  0; z-index: 1;" 
-00166f00: 636c 6173 733d 5c27 7465 7874 2d63 656e  class=\'text-cen
-00166f10: 7465 725c 273e 4d6f 7265 3f3c 2f74 683e  ter\'>More?</th>
-00166f20: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00166f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166f40: 2020 2020 2020 2020 2020 3c2f 7472 3e5c            </tr>\
-00166f50: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00166f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166f70: 2020 2020 203c 2f74 6865 6164 3e5c 6e20       </thead>\n 
+00166c80: 2020 2020 2020 2020 203c 7472 3e5c 6e20           <tr>\n 
+00166c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166cb0: 2020 2020 2020 2020 2020 203c 7468 2073             <th s
+00166cc0: 7479 6c65 3d22 6261 636b 6772 6f75 6e64  tyle="background
+00166cd0: 2d63 6f6c 6f72 3a20 7768 6974 653b 2070  -color: white; p
+00166ce0: 6f73 6974 696f 6e3a 2073 7469 636b 793b  osition: sticky;
+00166cf0: 2074 6f70 3a20 303b 207a 2d69 6e64 6578   top: 0; z-index
+00166d00: 3a20 313b 223e 536f 7572 6365 3c2f 7468  : 1;">Source</th
+00166d10: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+00166d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166d30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00166d40: 7468 2073 7479 6c65 3d22 6261 636b 6772  th style="backgr
+00166d50: 6f75 6e64 2d63 6f6c 6f72 3a20 7768 6974  ound-color: whit
+00166d60: 653b 2070 6f73 6974 696f 6e3a 2073 7469  e; position: sti
+00166d70: 636b 793b 2074 6f70 3a20 303b 207a 2d69  cky; top: 0; z-i
+00166d80: 6e64 6578 3a20 313b 223e 5461 626c 653c  ndex: 1;">Table<
+00166d90: 2f74 683e 5c6e 2020 2020 2020 2020 2020  /th>\n          
+00166da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166dc0: 2020 3c74 6820 7374 796c 653d 2262 6163    <th style="bac
+00166dd0: 6b67 726f 756e 642d 636f 6c6f 723a 2077  kground-color: w
+00166de0: 6869 7465 3b20 706f 7369 7469 6f6e 3a20  hite; position: 
+00166df0: 7374 6963 6b79 3b20 746f 703a 2030 3b20  sticky; top: 0; 
+00166e00: 7a2d 696e 6465 783a 2031 3b22 3e44 6573  z-index: 1;">Des
+00166e10: 6372 6970 7469 6f6e 3c2f 7468 3e5c 6e20  cription</th>\n 
+00166e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166e40: 2020 2020 2020 2020 2020 203c 7468 2073             <th s
+00166e50: 7479 6c65 3d22 6261 636b 6772 6f75 6e64  tyle="background
+00166e60: 2d63 6f6c 6f72 3a20 7768 6974 653b 2070  -color: white; p
+00166e70: 6f73 6974 696f 6e3a 2073 7469 636b 793b  osition: sticky;
+00166e80: 2074 6f70 3a20 303b 207a 2d69 6e64 6578   top: 0; z-index
+00166e90: 3a20 313b 223e 4c69 6e6b 3c2f 7468 3e5c  : 1;">Link</th>\
+00166ea0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00166eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166ec0: 2020 2020 2020 2020 2020 2020 203c 7468               <th
+00166ed0: 2073 7479 6c65 3d22 7769 6474 683a 2031   style="width: 1
+00166ee0: 7078 3b20 6261 636b 6772 6f75 6e64 2d63  px; background-c
+00166ef0: 6f6c 6f72 3a20 7768 6974 653b 2070 6f73  olor: white; pos
+00166f00: 6974 696f 6e3a 2073 7469 636b 793b 2074  ition: sticky; t
+00166f10: 6f70 3a20 303b 207a 2d69 6e64 6578 3a20  op: 0; z-index: 
+00166f20: 313b 2220 636c 6173 733d 5c27 7465 7874  1;" class=\'text
+00166f30: 2d63 656e 7465 725c 273e 4d6f 7265 3f3c  -center\'>More?<
+00166f40: 2f74 683e 5c6e 2020 2020 2020 2020 2020  /th>\n          
+00166f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00166f60: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00166f70: 7472 3e5c 6e20 2020 2020 2020 2020 2020  tr>\n           
 00166f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166fa0: 2020 203c 7462 6f64 793e 5c6e 2020 2020     <tbody>\n    
+00166f90: 2020 2020 2020 2020 203c 2f74 6865 6164           </thead
+00166fa0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
 00166fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166fd0: 2020 2020 3c74 725c 6e20 2020 2020 2020      <tr\n       
+00166fc0: 2020 2020 2020 203c 7462 6f64 793e 5c6e         <tbody>\n
+00166fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00166fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00166ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167000: 2020 2020 206e 672d 7265 7065 6174 2d73       ng-repeat-s
-00167010: 7461 7274 3d22 736f 7572 6365 2069 6e20  tart="source in 
-00167020: 6d6f 6465 6c2e 736f 7572 6365 7320 7472  model.sources tr
-00167030: 6163 6b20 6279 2073 6f75 7263 652e 6e61  ack by source.na
-00167040: 6d65 225c 6e20 2020 2020 2020 2020 2020  me"\n           
-00167050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167070: 206e 672d 636c 6963 6b3d 2274 6f67 676c   ng-click="toggl
-00167080: 655f 736f 7572 6365 5f65 7870 616e 6465  e_source_expande
-00167090: 6428 736f 7572 6365 2922 5c6e 2020 2020  d(source)"\n    
-001670a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001670b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001670c0: 2020 2020 2020 2020 636c 6173 733d 2263          class="c
-001670d0: 6f6c 756d 6e2d 726f 7722 5c6e 2020 2020  olumn-row"\n    
-001670e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001670f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167100: 2020 2020 2020 2020 6e67 2d63 6c61 7373          ng-class
-00167110: 3d22 7b5c 2763 6f6c 756d 6e2d 726f 772d  ="{\'column-row-
-00167120: 7365 6c65 6374 6564 5c27 3a20 736f 7572  selected\': sour
-00167130: 6365 2e65 7870 616e 6465 647d 225c 6e20  ce.expanded}"\n 
-00167140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167160: 2020 2020 2020 2020 2020 206e 672d 7374             ng-st
-00167170: 796c 653d 227b 6375 7273 6f72 3a20 6861  yle="{cursor: ha
-00167180: 735f 6d6f 7265 5f69 6e66 6f28 736f 7572  s_more_info(sour
-00167190: 6365 2920 3f20 5c27 706f 696e 7465 725c  ce) ? \'pointer\
-001671a0: 2720 3a20 5c27 6175 746f 5c27 7d22 3e5c  ' : \'auto\'}">\
-001671b0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-001671c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001671d0: 2020 2020 2020 2020 2020 2020 203c 7464               <td
-001671e0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+00166ff0: 2020 2020 2020 2020 3c74 725c 6e20 2020          <tr\n   
+00167000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167020: 2020 2020 2020 2020 206e 672d 7265 7065           ng-repe
+00167030: 6174 2d73 7461 7274 3d22 736f 7572 6365  at-start="source
+00167040: 2069 6e20 6d6f 6465 6c2e 736f 7572 6365   in model.source
+00167050: 7320 7472 6163 6b20 6279 2073 6f75 7263  s track by sourc
+00167060: 652e 6e61 6d65 225c 6e20 2020 2020 2020  e.name"\n       
+00167070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167090: 2020 2020 206e 672d 636c 6963 6b3d 2274       ng-click="t
+001670a0: 6f67 676c 655f 736f 7572 6365 5f65 7870  oggle_source_exp
+001670b0: 616e 6465 6428 736f 7572 6365 2922 5c6e  anded(source)"\n
+001670c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001670d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001670e0: 2020 2020 2020 2020 2020 2020 636c 6173              clas
+001670f0: 733d 2263 6f6c 756d 6e2d 726f 7722 5c6e  s="column-row"\n
+00167100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167120: 2020 2020 2020 2020 2020 2020 6e67 2d63              ng-c
+00167130: 6c61 7373 3d22 7b5c 2763 6f6c 756d 6e2d  lass="{\'column-
+00167140: 726f 772d 7365 6c65 6374 6564 5c27 3a20  row-selected\': 
+00167150: 736f 7572 6365 2e65 7870 616e 6465 647d  source.expanded}
+00167160: 225c 6e20 2020 2020 2020 2020 2020 2020  "\n             
+00167170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167180: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00167190: 672d 7374 796c 653d 227b 6375 7273 6f72  g-style="{cursor
+001671a0: 3a20 6861 735f 6d6f 7265 5f69 6e66 6f28  : has_more_info(
+001671b0: 736f 7572 6365 2920 3f20 5c27 706f 696e  source) ? \'poin
+001671c0: 7465 725c 2720 3a20 5c27 6175 746f 5c27  ter\' : \'auto\'
+001671d0: 7d22 3e5c 6e20 2020 2020 2020 2020 2020  }">\n           
+001671e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001671f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167210: 2020 203c 6469 763e 5c6e 2020 2020 2020     <div>\n      
+00167200: 203c 7464 3e5c 6e20 2020 2020 2020 2020   <td>\n         
+00167210: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00167220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167240: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00167250: 7061 6e20 636c 6173 733d 5c27 7465 7874  pan class=\'text
-00167260: 2d64 6172 6b5c 273e 7b7b 2073 6f75 7263  -dark\'>{{ sourc
-00167270: 652e 736f 7572 6365 5f6e 616d 6520 7d7d  e.source_name }}
-00167280: 3c2f 7370 616e 3e5c 6e20 2020 2020 2020  </span>\n       
-00167290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001672a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001672b0: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-001672c0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-001672d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001672e0: 2020 2020 2020 2020 2020 2020 203c 2f74               </t
-001672f0: 643e 5c6e 2020 2020 2020 2020 2020 2020  d>\n            
+00167230: 2020 2020 2020 203c 6469 763e 5c6e 2020         <div>\n  
+00167240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167270: 2020 3c73 7061 6e20 636c 6173 733d 5c27    <span class=\'
+00167280: 7465 7874 2d64 6172 6b5c 273e 7b7b 2073  text-dark\'>{{ s
+00167290: 6f75 7263 652e 736f 7572 6365 5f6e 616d  ource.source_nam
+001672a0: 6520 7d7d 3c2f 7370 616e 3e5c 6e20 2020  e }}</span>\n   
+001672b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001672c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001672d0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+001672e0: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
+001672f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00167300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167320: 3c74 643e 5c6e 2020 2020 2020 2020 2020  <td>\n          
+00167310: 203c 2f74 643e 5c6e 2020 2020 2020 2020   </td>\n        
+00167320: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00167330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167350: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
-00167360: 733d 5c27 7465 7874 2d64 6172 6b5c 273e  s=\'text-dark\'>
-00167370: 7b7b 2073 6f75 7263 652e 6e61 6d65 207d  {{ source.name }
-00167380: 7d3c 2f70 3e5c 6e20 2020 2020 2020 2020  }</p>\n         
-00167390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001673a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001673b0: 2020 203c 2f74 643e 5c6e 2020 2020 2020     </td>\n      
+00167340: 2020 2020 3c74 643e 5c6e 2020 2020 2020      <td>\n      
+00167350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167370: 2020 2020 2020 2020 2020 3c73 7061 6e20            <span 
+00167380: 636c 6173 733d 5c27 7465 7874 2d64 6172  class=\'text-dar
+00167390: 6b5c 273e 7b7b 2073 6f75 7263 652e 6e61  k\'>{{ source.na
+001673a0: 6d65 207d 7d3c 2f70 3e5c 6e20 2020 2020  me }}</p>\n     
+001673b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001673c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001673d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001673e0: 2020 2020 2020 3c74 6420 7374 796c 653d        <td style=
-001673f0: 2274 6578 742d 6f76 6572 666c 6f77 3a20  "text-overflow: 
-00167400: 656c 6c69 7073 6973 3b20 6f76 6572 666c  ellipsis; overfl
-00167410: 6f77 2d78 3a20 6869 6464 656e 3b20 7768  ow-x: hidden; wh
-00167420: 6974 652d 7370 6163 653a 206e 6f77 7261  ite-space: nowra
-00167430: 703b 206d 6178 2d77 6964 7468 3a20 3170  p; max-width: 1p
-00167440: 783b 223e 5c6e 2020 2020 2020 2020 2020  x;">\n          
-00167450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167470: 2020 2020 2020 3c73 7061 6e20 6e67 2d73        <span ng-s
-00167480: 686f 773d 2221 636f 6c75 6d6e 2e65 7870  how="!column.exp
-00167490: 616e 6465 6422 3e7b 7b20 736f 7572 6365  anded">{{ source
-001674a0: 2e64 6573 6372 6970 7469 6f6e 207d 7d3c  .description }}<
-001674b0: 2f73 7061 6e3e 5c6e 2020 2020 2020 2020  /span>\n        
-001674c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001674d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001674e0: 2020 2020 3c2f 7464 3e5c 6e20 2020 2020      </td>\n     
+001673d0: 2020 2020 2020 203c 2f74 643e 5c6e 2020         </td>\n  
+001673e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001673f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167400: 2020 2020 2020 2020 2020 3c74 6420 7374            <td st
+00167410: 796c 653d 2274 6578 742d 6f76 6572 666c  yle="text-overfl
+00167420: 6f77 3a20 656c 6c69 7073 6973 3b20 6f76  ow: ellipsis; ov
+00167430: 6572 666c 6f77 2d78 3a20 6869 6464 656e  erflow-x: hidden
+00167440: 3b20 7768 6974 652d 7370 6163 653a 206e  ; white-space: n
+00167450: 6f77 7261 703b 206d 6178 2d77 6964 7468  owrap; max-width
+00167460: 3a20 3170 783b 223e 5c6e 2020 2020 2020  : 1px;">\n      
+00167470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167490: 2020 2020 2020 2020 2020 3c73 7061 6e20            <span 
+001674a0: 6e67 2d73 686f 773d 2221 636f 6c75 6d6e  ng-show="!column
+001674b0: 2e65 7870 616e 6465 6422 3e7b 7b20 736f  .expanded">{{ so
+001674c0: 7572 6365 2e64 6573 6372 6970 7469 6f6e  urce.description
+001674d0: 207d 7d3c 2f73 7061 6e3e 5c6e 2020 2020   }}</span>\n    
+001674e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001674f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167510: 2020 2020 2020 203c 7464 3e5c 6e20 2020         <td>\n   
+00167500: 2020 2020 2020 2020 3c2f 7464 3e5c 6e20          </td>\n 
+00167510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00167520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167540: 2020 2020 2020 2020 2020 2020 203c 6120               <a 
-00167550: 7569 2d73 7265 663d 2264 6274 2e73 6f75  ui-sref="dbt.sou
-00167560: 7263 6528 7b75 6e69 7175 655f 6964 3a20  rce({unique_id: 
-00167570: 736f 7572 6365 2e75 6e69 7175 655f 6964  source.unique_id
-00167580: 7d29 223e 5669 6577 2064 6f63 733c 2f61  })">View docs</a
-00167590: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-001675a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001675b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-001675c0: 2f74 643e 5c6e 2020 2020 2020 2020 2020  /td>\n          
+00167530: 2020 2020 2020 2020 2020 203c 7464 3e5c             <td>\
+00167540: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00167550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167570: 203c 6120 7569 2d73 7265 663d 2264 6274   <a ui-sref="dbt
+00167580: 2e73 6f75 7263 6528 7b75 6e69 7175 655f  .source({unique_
+00167590: 6964 3a20 736f 7572 6365 2e75 6e69 7175  id: source.uniqu
+001675a0: 655f 6964 7d29 223e 5669 6577 2064 6f63  e_id})">View doc
+001675b0: 733c 2f61 3e5c 6e20 2020 2020 2020 2020  s</a>\n         
+001675c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001675d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001675e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001675f0: 2020 3c74 6420 636c 6173 733d 5c27 7465    <td class=\'te
-00167600: 7874 2d63 656e 7465 725c 273e 5c6e 2020  xt-center\'>\n  
-00167610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167630: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00167640: 7061 6e20 636c 6173 733d 5c27 7465 7874  pan class=\'text
-00167650: 2d6c 6967 6874 5c27 206e 672d 7368 6f77  -light\' ng-show
-00167660: 3d22 6861 735f 6d6f 7265 5f69 6e66 6f28  ="has_more_info(
-00167670: 736f 7572 6365 2922 3e5c 6e20 2020 2020  source)">\n     
-00167680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001676a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-001676b0: 7370 616e 206e 672d 6966 3d22 736f 7572  span ng-if="sour
-001676c0: 6365 2e65 7870 616e 6465 6422 3e5c 6e20  ce.expanded">\n 
-001676d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001676e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001676f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167700: 2020 2020 2020 203c 7376 6720 636c 6173         <svg clas
-00167710: 733d 2269 636e 223e 3c75 7365 2078 6c69  s="icn"><use xli
-00167720: 6e6b 3a68 7265 663d 2223 6963 6e2d 7570  nk:href="#icn-up
-00167730: 223e 3c2f 7573 653e 3c2f 7376 673e 5c6e  "></use></svg>\n
-00167740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167770: 2020 2020 3c2f 7370 616e 3e5c 6e20 2020      </span>\n   
+001675e0: 2020 203c 2f74 643e 5c6e 2020 2020 2020     </td>\n      
+001675f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167610: 2020 2020 2020 3c74 6420 636c 6173 733d        <td class=
+00167620: 5c27 7465 7874 2d63 656e 7465 725c 273e  \'text-center\'>
+00167630: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00167640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167660: 2020 3c73 7061 6e20 636c 6173 733d 5c27    <span class=\'
+00167670: 7465 7874 2d6c 6967 6874 5c27 206e 672d  text-light\' ng-
+00167680: 7368 6f77 3d22 6861 735f 6d6f 7265 5f69  show="has_more_i
+00167690: 6e66 6f28 736f 7572 6365 2922 3e5c 6e20  nfo(source)">\n 
+001676a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001676b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001676c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001676d0: 2020 203c 7370 616e 206e 672d 6966 3d22     <span ng-if="
+001676e0: 736f 7572 6365 2e65 7870 616e 6465 6422  source.expanded"
+001676f0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+00167700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167720: 2020 2020 2020 2020 2020 203c 7376 6720             <svg 
+00167730: 636c 6173 733d 2269 636e 223e 3c75 7365  class="icn"><use
+00167740: 2078 6c69 6e6b 3a68 7265 663d 2223 6963   xlink:href="#ic
+00167750: 6e2d 7570 223e 3c2f 7573 653e 3c2f 7376  n-up"></use></sv
+00167760: 673e 5c6e 2020 2020 2020 2020 2020 2020  g>\n            
+00167770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00167780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001677a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001677b0: 203c 7370 616e 206e 672d 6966 3d22 2173   <span ng-if="!s
-001677c0: 6f75 7263 652e 6578 7061 6e64 6564 223e  ource.expanded">
-001677d0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-001677e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001677f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167800: 2020 2020 2020 2020 2020 3c73 7667 2063            <svg c
-00167810: 6c61 7373 3d22 6963 6e22 3e3c 7573 6520  lass="icn"><use 
-00167820: 786c 696e 6b3a 6872 6566 3d22 2369 636e  xlink:href="#icn
-00167830: 2d72 6967 6874 223e 3c2f 7573 653e 3c2f  -right"></use></
-00167840: 7376 673e 5c6e 2020 2020 2020 2020 2020  svg>\n          
-00167850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167870: 2020 2020 2020 2020 2020 3c2f 7370 616e            </span
-00167880: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-00167890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001678a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001678b0: 2020 203c 2f73 7061 6e3e 5c6e 2020 2020     </span>\n    
+00167790: 2020 2020 2020 2020 3c2f 7370 616e 3e5c          </span>\
+001677a0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+001677b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001677c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001677d0: 2020 2020 203c 7370 616e 206e 672d 6966       <span ng-if
+001677e0: 3d22 2173 6f75 7263 652e 6578 7061 6e64  ="!source.expand
+001677f0: 6564 223e 5c6e 2020 2020 2020 2020 2020  ed">\n          
+00167800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167820: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+00167830: 7667 2063 6c61 7373 3d22 6963 6e22 3e3c  vg class="icn"><
+00167840: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
+00167850: 2369 636e 2d72 6967 6874 223e 3c2f 7573  #icn-right"></us
+00167860: 653e 3c2f 7376 673e 5c6e 2020 2020 2020  e></svg>\n      
+00167870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167890: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+001678a0: 7370 616e 3e5c 6e20 2020 2020 2020 2020  span>\n         
+001678b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001678c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001678d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001678e0: 2020 2020 2020 2020 3c2f 7464 3e5c 6e20          </td>\n 
+001678d0: 2020 2020 2020 203c 2f73 7061 6e3e 5c6e         </span>\n
+001678e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001678f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167910: 2020 2020 2020 203c 2f74 723e 5c6e 2020         </tr>\n  
+00167900: 2020 2020 2020 2020 2020 2020 3c2f 7464              </td
+00167910: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
 00167920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167940: 2020 2020 2020 3c74 7220 6e67 2d72 6570        <tr ng-rep
-00167950: 6561 742d 656e 6420 6e67 2d73 686f 773d  eat-end ng-show=
-00167960: 2273 6f75 7263 652e 6578 7061 6e64 6564  "source.expanded
-00167970: 2220 7374 796c 653d 2262 6163 6b67 726f  " style="backgro
-00167980: 756e 642d 636f 6c6f 723a 2077 6869 7465  und-color: white
-00167990: 3b20 7061 6464 696e 673a 2031 3070 7822  ; padding: 10px"
-001679a0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-001679b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001679c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-001679d0: 7464 2063 6f6c 7370 616e 3d22 3522 2063  td colspan="5" c
-001679e0: 6c61 7373 3d22 636f 6c75 6d6e 2d65 7870  lass="column-exp
-001679f0: 616e 6465 6422 3e5c 6e20 2020 2020 2020  anded">\n       
-00167a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167a20: 2020 2020 2020 2020 203c 6469 7620 7374           <div st
-00167a30: 796c 653d 2270 6164 6469 6e67 3a20 3570  yle="padding: 5p
-00167a40: 7820 3230 7078 223e 5c6e 2020 2020 2020  x 20px">\n      
-00167a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167a70: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00167a80: 6976 2073 7479 6c65 3d22 6d61 7267 696e  iv style="margin
-00167a90: 2d62 6f74 746f 6d3a 2031 3570 7822 3e5c  -bottom: 15px">\
-00167aa0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00167ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167ad0: 2020 2020 2020 2020 203c 6835 3e44 6573           <h5>Des
-00167ae0: 6372 6970 7469 6f6e 3c2f 6835 3e5c 6e20  cription</h5>\n 
-00167af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167b20: 2020 2020 2020 203c 7370 616e 206d 6172         <span mar
-00167b30: 6b65 643d 2273 6f75 7263 652e 6465 7363  ked="source.desc
-00167b40: 7269 7074 696f 6e22 3e3c 2f73 7061 6e3e  ription"></span>
-00167b50: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00167b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167b80: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
+00167930: 2020 2020 2020 2020 2020 203c 2f74 723e             </tr>
+00167940: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00167950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167960: 2020 2020 2020 2020 2020 3c74 7220 6e67            <tr ng
+00167970: 2d72 6570 6561 742d 656e 6420 6e67 2d73  -repeat-end ng-s
+00167980: 686f 773d 2273 6f75 7263 652e 6578 7061  how="source.expa
+00167990: 6e64 6564 2220 7374 796c 653d 2262 6163  nded" style="bac
+001679a0: 6b67 726f 756e 642d 636f 6c6f 723a 2077  kground-color: w
+001679b0: 6869 7465 3b20 7061 6464 696e 673a 2031  hite; padding: 1
+001679c0: 3070 7822 3e5c 6e20 2020 2020 2020 2020  0px">\n         
+001679d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001679e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001679f0: 2020 203c 7464 2063 6f6c 7370 616e 3d22     <td colspan="
+00167a00: 3522 2063 6c61 7373 3d22 636f 6c75 6d6e  5" class="column
+00167a10: 2d65 7870 616e 6465 6422 3e5c 6e20 2020  -expanded">\n   
+00167a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167a40: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00167a50: 7620 7374 796c 653d 2270 6164 6469 6e67  v style="padding
+00167a60: 3a20 3570 7820 3230 7078 223e 5c6e 2020  : 5px 20px">\n  
+00167a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167aa0: 2020 3c64 6976 2073 7479 6c65 3d22 6d61    <div style="ma
+00167ab0: 7267 696e 2d62 6f74 746f 6d3a 2031 3570  rgin-bottom: 15p
+00167ac0: 7822 3e5c 6e20 2020 2020 2020 2020 2020  x">\n           
+00167ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167af0: 2020 2020 2020 2020 2020 2020 203c 6835               <h5
+00167b00: 3e44 6573 6372 6970 7469 6f6e 3c2f 6835  >Description</h5
+00167b10: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+00167b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167b40: 2020 2020 2020 2020 2020 203c 7370 616e             <span
+00167b50: 206d 6172 6b65 643d 2273 6f75 7263 652e   marked="source.
+00167b60: 6465 7363 7269 7074 696f 6e22 3e3c 2f73  description"></s
+00167b70: 7061 6e3e 5c6e 2020 2020 2020 2020 2020  pan>\n          
+00167b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00167b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167bb0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00167bc0: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
+00167ba0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00167bb0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00167bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00167bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167bf0: 2020 3c2f 7464 3e5c 6e20 2020 2020 2020    </td>\n       
+00167be0: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
+00167bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00167c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167c20: 203c 2f74 723e 5c6e 2020 2020 2020 2020   </tr>\n        
+00167c10: 2020 2020 2020 3c2f 7464 3e5c 6e20 2020        </td>\n   
+00167c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00167c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167c40: 2020 2020 2020 2020 2020 2020 3c2f 7462              </tb
-00167c50: 6f64 793e 5c6e 2020 2020 2020 2020 2020  ody>\n          
+00167c40: 2020 2020 203c 2f74 723e 5c6e 2020 2020       </tr>\n    
+00167c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00167c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167c70: 2020 2020 2020 3c2f 7461 626c 653e 5c6e        </table>\n
+00167c70: 3c2f 7462 6f64 793e 5c6e 2020 2020 2020  </tbody>\n      
 00167c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167c90: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00167ca0: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
-00167cb0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00167cc0: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
-00167cd0: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
-00167ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167cf0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-00167d00: 2020 2020 3c2f 7365 6374 696f 6e3e 5c6e      </section>\n
-00167d10: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
-00167d20: 2020 2020 3c2f 6469 763e 5c6e 3c2f 6469      </div>\n</di
-00167d30: 763e 5c6e 2729 7d5d 292c 652e 6578 706f  v>\n')}]),e.expo
-00167d40: 7274 733d 6e7d 2c66 756e 6374 696f 6e28  rts=n},function(
-00167d50: 652c 7429 7b76 6172 206e 3d22 2f64 6f63  e,t){var n="/doc
-00167d60: 732f 6d6f 6465 6c2e 6874 6d6c 223b 7769  s/model.html";wi
-00167d70: 6e64 6f77 2e61 6e67 756c 6172 2e6d 6f64  ndow.angular.mod
-00167d80: 756c 6528 226e 6722 292e 7275 6e28 5b22  ule("ng").run(["
-00167d90: 2474 656d 706c 6174 6543 6163 6865 222c  $templateCache",
-00167da0: 6675 6e63 7469 6f6e 2865 297b 652e 7075  function(e){e.pu
-00167db0: 7428 6e2c 273c 7374 796c 653e 5c6e 2f2a  t(n,'<style>\n/*
-00167dc0: 2054 4f44 4f20 2a2f 5c6e 2e73 6563 7469   TODO */\n.secti
-00167dd0: 6f6e 2d74 6172 6765 7420 7b5c 6e20 2020  on-target {\n   
-00167de0: 2074 6f70 3a20 2d38 656d 3b5c 6e7d 5c6e   top: -8em;\n}\n
-00167df0: 5c6e 2e6e 6f66 6c65 7820 7b5c 6e20 2020  \n.noflex {\n   
-00167e00: 2066 6c65 783a 2030 2030 2031 3630 7078   flex: 0 0 160px
-00167e10: 2021 696d 706f 7274 616e 743b 5c6e 7d5c   !important;\n}\
-00167e20: 6e5c 6e2e 6869 6768 6c69 6768 7420 7b5c  n\n.highlight {\
-00167e30: 6e20 2020 2063 6f6c 6f72 3a20 2332 3432  n    color: #242
-00167e40: 3932 653b 5c6e 2020 2020 6261 636b 6772  92e;\n    backgr
-00167e50: 6f75 6e64 2d63 6f6c 6f72 3a20 7768 6974  ound-color: whit
-00167e60: 653b 5c6e 7d5c 6e5c 6e3c 2f73 7479 6c65  e;\n}\n\n</style
-00167e70: 3e5c 6e5c 6e3c 6469 7620 636c 6173 733d  >\n\n<div class=
-00167e80: 5c27 6170 702d 7363 726f 6c6c 5c27 3e5c  \'app-scroll\'>\
-00167e90: 6e20 2020 203c 6469 7620 636c 6173 733d  n    <div class=
-00167ea0: 2261 7070 2d6c 696e 6b73 2061 7070 2d73  "app-links app-s
-00167eb0: 7469 636b 7922 3e5c 6e20 2020 2020 2020  ticky">\n       
-00167ec0: 203c 6469 7620 636c 6173 733d 2261 7070   <div class="app
-00167ed0: 2d74 6974 6c65 223e 5c6e 2020 2020 2020  -title">\n      
-00167ee0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00167ef0: 3d22 6170 702d 6672 616d 6520 6170 702d  ="app-frame app-
-00167f00: 7061 6420 6170 702d 666c 7573 682d 626f  pad app-flush-bo
-00167f10: 7474 6f6d 223e 5c6e 2020 2020 2020 2020  ttom">\n        
-00167f20: 2020 2020 2020 2020 3c68 3120 6e67 2d69          <h1 ng-i
-00167f30: 663d 226d 6f64 656c 2e64 6f63 732e 7368  f="model.docs.sh
-00167f40: 6f77 203d 3d3d 2066 616c 7365 223e 5c6e  ow === false">\n
-00167f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167f60: 2020 2020 3c73 6d61 6c6c 2063 6c61 7373      <small class
-00167f70: 3d5c 2774 6578 742d 626f 6c64 2074 6578  =\'text-bold tex
-00167f80: 742d 7269 6768 745c 273e 5c6e 2020 2020  t-right\'>\n    
-00167f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167fa0: 2020 2020 3c69 2064 6174 612d 6963 6f6e      <i data-icon
-00167fb0: 3d22 6579 6522 3e3c 2f69 3e5c 6e20 2020  ="eye"></i>\n   
-00167fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00167fd0: 2020 2020 2054 6869 7320 6d6f 6465 6c20       This model 
-00167fe0: 6973 2068 6964 6465 6e5c 6e20 2020 2020  is hidden\n     
-00167ff0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00168000: 2f73 6d61 6c6c 3e5c 6e20 2020 2020 2020  /small>\n       
-00168010: 2020 2020 2020 2020 203c 2f68 313e 5c6e           </h1>\n
-00168020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00168030: 3c68 313e 5c6e 2020 2020 2020 2020 2020  <h1>\n          
-00168040: 2020 2020 2020 2020 2020 3c73 7061 6e20            <span 
-00168050: 636c 6173 733d 2262 7265 616b 223e 7b7b  class="break">{{
-00168060: 206d 6f64 656c 2e6e 616d 6520 7d7d 3c2f   model.name }}</
-00168070: 7370 616e 3e5c 6e20 2020 2020 2020 2020  span>\n         
-00168080: 2020 2020 2020 2020 2020 203c 736d 616c             <smal
-00168090: 6c3e 7b7b 206d 6f64 656c 2e63 6f6e 6669  l>{{ model.confi
-001680a0: 672e 6d61 7465 7269 616c 697a 6564 207d  g.materialized }
-001680b0: 7d3c 2f73 6d61 6c6c 3e5c 6e20 2020 2020  }</small>\n     
-001680c0: 2020 2020 2020 2020 2020 203c 2f68 313e             </h1>
-001680d0: 5c6e 2020 2020 2020 2020 2020 2020 3c2f  \n            </
-001680e0: 6469 763e 5c6e 2020 2020 2020 2020 3c2f  div>\n        </
-001680f0: 6469 763e 5c6e 2020 2020 2020 2020 3c64  div>\n        <d
-00168100: 6976 2063 6c61 7373 3d22 6170 702d 6672  iv class="app-fr
-00168110: 616d 6520 6170 702d 7061 642d 6822 3e5c  ame app-pad-h">\
-00168120: 6e20 2020 2020 2020 2020 2020 203c 756c  n            <ul
-00168130: 2063 6c61 7373 3d22 6e61 7620 6e61 762d   class="nav nav-
-00168140: 7461 6273 223e 5c6e 2020 2020 2020 2020  tabs">\n        
-00168150: 2020 2020 2020 2020 3c6c 6920 7569 2d73          <li ui-s
-00168160: 7265 662d 6163 7469 7665 3d5c 2761 6374  ref-active=\'act
-00168170: 6976 655c 273e 3c61 2075 692d 7372 6566  ive\'><a ui-sref
-00168180: 3d22 6462 742e 6d6f 6465 6c28 7b5c 2723  ="dbt.model({\'#
-00168190: 5c27 3a20 5c27 6465 7461 696c 735c 277d  \': \'details\'}
-001681a0: 2922 3e44 6574 6169 6c73 3c2f 613e 3c2f  )">Details</a></
-001681b0: 6c69 3e5c 6e20 2020 2020 2020 2020 2020  li>\n           
-001681c0: 2020 2020 203c 6c69 2075 692d 7372 6566       <li ui-sref
-001681d0: 2d61 6374 6976 653d 5c27 6163 7469 7665  -active=\'active
-001681e0: 5c27 3e3c 6120 7569 2d73 7265 663d 2264  \'><a ui-sref="d
-001681f0: 6274 2e6d 6f64 656c 287b 5c27 235c 273a  bt.model({\'#\':
-00168200: 205c 2764 6573 6372 6970 7469 6f6e 5c27   \'description\'
-00168210: 7d29 223e 4465 7363 7269 7074 696f 6e3c  })">Description<
-00168220: 2f61 3e3c 2f6c 693e 5c6e 2020 2020 2020  /a></li>\n      
-00168230: 2020 2020 2020 2020 2020 3c6c 6920 7569            <li ui
-00168240: 2d73 7265 662d 6163 7469 7665 3d5c 2761  -sref-active=\'a
-00168250: 6374 6976 655c 273e 3c61 2075 692d 7372  ctive\'><a ui-sr
-00168260: 6566 3d22 6462 742e 6d6f 6465 6c28 7b5c  ef="dbt.model({\
-00168270: 2723 5c27 3a20 5c27 636f 6c75 6d6e 735c  '#\': \'columns\
-00168280: 277d 2922 3e43 6f6c 756d 6e73 3c2f 613e  '})">Columns</a>
-00168290: 3c2f 6c69 3e5c 6e20 2020 2020 2020 2020  </li>\n         
-001682a0: 2020 2020 2020 203c 6c69 2075 692d 7372         <li ui-sr
-001682b0: 6566 2d61 6374 6976 653d 5c27 6163 7469  ef-active=\'acti
-001682c0: 7665 5c27 206e 672d 7368 6f77 203d 2022  ve\' ng-show = "
-001682d0: 7265 6665 7265 6e63 6573 4c65 6e67 7468  referencesLength
-001682e0: 2021 3d20 3022 3e3c 6120 7569 2d73 7265   != 0"><a ui-sre
-001682f0: 663d 2264 6274 2e6d 6f64 656c 287b 5c27  f="dbt.model({\'
-00168300: 235c 273a 205c 2772 6566 6572 656e 6365  #\': \'reference
-00168310: 645f 6279 5c27 7d29 223e 5265 6665 7265  d_by\'})">Refere
-00168320: 6e63 6564 2042 793c 2f61 3e3c 2f6c 693e  nced By</a></li>
-00168330: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00168340: 2020 3c6c 6920 7569 2d73 7265 662d 6163    <li ui-sref-ac
-00168350: 7469 7665 3d5c 2761 6374 6976 655c 2720  tive=\'active\' 
-00168360: 6e67 2d73 686f 7720 3d20 2270 6172 656e  ng-show = "paren
-00168370: 7473 4c65 6e67 7468 2021 3d20 3022 3e3c  tsLength != 0"><
-00168380: 6120 7569 2d73 7265 663d 2264 6274 2e6d  a ui-sref="dbt.m
-00168390: 6f64 656c 287b 5c27 235c 273a 205c 2764  odel({\'#\': \'d
-001683a0: 6570 656e 6473 5f6f 6e5c 277d 2922 3e44  epends_on\'})">D
-001683b0: 6570 656e 6473 204f 6e3c 2f61 3e3c 2f6c  epends On</a></l
-001683c0: 693e 5c6e 2020 2020 2020 2020 2020 2020  i>\n            
-001683d0: 2020 2020 3c6c 6920 7569 2d73 7265 662d      <li ui-sref-
-001683e0: 6163 7469 7665 3d5c 2761 6374 6976 655c  active=\'active\
-001683f0: 273e 3c61 2075 692d 7372 6566 3d22 6462  '><a ui-sref="db
-00168400: 742e 6d6f 6465 6c28 7b5c 2723 5c27 3a20  t.model({\'#\': 
-00168410: 5c27 636f 6465 5c27 7d29 223e 436f 6465  \'code\'})">Code
-00168420: 3c2f 613e 3c2f 6c69 3e5c 6e20 2020 2020  </a></li>\n     
-00168430: 2020 2020 2020 203c 2f75 6c3e 5c6e 2020         </ul>\n  
-00168440: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
-00168450: 2020 3c2f 6469 763e 5c6e 2020 2020 3c64    </div>\n    <d
-00168460: 6976 2063 6c61 7373 3d22 6170 702d 6465  iv class="app-de
-00168470: 7461 696c 7322 3e5c 6e20 2020 2020 2020  tails">\n       
-00168480: 203c 6469 7620 636c 6173 733d 2261 7070   <div class="app
-00168490: 2d66 7261 6d65 2061 7070 2d70 6164 223e  -frame app-pad">
-001684a0: 5c6e 2020 2020 2020 2020 2020 2020 3c73  \n            <s
-001684b0: 6563 7469 6f6e 2063 6c61 7373 3d22 7365  ection class="se
-001684c0: 6374 696f 6e22 3e5c 6e20 2020 2020 2020  ction">\n       
-001684d0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-001684e0: 6173 733d 2273 6563 7469 6f6e 2d74 6172  ass="section-tar
-001684f0: 6765 7422 2069 643d 2264 6574 6169 6c73  get" id="details
-00168500: 223e 3c2f 6469 763e 5c6e 2020 2020 2020  "></div>\n      
-00168510: 2020 2020 2020 2020 2020 3c74 6162 6c65            <table
-00168520: 2d64 6574 6169 6c73 206d 6f64 656c 3d22  -details model="
-00168530: 6d6f 6465 6c22 3e3c 2f74 6162 6c65 2d64  model"></table-d
-00168540: 6574 6169 6c73 3e5c 6e20 2020 2020 2020  etails>\n       
-00168550: 2020 2020 203c 2f73 6563 7469 6f6e 3e5c       </section>\
-00168560: 6e5c 6e20 2020 2020 2020 2020 2020 203c  n\n            <
-00168570: 7365 6374 696f 6e20 636c 6173 733d 2273  section class="s
-00168580: 6563 7469 6f6e 223e 5c6e 2020 2020 2020  ection">\n      
-00168590: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-001685a0: 6c61 7373 3d22 7365 6374 696f 6e2d 7461  lass="section-ta
-001685b0: 7267 6574 2220 6964 3d22 6465 7363 7269  rget" id="descri
-001685c0: 7074 696f 6e22 3e3c 2f64 6976 3e5c 6e20  ption"></div>\n 
-001685d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-001685e0: 6469 7620 636c 6173 733d 2273 6563 7469  div class="secti
-001685f0: 6f6e 2d63 6f6e 7465 6e74 223e 5c6e 2020  on-content">\n  
-00168600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00168610: 2020 3c68 363e 4465 7363 7269 7074 696f    <h6>Descriptio
-00168620: 6e3c 2f68 363e 5c6e 2020 2020 2020 2020  n</h6>\n        
-00168630: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00168640: 2063 6c61 7373 3d22 7061 6e65 6c22 3e5c   class="panel">\
-00168650: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00168660: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00168670: 6173 733d 2270 616e 656c 2d62 6f64 7922  ass="panel-body"
-00168680: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-00168690: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-001686a0: 6469 7620 6e67 2d69 663d 226d 6f64 656c  div ng-if="model
-001686b0: 2e64 6573 6372 6970 7469 6f6e 2220 636c  .description" cl
-001686c0: 6173 733d 226d 6f64 656c 2d6d 6172 6b64  ass="model-markd
-001686d0: 6f77 6e22 206d 6172 6b65 643d 226d 6f64  own" marked="mod
-001686e0: 656c 2e64 6573 6372 6970 7469 6f6e 223e  el.description">
-001686f0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-00168700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00168710: 2020 2020 3c64 6976 206e 672d 6966 3d22      <div ng-if="
-00168720: 216d 6f64 656c 2e64 6573 6372 6970 7469  !model.descripti
-00168730: 6f6e 223e 5468 6973 207b 7b20 6d6f 6465  on">This {{ mode
-00168740: 6c2e 7265 736f 7572 6365 5f74 7970 6520  l.resource_type 
-00168750: 7d7d 2069 7320 6e6f 7420 6375 7272 656e  }} is not curren
-00168760: 746c 7920 646f 6375 6d65 6e74 6564 3c2f  tly documented</
-00168770: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
-00168780: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00168790: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
-001687a0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-001687b0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-001687c0: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
-001687d0: 2020 2020 2020 3c2f 7365 6374 696f 6e3e        </section>
-001687e0: 5c6e 5c6e 2020 2020 2020 2020 2020 2020  \n\n            
-001687f0: 3c73 6563 7469 6f6e 2063 6c61 7373 3d22  <section class="
-00168800: 7365 6374 696f 6e22 3e5c 6e20 2020 2020  section">\n     
-00168810: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00168820: 636c 6173 733d 2273 6563 7469 6f6e 2d74  class="section-t
-00168830: 6172 6765 7422 2069 643d 2263 6f6c 756d  arget" id="colum
-00168840: 6e73 223e 3c2f 6469 763e 5c6e 2020 2020  ns"></div>\n    
-00168850: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00168860: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
-00168870: 636f 6e74 656e 7422 3e5c 6e20 2020 2020  content">\n     
-00168880: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00168890: 6836 3e43 6f6c 756d 6e73 3c2f 6836 3e5c  h6>Columns</h6>\
-001688a0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-001688b0: 2020 2020 203c 636f 6c75 6d6e 2d64 6574       <column-det
-001688c0: 6169 6c73 206d 6f64 656c 3d22 6d6f 6465  ails model="mode
-001688d0: 6c22 202f 3e5c 6e20 2020 2020 2020 2020  l" />\n         
-001688e0: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
-001688f0: 2020 2020 2020 2020 2020 203c 2f73 6563             </sec
-00168900: 7469 6f6e 3e5c 6e5c 6e20 2020 2020 2020  tion>\n\n       
-00168910: 2020 2020 203c 7365 6374 696f 6e20 636c       <section cl
-00168920: 6173 733d 2273 6563 7469 6f6e 2220 6e67  ass="section" ng
-00168930: 2d73 686f 7720 3d20 2272 6566 6572 656e  -show = "referen
-00168940: 6365 734c 656e 6774 6820 213d 2030 223e  cesLength != 0">
-00168950: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00168960: 2020 3c64 6976 2063 6c61 7373 3d22 7365    <div class="se
-00168970: 6374 696f 6e2d 7461 7267 6574 2220 6964  ction-target" id
-00168980: 3d22 7265 6665 7265 6e63 6564 5f62 7922  ="referenced_by"
-00168990: 3e3c 2f64 6976 3e5c 6e20 2020 2020 2020  ></div>\n       
-001689a0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-001689b0: 6173 733d 2273 6563 7469 6f6e 2d63 6f6e  ass="section-con
-001689c0: 7465 6e74 223e 5c6e 2020 2020 2020 2020  tent">\n        
-001689d0: 2020 2020 2020 2020 2020 2020 3c68 363e              <h6>
-001689e0: 5265 6665 7265 6e63 6564 2042 793c 2f68  Referenced By</h
-001689f0: 363e 5c6e 2020 2020 2020 2020 2020 2020  6>\n            
-00168a00: 2020 2020 2020 2020 3c72 6566 6572 656e          <referen
-00168a10: 6365 2d6c 6973 7420 7265 6665 7265 6e63  ce-list referenc
-00168a20: 6573 3d22 7265 6665 7265 6e63 6573 2220  es="references" 
-00168a30: 6e6f 6465 3d22 6d6f 6465 6c22 202f 3e5c  node="model" />\
-00168a40: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00168a50: 203c 2f64 6976 3e5c 6e20 2020 2020 2020   </div>\n       
-00168a60: 2020 2020 203c 2f73 6563 7469 6f6e 3e5c       </section>\
-00168a70: 6e5c 6e20 2020 2020 2020 2020 2020 203c  n\n            <
-00168a80: 7365 6374 696f 6e20 636c 6173 733d 2273  section class="s
-00168a90: 6563 7469 6f6e 2220 6e67 2d73 686f 7720  ection" ng-show 
-00168aa0: 3d20 2270 6172 656e 7473 4c65 6e67 7468  = "parentsLength
-00168ab0: 2021 3d20 3022 3e5c 6e20 2020 2020 2020   != 0">\n       
-00168ac0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00168ad0: 6173 733d 2273 6563 7469 6f6e 2d74 6172  ass="section-tar
-00168ae0: 6765 7422 2069 643d 2264 6570 656e 6473  get" id="depends
-00168af0: 5f6f 6e22 3e3c 2f64 6976 3e5c 6e20 2020  _on"></div>\n   
-00168b00: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00168b10: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
-00168b20: 2d63 6f6e 7465 6e74 223e 5c6e 2020 2020  -content">\n    
-00168b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00168b40: 3c68 363e 4465 7065 6e64 7320 4f6e 3c2f  <h6>Depends On</
-00168b50: 6836 3e5c 6e20 2020 2020 2020 2020 2020  h6>\n           
-00168b60: 2020 2020 2020 2020 203c 7265 6665 7265           <refere
-00168b70: 6e63 652d 6c69 7374 2072 6566 6572 656e  nce-list referen
-00168b80: 6365 733d 2270 6172 656e 7473 2220 6e6f  ces="parents" no
-00168b90: 6465 3d22 6d6f 6465 6c22 202f 3e5c 6e20  de="model" />\n 
-00168ba0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00168bb0: 2f64 6976 3e5c 6e20 2020 2020 2020 2020  /div>\n         
-00168bc0: 2020 203c 2f73 6563 7469 6f6e 3e5c 6e5c     </section>\n\
-00168bd0: 6e20 2020 2020 2020 2020 2020 203c 7365  n            <se
-00168be0: 6374 696f 6e20 636c 6173 733d 2273 6563  ction class="sec
-00168bf0: 7469 6f6e 223e 5c6e 2020 2020 2020 2020  tion">\n        
-00168c00: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00168c10: 7373 3d22 7365 6374 696f 6e2d 7461 7267  ss="section-targ
-00168c20: 6574 2220 6964 3d22 636f 6465 223e 3c2f  et" id="code"></
-00168c30: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
-00168c40: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00168c50: 3d22 7365 6374 696f 6e2d 636f 6e74 656e  ="section-conten
-00168c60: 7422 3e5c 6e20 2020 2020 2020 2020 2020  t">\n           
-00168c70: 2020 2020 2020 2020 203c 636f 6465 2d62           <code-b
-00168c80: 6c6f 636b 2076 6572 7369 6f6e 733d 2276  lock versions="v
-00168c90: 6572 7369 6f6e 7322 2064 6566 6175 6c74  ersions" default
-00168ca0: 3d22 6465 6661 756c 745f 7665 7273 696f  ="default_versio
-00168cb0: 6e22 206c 616e 6775 6167 653d 226c 616e  n" language="lan
-00168cc0: 6775 6167 6522 3e3c 2f63 6f64 652d 626c  guage"></code-bl
-00168cd0: 6f63 6b3e 5c6e 2020 2020 2020 2020 2020  ock>\n          
-00168ce0: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
-00168cf0: 2020 2020 2020 2020 2020 3c2f 7365 6374            </sect
-00168d00: 696f 6e3e 5c6e 2020 2020 2020 2020 3c2f  ion>\n        </
-00168d10: 6469 763e 5c6e 2020 2020 3c2f 6469 763e  div>\n    </div>
-00168d20: 5c6e 3c2f 6469 763e 5c6e 2729 7d5d 292c  \n</div>\n')}]),
-00168d30: 652e 6578 706f 7274 733d 6e7d 2c66 756e  e.exports=n},fun
-00168d40: 6374 696f 6e28 652c 7429 7b76 6172 206e  ction(e,t){var n
-00168d50: 3d22 2f64 6f63 732f 736e 6170 7368 6f74  ="/docs/snapshot
-00168d60: 2e68 746d 6c22 3b77 696e 646f 772e 616e  .html";window.an
-00168d70: 6775 6c61 722e 6d6f 6475 6c65 2822 6e67  gular.module("ng
-00168d80: 2229 2e72 756e 285b 2224 7465 6d70 6c61  ").run(["$templa
-00168d90: 7465 4361 6368 6522 2c66 756e 6374 696f  teCache",functio
-00168da0: 6e28 6529 7b65 2e70 7574 286e 2c27 3c73  n(e){e.put(n,'<s
-00168db0: 7479 6c65 3e5c 6e2f 2a20 544f 444f 202a  tyle>\n/* TODO *
-00168dc0: 2f5c 6e2e 7365 6374 696f 6e2d 7461 7267  /\n.section-targ
-00168dd0: 6574 207b 5c6e 2020 2020 746f 703a 202d  et {\n    top: -
-00168de0: 3865 6d3b 5c6e 7d5c 6e5c 6e2e 6e6f 666c  8em;\n}\n\n.nofl
-00168df0: 6578 207b 5c6e 2020 2020 666c 6578 3a20  ex {\n    flex: 
-00168e00: 3020 3020 3136 3070 7820 2169 6d70 6f72  0 0 160px !impor
-00168e10: 7461 6e74 3b5c 6e7d 5c6e 5c6e 2e68 6967  tant;\n}\n\n.hig
-00168e20: 686c 6967 6874 207b 5c6e 2020 2020 636f  hlight {\n    co
-00168e30: 6c6f 723a 2023 3234 3239 3265 3b5c 6e20  lor: #24292e;\n 
-00168e40: 2020 2062 6163 6b67 726f 756e 642d 636f     background-co
-00168e50: 6c6f 723a 2077 6869 7465 3b5c 6e7d 5c6e  lor: white;\n}\n
-00168e60: 5c6e 3c2f 7374 796c 653e 5c6e 5c6e 3c64  \n</style>\n\n<d
-00168e70: 6976 2063 6c61 7373 3d5c 2761 7070 2d73  iv class=\'app-s
-00168e80: 6372 6f6c 6c5c 273e 5c6e 2020 2020 3c64  croll\'>\n    <d
-00168e90: 6976 2063 6c61 7373 3d22 6170 702d 6c69  iv class="app-li
-00168ea0: 6e6b 7320 6170 702d 7374 6963 6b79 223e  nks app-sticky">
-00168eb0: 5c6e 2020 2020 2020 2020 3c64 6976 2063  \n        <div c
-00168ec0: 6c61 7373 3d22 6170 702d 7469 746c 6522  lass="app-title"
-00168ed0: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
-00168ee0: 6469 7620 636c 6173 733d 2261 7070 2d66  div class="app-f
-00168ef0: 7261 6d65 2061 7070 2d70 6164 2061 7070  rame app-pad app
-00168f00: 2d66 6c75 7368 2d62 6f74 746f 6d22 3e5c  -flush-bottom">\
-00168f10: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00168f20: 203c 6831 206e 672d 6966 3d22 6d6f 6465   <h1 ng-if="mode
-00168f30: 6c2e 646f 6373 2e73 686f 7720 3d3d 3d20  l.docs.show === 
-00168f40: 6661 6c73 6522 3e5c 6e20 2020 2020 2020  false">\n       
-00168f50: 2020 2020 2020 2020 2020 2020 203c 736d               <sm
-00168f60: 616c 6c20 636c 6173 733d 5c27 7465 7874  all class=\'text
-00168f70: 2d62 6f6c 6420 7465 7874 2d72 6967 6874  -bold text-right
-00168f80: 5c27 3e5c 6e20 2020 2020 2020 2020 2020  \'>\n           
-00168f90: 2020 2020 2020 2020 2020 2020 203c 6920               <i 
-00168fa0: 6461 7461 2d69 636f 6e3d 2265 7965 223e  data-icon="eye">
-00168fb0: 3c2f 693e 5c6e 2020 2020 2020 2020 2020  </i>\n          
-00168fc0: 2020 2020 2020 2020 2020 2020 2020 5468                Th
-00168fd0: 6973 207b 7b20 6d6f 6465 6c2e 7265 736f  is {{ model.reso
-00168fe0: 7572 6365 5f74 7970 6520 7d7d 2069 7320  urce_type }} is 
-00168ff0: 6869 6464 656e 5c6e 2020 2020 2020 2020  hidden\n        
-00169000: 2020 2020 2020 2020 2020 2020 3c2f 736d              </sm
-00169010: 616c 6c3e 5c6e 2020 2020 2020 2020 2020  all>\n          
-00169020: 2020 2020 2020 3c2f 6831 3e5c 6e20 2020        </h1>\n   
-00169030: 2020 2020 2020 2020 2020 2020 203c 6831               <h1
-00169040: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-00169050: 2020 2020 2020 203c 7370 616e 2063 6c61         <span cla
-00169060: 7373 3d22 6272 6561 6b22 3e7b 7b20 6d6f  ss="break">{{ mo
-00169070: 6465 6c2e 6e61 6d65 207d 7d3c 2f73 7061  del.name }}</spa
-00169080: 6e3e 5c6e 2020 2020 2020 2020 2020 2020  n>\n            
-00169090: 2020 2020 2020 2020 3c73 6d61 6c6c 3e7b          <small>{
-001690a0: 7b20 6d6f 6465 6c2e 636f 6e66 6967 2e6d  { model.config.m
-001690b0: 6174 6572 6961 6c69 7a65 6420 7d7d 3c2f  aterialized }}</
-001690c0: 736d 616c 6c3e 5c6e 2020 2020 2020 2020  small>\n        
-001690d0: 2020 2020 2020 2020 3c2f 6831 3e5c 6e20          </h1>\n 
-001690e0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-001690f0: 3e5c 6e20 2020 2020 2020 203c 2f64 6976  >\n        </div
-00169100: 3e5c 6e20 2020 2020 2020 203c 6469 7620  >\n        <div 
-00169110: 636c 6173 733d 2261 7070 2d66 7261 6d65  class="app-frame
-00169120: 2061 7070 2d70 6164 2d68 223e 5c6e 2020   app-pad-h">\n  
-00169130: 2020 2020 2020 2020 2020 3c75 6c20 636c            <ul cl
-00169140: 6173 733d 226e 6176 206e 6176 2d74 6162  ass="nav nav-tab
-00169150: 7322 3e5c 6e20 2020 2020 2020 2020 2020  s">\n           
-00169160: 2020 2020 203c 6c69 2075 692d 7372 6566       <li ui-sref
-00169170: 2d61 6374 6976 653d 5c27 6163 7469 7665  -active=\'active
-00169180: 5c27 3e3c 6120 7569 2d73 7265 663d 2264  \'><a ui-sref="d
-00169190: 6274 2e73 6e61 7073 686f 7428 7b5c 2723  bt.snapshot({\'#
-001691a0: 5c27 3a20 5c27 6465 7461 696c 735c 277d  \': \'details\'}
-001691b0: 2922 3e44 6574 6169 6c73 3c2f 613e 3c2f  )">Details</a></
-001691c0: 6c69 3e5c 6e20 2020 2020 2020 2020 2020  li>\n           
-001691d0: 2020 2020 203c 6c69 2075 692d 7372 6566       <li ui-sref
-001691e0: 2d61 6374 6976 653d 5c27 6163 7469 7665  -active=\'active
-001691f0: 5c27 3e3c 6120 7569 2d73 7265 663d 2264  \'><a ui-sref="d
-00169200: 6274 2e73 6e61 7073 686f 7428 7b5c 2723  bt.snapshot({\'#
-00169210: 5c27 3a20 5c27 6465 7363 7269 7074 696f  \': \'descriptio
-00169220: 6e5c 277d 2922 3e44 6573 6372 6970 7469  n\'})">Descripti
-00169230: 6f6e 3c2f 613e 3c2f 6c69 3e5c 6e20 2020  on</a></li>\n   
-00169240: 2020 2020 2020 2020 2020 2020 203c 6c69               <li
-00169250: 2075 692d 7372 6566 2d61 6374 6976 653d   ui-sref-active=
-00169260: 5c27 6163 7469 7665 5c27 3e3c 6120 7569  \'active\'><a ui
-00169270: 2d73 7265 663d 2264 6274 2e73 6e61 7073  -sref="dbt.snaps
-00169280: 686f 7428 7b5c 2723 5c27 3a20 5c27 636f  hot({\'#\': \'co
-00169290: 6c75 6d6e 735c 277d 2922 3e43 6f6c 756d  lumns\'})">Colum
-001692a0: 6e73 3c2f 613e 3c2f 6c69 3e5c 6e20 2020  ns</a></li>\n   
-001692b0: 2020 2020 2020 2020 2020 2020 203c 6c69               <li
-001692c0: 2075 692d 7372 6566 2d61 6374 6976 653d   ui-sref-active=
-001692d0: 5c27 6163 7469 7665 5c27 206e 672d 7368  \'active\' ng-sh
-001692e0: 6f77 203d 2022 7265 6665 7265 6e63 6573  ow = "references
-001692f0: 4c65 6e67 7468 2021 3d20 3022 3e3c 6120  Length != 0"><a 
-00169300: 7569 2d73 7265 663d 2264 6274 2e73 6e61  ui-sref="dbt.sna
-00169310: 7073 686f 7428 7b5c 2723 5c27 3a20 5c27  pshot({\'#\': \'
-00169320: 7265 6665 7265 6e63 6564 5f62 795c 277d  referenced_by\'}
-00169330: 2922 3e52 6566 6572 656e 6365 6420 4279  )">Referenced By
-00169340: 3c2f 613e 3c2f 6c69 3e5c 6e20 2020 2020  </a></li>\n     
-00169350: 2020 2020 2020 2020 2020 203c 6c69 2075             <li u
-00169360: 692d 7372 6566 2d61 6374 6976 653d 5c27  i-sref-active=\'
-00169370: 6163 7469 7665 5c27 206e 672d 7368 6f77  active\' ng-show
-00169380: 203d 2022 7061 7265 6e74 734c 656e 6774   = "parentsLengt
-00169390: 6820 213d 2030 223e 3c61 2075 692d 7372  h != 0"><a ui-sr
-001693a0: 6566 3d22 6462 742e 736e 6170 7368 6f74  ef="dbt.snapshot
-001693b0: 287b 5c27 235c 273a 205c 2764 6570 656e  ({\'#\': \'depen
-001693c0: 6473 5f6f 6e5c 277d 2922 3e44 6570 656e  ds_on\'})">Depen
-001693d0: 6473 204f 6e3c 2f61 3e3c 2f6c 693e 5c6e  ds On</a></li>\n
-001693e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001693f0: 3c6c 6920 7569 2d73 7265 662d 6163 7469  <li ui-sref-acti
-00169400: 7665 3d5c 2761 6374 6976 655c 273e 3c61  ve=\'active\'><a
-00169410: 2075 692d 7372 6566 3d22 6462 742e 736e   ui-sref="dbt.sn
-00169420: 6170 7368 6f74 287b 5c27 235c 273a 205c  apshot({\'#\': \
-00169430: 2763 6f64 655c 277d 2922 3e53 514c 3c2f  'code\'})">SQL</
-00169440: 613e 3c2f 6c69 3e5c 6e20 2020 2020 2020  a></li>\n       
-00169450: 2020 2020 203c 2f75 6c3e 5c6e 2020 2020       </ul>\n    
-00169460: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
-00169470: 3c2f 6469 763e 5c6e 2020 2020 3c64 6976  </div>\n    <div
-00169480: 2063 6c61 7373 3d22 6170 702d 6465 7461   class="app-deta
-00169490: 696c 7322 3e5c 6e20 2020 2020 2020 203c  ils">\n        <
-001694a0: 6469 7620 636c 6173 733d 2261 7070 2d66  div class="app-f
-001694b0: 7261 6d65 2061 7070 2d70 6164 223e 5c6e  rame app-pad">\n
-001694c0: 2020 2020 2020 2020 2020 2020 3c73 6563              <sec
-001694d0: 7469 6f6e 2063 6c61 7373 3d22 7365 6374  tion class="sect
-001694e0: 696f 6e22 3e5c 6e20 2020 2020 2020 2020  ion">\n         
-001694f0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-00169500: 733d 2273 6563 7469 6f6e 2d74 6172 6765  s="section-targe
-00169510: 7422 2069 643d 2264 6574 6169 6c73 223e  t" id="details">
-00169520: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-00169530: 2020 2020 2020 2020 3c74 6162 6c65 2d64          <table-d
-00169540: 6574 6169 6c73 206d 6f64 656c 3d22 6d6f  etails model="mo
-00169550: 6465 6c22 202f 3e5c 6e20 2020 2020 2020  del" />\n       
-00169560: 2020 2020 203c 2f73 6563 7469 6f6e 3e5c       </section>\
-00169570: 6e5c 6e20 2020 2020 2020 2020 2020 203c  n\n            <
-00169580: 7365 6374 696f 6e20 636c 6173 733d 2273  section class="s
-00169590: 6563 7469 6f6e 223e 5c6e 2020 2020 2020  ection">\n      
-001695a0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-001695b0: 6c61 7373 3d22 7365 6374 696f 6e2d 7461  lass="section-ta
-001695c0: 7267 6574 2220 6964 3d22 6465 7363 7269  rget" id="descri
-001695d0: 7074 696f 6e22 3e3c 2f64 6976 3e5c 6e20  ption"></div>\n 
-001695e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-001695f0: 6469 7620 636c 6173 733d 2273 6563 7469  div class="secti
-00169600: 6f6e 2d63 6f6e 7465 6e74 223e 5c6e 2020  on-content">\n  
-00169610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00169620: 2020 3c68 363e 4465 7363 7269 7074 696f    <h6>Descriptio
-00169630: 6e3c 2f68 363e 5c6e 2020 2020 2020 2020  n</h6>\n        
-00169640: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00169650: 2063 6c61 7373 3d22 7061 6e65 6c22 3e5c   class="panel">\
-00169660: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00169670: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00169680: 6173 733d 2270 616e 656c 2d62 6f64 7922  ass="panel-body"
-00169690: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-001696a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-001696b0: 6469 7620 6e67 2d69 663d 226d 6f64 656c  div ng-if="model
-001696c0: 2e64 6573 6372 6970 7469 6f6e 2220 636c  .description" cl
-001696d0: 6173 733d 226d 6f64 656c 2d6d 6172 6b64  ass="model-markd
-001696e0: 6f77 6e22 206d 6172 6b65 643d 226d 6f64  own" marked="mod
-001696f0: 656c 2e64 6573 6372 6970 7469 6f6e 223e  el.description">
-00169700: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-00169710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00169720: 2020 2020 3c64 6976 206e 672d 6966 3d22      <div ng-if="
-00169730: 216d 6f64 656c 2e64 6573 6372 6970 7469  !model.descripti
-00169740: 6f6e 223e 5468 6973 207b 7b20 6d6f 6465  on">This {{ mode
-00169750: 6c2e 7265 736f 7572 6365 5f74 7970 6520  l.resource_type 
-00169760: 7d7d 2069 7320 6e6f 7420 6375 7272 656e  }} is not curren
-00169770: 746c 7920 646f 6375 6d65 6e74 6564 3c2f  tly documented</
-00169780: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
-00169790: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-001697a0: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
-001697b0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-001697c0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-001697d0: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
-001697e0: 2020 2020 2020 3c2f 7365 6374 696f 6e3e        </section>
-001697f0: 5c6e 5c6e 2020 2020 2020 2020 2020 2020  \n\n            
-00169800: 3c73 6563 7469 6f6e 2063 6c61 7373 3d22  <section class="
-00169810: 7365 6374 696f 6e22 3e5c 6e20 2020 2020  section">\n     
-00169820: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00169830: 636c 6173 733d 2273 6563 7469 6f6e 2d74  class="section-t
-00169840: 6172 6765 7422 2069 643d 2263 6f6c 756d  arget" id="colum
-00169850: 6e73 223e 3c2f 6469 763e 5c6e 2020 2020  ns"></div>\n    
-00169860: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00169870: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
-00169880: 636f 6e74 656e 7422 3e5c 6e20 2020 2020  content">\n     
-00169890: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-001698a0: 6836 3e43 6f6c 756d 6e73 3c2f 6836 3e5c  h6>Columns</h6>\
-001698b0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-001698c0: 2020 2020 203c 636f 6c75 6d6e 2d64 6574       <column-det
-001698d0: 6169 6c73 206d 6f64 656c 3d22 6d6f 6465  ails model="mode
-001698e0: 6c22 202f 3e5c 6e20 2020 2020 2020 2020  l" />\n         
-001698f0: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
-00169900: 2020 2020 2020 2020 2020 203c 2f73 6563             </sec
-00169910: 7469 6f6e 3e5c 6e5c 6e20 2020 2020 2020  tion>\n\n       
-00169920: 2020 2020 203c 7365 6374 696f 6e20 636c       <section cl
-00169930: 6173 733d 2273 6563 7469 6f6e 2220 6e67  ass="section" ng
-00169940: 2d73 686f 7720 3d20 2272 6566 6572 656e  -show = "referen
-00169950: 6365 734c 656e 6774 6820 213d 2030 223e  cesLength != 0">
-00169960: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00169970: 2020 3c64 6976 2063 6c61 7373 3d22 7365    <div class="se
-00169980: 6374 696f 6e2d 7461 7267 6574 2220 6964  ction-target" id
-00169990: 3d22 7265 6665 7265 6e63 6564 5f62 7922  ="referenced_by"
-001699a0: 3e3c 2f64 6976 3e5c 6e20 2020 2020 2020  ></div>\n       
-001699b0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-001699c0: 6173 733d 2273 6563 7469 6f6e 2d63 6f6e  ass="section-con
-001699d0: 7465 6e74 223e 5c6e 2020 2020 2020 2020  tent">\n        
-001699e0: 2020 2020 2020 2020 2020 2020 3c68 363e              <h6>
-001699f0: 5265 6665 7265 6e63 6564 2042 793c 2f68  Referenced By</h
-00169a00: 363e 5c6e 2020 2020 2020 2020 2020 2020  6>\n            
-00169a10: 2020 2020 2020 2020 3c72 6566 6572 656e          <referen
-00169a20: 6365 2d6c 6973 7420 7265 6665 7265 6e63  ce-list referenc
-00169a30: 6573 3d22 7265 6665 7265 6e63 6573 2220  es="references" 
-00169a40: 6e6f 6465 3d22 6d6f 6465 6c22 202f 3e5c  node="model" />\
-00169a50: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00169a60: 203c 2f64 6976 3e5c 6e20 2020 2020 2020   </div>\n       
-00169a70: 2020 2020 203c 2f73 6563 7469 6f6e 3e5c       </section>\
-00169a80: 6e5c 6e20 2020 2020 2020 2020 2020 203c  n\n            <
-00169a90: 7365 6374 696f 6e20 636c 6173 733d 2273  section class="s
-00169aa0: 6563 7469 6f6e 2220 6e67 2d73 686f 7720  ection" ng-show 
-00169ab0: 3d20 2270 6172 656e 7473 4c65 6e67 7468  = "parentsLength
-00169ac0: 2021 3d20 3022 3e5c 6e20 2020 2020 2020   != 0">\n       
-00169ad0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00169ae0: 6173 733d 2273 6563 7469 6f6e 2d74 6172  ass="section-tar
-00169af0: 6765 7422 2069 643d 2264 6570 656e 6473  get" id="depends
-00169b00: 5f6f 6e22 3e3c 2f64 6976 3e5c 6e20 2020  _on"></div>\n   
-00169b10: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00169b20: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
-00169b30: 2d63 6f6e 7465 6e74 223e 5c6e 2020 2020  -content">\n    
-00169b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00169b50: 3c68 363e 4465 7065 6e64 7320 4f6e 3c2f  <h6>Depends On</
-00169b60: 6836 3e5c 6e20 2020 2020 2020 2020 2020  h6>\n           
-00169b70: 2020 2020 2020 2020 203c 7265 6665 7265           <refere
-00169b80: 6e63 652d 6c69 7374 2072 6566 6572 656e  nce-list referen
-00169b90: 6365 733d 2270 6172 656e 7473 2220 6e6f  ces="parents" no
-00169ba0: 6465 3d22 6d6f 6465 6c22 202f 3e5c 6e20  de="model" />\n 
-00169bb0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00169bc0: 2f64 6976 3e5c 6e20 2020 2020 2020 2020  /div>\n         
-00169bd0: 2020 203c 2f73 6563 7469 6f6e 3e5c 6e5c     </section>\n\
-00169be0: 6e20 2020 2020 2020 2020 2020 203c 7365  n            <se
-00169bf0: 6374 696f 6e20 636c 6173 733d 2273 6563  ction class="sec
-00169c00: 7469 6f6e 223e 5c6e 2020 2020 2020 2020  tion">\n        
-00169c10: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00169c20: 7373 3d22 7365 6374 696f 6e2d 7461 7267  ss="section-targ
-00169c30: 6574 2220 6964 3d22 636f 6465 223e 3c2f  et" id="code"></
-00169c40: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
-00169c50: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00169c60: 3d22 7365 6374 696f 6e2d 636f 6e74 656e  ="section-conten
-00169c70: 7422 3e5c 6e20 2020 2020 2020 2020 2020  t">\n           
-00169c80: 2020 2020 2020 2020 203c 636f 6465 2d62           <code-b
-00169c90: 6c6f 636b 2076 6572 7369 6f6e 733d 2276  lock versions="v
-00169ca0: 6572 7369 6f6e 7322 2064 6566 6175 6c74  ersions" default
-00169cb0: 3d22 6465 6661 756c 745f 7665 7273 696f  ="default_versio
-00169cc0: 6e22 206c 616e 6775 6167 653d 226c 616e  n" language="lan
-00169cd0: 6775 6167 6522 3e3c 2f63 6f64 652d 626c  guage"></code-bl
-00169ce0: 6f63 6b3e 5c6e 2020 2020 2020 2020 2020  ock>\n          
-00169cf0: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
-00169d00: 2020 2020 2020 2020 2020 3c2f 7365 6374            </sect
-00169d10: 696f 6e3e 5c6e 2020 2020 2020 2020 3c2f  ion>\n        </
-00169d20: 6469 763e 5c6e 2020 2020 3c2f 6469 763e  div>\n    </div>
-00169d30: 5c6e 3c2f 6469 763e 5c6e 2729 7d5d 292c  \n</div>\n')}]),
-00169d40: 652e 6578 706f 7274 733d 6e7d 2c66 756e  e.exports=n},fun
-00169d50: 6374 696f 6e28 652c 7429 7b76 6172 206e  ction(e,t){var n
-00169d60: 3d22 2f64 6f63 732f 7365 6564 2e68 746d  ="/docs/seed.htm
-00169d70: 6c22 3b77 696e 646f 772e 616e 6775 6c61  l";window.angula
-00169d80: 722e 6d6f 6475 6c65 2822 6e67 2229 2e72  r.module("ng").r
-00169d90: 756e 285b 2224 7465 6d70 6c61 7465 4361  un(["$templateCa
-00169da0: 6368 6522 2c66 756e 6374 696f 6e28 6529  che",function(e)
-00169db0: 7b65 2e70 7574 286e 2c27 3c73 7479 6c65  {e.put(n,'<style
-00169dc0: 3e5c 6e2f 2a20 544f 444f 202a 2f5c 6e2e  >\n/* TODO */\n.
-00169dd0: 7365 6374 696f 6e2d 7461 7267 6574 207b  section-target {
-00169de0: 5c6e 2020 2020 746f 703a 202d 3865 6d3b  \n    top: -8em;
-00169df0: 5c6e 7d5c 6e5c 6e2e 6e6f 666c 6578 207b  \n}\n\n.noflex {
-00169e00: 5c6e 2020 2020 666c 6578 3a20 3020 3020  \n    flex: 0 0 
-00169e10: 3136 3070 7820 2169 6d70 6f72 7461 6e74  160px !important
-00169e20: 3b5c 6e7d 5c6e 5c6e 2e68 6967 686c 6967  ;\n}\n\n.highlig
-00169e30: 6874 207b 5c6e 2020 2020 636f 6c6f 723a  ht {\n    color:
-00169e40: 2023 3234 3239 3265 3b5c 6e20 2020 2062   #24292e;\n    b
-00169e50: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
-00169e60: 2077 6869 7465 3b5c 6e7d 5c6e 5c6e 3c2f   white;\n}\n\n</
-00169e70: 7374 796c 653e 5c6e 5c6e 3c64 6976 2063  style>\n\n<div c
-00169e80: 6c61 7373 3d5c 2761 7070 2d73 6372 6f6c  lass=\'app-scrol
-00169e90: 6c5c 273e 5c6e 2020 2020 3c64 6976 2063  l\'>\n    <div c
-00169ea0: 6c61 7373 3d22 6170 702d 6c69 6e6b 7320  lass="app-links 
-00169eb0: 6170 702d 7374 6963 6b79 223e 5c6e 2020  app-sticky">\n  
-00169ec0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00169ed0: 3d22 6170 702d 7469 746c 6522 3e5c 6e20  ="app-title">\n 
-00169ee0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00169ef0: 636c 6173 733d 2261 7070 2d66 7261 6d65  class="app-frame
-00169f00: 2061 7070 2d70 6164 2061 7070 2d66 6c75   app-pad app-flu
-00169f10: 7368 2d62 6f74 746f 6d22 3e5c 6e20 2020  sh-bottom">\n   
-00169f20: 2020 2020 2020 2020 2020 2020 203c 6831               <h1
-00169f30: 206e 672d 6966 3d22 6d6f 6465 6c2e 646f   ng-if="model.do
-00169f40: 6373 2e73 686f 7720 3d3d 3d20 6661 6c73  cs.show === fals
-00169f50: 6522 3e5c 6e20 2020 2020 2020 2020 2020  e">\n           
-00169f60: 2020 2020 2020 2020 203c 736d 616c 6c20           <small 
-00169f70: 636c 6173 733d 5c27 7465 7874 2d62 6f6c  class=\'text-bol
-00169f80: 6420 7465 7874 2d72 6967 6874 5c27 3e5c  d text-right\'>\
-00169f90: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00169fa0: 2020 2020 2020 2020 203c 6920 6461 7461           <i data
-00169fb0: 2d69 636f 6e3d 2265 7965 223e 3c2f 693e  -icon="eye"></i>
-00169fc0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00169fd0: 2020 2020 2020 2020 2020 5468 6973 207b            This {
-00169fe0: 7b20 6d6f 6465 6c2e 7265 736f 7572 6365  { model.resource
-00169ff0: 5f74 7970 6520 7d7d 2069 7320 6869 6464  _type }} is hidd
-0016a000: 656e 5c6e 2020 2020 2020 2020 2020 2020  en\n            
-0016a010: 2020 2020 2020 2020 3c2f 736d 616c 6c3e          </small>
-0016a020: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0016a030: 2020 3c2f 6831 3e5c 6e20 2020 2020 2020    </h1>\n       
-0016a040: 2020 2020 2020 2020 203c 6831 3e5c 6e20           <h1>\n 
-0016a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016a060: 2020 203c 7370 616e 2063 6c61 7373 3d22     <span class="
-0016a070: 6272 6561 6b22 3e7b 7b20 6d6f 6465 6c2e  break">{{ model.
-0016a080: 6e61 6d65 207d 7d3c 2f73 7061 6e3e 5c6e  name }}</span>\n
-0016a090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016a0a0: 2020 2020 3c73 6d61 6c6c 3e7b 7b20 6d6f      <small>{{ mo
-0016a0b0: 6465 6c2e 636f 6e66 6967 2e6d 6174 6572  del.config.mater
-0016a0c0: 6961 6c69 7a65 6420 7d7d 3c2f 736d 616c  ialized }}</smal
-0016a0d0: 6c3e 5c6e 2020 2020 2020 2020 2020 2020  l>\n            
-0016a0e0: 2020 2020 3c2f 6831 3e5c 6e20 2020 2020      </h1>\n     
-0016a0f0: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
-0016a100: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
-0016a110: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0016a120: 733d 2261 7070 2d66 7261 6d65 2061 7070  s="app-frame app
-0016a130: 2d70 6164 2d68 223e 5c6e 2020 2020 2020  -pad-h">\n      
-0016a140: 2020 2020 2020 3c75 6c20 636c 6173 733d        <ul class=
-0016a150: 226e 6176 206e 6176 2d74 6162 7322 3e5c  "nav nav-tabs">\
-0016a160: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016a170: 203c 6c69 2075 692d 7372 6566 2d61 6374   <li ui-sref-act
-0016a180: 6976 653d 5c27 6163 7469 7665 5c27 3e3c  ive=\'active\'><
-0016a190: 6120 7569 2d73 7265 663d 2264 6274 2e73  a ui-sref="dbt.s
-0016a1a0: 6565 6428 7b5c 2723 5c27 3a20 5c27 6465  eed({\'#\': \'de
-0016a1b0: 7461 696c 735c 277d 2922 3e44 6574 6169  tails\'})">Detai
-0016a1c0: 6c73 3c2f 613e 3c2f 6c69 3e5c 6e20 2020  ls</a></li>\n   
-0016a1d0: 2020 2020 2020 2020 2020 2020 203c 6c69               <li
-0016a1e0: 2075 692d 7372 6566 2d61 6374 6976 653d   ui-sref-active=
-0016a1f0: 5c27 6163 7469 7665 5c27 3e3c 6120 7569  \'active\'><a ui
-0016a200: 2d73 7265 663d 2264 6274 2e73 6565 6428  -sref="dbt.seed(
-0016a210: 7b5c 2723 5c27 3a20 5c27 6465 7363 7269  {\'#\': \'descri
-0016a220: 7074 696f 6e5c 277d 2922 3e44 6573 6372  ption\'})">Descr
-0016a230: 6970 7469 6f6e 3c2f 613e 3c2f 6c69 3e5c  iption</a></li>\
-0016a240: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016a250: 203c 6c69 2075 692d 7372 6566 2d61 6374   <li ui-sref-act
-0016a260: 6976 653d 5c27 6163 7469 7665 5c27 3e3c  ive=\'active\'><
-0016a270: 6120 7569 2d73 7265 663d 2264 6274 2e73  a ui-sref="dbt.s
-0016a280: 6565 6428 7b5c 2723 5c27 3a20 5c27 636f  eed({\'#\': \'co
-0016a290: 6c75 6d6e 735c 277d 2922 3e43 6f6c 756d  lumns\'})">Colum
-0016a2a0: 6e73 3c2f 613e 3c2f 6c69 3e5c 6e20 2020  ns</a></li>\n   
-0016a2b0: 2020 2020 2020 2020 2020 2020 203c 6c69               <li
-0016a2c0: 2075 692d 7372 6566 2d61 6374 6976 653d   ui-sref-active=
-0016a2d0: 5c27 6163 7469 7665 5c27 206e 672d 7368  \'active\' ng-sh
-0016a2e0: 6f77 203d 2022 7265 6665 7265 6e63 6573  ow = "references
-0016a2f0: 4c65 6e67 7468 2021 3d20 3022 3e3c 6120  Length != 0"><a 
-0016a300: 7569 2d73 7265 663d 2264 6274 2e73 6565  ui-sref="dbt.see
-0016a310: 6428 7b5c 2723 5c27 3a20 5c27 7265 6665  d({\'#\': \'refe
-0016a320: 7265 6e63 6564 5f62 795c 277d 2922 3e52  renced_by\'})">R
-0016a330: 6566 6572 656e 6365 6420 4279 3c2f 613e  eferenced By</a>
-0016a340: 3c2f 6c69 3e5c 6e20 2020 2020 2020 2020  </li>\n         
-0016a350: 2020 2020 2020 203c 6c69 2075 692d 7372         <li ui-sr
-0016a360: 6566 2d61 6374 6976 653d 5c27 6163 7469  ef-active=\'acti
-0016a370: 7665 5c27 206e 672d 7368 6f77 203d 2022  ve\' ng-show = "
-0016a380: 7061 7265 6e74 734c 656e 6774 6820 213d  parentsLength !=
-0016a390: 2030 223e 3c61 2075 692d 7372 6566 3d22   0"><a ui-sref="
-0016a3a0: 6462 742e 7365 6564 287b 5c27 235c 273a  dbt.seed({\'#\':
-0016a3b0: 205c 2764 6570 656e 6473 5f6f 6e5c 277d   \'depends_on\'}
-0016a3c0: 2922 3e44 6570 656e 6473 204f 6e3c 2f61  )">Depends On</a
-0016a3d0: 3e3c 2f6c 693e 5c6e 2020 2020 2020 2020  ></li>\n        
-0016a3e0: 2020 2020 2020 2020 3c6c 6920 7569 2d73          <li ui-s
-0016a3f0: 7265 662d 6163 7469 7665 3d5c 2761 6374  ref-active=\'act
-0016a400: 6976 655c 273e 3c61 2075 692d 7372 6566  ive\'><a ui-sref
-0016a410: 3d22 6462 742e 7365 6564 287b 5c27 235c  ="dbt.seed({\'#\
-0016a420: 273a 205c 2763 6f64 655c 277d 2922 3e53  ': \'code\'})">S
-0016a430: 514c 3c2f 613e 3c2f 6c69 3e5c 6e20 2020  QL</a></li>\n   
-0016a440: 2020 2020 2020 2020 203c 2f75 6c3e 5c6e           </ul>\n
-0016a450: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
-0016a460: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
-0016a470: 3c64 6976 2063 6c61 7373 3d22 6170 702d  <div class="app-
-0016a480: 6465 7461 696c 7322 3e5c 6e20 2020 2020  details">\n     
-0016a490: 2020 203c 6469 7620 636c 6173 733d 2261     <div class="a
-0016a4a0: 7070 2d66 7261 6d65 2061 7070 2d70 6164  pp-frame app-pad
-0016a4b0: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
-0016a4c0: 3c73 6563 7469 6f6e 2063 6c61 7373 3d22  <section class="
-0016a4d0: 7365 6374 696f 6e22 3e5c 6e20 2020 2020  section">\n     
-0016a4e0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0016a4f0: 636c 6173 733d 2273 6563 7469 6f6e 2d74  class="section-t
-0016a500: 6172 6765 7422 2069 643d 2264 6574 6169  arget" id="detai
-0016a510: 6c73 223e 3c2f 6469 763e 5c6e 2020 2020  ls"></div>\n    
-0016a520: 2020 2020 2020 2020 2020 2020 3c74 6162              <tab
-0016a530: 6c65 2d64 6574 6169 6c73 206d 6f64 656c  le-details model
-0016a540: 3d22 6d6f 6465 6c22 202f 3e5c 6e20 2020  ="model" />\n   
-0016a550: 2020 2020 2020 2020 203c 2f73 6563 7469           </secti
-0016a560: 6f6e 3e5c 6e5c 6e20 2020 2020 2020 2020  on>\n\n         
-0016a570: 2020 203c 7365 6374 696f 6e20 636c 6173     <section clas
-0016a580: 733d 2273 6563 7469 6f6e 223e 5c6e 2020  s="section">\n  
-0016a590: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0016a5a0: 6976 2063 6c61 7373 3d22 7365 6374 696f  iv class="sectio
-0016a5b0: 6e2d 7461 7267 6574 2220 6964 3d22 6465  n-target" id="de
-0016a5c0: 7363 7269 7074 696f 6e22 3e3c 2f64 6976  scription"></div
-0016a5d0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016a5e0: 2020 203c 6469 7620 636c 6173 733d 2273     <div class="s
-0016a5f0: 6563 7469 6f6e 2d63 6f6e 7465 6e74 223e  ection-content">
-0016a600: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0016a610: 2020 2020 2020 3c68 363e 4465 7363 7269        <h6>Descri
-0016a620: 7074 696f 6e3c 2f68 363e 5c6e 2020 2020  ption</h6>\n    
-0016a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016a640: 3c64 6976 2063 6c61 7373 3d22 7061 6e65  <div class="pane
-0016a650: 6c22 3e5c 6e20 2020 2020 2020 2020 2020  l">\n           
-0016a660: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0016a670: 7620 636c 6173 733d 2270 616e 656c 2d62  v class="panel-b
-0016a680: 6f64 7922 3e5c 6e20 2020 2020 2020 2020  ody">\n         
-0016a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016a6a0: 2020 203c 6469 7620 6e67 2d69 663d 226d     <div ng-if="m
-0016a6b0: 6f64 656c 2e64 6573 6372 6970 7469 6f6e  odel.description
-0016a6c0: 2220 636c 6173 733d 226d 6f64 656c 2d6d  " class="model-m
-0016a6d0: 6172 6b64 6f77 6e22 206d 6172 6b65 643d  arkdown" marked=
-0016a6e0: 226d 6f64 656c 2e64 6573 6372 6970 7469  "model.descripti
-0016a6f0: 6f6e 223e 3c2f 6469 763e 5c6e 2020 2020  on"></div>\n    
-0016a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016a710: 2020 2020 2020 2020 3c64 6976 206e 672d          <div ng-
-0016a720: 6966 3d22 216d 6f64 656c 2e64 6573 6372  if="!model.descr
-0016a730: 6970 7469 6f6e 223e 5468 6973 207b 7b20  iption">This {{ 
-0016a740: 6d6f 6465 6c2e 7265 736f 7572 6365 5f74  model.resource_t
-0016a750: 7970 6520 7d7d 2069 7320 6e6f 7420 6375  ype }} is not cu
-0016a760: 7272 656e 746c 7920 646f 6375 6d65 6e74  rrently document
-0016a770: 6564 3c2f 6469 763e 5c6e 2020 2020 2020  ed</div>\n      
-0016a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016a790: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
-0016a7a0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-0016a7b0: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
-0016a7c0: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
-0016a7d0: 2020 2020 2020 2020 2020 3c2f 7365 6374            </sect
-0016a7e0: 696f 6e3e 5c6e 2020 2020 2020 2020 2020  ion>\n          
-0016a7f0: 2020 3c73 6563 7469 6f6e 2063 6c61 7373    <section class
-0016a800: 3d22 7365 6374 696f 6e22 3e5c 6e20 2020  ="section">\n   
-0016a810: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0016a820: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
-0016a830: 2d74 6172 6765 7422 2069 643d 2263 6f6c  -target" id="col
-0016a840: 756d 6e73 223e 3c2f 6469 763e 5c6e 2020  umns"></div>\n  
-0016a850: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0016a860: 6976 2063 6c61 7373 3d22 7365 6374 696f  iv class="sectio
-0016a870: 6e2d 636f 6e74 656e 7422 3e5c 6e20 2020  n-content">\n   
-0016a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016a890: 203c 6836 3e43 6f6c 756d 6e73 3c2f 6836   <h6>Columns</h6
-0016a8a0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016a8b0: 2020 2020 2020 203c 636f 6c75 6d6e 2d64         <column-d
-0016a8c0: 6574 6169 6c73 206d 6f64 656c 3d22 6d6f  etails model="mo
-0016a8d0: 6465 6c22 202f 3e5c 6e20 2020 2020 2020  del" />\n       
-0016a8e0: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-0016a8f0: 6e20 2020 2020 2020 2020 2020 203c 2f73  n            </s
-0016a900: 6563 7469 6f6e 3e5c 6e5c 6e20 2020 2020  ection>\n\n     
-0016a910: 2020 2020 2020 203c 7365 6374 696f 6e20         <section 
-0016a920: 636c 6173 733d 2273 6563 7469 6f6e 2220  class="section" 
-0016a930: 6e67 2d73 686f 7720 3d20 2272 6566 6572  ng-show = "refer
-0016a940: 656e 6365 734c 656e 6774 6820 213d 2030  encesLength != 0
-0016a950: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
-0016a960: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0016a970: 7365 6374 696f 6e2d 7461 7267 6574 2220  section-target" 
-0016a980: 6964 3d22 7265 6665 7265 6e63 6564 5f62  id="referenced_b
-0016a990: 7922 3e3c 2f64 6976 3e5c 6e20 2020 2020  y"></div>\n     
-0016a9a0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0016a9b0: 636c 6173 733d 2273 6563 7469 6f6e 2d63  class="section-c
-0016a9c0: 6f6e 7465 6e74 223e 5c6e 2020 2020 2020  ontent">\n      
-0016a9d0: 2020 2020 2020 2020 2020 2020 2020 3c68                <h
-0016a9e0: 363e 5265 6665 7265 6e63 6564 2042 793c  6>Referenced By<
-0016a9f0: 2f68 363e 5c6e 2020 2020 2020 2020 2020  /h6>\n          
-0016aa00: 2020 2020 2020 2020 2020 3c72 6566 6572            <refer
-0016aa10: 656e 6365 2d6c 6973 7420 7265 6665 7265  ence-list refere
-0016aa20: 6e63 6573 3d22 7265 6665 7265 6e63 6573  nces="references
-0016aa30: 2220 6e6f 6465 3d22 6d6f 6465 6c22 202f  " node="model" /
-0016aa40: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016aa50: 2020 203c 2f64 6976 3e5c 6e20 2020 2020     </div>\n     
-0016aa60: 2020 2020 2020 203c 2f73 6563 7469 6f6e         </section
-0016aa70: 3e5c 6e5c 6e20 2020 2020 2020 2020 2020  >\n\n           
-0016aa80: 203c 7365 6374 696f 6e20 636c 6173 733d   <section class=
-0016aa90: 2273 6563 7469 6f6e 2220 6e67 2d73 686f  "section" ng-sho
-0016aaa0: 7720 3d20 2270 6172 656e 7473 4c65 6e67  w = "parentsLeng
-0016aab0: 7468 2021 3d20 3022 3e5c 6e20 2020 2020  th != 0">\n     
-0016aac0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0016aad0: 636c 6173 733d 2273 6563 7469 6f6e 2d74  class="section-t
-0016aae0: 6172 6765 7422 2069 643d 2264 6570 656e  arget" id="depen
-0016aaf0: 6473 5f6f 6e22 3e3c 2f64 6976 3e5c 6e20  ds_on"></div>\n 
-0016ab00: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016ab10: 6469 7620 636c 6173 733d 2273 6563 7469  div class="secti
-0016ab20: 6f6e 2d63 6f6e 7465 6e74 223e 5c6e 2020  on-content">\n  
-0016ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016ab40: 2020 3c68 363e 4465 7065 6e64 7320 4f6e    <h6>Depends On
-0016ab50: 3c2f 6836 3e5c 6e20 2020 2020 2020 2020  </h6>\n         
-0016ab60: 2020 2020 2020 2020 2020 203c 7265 6665             <refe
-0016ab70: 7265 6e63 652d 6c69 7374 2072 6566 6572  rence-list refer
-0016ab80: 656e 6365 733d 2270 6172 656e 7473 2220  ences="parents" 
-0016ab90: 6e6f 6465 3d22 6d6f 6465 6c22 202f 3e5c  node="model" />\
-0016aba0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016abb0: 203c 2f64 6976 3e5c 6e20 2020 2020 2020   </div>\n       
-0016abc0: 2020 2020 203c 2f73 6563 7469 6f6e 3e5c       </section>\
-0016abd0: 6e5c 6e20 2020 2020 2020 2020 2020 203c  n\n            <
-0016abe0: 7365 6374 696f 6e20 636c 6173 733d 2273  section class="s
-0016abf0: 6563 7469 6f6e 223e 5c6e 2020 2020 2020  ection">\n      
-0016ac00: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0016ac10: 6c61 7373 3d22 7365 6374 696f 6e2d 7461  lass="section-ta
-0016ac20: 7267 6574 2220 6964 3d22 636f 6465 223e  rget" id="code">
-0016ac30: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-0016ac40: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0016ac50: 7373 3d22 7365 6374 696f 6e2d 636f 6e74  ss="section-cont
-0016ac60: 656e 7422 3e5c 6e20 2020 2020 2020 2020  ent">\n         
-0016ac70: 2020 2020 2020 2020 2020 203c 636f 6465             <code
-0016ac80: 2d62 6c6f 636b 2076 6572 7369 6f6e 733d  -block versions=
-0016ac90: 2276 6572 7369 6f6e 7322 2064 6566 6175  "versions" defau
-0016aca0: 6c74 3d22 6465 6661 756c 745f 7665 7273  lt="default_vers
-0016acb0: 696f 6e22 206c 616e 6775 6167 653d 226c  ion" language="l
-0016acc0: 616e 6775 6167 6522 3e3c 2f63 6f64 652d  anguage"></code-
-0016acd0: 626c 6f63 6b3e 5c6e 2020 2020 2020 2020  block>\n        
-0016ace0: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
-0016acf0: 2020 2020 2020 2020 2020 2020 3c2f 7365              </se
-0016ad00: 6374 696f 6e3e 5c6e 2020 2020 2020 2020  ction>\n        
-0016ad10: 3c2f 6469 763e 5c6e 2020 2020 3c2f 6469  </div>\n    </di
-0016ad20: 763e 5c6e 3c2f 6469 763e 5c6e 2729 7d5d  v>\n</div>\n')}]
-0016ad30: 292c 652e 6578 706f 7274 733d 6e7d 2c66  ),e.exports=n},f
-0016ad40: 756e 6374 696f 6e28 652c 7429 7b76 6172  unction(e,t){var
-0016ad50: 206e 3d22 2f64 6f63 732f 756e 6974 5f74   n="/docs/unit_t
-0016ad60: 6573 742e 6874 6d6c 223b 7769 6e64 6f77  est.html";window
-0016ad70: 2e61 6e67 756c 6172 2e6d 6f64 756c 6528  .angular.module(
-0016ad80: 226e 6722 292e 7275 6e28 5b22 2474 656d  "ng").run(["$tem
-0016ad90: 706c 6174 6543 6163 6865 222c 6675 6e63  plateCache",func
-0016ada0: 7469 6f6e 2865 297b 652e 7075 7428 6e2c  tion(e){e.put(n,
-0016adb0: 273c 7374 796c 653e 5c6e 2f2a 2054 4f44  '<style>\n/* TOD
-0016adc0: 4f20 2a2f 5c6e 2e73 6563 7469 6f6e 2d74  O */\n.section-t
-0016add0: 6172 6765 7420 7b5c 6e20 2020 2074 6f70  arget {\n    top
-0016ade0: 3a20 2d38 656d 3b5c 6e7d 5c6e 5c6e 2e6e  : -8em;\n}\n\n.n
-0016adf0: 6f66 6c65 7820 7b5c 6e20 2020 2066 6c65  oflex {\n    fle
-0016ae00: 783a 2030 2030 2031 3630 7078 2021 696d  x: 0 0 160px !im
-0016ae10: 706f 7274 616e 743b 5c6e 7d5c 6e5c 6e2e  portant;\n}\n\n.
-0016ae20: 6869 6768 6c69 6768 7420 7b5c 6e20 2020  highlight {\n   
-0016ae30: 2063 6f6c 6f72 3a20 2332 3432 3932 653b   color: #24292e;
-0016ae40: 5c6e 2020 2020 6261 636b 6772 6f75 6e64  \n    background
-0016ae50: 2d63 6f6c 6f72 3a20 7768 6974 653b 5c6e  -color: white;\n
-0016ae60: 7d5c 6e5c 6e3c 2f73 7479 6c65 3e5c 6e5c  }\n\n</style>\n\
-0016ae70: 6e3c 6469 7620 636c 6173 733d 5c27 6170  n<div class=\'ap
-0016ae80: 702d 7363 726f 6c6c 5c27 3e5c 6e20 2020  p-scroll\'>\n   
-0016ae90: 203c 6469 7620 636c 6173 733d 2261 7070   <div class="app
-0016aea0: 2d6c 696e 6b73 2061 7070 2d73 7469 636b  -links app-stick
-0016aeb0: 7922 3e5c 6e20 2020 2020 2020 203c 6469  y">\n        <di
-0016aec0: 7620 636c 6173 733d 2261 7070 2d74 6974  v class="app-tit
-0016aed0: 6c65 223e 5c6e 2020 2020 2020 2020 2020  le">\n          
-0016aee0: 2020 3c64 6976 2063 6c61 7373 3d22 6170    <div class="ap
-0016aef0: 702d 6672 616d 6520 6170 702d 7061 6420  p-frame app-pad 
-0016af00: 6170 702d 666c 7573 682d 626f 7474 6f6d  app-flush-bottom
-0016af10: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
-0016af20: 2020 2020 3c68 313e 5c6e 2020 2020 2020      <h1>\n      
-0016af30: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-0016af40: 7061 6e20 636c 6173 733d 2262 7265 616b  pan class="break
-0016af50: 223e 7b7b 206d 6f64 656c 2e6e 616d 6520  ">{{ model.name 
-0016af60: 7d7d 3c2f 7370 616e 3e5c 6e20 2020 2020  }}</span>\n     
-0016af70: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016af80: 736d 616c 6c3e 756e 6974 2074 6573 743c  small>unit test<
-0016af90: 2f73 6d61 6c6c 3e5c 6e20 2020 2020 2020  /small>\n       
-0016afa0: 2020 2020 2020 2020 203c 2f68 313e 5c6e           </h1>\n
-0016afb0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-0016afc0: 763e 5c6e 2020 2020 2020 2020 3c2f 6469  v>\n        </di
-0016afd0: 763e 5c6e 2020 2020 2020 2020 3c64 6976  v>\n        <div
-0016afe0: 2063 6c61 7373 3d22 6170 702d 6672 616d   class="app-fram
-0016aff0: 6520 6170 702d 7061 642d 6822 3e5c 6e20  e app-pad-h">\n 
-0016b000: 2020 2020 2020 2020 2020 203c 756c 2063             <ul c
-0016b010: 6c61 7373 3d22 6e61 7620 6e61 762d 7461  lass="nav nav-ta
-0016b020: 6273 223e 5c6e 2020 2020 2020 2020 2020  bs">\n          
-0016b030: 2020 2020 2020 3c6c 6920 7569 2d73 7265        <li ui-sre
-0016b040: 662d 6163 7469 7665 3d5c 2761 6374 6976  f-active=\'activ
-0016b050: 655c 273e 3c61 2075 692d 7372 6566 3d22  e\'><a ui-sref="
-0016b060: 6462 742e 756e 6974 5f74 6573 7428 7b5c  dbt.unit_test({\
-0016b070: 2723 5c27 3a20 5c27 6465 7363 7269 7074  '#\': \'descript
-0016b080: 696f 6e5c 277d 2922 3e44 6573 6372 6970  ion\'})">Descrip
-0016b090: 7469 6f6e 3c2f 613e 3c2f 6c69 3e5c 6e20  tion</a></li>\n 
-0016b0a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016b0b0: 6c69 2075 692d 7372 6566 2d61 6374 6976  li ui-sref-activ
-0016b0c0: 653d 5c27 6163 7469 7665 5c27 206e 672d  e=\'active\' ng-
-0016b0d0: 7368 6f77 203d 2022 7061 7265 6e74 734c  show = "parentsL
-0016b0e0: 656e 6774 6820 213d 2030 223e 3c61 2075  ength != 0"><a u
-0016b0f0: 692d 7372 6566 3d22 6462 742e 756e 6974  i-sref="dbt.unit
-0016b100: 5f74 6573 7428 7b5c 2723 5c27 3a20 5c27  _test({\'#\': \'
-0016b110: 6465 7065 6e64 735f 6f6e 5c27 7d29 223e  depends_on\'})">
-0016b120: 4465 7065 6e64 7320 4f6e 3c2f 613e 3c2f  Depends On</a></
-0016b130: 6c69 3e5c 6e20 2020 2020 2020 2020 2020  li>\n           
-0016b140: 203c 2f75 6c3e 5c6e 2020 2020 2020 2020   </ul>\n        
-0016b150: 3c2f 6469 763e 5c6e 2020 2020 3c2f 6469  </div>\n    </di
-0016b160: 763e 5c6e 2020 2020 3c64 6976 2063 6c61  v>\n    <div cla
-0016b170: 7373 3d22 6170 702d 6465 7461 696c 7322  ss="app-details"
-0016b180: 3e5c 6e20 2020 2020 2020 203c 6469 7620  >\n        <div 
-0016b190: 636c 6173 733d 2261 7070 2d66 7261 6d65  class="app-frame
-0016b1a0: 2061 7070 2d70 6164 223e 5c6e 2020 2020   app-pad">\n    
-0016b1b0: 2020 2020 2020 2020 3c73 6563 7469 6f6e          <section
-0016b1c0: 2063 6c61 7373 3d22 7365 6374 696f 6e22   class="section"
-0016b1d0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016b1e0: 2020 203c 6469 7620 636c 6173 733d 2273     <div class="s
-0016b1f0: 6563 7469 6f6e 2d74 6172 6765 7422 2069  ection-target" i
-0016b200: 643d 2264 6573 6372 6970 7469 6f6e 223e  d="description">
-0016b210: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-0016b220: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0016b230: 7373 3d22 7365 6374 696f 6e2d 636f 6e74  ss="section-cont
-0016b240: 656e 7422 3e5c 6e20 2020 2020 2020 2020  ent">\n         
-0016b250: 2020 2020 2020 2020 2020 203c 6836 3e44             <h6>D
-0016b260: 6573 6372 6970 7469 6f6e 3c2f 6836 3e5c  escription</h6>\
-0016b270: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016b280: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0016b290: 2270 616e 656c 223e 5c6e 2020 2020 2020  "panel">\n      
-0016b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016b2b0: 2020 3c64 6976 2063 6c61 7373 3d22 7061    <div class="pa
-0016b2c0: 6e65 6c2d 626f 6479 223e 5c6e 2020 2020  nel-body">\n    
-0016b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016b2e0: 2020 2020 2020 2020 3c64 6976 206e 672d          <div ng-
-0016b2f0: 6966 3d22 6d6f 6465 6c2e 6465 7363 7269  if="model.descri
-0016b300: 7074 696f 6e22 2063 6c61 7373 3d22 6d6f  ption" class="mo
-0016b310: 6465 6c2d 6d61 726b 646f 776e 2220 6d61  del-markdown" ma
-0016b320: 726b 6564 3d22 6d6f 6465 6c2e 6465 7363  rked="model.desc
-0016b330: 7269 7074 696f 6e22 3e3c 2f64 6976 3e5c  ription"></div>\
-0016b340: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016b350: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0016b360: 7620 6e67 2d69 663d 2221 6d6f 6465 6c2e  v ng-if="!model.
-0016b370: 6465 7363 7269 7074 696f 6e22 3e54 6869  description">Thi
-0016b380: 7320 7b7b 206d 6f64 656c 2e72 6573 6f75  s {{ model.resou
-0016b390: 7263 655f 7479 7065 207d 7d20 6973 206e  rce_type }} is n
-0016b3a0: 6f74 2063 7572 7265 6e74 6c79 2064 6f63  ot currently doc
-0016b3b0: 756d 656e 7465 643c 2f64 6976 3e5c 6e20  umented</div>\n 
-0016b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016b3d0: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
-0016b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016b3f0: 2020 203c 2f64 6976 3e5c 6e20 2020 2020     </div>\n     
-0016b400: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-0016b410: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
-0016b420: 2f73 6563 7469 6f6e 3e5c 6e5c 6e20 2020  /section>\n\n   
-0016b430: 2020 2020 2020 2020 203c 7365 6374 696f           <sectio
-0016b440: 6e20 636c 6173 733d 2273 6563 7469 6f6e  n class="section
-0016b450: 2220 6e67 2d73 686f 7720 3d20 2270 6172  " ng-show = "par
-0016b460: 656e 7473 4c65 6e67 7468 2021 3d20 3022  entsLength != 0"
-0016b470: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016b480: 2020 203c 6469 7620 636c 6173 733d 2273     <div class="s
-0016b490: 6563 7469 6f6e 2d74 6172 6765 7422 2069  ection-target" i
-0016b4a0: 643d 2264 6570 656e 6473 5f6f 6e22 3e3c  d="depends_on"><
-0016b4b0: 2f64 6976 3e5c 6e20 2020 2020 2020 2020  /div>\n         
-0016b4c0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0016b4d0: 733d 2273 6563 7469 6f6e 2d63 6f6e 7465  s="section-conte
-0016b4e0: 6e74 223e 5c6e 2020 2020 2020 2020 2020  nt">\n          
-0016b4f0: 2020 2020 2020 2020 2020 3c68 363e 4465            <h6>De
-0016b500: 7065 6e64 7320 4f6e 3c2f 6836 3e5c 6e20  pends On</h6>\n 
-0016b510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016b520: 2020 203c 7265 6665 7265 6e63 652d 6c69     <reference-li
-0016b530: 7374 2072 6566 6572 656e 6365 733d 2270  st references="p
-0016b540: 6172 656e 7473 2220 6e6f 6465 3d22 6d6f  arents" node="mo
-0016b550: 6465 6c22 202f 3e5c 6e20 2020 2020 2020  del" />\n       
-0016b560: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-0016b570: 6e20 2020 2020 2020 2020 2020 203c 2f73  n            </s
-0016b580: 6563 7469 6f6e 3e5c 6e5c 6e20 2020 2020  ection>\n\n     
-0016b590: 2020 203c 2f64 6976 3e5c 6e20 2020 203c     </div>\n    <
-0016b5a0: 2f64 6976 3e5c 6e3c 2f64 6976 3e5c 6e27  /div>\n</div>\n'
-0016b5b0: 297d 5d29 2c65 2e65 7870 6f72 7473 3d6e  )}]),e.exports=n
-0016b5c0: 7d2c 6675 6e63 7469 6f6e 2865 2c74 297b  },function(e,t){
-0016b5d0: 7661 7220 6e3d 222f 646f 6373 2f74 6573  var n="/docs/tes
-0016b5e0: 742e 6874 6d6c 223b 7769 6e64 6f77 2e61  t.html";window.a
-0016b5f0: 6e67 756c 6172 2e6d 6f64 756c 6528 226e  ngular.module("n
-0016b600: 6722 292e 7275 6e28 5b22 2474 656d 706c  g").run(["$templ
-0016b610: 6174 6543 6163 6865 222c 6675 6e63 7469  ateCache",functi
-0016b620: 6f6e 2865 297b 652e 7075 7428 6e2c 273c  on(e){e.put(n,'<
-0016b630: 7374 796c 653e 5c6e 2f2a 2054 4f44 4f20  style>\n/* TODO 
-0016b640: 2a2f 5c6e 2e73 6563 7469 6f6e 2d74 6172  */\n.section-tar
-0016b650: 6765 7420 7b5c 6e20 2020 2074 6f70 3a20  get {\n    top: 
-0016b660: 2d38 656d 3b5c 6e7d 5c6e 5c6e 2e6e 6f66  -8em;\n}\n\n.nof
-0016b670: 6c65 7820 7b5c 6e20 2020 2066 6c65 783a  lex {\n    flex:
-0016b680: 2030 2030 2031 3630 7078 2021 696d 706f   0 0 160px !impo
-0016b690: 7274 616e 743b 5c6e 7d5c 6e5c 6e2e 6869  rtant;\n}\n\n.hi
-0016b6a0: 6768 6c69 6768 7420 7b5c 6e20 2020 2063  ghlight {\n    c
-0016b6b0: 6f6c 6f72 3a20 2332 3432 3932 653b 5c6e  olor: #24292e;\n
-0016b6c0: 2020 2020 6261 636b 6772 6f75 6e64 2d63      background-c
-0016b6d0: 6f6c 6f72 3a20 7768 6974 653b 5c6e 7d5c  olor: white;\n}\
-0016b6e0: 6e5c 6e3c 2f73 7479 6c65 3e5c 6e5c 6e3c  n\n</style>\n\n<
-0016b6f0: 6469 7620 636c 6173 733d 5c27 6170 702d  div class=\'app-
-0016b700: 7363 726f 6c6c 5c27 3e5c 6e20 2020 203c  scroll\'>\n    <
-0016b710: 6469 7620 636c 6173 733d 2261 7070 2d6c  div class="app-l
-0016b720: 696e 6b73 2061 7070 2d73 7469 636b 7922  inks app-sticky"
-0016b730: 3e5c 6e20 2020 2020 2020 203c 6469 7620  >\n        <div 
-0016b740: 636c 6173 733d 2261 7070 2d74 6974 6c65  class="app-title
-0016b750: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
-0016b760: 3c64 6976 2063 6c61 7373 3d22 6170 702d  <div class="app-
-0016b770: 6672 616d 6520 6170 702d 7061 6420 6170  frame app-pad ap
-0016b780: 702d 666c 7573 682d 626f 7474 6f6d 223e  p-flush-bottom">
-0016b790: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0016b7a0: 2020 3c68 313e 5c6e 2020 2020 2020 2020    <h1>\n        
-0016b7b0: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
-0016b7c0: 6e20 636c 6173 733d 2262 7265 616b 223e  n class="break">
-0016b7d0: 7b7b 206d 6f64 656c 2e6e 616d 6520 7d7d  {{ model.name }}
-0016b7e0: 3c2f 7370 616e 3e5c 6e20 2020 2020 2020  </span>\n       
-0016b7f0: 2020 2020 2020 2020 2020 2020 203c 736d               <sm
-0016b800: 616c 6c3e 7465 7374 3c2f 736d 616c 6c3e  all>test</small>
-0016b810: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0016b820: 2020 3c2f 6831 3e5c 6e20 2020 2020 2020    </h1>\n       
-0016b830: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
-0016b840: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
-0016b850: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0016b860: 2261 7070 2d66 7261 6d65 2061 7070 2d70  "app-frame app-p
-0016b870: 6164 2d68 223e 5c6e 2020 2020 2020 2020  ad-h">\n        
-0016b880: 2020 2020 3c75 6c20 636c 6173 733d 226e      <ul class="n
-0016b890: 6176 206e 6176 2d74 6162 7322 3e5c 6e20  av nav-tabs">\n 
-0016b8a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016b8b0: 6c69 2075 692d 7372 6566 2d61 6374 6976  li ui-sref-activ
-0016b8c0: 653d 5c27 6163 7469 7665 5c27 3e3c 6120  e=\'active\'><a 
-0016b8d0: 7569 2d73 7265 663d 2264 6274 2e74 6573  ui-sref="dbt.tes
-0016b8e0: 7428 7b5c 2723 5c27 3a20 5c27 6465 7363  t({\'#\': \'desc
-0016b8f0: 7269 7074 696f 6e5c 277d 2922 3e44 6573  ription\'})">Des
-0016b900: 6372 6970 7469 6f6e 3c2f 613e 3c2f 6c69  cription</a></li
-0016b910: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016b920: 2020 203c 6c69 2075 692d 7372 6566 2d61     <li ui-sref-a
-0016b930: 6374 6976 653d 5c27 6163 7469 7665 5c27  ctive=\'active\'
-0016b940: 206e 672d 7368 6f77 203d 2022 7061 7265   ng-show = "pare
-0016b950: 6e74 734c 656e 6774 6820 213d 2030 223e  ntsLength != 0">
-0016b960: 3c61 2075 692d 7372 6566 3d22 6462 742e  <a ui-sref="dbt.
-0016b970: 7465 7374 287b 5c27 235c 273a 205c 2764  test({\'#\': \'d
-0016b980: 6570 656e 6473 5f6f 6e5c 277d 2922 3e44  epends_on\'})">D
-0016b990: 6570 656e 6473 204f 6e3c 2f61 3e3c 2f6c  epends On</a></l
-0016b9a0: 693e 5c6e 2020 2020 2020 2020 2020 2020  i>\n            
-0016b9b0: 2020 2020 3c6c 6920 7569 2d73 7265 662d      <li ui-sref-
-0016b9c0: 6163 7469 7665 3d5c 2761 6374 6976 655c  active=\'active\
-0016b9d0: 273e 3c61 2075 692d 7372 6566 3d22 6462  '><a ui-sref="db
-0016b9e0: 742e 7465 7374 287b 5c27 235c 273a 205c  t.test({\'#\': \
-0016b9f0: 2763 6f64 655c 277d 2922 3e53 514c 3c2f  'code\'})">SQL</
-0016ba00: 613e 3c2f 6c69 3e5c 6e20 2020 2020 2020  a></li>\n       
-0016ba10: 2020 2020 203c 2f75 6c3e 5c6e 2020 2020       </ul>\n    
-0016ba20: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
-0016ba30: 3c2f 6469 763e 5c6e 2020 2020 3c64 6976  </div>\n    <div
-0016ba40: 2063 6c61 7373 3d22 6170 702d 6465 7461   class="app-deta
-0016ba50: 696c 7322 3e5c 6e20 2020 2020 2020 203c  ils">\n        <
-0016ba60: 6469 7620 636c 6173 733d 2261 7070 2d66  div class="app-f
-0016ba70: 7261 6d65 2061 7070 2d70 6164 223e 5c6e  rame app-pad">\n
-0016ba80: 2020 2020 2020 2020 2020 2020 3c73 6563              <sec
-0016ba90: 7469 6f6e 2063 6c61 7373 3d22 7365 6374  tion class="sect
-0016baa0: 696f 6e22 3e5c 6e20 2020 2020 2020 2020  ion">\n         
-0016bab0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0016bac0: 733d 2273 6563 7469 6f6e 2d74 6172 6765  s="section-targe
-0016bad0: 7422 2069 643d 2264 6573 6372 6970 7469  t" id="descripti
-0016bae0: 6f6e 223e 3c2f 6469 763e 5c6e 2020 2020  on"></div>\n    
-0016baf0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-0016bb00: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
-0016bb10: 636f 6e74 656e 7422 3e5c 6e20 2020 2020  content">\n     
-0016bb20: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016bb30: 6836 3e44 6573 6372 6970 7469 6f6e 3c2f  h6>Description</
-0016bb40: 6836 3e5c 6e20 2020 2020 2020 2020 2020  h6>\n           
-0016bb50: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0016bb60: 6173 733d 2270 616e 656c 223e 5c6e 2020  ass="panel">\n  
-0016bb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016bb80: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0016bb90: 3d22 7061 6e65 6c2d 626f 6479 223e 5c6e  ="panel-body">\n
-0016bba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016bbb0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-0016bbc0: 206e 672d 6966 3d22 6d6f 6465 6c2e 6465   ng-if="model.de
-0016bbd0: 7363 7269 7074 696f 6e22 2063 6c61 7373  scription" class
-0016bbe0: 3d22 6d6f 6465 6c2d 6d61 726b 646f 776e  ="model-markdown
-0016bbf0: 2220 6d61 726b 6564 3d22 6d6f 6465 6c2e  " marked="model.
-0016bc00: 6465 7363 7269 7074 696f 6e22 3e3c 2f64  description"></d
-0016bc10: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
-0016bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016bc30: 203c 6469 7620 6e67 2d69 663d 2221 6d6f   <div ng-if="!mo
-0016bc40: 6465 6c2e 6465 7363 7269 7074 696f 6e22  del.description"
-0016bc50: 3e54 6869 7320 7b7b 206d 6f64 656c 2e72  >This {{ model.r
-0016bc60: 6573 6f75 7263 655f 7479 7065 207d 7d20  esource_type }} 
-0016bc70: 6973 206e 6f74 2063 7572 7265 6e74 6c79  is not currently
-0016bc80: 2064 6f63 756d 656e 7465 643c 2f64 6976   documented</div
-0016bc90: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016bca0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
-0016bcb0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016bcc0: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
-0016bcd0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016bce0: 2f64 6976 3e5c 6e20 2020 2020 2020 2020  /div>\n         
-0016bcf0: 2020 203c 2f73 6563 7469 6f6e 3e5c 6e5c     </section>\n\
-0016bd00: 6e20 2020 2020 2020 2020 2020 203c 7365  n            <se
-0016bd10: 6374 696f 6e20 636c 6173 733d 2273 6563  ction class="sec
-0016bd20: 7469 6f6e 2220 6e67 2d73 686f 7720 3d20  tion" ng-show = 
-0016bd30: 2270 6172 656e 7473 4c65 6e67 7468 2021  "parentsLength !
-0016bd40: 3d20 3022 3e5c 6e20 2020 2020 2020 2020  = 0">\n         
-0016bd50: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0016bd60: 733d 2273 6563 7469 6f6e 2d74 6172 6765  s="section-targe
-0016bd70: 7422 2069 643d 2264 6570 656e 6473 5f6f  t" id="depends_o
-0016bd80: 6e22 3e3c 2f64 6976 3e5c 6e20 2020 2020  n"></div>\n     
-0016bd90: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0016bda0: 636c 6173 733d 2273 6563 7469 6f6e 2d63  class="section-c
-0016bdb0: 6f6e 7465 6e74 223e 5c6e 2020 2020 2020  ontent">\n      
-0016bdc0: 2020 2020 2020 2020 2020 2020 2020 3c68                <h
-0016bdd0: 363e 4465 7065 6e64 7320 4f6e 3c2f 6836  6>Depends On</h6
-0016bde0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016bdf0: 2020 2020 2020 203c 7265 6665 7265 6e63         <referenc
-0016be00: 652d 6c69 7374 2072 6566 6572 656e 6365  e-list reference
-0016be10: 733d 2270 6172 656e 7473 2220 6e6f 6465  s="parents" node
-0016be20: 3d22 6d6f 6465 6c22 202f 3e5c 6e20 2020  ="model" />\n   
-0016be30: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-0016be40: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
-0016be50: 203c 2f73 6563 7469 6f6e 3e5c 6e5c 6e20   </section>\n\n 
-0016be60: 2020 2020 2020 2020 2020 203c 7365 6374             <sect
-0016be70: 696f 6e20 636c 6173 733d 2273 6563 7469  ion class="secti
-0016be80: 6f6e 223e 5c6e 2020 2020 2020 2020 2020  on">\n          
-0016be90: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0016bea0: 3d22 7365 6374 696f 6e2d 7461 7267 6574  ="section-target
-0016beb0: 2220 6964 3d22 636f 6465 223e 3c2f 6469  " id="code"></di
-0016bec0: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
-0016bed0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0016bee0: 7365 6374 696f 6e2d 636f 6e74 656e 7422  section-content"
-0016bef0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016bf00: 2020 2020 2020 203c 636f 6465 2d62 6c6f         <code-blo
-0016bf10: 636b 2076 6572 7369 6f6e 733d 2276 6572  ck versions="ver
-0016bf20: 7369 6f6e 7322 2064 6566 6175 6c74 3d22  sions" default="
-0016bf30: 6465 6661 756c 745f 7665 7273 696f 6e22  default_version"
-0016bf40: 206c 616e 6775 6167 653d 226c 616e 6775   language="langu
-0016bf50: 6167 6522 3e3c 2f63 6f64 652d 626c 6f63  age"></code-bloc
-0016bf60: 6b3e 5c6e 2020 2020 2020 2020 2020 2020  k>\n            
-0016bf70: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
-0016bf80: 2020 2020 2020 2020 3c2f 7365 6374 696f          </sectio
-0016bf90: 6e3e 5c6e 2020 2020 2020 2020 3c2f 6469  n>\n        </di
-0016bfa0: 763e 5c6e 2020 2020 3c2f 6469 763e 5c6e  v>\n    </div>\n
-0016bfb0: 3c2f 6469 763e 5c6e 2729 7d5d 292c 652e  </div>\n')}]),e.
-0016bfc0: 6578 706f 7274 733d 6e7d 2c66 756e 6374  exports=n},funct
-0016bfd0: 696f 6e28 652c 7429 7b76 6172 206e 3d22  ion(e,t){var n="
-0016bfe0: 2f64 6f63 732f 616e 616c 7973 6973 2e68  /docs/analysis.h
-0016bff0: 746d 6c22 3b77 696e 646f 772e 616e 6775  tml";window.angu
-0016c000: 6c61 722e 6d6f 6475 6c65 2822 6e67 2229  lar.module("ng")
-0016c010: 2e72 756e 285b 2224 7465 6d70 6c61 7465  .run(["$template
-0016c020: 4361 6368 6522 2c66 756e 6374 696f 6e28  Cache",function(
-0016c030: 6529 7b65 2e70 7574 286e 2c27 3c73 7479  e){e.put(n,'<sty
-0016c040: 6c65 3e5c 6e2f 2a20 544f 444f 202a 2f5c  le>\n/* TODO */\
-0016c050: 6e2e 7365 6374 696f 6e2d 7461 7267 6574  n.section-target
-0016c060: 207b 5c6e 2020 2020 746f 703a 202d 3865   {\n    top: -8e
-0016c070: 6d3b 5c6e 7d5c 6e5c 6e2e 6e6f 666c 6578  m;\n}\n\n.noflex
-0016c080: 207b 5c6e 2020 2020 666c 6578 3a20 3020   {\n    flex: 0 
-0016c090: 3020 3136 3070 7820 2169 6d70 6f72 7461  0 160px !importa
-0016c0a0: 6e74 3b5c 6e7d 5c6e 5c6e 2e68 6967 686c  nt;\n}\n\n.highl
-0016c0b0: 6967 6874 207b 5c6e 2020 2020 636f 6c6f  ight {\n    colo
-0016c0c0: 723a 2023 3234 3239 3265 3b5c 6e20 2020  r: #24292e;\n   
-0016c0d0: 2062 6163 6b67 726f 756e 642d 636f 6c6f   background-colo
-0016c0e0: 723a 2077 6869 7465 3b5c 6e7d 5c6e 5c6e  r: white;\n}\n\n
-0016c0f0: 3c2f 7374 796c 653e 5c6e 5c6e 3c64 6976  </style>\n\n<div
-0016c100: 2063 6c61 7373 3d5c 2761 7070 2d73 6372   class=\'app-scr
-0016c110: 6f6c 6c5c 273e 5c6e 2020 2020 3c64 6976  oll\'>\n    <div
-0016c120: 2063 6c61 7373 3d22 6170 702d 6c69 6e6b   class="app-link
-0016c130: 7320 6170 702d 7374 6963 6b79 223e 5c6e  s app-sticky">\n
-0016c140: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0016c150: 7373 3d22 6170 702d 7469 746c 6522 3e5c  ss="app-title">\
-0016c160: 6e20 2020 2020 2020 2020 2020 203c 6469  n            <di
-0016c170: 7620 636c 6173 733d 2261 7070 2d66 7261  v class="app-fra
-0016c180: 6d65 2061 7070 2d70 6164 2061 7070 2d66  me app-pad app-f
-0016c190: 6c75 7368 2d62 6f74 746f 6d22 3e5c 6e20  lush-bottom">\n 
-0016c1a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016c1b0: 6831 206e 672d 6966 3d22 6d6f 6465 6c2e  h1 ng-if="model.
-0016c1c0: 646f 6373 2e73 686f 7720 3d3d 3d20 6661  docs.show === fa
-0016c1d0: 6c73 6522 3e5c 6e20 2020 2020 2020 2020  lse">\n         
-0016c1e0: 2020 2020 2020 2020 2020 203c 736d 616c             <smal
-0016c1f0: 6c20 636c 6173 733d 5c27 7465 7874 2d62  l class=\'text-b
-0016c200: 6f6c 6420 7465 7874 2d72 6967 6874 5c27  old text-right\'
-0016c210: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016c220: 2020 2020 2020 2020 2020 203c 6920 6461             <i da
-0016c230: 7461 2d69 636f 6e3d 2265 7965 223e 3c2f  ta-icon="eye"></
-0016c240: 693e 5c6e 2020 2020 2020 2020 2020 2020  i>\n            
-0016c250: 2020 2020 2020 2020 2020 2020 5468 6973              This
-0016c260: 207b 7b20 6d6f 6465 6c2e 7265 736f 7572   {{ model.resour
-0016c270: 6365 5f74 7970 6520 7d7d 2069 7320 6869  ce_type }} is hi
-0016c280: 6464 656e 5c6e 2020 2020 2020 2020 2020  dden\n          
-0016c290: 2020 2020 2020 2020 2020 3c2f 736d 616c            </smal
-0016c2a0: 6c3e 5c6e 2020 2020 2020 2020 2020 2020  l>\n            
-0016c2b0: 2020 2020 3c2f 6831 3e5c 6e20 2020 2020      </h1>\n     
-0016c2c0: 2020 2020 2020 2020 2020 203c 6831 3e5c             <h1>\
-0016c2d0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016c2e0: 2020 2020 203c 7370 616e 2063 6c61 7373       <span class
-0016c2f0: 3d22 6272 6561 6b22 3e7b 7b20 6d6f 6465  ="break">{{ mode
-0016c300: 6c2e 6e61 6d65 207d 7d3c 2f73 7061 6e3e  l.name }}</span>
-0016c310: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0016c320: 2020 2020 2020 3c73 6d61 6c6c 3e41 6e61        <small>Ana
-0016c330: 6c79 7369 733c 2f73 6d61 6c6c 3e5c 6e20  lysis</small>\n 
-0016c340: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016c350: 2f68 313e 5c6e 2020 2020 2020 2020 2020  /h1>\n          
-0016c360: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
-0016c370: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
-0016c380: 2020 3c64 6976 2063 6c61 7373 3d22 6170    <div class="ap
-0016c390: 702d 6672 616d 6520 6170 702d 7061 642d  p-frame app-pad-
-0016c3a0: 6822 3e5c 6e20 2020 2020 2020 2020 2020  h">\n           
-0016c3b0: 203c 756c 2063 6c61 7373 3d22 6e61 7620   <ul class="nav 
-0016c3c0: 6e61 762d 7461 6273 223e 5c6e 2020 2020  nav-tabs">\n    
-0016c3d0: 2020 2020 2020 2020 2020 2020 3c6c 6920              <li 
-0016c3e0: 7569 2d73 7265 662d 6163 7469 7665 3d5c  ui-sref-active=\
-0016c3f0: 2761 6374 6976 655c 273e 3c61 2075 692d  'active\'><a ui-
-0016c400: 7372 6566 3d22 6462 742e 616e 616c 7973  sref="dbt.analys
-0016c410: 6973 287b 5c27 235c 273a 205c 2764 6573  is({\'#\': \'des
-0016c420: 6372 6970 7469 6f6e 5c27 7d29 223e 4465  cription\'})">De
-0016c430: 7363 7269 7074 696f 6e3c 2f61 3e3c 2f6c  scription</a></l
-0016c440: 693e 5c6e 2020 2020 2020 2020 2020 2020  i>\n            
-0016c450: 2020 2020 3c6c 6920 7569 2d73 7265 662d      <li ui-sref-
-0016c460: 6163 7469 7665 3d5c 2761 6374 6976 655c  active=\'active\
-0016c470: 2720 6e67 2d73 686f 7720 3d20 2270 6172  ' ng-show = "par
-0016c480: 656e 7473 4c65 6e67 7468 2021 3d20 3022  entsLength != 0"
-0016c490: 3e3c 6120 7569 2d73 7265 663d 2264 6274  ><a ui-sref="dbt
-0016c4a0: 2e61 6e61 6c79 7369 7328 7b5c 2723 5c27  .analysis({\'#\'
-0016c4b0: 3a20 5c27 6465 7065 6e64 735f 6f6e 5c27  : \'depends_on\'
-0016c4c0: 7d29 223e 4465 7065 6e64 7320 4f6e 3c2f  })">Depends On</
-0016c4d0: 613e 3c2f 6c69 3e5c 6e20 2020 2020 2020  a></li>\n       
-0016c4e0: 2020 2020 2020 2020 203c 6c69 2075 692d           <li ui-
-0016c4f0: 7372 6566 2d61 6374 6976 653d 5c27 6163  sref-active=\'ac
-0016c500: 7469 7665 5c27 3e3c 6120 7569 2d73 7265  tive\'><a ui-sre
-0016c510: 663d 2264 6274 2e61 6e61 6c79 7369 7328  f="dbt.analysis(
-0016c520: 7b5c 2723 5c27 3a20 5c27 7371 6c5c 277d  {\'#\': \'sql\'}
-0016c530: 2922 3e53 514c 3c2f 613e 3c2f 6c69 3e5c  )">SQL</a></li>\
-0016c540: 6e20 2020 2020 2020 2020 2020 203c 2f75  n            </u
-0016c550: 6c3e 5c6e 2020 2020 2020 2020 3c2f 6469  l>\n        </di
-0016c560: 763e 5c6e 2020 2020 3c2f 6469 763e 5c6e  v>\n    </div>\n
-0016c570: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0016c580: 6170 702d 6465 7461 696c 7322 3e5c 6e20  app-details">\n 
-0016c590: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0016c5a0: 733d 2261 7070 2d66 7261 6d65 2061 7070  s="app-frame app
-0016c5b0: 2d70 6164 223e 5c6e 5c6e 2020 2020 2020  -pad">\n\n      
-0016c5c0: 2020 2020 2020 3c73 6563 7469 6f6e 2063        <section c
-0016c5d0: 6c61 7373 3d22 7365 6374 696f 6e22 3e5c  lass="section">\
-0016c5e0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016c5f0: 203c 6469 7620 636c 6173 733d 2273 6563   <div class="sec
-0016c600: 7469 6f6e 2d74 6172 6765 7422 2069 643d  tion-target" id=
-0016c610: 2264 6573 6372 6970 7469 6f6e 223e 3c2f  "description"></
-0016c620: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
-0016c630: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0016c640: 3d22 7365 6374 696f 6e2d 636f 6e74 656e  ="section-conten
-0016c650: 7422 3e5c 6e20 2020 2020 2020 2020 2020  t">\n           
-0016c660: 2020 2020 2020 2020 203c 6836 3e44 6573           <h6>Des
-0016c670: 6372 6970 7469 6f6e 3c2f 6836 3e5c 6e20  cription</h6>\n 
-0016c680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016c690: 2020 203c 6469 7620 636c 6173 733d 2270     <div class="p
-0016c6a0: 616e 656c 223e 5c6e 2020 2020 2020 2020  anel">\n        
-0016c6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016c6c0: 3c64 6976 2063 6c61 7373 3d22 7061 6e65  <div class="pane
-0016c6d0: 6c2d 626f 6479 223e 5c6e 2020 2020 2020  l-body">\n      
-0016c6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016c6f0: 2020 2020 2020 3c64 6976 206e 672d 6966        <div ng-if
-0016c700: 3d22 6d6f 6465 6c2e 6465 7363 7269 7074  ="model.descript
-0016c710: 696f 6e22 2063 6c61 7373 3d22 6d6f 6465  ion" class="mode
-0016c720: 6c2d 6d61 726b 646f 776e 2220 6d61 726b  l-markdown" mark
-0016c730: 6564 3d22 6d6f 6465 6c2e 6465 7363 7269  ed="model.descri
-0016c740: 7074 696f 6e22 3e3c 2f64 6976 3e5c 6e20  ption"></div>\n 
-0016c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016c760: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0016c770: 6e67 2d69 663d 2221 6d6f 6465 6c2e 6465  ng-if="!model.de
-0016c780: 7363 7269 7074 696f 6e22 3e54 6869 7320  scription">This 
-0016c790: 7b7b 206d 6f64 656c 2e72 6573 6f75 7263  {{ model.resourc
-0016c7a0: 655f 7479 7065 207d 7d20 6973 206e 6f74  e_type }} is not
-0016c7b0: 2063 7572 7265 6e74 6c79 2064 6f63 756d   currently docum
-0016c7c0: 656e 7465 643c 2f64 6976 3e5c 6e20 2020  ented</div>\n   
-0016c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016c7e0: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
-0016c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016c800: 203c 2f64 6976 3e5c 6e20 2020 2020 2020   </div>\n       
-0016c810: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-0016c820: 6e20 2020 2020 2020 2020 2020 203c 2f73  n            </s
-0016c830: 6563 7469 6f6e 3e5c 6e5c 6e20 2020 2020  ection>\n\n     
-0016c840: 2020 2020 2020 203c 7365 6374 696f 6e20         <section 
-0016c850: 636c 6173 733d 2273 6563 7469 6f6e 2220  class="section" 
-0016c860: 6e67 2d73 686f 7720 3d20 2270 6172 656e  ng-show = "paren
-0016c870: 7473 4c65 6e67 7468 2021 3d20 3022 3e5c  tsLength != 0">\
-0016c880: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016c890: 203c 6469 7620 636c 6173 733d 2273 6563   <div class="sec
-0016c8a0: 7469 6f6e 2d74 6172 6765 7422 2069 643d  tion-target" id=
-0016c8b0: 2264 6570 656e 6473 5f6f 6e22 3e3c 2f64  "depends_on"></d
-0016c8c0: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
-0016c8d0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0016c8e0: 2273 6563 7469 6f6e 2d63 6f6e 7465 6e74  "section-content
-0016c8f0: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
-0016c900: 2020 2020 2020 2020 3c68 363e 4465 7065          <h6>Depe
-0016c910: 6e64 7320 4f6e 3c2f 6836 3e5c 6e20 2020  nds On</h6>\n   
-0016c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016c930: 203c 7265 6665 7265 6e63 652d 6c69 7374   <reference-list
-0016c940: 2072 6566 6572 656e 6365 733d 2270 6172   references="par
-0016c950: 656e 7473 2220 2f3e 5c6e 2020 2020 2020  ents" />\n      
-0016c960: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-0016c970: 5c6e 2020 2020 2020 2020 2020 2020 3c2f  \n            </
-0016c980: 7365 6374 696f 6e3e 5c6e 5c6e 2020 2020  section>\n\n    
-0016c990: 2020 2020 2020 2020 3c73 6563 7469 6f6e          <section
-0016c9a0: 2063 6c61 7373 3d22 7365 6374 696f 6e22   class="section"
-0016c9b0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016c9c0: 2020 203c 6469 7620 636c 6173 733d 2273     <div class="s
-0016c9d0: 6563 7469 6f6e 2d74 6172 6765 7422 2069  ection-target" i
-0016c9e0: 643d 2273 716c 223e 3c2f 6469 763e 5c6e  d="sql"></div>\n
-0016c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016ca00: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
-0016ca10: 696f 6e2d 636f 6e74 656e 7422 3e5c 6e20  ion-content">\n 
-0016ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016ca30: 2020 203c 636f 6465 2d62 6c6f 636b 2076     <code-block v
-0016ca40: 6572 7369 6f6e 733d 2276 6572 7369 6f6e  ersions="version
-0016ca50: 7322 2064 6566 6175 6c74 3d22 6465 6661  s" default="defa
-0016ca60: 756c 745f 7665 7273 696f 6e22 206c 616e  ult_version" lan
-0016ca70: 6775 6167 653d 226c 616e 6775 6167 6522  guage="language"
-0016ca80: 3e3c 2f63 6f64 652d 626c 6f63 6b3e 5c6e  ></code-block>\n
-0016ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016caa0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-0016cab0: 2020 2020 3c2f 7365 6374 696f 6e3e 5c6e      </section>\n
-0016cac0: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
-0016cad0: 2020 2020 3c2f 6469 763e 5c6e 3c2f 6469      </div>\n</di
-0016cae0: 763e 5c6e 2729 7d5d 292c 652e 6578 706f  v>\n')}]),e.expo
-0016caf0: 7274 733d 6e7d 2c66 756e 6374 696f 6e28  rts=n},function(
-0016cb00: 652c 7429 7b76 6172 206e 3d22 2f64 6f63  e,t){var n="/doc
-0016cb10: 732f 6d61 6372 6f2e 6874 6d6c 223b 7769  s/macro.html";wi
-0016cb20: 6e64 6f77 2e61 6e67 756c 6172 2e6d 6f64  ndow.angular.mod
-0016cb30: 756c 6528 226e 6722 292e 7275 6e28 5b22  ule("ng").run(["
-0016cb40: 2474 656d 706c 6174 6543 6163 6865 222c  $templateCache",
-0016cb50: 6675 6e63 7469 6f6e 2865 297b 652e 7075  function(e){e.pu
-0016cb60: 7428 6e2c 273c 7374 796c 653e 5c6e 2f2a  t(n,'<style>\n/*
-0016cb70: 2054 4f44 4f20 2a2f 5c6e 2e73 6563 7469   TODO */\n.secti
-0016cb80: 6f6e 2d74 6172 6765 7420 7b5c 6e20 2020  on-target {\n   
-0016cb90: 2074 6f70 3a20 2d38 656d 3b5c 6e7d 5c6e   top: -8em;\n}\n
-0016cba0: 5c6e 2e6e 6f66 6c65 7820 7b5c 6e20 2020  \n.noflex {\n   
-0016cbb0: 2066 6c65 783a 2030 2030 2031 3630 7078   flex: 0 0 160px
-0016cbc0: 2021 696d 706f 7274 616e 743b 5c6e 7d5c   !important;\n}\
-0016cbd0: 6e5c 6e2e 6869 6768 6c69 6768 7420 7b5c  n\n.highlight {\
-0016cbe0: 6e20 2020 2063 6f6c 6f72 3a20 2332 3432  n    color: #242
-0016cbf0: 3932 653b 5c6e 2020 2020 6261 636b 6772  92e;\n    backgr
-0016cc00: 6f75 6e64 2d63 6f6c 6f72 3a20 7768 6974  ound-color: whit
-0016cc10: 653b 5c6e 7d5c 6e5c 6e3c 2f73 7479 6c65  e;\n}\n\n</style
-0016cc20: 3e5c 6e5c 6e3c 6469 7620 636c 6173 733d  >\n\n<div class=
-0016cc30: 5c27 6170 702d 7363 726f 6c6c 5c27 3e5c  \'app-scroll\'>\
-0016cc40: 6e20 2020 203c 6469 7620 636c 6173 733d  n    <div class=
-0016cc50: 2261 7070 2d6c 696e 6b73 2061 7070 2d73  "app-links app-s
-0016cc60: 7469 636b 7922 3e5c 6e20 2020 2020 2020  ticky">\n       
-0016cc70: 203c 6469 7620 636c 6173 733d 2261 7070   <div class="app
-0016cc80: 2d74 6974 6c65 223e 5c6e 2020 2020 2020  -title">\n      
-0016cc90: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0016cca0: 3d22 6170 702d 6672 616d 6520 6170 702d  ="app-frame app-
-0016ccb0: 7061 6420 6170 702d 666c 7573 682d 626f  pad app-flush-bo
-0016ccc0: 7474 6f6d 223e 5c6e 2020 2020 2020 2020  ttom">\n        
-0016ccd0: 2020 2020 2020 2020 3c68 313e 5c6e 2020          <h1>\n  
-0016cce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016ccf0: 2020 3c73 7061 6e20 636c 6173 733d 2262    <span class="b
-0016cd00: 7265 616b 223e 7b7b 206d 6163 726f 2e70  reak">{{ macro.p
-0016cd10: 6163 6b61 6765 5f6e 616d 6520 7d7d 2e7b  ackage_name }}.{
-0016cd20: 7b20 6d61 6372 6f2e 6e61 6d65 207d 7d3c  { macro.name }}<
-0016cd30: 2f73 7061 6e3e 5c6e 2020 2020 2020 2020  /span>\n        
-0016cd40: 2020 2020 2020 2020 2020 2020 3c73 6d61              <sma
-0016cd50: 6c6c 206e 672d 6966 3d22 6d61 6372 6f2e  ll ng-if="macro.
-0016cd60: 6973 5f61 6461 7074 6572 5f6d 6163 726f  is_adapter_macro
-0016cd70: 223e 6164 6170 7465 7220 6d61 6372 6f3c  ">adapter macro<
-0016cd80: 2f73 6d61 6c6c 3e5c 6e20 2020 2020 2020  /small>\n       
-0016cd90: 2020 2020 2020 2020 2020 2020 203c 736d               <sm
-0016cda0: 616c 6c20 6e67 2d69 663d 2221 6d61 6372  all ng-if="!macr
-0016cdb0: 6f2e 6973 5f61 6461 7074 6572 5f6d 6163  o.is_adapter_mac
-0016cdc0: 726f 223e 6d61 6372 6f3c 2f73 6d61 6c6c  ro">macro</small
-0016cdd0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016cde0: 2020 203c 2f68 313e 5c6e 2020 2020 2020     </h1>\n      
-0016cdf0: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
-0016ce00: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
-0016ce10: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0016ce20: 3d22 6170 702d 6672 616d 6520 6170 702d  ="app-frame app-
-0016ce30: 7061 642d 6822 3e5c 6e20 2020 2020 2020  pad-h">\n       
-0016ce40: 2020 2020 203c 756c 2063 6c61 7373 3d22       <ul class="
-0016ce50: 6e61 7620 6e61 762d 7461 6273 223e 5c6e  nav nav-tabs">\n
-0016ce60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016ce70: 3c6c 6920 7569 2d73 7265 662d 6163 7469  <li ui-sref-acti
-0016ce80: 7665 3d5c 2761 6374 6976 655c 273e 3c61  ve=\'active\'><a
-0016ce90: 2075 692d 7372 6566 3d22 6462 742e 6d61   ui-sref="dbt.ma
-0016cea0: 6372 6f28 7b5c 2723 5c27 3a20 5c27 6465  cro({\'#\': \'de
-0016ceb0: 7363 7269 7074 696f 6e5c 277d 2922 3e44  scription\'})">D
-0016cec0: 6573 6372 6970 7469 6f6e 3c2f 613e 3c2f  escription</a></
-0016ced0: 6c69 3e5c 6e20 2020 2020 2020 2020 2020  li>\n           
-0016cee0: 2020 2020 203c 6c69 2075 692d 7372 6566       <li ui-sref
-0016cef0: 2d61 6374 6976 653d 5c27 6163 7469 7665  -active=\'active
-0016cf00: 5c27 3e3c 6120 7569 2d73 7265 663d 2264  \'><a ui-sref="d
-0016cf10: 6274 2e6d 6163 726f 287b 5c27 235c 273a  bt.macro({\'#\':
-0016cf20: 205c 2761 7267 756d 656e 7473 5c27 7d29   \'arguments\'})
-0016cf30: 223e 4172 6775 6d65 6e74 733c 2f61 3e3c  ">Arguments</a><
-0016cf40: 2f6c 693e 5c6e 2020 2020 2020 2020 2020  /li>\n          
-0016cf50: 2020 2020 2020 3c6c 6920 7569 2d73 7265        <li ui-sre
-0016cf60: 662d 6163 7469 7665 3d5c 2761 6374 6976  f-active=\'activ
-0016cf70: 655c 2720 6e67 2d73 686f 7720 3d20 2272  e\' ng-show = "r
-0016cf80: 6566 6572 656e 6365 734c 656e 6774 6820  eferencesLength 
-0016cf90: 213d 2030 223e 3c61 2075 692d 7372 6566  != 0"><a ui-sref
-0016cfa0: 3d22 6462 742e 6d61 6372 6f28 7b5c 2723  ="dbt.macro({\'#
-0016cfb0: 5c27 3a20 5c27 7265 6665 7265 6e63 6564  \': \'referenced
-0016cfc0: 5f62 795c 277d 2922 3e52 6566 6572 656e  _by\'})">Referen
-0016cfd0: 6365 6420 4279 3c2f 613e 3c2f 6c69 3e5c  ced By</a></li>\
-0016cfe0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016cff0: 203c 6c69 2075 692d 7372 6566 2d61 6374   <li ui-sref-act
-0016d000: 6976 653d 5c27 6163 7469 7665 5c27 206e  ive=\'active\' n
-0016d010: 672d 7368 6f77 203d 2022 7061 7265 6e74  g-show = "parent
-0016d020: 734c 656e 6774 6820 213d 2030 223e 3c61  sLength != 0"><a
-0016d030: 2075 692d 7372 6566 3d22 6462 742e 6d61   ui-sref="dbt.ma
-0016d040: 6372 6f28 7b5c 2723 5c27 3a20 5c27 6465  cro({\'#\': \'de
-0016d050: 7065 6e64 735f 6f6e 5c27 7d29 223e 4465  pends_on\'})">De
-0016d060: 7065 6e64 7320 4f6e 3c2f 613e 3c2f 6c69  pends On</a></li
-0016d070: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016d080: 2020 203c 6c69 2075 692d 7372 6566 2d61     <li ui-sref-a
-0016d090: 6374 6976 653d 5c27 6163 7469 7665 5c27  ctive=\'active\'
-0016d0a0: 3e3c 6120 7569 2d73 7265 663d 2264 6274  ><a ui-sref="dbt
-0016d0b0: 2e6d 6163 726f 287b 5c27 235c 273a 205c  .macro({\'#\': \
-0016d0c0: 2763 6f64 655c 277d 2922 3e43 6f64 653c  'code\'})">Code<
-0016d0d0: 2f61 3e3c 2f6c 693e 5c6e 2020 2020 2020  /a></li>\n      
-0016d0e0: 2020 2020 2020 3c2f 756c 3e5c 6e20 2020        </ul>\n   
-0016d0f0: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
-0016d100: 203c 2f64 6976 3e5c 6e20 2020 203c 6469   </div>\n    <di
-0016d110: 7620 636c 6173 733d 2261 7070 2d64 6574  v class="app-det
-0016d120: 6169 6c73 223e 5c6e 2020 2020 2020 2020  ails">\n        
-0016d130: 3c64 6976 2063 6c61 7373 3d22 6170 702d  <div class="app-
-0016d140: 6672 616d 6520 6170 702d 7061 6422 3e5c  frame app-pad">\
-0016d150: 6e20 2020 2020 2020 2020 2020 203c 7365  n            <se
-0016d160: 6374 696f 6e20 636c 6173 733d 2273 6563  ction class="sec
-0016d170: 7469 6f6e 223e 5c6e 2020 2020 2020 2020  tion">\n        
-0016d180: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0016d190: 7373 3d22 7365 6374 696f 6e2d 7461 7267  ss="section-targ
-0016d1a0: 6574 2220 6964 3d22 6465 7363 7269 7074  et" id="descript
-0016d1b0: 696f 6e22 3e3c 2f64 6976 3e5c 6e20 2020  ion"></div>\n   
-0016d1c0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0016d1d0: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
-0016d1e0: 2d63 6f6e 7465 6e74 223e 5c6e 2020 2020  -content">\n    
-0016d1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d200: 3c68 363e 4465 7363 7269 7074 696f 6e3c  <h6>Description<
-0016d210: 2f68 363e 5c6e 2020 2020 2020 2020 2020  /h6>\n          
-0016d220: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0016d230: 6c61 7373 3d22 7061 6e65 6c22 3e5c 6e20  lass="panel">\n 
-0016d240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d250: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0016d260: 733d 2270 616e 656c 2d62 6f64 7922 3e5c  s="panel-body">\
-0016d270: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016d280: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0016d290: 7620 6e67 2d69 663d 226d 6163 726f 2e64  v ng-if="macro.d
-0016d2a0: 6573 6372 6970 7469 6f6e 2220 636c 6173  escription" clas
-0016d2b0: 733d 226d 6f64 656c 2d6d 6172 6b64 6f77  s="model-markdow
-0016d2c0: 6e22 206d 6172 6b65 643d 226d 6163 726f  n" marked="macro
-0016d2d0: 2e64 6573 6372 6970 7469 6f6e 223e 3c2f  .description"></
-0016d2e0: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
-0016d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d300: 2020 3c64 6976 206e 672d 6966 3d22 216d    <div ng-if="!m
-0016d310: 6163 726f 2e64 6573 6372 6970 7469 6f6e  acro.description
-0016d320: 223e 5468 6973 207b 7b20 6d61 6372 6f2e  ">This {{ macro.
-0016d330: 7265 736f 7572 6365 5f74 7970 6520 7d7d  resource_type }}
-0016d340: 2069 7320 6e6f 7420 6375 7272 656e 746c   is not currentl
-0016d350: 7920 646f 6375 6d65 6e74 6564 3c2f 6469  y documented</di
-0016d360: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
-0016d370: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-0016d380: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
-0016d390: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
-0016d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d3b0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-0016d3c0: 2020 2020 3c2f 7365 6374 696f 6e3e 5c6e      </section>\n
-0016d3d0: 5c6e 2020 2020 2020 2020 2020 2020 3c73  \n            <s
-0016d3e0: 6563 7469 6f6e 2063 6c61 7373 3d22 7365  ection class="se
-0016d3f0: 6374 696f 6e22 3e5c 6e20 2020 2020 2020  ction">\n       
-0016d400: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0016d410: 6173 733d 2273 6563 7469 6f6e 2d74 6172  ass="section-tar
-0016d420: 6765 7422 2069 643d 2261 7267 756d 656e  get" id="argumen
-0016d430: 7473 223e 3c2f 6469 763e 5c6e 2020 2020  ts"></div>\n    
-0016d440: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-0016d450: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
-0016d460: 636f 6e74 656e 7422 3e5c 6e20 2020 2020  content">\n     
-0016d470: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016d480: 6836 3e41 7267 756d 656e 7473 3c2f 6836  h6>Arguments</h6
-0016d490: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016d4a0: 2020 2020 2020 203c 6d61 6372 6f2d 6172         <macro-ar
-0016d4b0: 6775 6d65 6e74 7320 6d61 6372 6f3d 226d  guments macro="m
-0016d4c0: 6163 726f 223e 3c2f 6d61 6372 6f2d 6172  acro"></macro-ar
-0016d4d0: 6775 6d65 6e74 733e 5c6e 2020 2020 2020  guments>\n      
-0016d4e0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-0016d4f0: 5c6e 2020 2020 2020 2020 2020 2020 3c2f  \n            </
-0016d500: 7365 6374 696f 6e3e 5c6e 5c6e 2020 2020  section>\n\n    
-0016d510: 2020 2020 2020 2020 3c73 6563 7469 6f6e          <section
-0016d520: 2063 6c61 7373 3d22 7365 6374 696f 6e22   class="section"
-0016d530: 206e 672d 7368 6f77 203d 2022 7265 6665   ng-show = "refe
-0016d540: 7265 6e63 6573 4c65 6e67 7468 2021 3d20  rencesLength != 
-0016d550: 3022 3e5c 6e20 2020 2020 2020 2020 2020  0">\n           
-0016d560: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0016d570: 2273 6563 7469 6f6e 2d74 6172 6765 7422  "section-target"
-0016d580: 2069 643d 2272 6566 6572 656e 6365 645f   id="referenced_
-0016d590: 6279 223e 3c2f 6469 763e 5c6e 2020 2020  by"></div>\n    
-0016d5a0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-0016d5b0: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
-0016d5c0: 636f 6e74 656e 7422 3e5c 6e20 2020 2020  content">\n     
-0016d5d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016d5e0: 6836 3e52 6566 6572 656e 6365 6420 4279  h6>Referenced By
-0016d5f0: 3c2f 6836 3e5c 6e20 2020 2020 2020 2020  </h6>\n         
-0016d600: 2020 2020 2020 2020 2020 203c 7265 6665             <refe
-0016d610: 7265 6e63 652d 6c69 7374 2072 6566 6572  rence-list refer
-0016d620: 656e 6365 733d 2272 6566 6572 656e 6365  ences="reference
-0016d630: 7322 206e 6f64 653d 226d 6163 726f 2220  s" node="macro" 
-0016d640: 2f3e 5c6e 2020 2020 2020 2020 2020 2020  />\n            
-0016d650: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
-0016d660: 2020 2020 2020 2020 3c2f 7365 6374 696f          </sectio
-0016d670: 6e3e 5c6e 5c6e 2020 2020 2020 2020 2020  n>\n\n          
-0016d680: 2020 3c73 6563 7469 6f6e 2063 6c61 7373    <section class
-0016d690: 3d22 7365 6374 696f 6e22 206e 672d 7368  ="section" ng-sh
-0016d6a0: 6f77 203d 2022 7061 7265 6e74 734c 656e  ow = "parentsLen
-0016d6b0: 6774 6820 213d 2030 223e 5c6e 2020 2020  gth != 0">\n    
-0016d6c0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-0016d6d0: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
-0016d6e0: 7461 7267 6574 2220 6964 3d22 6465 7065  target" id="depe
-0016d6f0: 6e64 735f 6f6e 223e 3c2f 6469 763e 5c6e  nds_on"></div>\n
-0016d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d710: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
-0016d720: 696f 6e2d 636f 6e74 656e 7422 3e5c 6e20  ion-content">\n 
-0016d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016d740: 2020 203c 6836 3e44 6570 656e 6473 204f     <h6>Depends O
-0016d750: 6e3c 2f68 363e 5c6e 2020 2020 2020 2020  n</h6>\n        
-0016d760: 2020 2020 2020 2020 2020 2020 3c72 6566              <ref
-0016d770: 6572 656e 6365 2d6c 6973 7420 7265 6665  erence-list refe
-0016d780: 7265 6e63 6573 3d22 7061 7265 6e74 7322  rences="parents"
-0016d790: 206e 6f64 653d 226d 6163 726f 2220 2f3e   node="macro" />
-0016d7a0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0016d7b0: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
-0016d7c0: 2020 2020 2020 3c2f 7365 6374 696f 6e3e        </section>
-0016d7d0: 5c6e 5c6e 2020 2020 2020 2020 2020 2020  \n\n            
-0016d7e0: 3c73 6563 7469 6f6e 2063 6c61 7373 3d22  <section class="
-0016d7f0: 7365 6374 696f 6e22 3e5c 6e20 2020 2020  section">\n     
-0016d800: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0016d810: 636c 6173 733d 2273 6563 7469 6f6e 2d74  class="section-t
-0016d820: 6172 6765 7422 2069 643d 2263 6f64 6522  arget" id="code"
-0016d830: 3e3c 2f64 6976 3e5c 6e20 2020 2020 2020  ></div>\n       
-0016d840: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0016d850: 6173 733d 2273 6563 7469 6f6e 2d63 6f6e  ass="section-con
-0016d860: 7465 6e74 223e 5c6e 2020 2020 2020 2020  tent">\n        
-0016d870: 2020 2020 2020 2020 2020 2020 3c63 6f64              <cod
-0016d880: 652d 626c 6f63 6b20 7665 7273 696f 6e73  e-block versions
-0016d890: 3d22 7665 7273 696f 6e73 2220 6465 6661  ="versions" defa
-0016d8a0: 756c 743d 2264 6566 6175 6c74 5f76 6572  ult="default_ver
-0016d8b0: 7369 6f6e 2220 6c61 6e67 7561 6765 3d22  sion" language="
-0016d8c0: 6c61 6e67 7561 6765 223e 3c2f 636f 6465  language"></code
-0016d8d0: 2d62 6c6f 636b 3e5c 6e20 2020 2020 2020  -block>\n       
-0016d8e0: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-0016d8f0: 6e20 2020 2020 2020 2020 2020 203c 2f73  n            </s
-0016d900: 6563 7469 6f6e 3e5c 6e20 2020 2020 2020  ection>\n       
-0016d910: 203c 2f64 6976 3e5c 6e20 2020 203c 2f64   </div>\n    </d
-0016d920: 6976 3e5c 6e3c 2f64 6976 3e5c 6e27 297d  iv>\n</div>\n')}
-0016d930: 5d29 2c65 2e65 7870 6f72 7473 3d6e 7d2c  ]),e.exports=n},
-0016d940: 6675 6e63 7469 6f6e 2865 2c74 297b 7661  function(e,t){va
-0016d950: 7220 6e3d 222f 646f 6373 2f65 7870 6f73  r n="/docs/expos
-0016d960: 7572 652e 6874 6d6c 223b 7769 6e64 6f77  ure.html";window
-0016d970: 2e61 6e67 756c 6172 2e6d 6f64 756c 6528  .angular.module(
-0016d980: 226e 6722 292e 7275 6e28 5b22 2474 656d  "ng").run(["$tem
-0016d990: 706c 6174 6543 6163 6865 222c 6675 6e63  plateCache",func
-0016d9a0: 7469 6f6e 2865 297b 652e 7075 7428 6e2c  tion(e){e.put(n,
-0016d9b0: 273c 7374 796c 653e 5c6e 2f2a 2054 4f44  '<style>\n/* TOD
-0016d9c0: 4f20 2a2f 5c6e 2e73 6563 7469 6f6e 2d74  O */\n.section-t
-0016d9d0: 6172 6765 7420 7b5c 6e20 2020 2074 6f70  arget {\n    top
-0016d9e0: 3a20 2d38 656d 3b5c 6e7d 5c6e 5c6e 2e6e  : -8em;\n}\n\n.n
-0016d9f0: 6f66 6c65 7820 7b5c 6e20 2020 2066 6c65  oflex {\n    fle
-0016da00: 783a 2030 2030 2031 3630 7078 2021 696d  x: 0 0 160px !im
-0016da10: 706f 7274 616e 743b 5c6e 7d5c 6e5c 6e2e  portant;\n}\n\n.
-0016da20: 6869 6768 6c69 6768 7420 7b5c 6e20 2020  highlight {\n   
-0016da30: 2063 6f6c 6f72 3a20 2332 3432 3932 653b   color: #24292e;
-0016da40: 5c6e 2020 2020 6261 636b 6772 6f75 6e64  \n    background
-0016da50: 2d63 6f6c 6f72 3a20 7768 6974 653b 5c6e  -color: white;\n
-0016da60: 7d5c 6e5c 6e3c 2f73 7479 6c65 3e5c 6e5c  }\n\n</style>\n\
-0016da70: 6e3c 6469 7620 636c 6173 733d 5c27 6170  n<div class=\'ap
-0016da80: 702d 7363 726f 6c6c 5c27 3e5c 6e20 2020  p-scroll\'>\n   
-0016da90: 203c 6469 7620 636c 6173 733d 2261 7070   <div class="app
-0016daa0: 2d6c 696e 6b73 2061 7070 2d73 7469 636b  -links app-stick
-0016dab0: 7922 3e5c 6e20 2020 2020 2020 203c 6469  y">\n        <di
-0016dac0: 7620 636c 6173 733d 2261 7070 2d74 6974  v class="app-tit
-0016dad0: 6c65 223e 5c6e 2020 2020 2020 2020 2020  le">\n          
-0016dae0: 2020 3c64 6976 2063 6c61 7373 3d22 6170    <div class="ap
-0016daf0: 702d 6672 616d 6520 6170 702d 7061 6420  p-frame app-pad 
-0016db00: 6170 702d 666c 7573 682d 626f 7474 6f6d  app-flush-bottom
-0016db10: 223e 5c6e 5c6e 2020 2020 2020 2020 2020  ">\n\n          
-0016db20: 2020 2020 2020 3c68 313e 5c6e 2020 2020        <h1>\n    
-0016db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016db40: 3c73 7061 6e20 636c 6173 733d 2262 7265  <span class="bre
-0016db50: 616b 223e 7b7b 2065 7870 6f73 7572 652e  ak">{{ exposure.
-0016db60: 6c61 6265 6c20 7d7d 3c2f 7370 616e 3e5c  label }}</span>\
-0016db70: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016db80: 2020 2020 203c 736d 616c 6c3e 6578 706f       <small>expo
-0016db90: 7375 7265 3c2f 736d 616c 6c3e 5c6e 5c6e  sure</small>\n\n
-0016dba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016dbb0: 2020 2020 3c64 6976 2063 6c61 7373 3d5c      <div class=\
-0016dbc0: 2770 756c 6c2d 7269 6768 745c 2720 6e67  'pull-right\' ng
-0016dbd0: 2d73 686f 773d 2265 7870 6f73 7572 652e  -show="exposure.
-0016dbe0: 7572 6c22 3e5c 6e20 2020 2020 2020 2020  url">\n         
-0016dbf0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016dc00: 6120 636c 6173 733d 5c27 6274 6e20 7465  a class=\'btn te
-0016dc10: 7874 2d77 6869 7465 2062 746e 2d70 7269  xt-white btn-pri
-0016dc20: 6d61 7279 2062 746e 2d73 6d5c 2720 6e67  mary btn-sm\' ng
-0016dc30: 2d68 7265 663d 227b 7b20 6578 706f 7375  -href="{{ exposu
-0016dc40: 7265 2e75 726c 207d 7d22 2074 6172 6765  re.url }}" targe
-0016dc50: 743d 225f 626c 616e 6b22 3e56 6965 7720  t="_blank">View 
-0016dc60: 7468 6973 2065 7870 6f73 7572 653c 2f61  this exposure</a
-0016dc70: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016dc80: 2020 2020 2020 203c 2f64 6976 3e5c 6e5c         </div>\n\
-0016dc90: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016dca0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0016dcb0: 5c27 636c 6561 7266 6978 5c27 3e3c 2f64  \'clearfix\'></d
-0016dcc0: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
-0016dcd0: 2020 2020 203c 2f68 313e 5c6e 5c6e 2020       </h1>\n\n  
-0016dce0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-0016dcf0: 5c6e 2020 2020 2020 2020 3c2f 6469 763e  \n        </div>
-0016dd00: 5c6e 2020 2020 2020 2020 3c64 6976 2063  \n        <div c
-0016dd10: 6c61 7373 3d22 6170 702d 6672 616d 6520  lass="app-frame 
-0016dd20: 6170 702d 7061 642d 6822 3e5c 6e20 2020  app-pad-h">\n   
-0016dd30: 2020 2020 2020 2020 203c 756c 2063 6c61           <ul cla
-0016dd40: 7373 3d22 6e61 7620 6e61 762d 7461 6273  ss="nav nav-tabs
-0016dd50: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
-0016dd60: 2020 2020 3c6c 6920 7569 2d73 7265 662d      <li ui-sref-
-0016dd70: 6163 7469 7665 3d5c 2761 6374 6976 655c  active=\'active\
-0016dd80: 273e 3c61 2075 692d 7372 6566 3d22 6462  '><a ui-sref="db
-0016dd90: 742e 6578 706f 7375 7265 287b 5c27 235c  t.exposure({\'#\
-0016dda0: 273a 205c 2764 6574 6169 6c73 5c27 7d29  ': \'details\'})
-0016ddb0: 223e 4465 7461 696c 733c 2f61 3e3c 2f6c  ">Details</a></l
-0016ddc0: 693e 5c6e 2020 2020 2020 2020 2020 2020  i>\n            
-0016ddd0: 2020 2020 3c6c 6920 7569 2d73 7265 662d      <li ui-sref-
-0016dde0: 6163 7469 7665 3d5c 2761 6374 6976 655c  active=\'active\
-0016ddf0: 273e 3c61 2075 692d 7372 6566 3d22 6462  '><a ui-sref="db
-0016de00: 742e 6578 706f 7375 7265 287b 5c27 235c  t.exposure({\'#\
-0016de10: 273a 205c 2764 6573 6372 6970 7469 6f6e  ': \'description
-0016de20: 5c27 7d29 223e 4465 7363 7269 7074 696f  \'})">Descriptio
-0016de30: 6e3c 2f61 3e3c 2f6c 693e 5c6e 2020 2020  n</a></li>\n    
-0016de40: 2020 2020 2020 2020 2020 2020 3c6c 6920              <li 
-0016de50: 7569 2d73 7265 662d 6163 7469 7665 3d5c  ui-sref-active=\
-0016de60: 2761 6374 6976 655c 2720 6e67 2d73 686f  'active\' ng-sho
-0016de70: 7720 3d20 2270 6172 656e 7473 4c65 6e67  w = "parentsLeng
-0016de80: 7468 2021 3d20 3022 3e3c 6120 7569 2d73  th != 0"><a ui-s
-0016de90: 7265 663d 2264 6274 2e65 7870 6f73 7572  ref="dbt.exposur
-0016dea0: 6528 7b5c 2723 5c27 3a20 5c27 6465 7065  e({\'#\': \'depe
-0016deb0: 6e64 735f 6f6e 5c27 7d29 223e 4465 7065  nds_on\'})">Depe
-0016dec0: 6e64 7320 4f6e 3c2f 613e 3c2f 6c69 3e5c  nds On</a></li>\
-0016ded0: 6e20 2020 2020 2020 2020 2020 203c 2f75  n            </u
-0016dee0: 6c3e 5c6e 2020 2020 2020 2020 3c2f 6469  l>\n        </di
-0016def0: 763e 5c6e 2020 2020 3c2f 6469 763e 5c6e  v>\n    </div>\n
-0016df00: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0016df10: 6170 702d 6465 7461 696c 7322 3e5c 6e20  app-details">\n 
-0016df20: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0016df30: 733d 2261 7070 2d66 7261 6d65 2061 7070  s="app-frame app
-0016df40: 2d70 6164 223e 5c6e 5c6e 2020 2020 2020  -pad">\n\n      
-0016df50: 2020 2020 2020 3c73 6563 7469 6f6e 2063        <section c
-0016df60: 6c61 7373 3d22 7365 6374 696f 6e22 3e5c  lass="section">\
-0016df70: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016df80: 203c 6469 7620 636c 6173 733d 2273 6563   <div class="sec
-0016df90: 7469 6f6e 2d74 6172 6765 7422 2069 643d  tion-target" id=
-0016dfa0: 2264 6574 6169 6c73 223e 3c2f 6469 763e  "details"></div>
-0016dfb0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0016dfc0: 2020 3c74 6162 6c65 2d64 6574 6169 6c73    <table-details
-0016dfd0: 206d 6f64 656c 3d22 6578 706f 7375 7265   model="exposure
-0016dfe0: 2220 6578 7472 6173 3d22 6578 7472 615f  " extras="extra_
-0016dff0: 7461 626c 655f 6669 656c 6473 2220 2f3e  table_fields" />
-0016e000: 5c6e 2020 2020 2020 2020 2020 2020 3c2f  \n            </
-0016e010: 7365 6374 696f 6e3e 5c6e 5c6e 2020 2020  section>\n\n    
-0016e020: 2020 2020 2020 2020 3c73 6563 7469 6f6e          <section
-0016e030: 2063 6c61 7373 3d22 7365 6374 696f 6e22   class="section"
-0016e040: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016e050: 2020 203c 6469 7620 636c 6173 733d 2273     <div class="s
-0016e060: 6563 7469 6f6e 2d74 6172 6765 7422 2069  ection-target" i
-0016e070: 643d 2264 6573 6372 6970 7469 6f6e 223e  d="description">
-0016e080: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-0016e090: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-0016e0a0: 7373 3d22 7365 6374 696f 6e2d 636f 6e74  ss="section-cont
-0016e0b0: 656e 7422 3e5c 6e20 2020 2020 2020 2020  ent">\n         
-0016e0c0: 2020 2020 2020 2020 2020 203c 6836 3e44             <h6>D
-0016e0d0: 6573 6372 6970 7469 6f6e 3c2f 6836 3e5c  escription</h6>\
-0016e0e0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016e0f0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0016e100: 2270 616e 656c 223e 5c6e 2020 2020 2020  "panel">\n      
-0016e110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016e120: 2020 3c64 6976 2063 6c61 7373 3d22 7061    <div class="pa
-0016e130: 6e65 6c2d 626f 6479 223e 5c6e 2020 2020  nel-body">\n    
-0016e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016e150: 2020 2020 2020 2020 3c64 6976 206e 672d          <div ng-
-0016e160: 6966 3d22 6578 706f 7375 7265 2e64 6573  if="exposure.des
-0016e170: 6372 6970 7469 6f6e 2220 636c 6173 733d  cription" class=
-0016e180: 226d 6f64 656c 2d6d 6172 6b64 6f77 6e22  "model-markdown"
-0016e190: 206d 6172 6b65 643d 2265 7870 6f73 7572   marked="exposur
-0016e1a0: 652e 6465 7363 7269 7074 696f 6e22 3e3c  e.description"><
-0016e1b0: 2f64 6976 3e5c 6e20 2020 2020 2020 2020  /div>\n         
-0016e1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016e1d0: 2020 203c 6469 7620 6e67 2d69 663d 2221     <div ng-if="!
-0016e1e0: 6578 706f 7375 7265 2e64 6573 6372 6970  exposure.descrip
-0016e1f0: 7469 6f6e 223e 5468 6973 207b 7b20 6578  tion">This {{ ex
-0016e200: 706f 7375 7265 2e72 6573 6f75 7263 655f  posure.resource_
-0016e210: 7479 7065 207d 7d20 6973 206e 6f74 2063  type }} is not c
-0016e220: 7572 7265 6e74 6c79 2064 6f63 756d 656e  urrently documen
-0016e230: 7465 643c 2f64 6976 3e5c 6e20 2020 2020  ted</div>\n     
-0016e240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016e250: 2020 203c 2f64 6976 3e5c 6e20 2020 2020     </div>\n     
-0016e260: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016e270: 2f64 6976 3e5c 6e20 2020 2020 2020 2020  /div>\n         
-0016e280: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
-0016e290: 2020 2020 2020 2020 2020 203c 2f73 6563             </sec
-0016e2a0: 7469 6f6e 3e5c 6e5c 6e20 2020 2020 2020  tion>\n\n       
-0016e2b0: 2020 2020 203c 7365 6374 696f 6e20 636c       <section cl
-0016e2c0: 6173 733d 2273 6563 7469 6f6e 2220 6e67  ass="section" ng
-0016e2d0: 2d73 686f 7720 3d20 2270 6172 656e 7473  -show = "parents
-0016e2e0: 4c65 6e67 7468 2021 3d20 3022 3e5c 6e20  Length != 0">\n 
-0016e2f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016e300: 6469 7620 636c 6173 733d 2273 6563 7469  div class="secti
-0016e310: 6f6e 2d74 6172 6765 7422 2069 643d 2264  on-target" id="d
-0016e320: 6570 656e 6473 5f6f 6e22 3e3c 2f64 6976  epends_on"></div
-0016e330: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016e340: 2020 203c 6469 7620 636c 6173 733d 2273     <div class="s
-0016e350: 6563 7469 6f6e 2d63 6f6e 7465 6e74 223e  ection-content">
-0016e360: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0016e370: 2020 2020 2020 3c68 363e 4465 7065 6e64        <h6>Depend
-0016e380: 7320 4f6e 3c2f 6836 3e5c 6e20 2020 2020  s On</h6>\n     
-0016e390: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016e3a0: 7265 6665 7265 6e63 652d 6c69 7374 2072  reference-list r
-0016e3b0: 6566 6572 656e 6365 733d 2270 6172 656e  eferences="paren
-0016e3c0: 7473 2220 6e6f 6465 3d22 6578 706f 7375  ts" node="exposu
-0016e3d0: 7265 2220 2f3e 5c6e 2020 2020 2020 2020  re" />\n        
-0016e3e0: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
-0016e3f0: 2020 2020 2020 2020 2020 2020 3c2f 7365              </se
-0016e400: 6374 696f 6e3e 5c6e 5c6e 2020 2020 2020  ction>\n\n      
-0016e410: 2020 3c2f 6469 763e 5c6e 2020 2020 3c2f    </div>\n    </
-0016e420: 6469 763e 5c6e 3c2f 6469 763e 5c6e 2729  div>\n</div>\n')
-0016e430: 7d5d 292c 652e 6578 706f 7274 733d 6e7d  }]),e.exports=n}
-0016e440: 2c66 756e 6374 696f 6e28 652c 7429 7b76  ,function(e,t){v
-0016e450: 6172 206e 3d22 2f64 6f63 732f 6d65 7472  ar n="/docs/metr
-0016e460: 6963 2e68 746d 6c22 3b77 696e 646f 772e  ic.html";window.
-0016e470: 616e 6775 6c61 722e 6d6f 6475 6c65 2822  angular.module("
-0016e480: 6e67 2229 2e72 756e 285b 2224 7465 6d70  ng").run(["$temp
-0016e490: 6c61 7465 4361 6368 6522 2c66 756e 6374  lateCache",funct
-0016e4a0: 696f 6e28 6529 7b65 2e70 7574 286e 2c27  ion(e){e.put(n,'
-0016e4b0: 3c73 7479 6c65 3e5c 6e2f 2a20 544f 444f  <style>\n/* TODO
-0016e4c0: 202a 2f5c 6e2e 7365 6374 696f 6e2d 7461   */\n.section-ta
-0016e4d0: 7267 6574 207b 5c6e 2020 2020 746f 703a  rget {\n    top:
-0016e4e0: 202d 3865 6d3b 5c6e 7d5c 6e5c 6e2e 6e6f   -8em;\n}\n\n.no
-0016e4f0: 666c 6578 207b 5c6e 2020 2020 666c 6578  flex {\n    flex
-0016e500: 3a20 3020 3020 3136 3070 7820 2169 6d70  : 0 0 160px !imp
-0016e510: 6f72 7461 6e74 3b5c 6e7d 5c6e 5c6e 2e68  ortant;\n}\n\n.h
-0016e520: 6967 686c 6967 6874 207b 5c6e 2020 2020  ighlight {\n    
-0016e530: 636f 6c6f 723a 2023 3234 3239 3265 3b5c  color: #24292e;\
-0016e540: 6e20 2020 2062 6163 6b67 726f 756e 642d  n    background-
-0016e550: 636f 6c6f 723a 2077 6869 7465 3b5c 6e7d  color: white;\n}
-0016e560: 5c6e 5c6e 3c2f 7374 796c 653e 5c6e 5c6e  \n\n</style>\n\n
-0016e570: 3c64 6976 2063 6c61 7373 3d5c 2761 7070  <div class=\'app
-0016e580: 2d73 6372 6f6c 6c5c 273e 5c6e 2020 2020  -scroll\'>\n    
-0016e590: 3c64 6976 2063 6c61 7373 3d22 6170 702d  <div class="app-
-0016e5a0: 6c69 6e6b 7320 6170 702d 7374 6963 6b79  links app-sticky
-0016e5b0: 223e 5c6e 2020 2020 2020 2020 3c64 6976  ">\n        <div
-0016e5c0: 2063 6c61 7373 3d22 6170 702d 7469 746c   class="app-titl
-0016e5d0: 6522 3e5c 6e20 2020 2020 2020 2020 2020  e">\n           
-0016e5e0: 203c 6469 7620 636c 6173 733d 2261 7070   <div class="app
-0016e5f0: 2d66 7261 6d65 2061 7070 2d70 6164 2061  -frame app-pad a
-0016e600: 7070 2d66 6c75 7368 2d62 6f74 746f 6d22  pp-flush-bottom"
-0016e610: 3e5c 6e5c 6e20 2020 2020 2020 2020 2020  >\n\n           
-0016e620: 2020 2020 203c 6831 3e5c 6e20 2020 2020       <h1>\n     
-0016e630: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016e640: 7370 616e 2063 6c61 7373 3d22 6272 6561  span class="brea
-0016e650: 6b22 3e7b 7b20 6d65 7472 6963 2e6c 6162  k">{{ metric.lab
-0016e660: 656c 207d 7d3c 2f73 7061 6e3e 5c6e 2020  el }}</span>\n  
-0016e670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016e680: 2020 3c73 6d61 6c6c 3e6d 6574 7269 633c    <small>metric<
-0016e690: 2f73 6d61 6c6c 3e5c 6e5c 6e20 2020 2020  /small>\n\n     
-0016e6a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016e6b0: 6469 7620 636c 6173 733d 5c27 636c 6561  div class=\'clea
-0016e6c0: 7266 6978 5c27 3e3c 2f64 6976 3e5c 6e20  rfix\'></div>\n 
-0016e6d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016e6e0: 2f68 313e 5c6e 5c6e 2020 2020 2020 2020  /h1>\n\n        
-0016e6f0: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
-0016e700: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
-0016e710: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0016e720: 6170 702d 6672 616d 6520 6170 702d 7061  app-frame app-pa
-0016e730: 642d 6822 3e5c 6e20 2020 2020 2020 2020  d-h">\n         
-0016e740: 2020 203c 756c 2063 6c61 7373 3d22 6e61     <ul class="na
-0016e750: 7620 6e61 762d 7461 6273 223e 5c6e 2020  v nav-tabs">\n  
-0016e760: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
-0016e770: 6920 7569 2d73 7265 662d 6163 7469 7665  i ui-sref-active
-0016e780: 3d5c 2761 6374 6976 655c 273e 3c61 2075  =\'active\'><a u
-0016e790: 692d 7372 6566 3d22 6462 742e 6d65 7472  i-sref="dbt.metr
-0016e7a0: 6963 287b 5c27 235c 273a 205c 2764 6574  ic({\'#\': \'det
-0016e7b0: 6169 6c73 5c27 7d29 223e 4465 7461 696c  ails\'})">Detail
-0016e7c0: 733c 2f61 3e3c 2f6c 693e 5c6e 2020 2020  s</a></li>\n    
-0016e7d0: 2020 2020 2020 2020 2020 2020 3c6c 6920              <li 
-0016e7e0: 7569 2d73 7265 662d 6163 7469 7665 3d5c  ui-sref-active=\
-0016e7f0: 2761 6374 6976 655c 273e 3c61 2075 692d  'active\'><a ui-
-0016e800: 7372 6566 3d22 6462 742e 6d65 7472 6963  sref="dbt.metric
-0016e810: 287b 5c27 235c 273a 205c 2764 6573 6372  ({\'#\': \'descr
-0016e820: 6970 7469 6f6e 5c27 7d29 223e 4465 7363  iption\'})">Desc
-0016e830: 7269 7074 696f 6e3c 2f61 3e3c 2f6c 693e  ription</a></li>
-0016e840: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0016e850: 2020 3c6c 6920 7569 2d73 7265 662d 6163    <li ui-sref-ac
-0016e860: 7469 7665 3d5c 2761 6374 6976 655c 2720  tive=\'active\' 
-0016e870: 6e67 2d73 686f 7720 3d20 2270 6172 656e  ng-show = "paren
-0016e880: 7473 4c65 6e67 7468 2021 3d20 3022 3e3c  tsLength != 0"><
-0016e890: 6120 7569 2d73 7265 663d 2264 6274 2e6d  a ui-sref="dbt.m
-0016e8a0: 6574 7269 6328 7b5c 2723 5c27 3a20 5c27  etric({\'#\': \'
-0016e8b0: 6465 7065 6e64 735f 6f6e 5c27 7d29 223e  depends_on\'})">
-0016e8c0: 4465 7065 6e64 7320 4f6e 3c2f 613e 3c2f  Depends On</a></
-0016e8d0: 6c69 3e5c 6e20 2020 2020 2020 2020 2020  li>\n           
-0016e8e0: 203c 2f75 6c3e 5c6e 2020 2020 2020 2020   </ul>\n        
-0016e8f0: 3c2f 6469 763e 5c6e 2020 2020 3c2f 6469  </div>\n    </di
-0016e900: 763e 5c6e 2020 2020 3c64 6976 2063 6c61  v>\n    <div cla
-0016e910: 7373 3d22 6170 702d 6465 7461 696c 7322  ss="app-details"
-0016e920: 3e5c 6e20 2020 2020 2020 203c 6469 7620  >\n        <div 
-0016e930: 636c 6173 733d 2261 7070 2d66 7261 6d65  class="app-frame
-0016e940: 2061 7070 2d70 6164 223e 5c6e 5c6e 2020   app-pad">\n\n  
-0016e950: 2020 2020 2020 2020 2020 3c73 6563 7469            <secti
-0016e960: 6f6e 2063 6c61 7373 3d22 7365 6374 696f  on class="sectio
-0016e970: 6e22 3e5c 6e20 2020 2020 2020 2020 2020  n">\n           
-0016e980: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0016e990: 2273 6563 7469 6f6e 2d74 6172 6765 7422  "section-target"
-0016e9a0: 2069 643d 2264 6574 6169 6c73 223e 3c2f   id="details"></
-0016e9b0: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
-0016e9c0: 2020 2020 2020 3c74 6162 6c65 2d64 6574        <table-det
-0016e9d0: 6169 6c73 206d 6f64 656c 3d22 6d65 7472  ails model="metr
-0016e9e0: 6963 2220 6578 7472 6173 3d22 6578 7472  ic" extras="extr
-0016e9f0: 615f 7461 626c 655f 6669 656c 6473 2220  a_table_fields" 
-0016ea00: 2f3e 5c6e 2020 2020 2020 2020 2020 2020  />\n            
-0016ea10: 3c2f 7365 6374 696f 6e3e 5c6e 5c6e 2020  </section>\n\n  
-0016ea20: 2020 2020 2020 2020 2020 3c73 6563 7469            <secti
-0016ea30: 6f6e 2063 6c61 7373 3d22 7365 6374 696f  on class="sectio
-0016ea40: 6e22 3e5c 6e20 2020 2020 2020 2020 2020  n">\n           
-0016ea50: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-0016ea60: 2273 6563 7469 6f6e 2d74 6172 6765 7422  "section-target"
-0016ea70: 2069 643d 2264 6573 6372 6970 7469 6f6e   id="description
-0016ea80: 223e 3c2f 6469 763e 5c6e 2020 2020 2020  "></div>\n      
-0016ea90: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0016eaa0: 6c61 7373 3d22 7365 6374 696f 6e2d 636f  lass="section-co
-0016eab0: 6e74 656e 7422 3e5c 6e20 2020 2020 2020  ntent">\n       
-0016eac0: 2020 2020 2020 2020 2020 2020 203c 6836               <h6
-0016ead0: 3e44 6573 6372 6970 7469 6f6e 3c2f 6836  >Description</h6
-0016eae0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016eaf0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
-0016eb00: 733d 2270 616e 656c 223e 5c6e 2020 2020  s="panel">\n    
-0016eb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016eb20: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0016eb30: 7061 6e65 6c2d 626f 6479 223e 5c6e 2020  panel-body">\n  
-0016eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016eb50: 2020 2020 2020 2020 2020 3c64 6976 206e            <div n
-0016eb60: 672d 6966 3d22 6d65 7472 6963 2e64 6573  g-if="metric.des
-0016eb70: 6372 6970 7469 6f6e 2220 636c 6173 733d  cription" class=
-0016eb80: 226d 6f64 656c 2d6d 6172 6b64 6f77 6e22  "model-markdown"
-0016eb90: 206d 6172 6b65 643d 226d 6574 7269 632e   marked="metric.
-0016eba0: 6465 7363 7269 7074 696f 6e22 3e3c 2f64  description"></d
-0016ebb0: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
-0016ebc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016ebd0: 203c 6469 7620 6e67 2d69 663d 2221 6d65   <div ng-if="!me
-0016ebe0: 7472 6963 2e64 6573 6372 6970 7469 6f6e  tric.description
-0016ebf0: 223e 5468 6973 207b 7b20 6d65 7472 6963  ">This {{ metric
-0016ec00: 2e72 6573 6f75 7263 655f 7479 7065 207d  .resource_type }
-0016ec10: 7d20 6973 206e 6f74 2063 7572 7265 6e74  } is not current
-0016ec20: 6c79 2064 6f63 756d 656e 7465 643c 2f64  ly documented</d
-0016ec30: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
-0016ec40: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-0016ec50: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
-0016ec60: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-0016ec70: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016ec80: 203c 2f64 6976 3e5c 6e20 2020 2020 2020   </div>\n       
-0016ec90: 2020 2020 203c 2f73 6563 7469 6f6e 3e5c       </section>\
-0016eca0: 6e5c 6e20 2020 2020 2020 2020 2020 203c  n\n            <
-0016ecb0: 7365 6374 696f 6e20 636c 6173 733d 2273  section class="s
-0016ecc0: 6563 7469 6f6e 2220 6e67 2d73 686f 7720  ection" ng-show 
-0016ecd0: 3d20 2270 6172 656e 7473 4c65 6e67 7468  = "parentsLength
-0016ece0: 2021 3d20 3022 3e5c 6e20 2020 2020 2020   != 0">\n       
-0016ecf0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0016ed00: 6173 733d 2273 6563 7469 6f6e 2d74 6172  ass="section-tar
-0016ed10: 6765 7422 2069 643d 2264 6570 656e 6473  get" id="depends
-0016ed20: 5f6f 6e22 3e3c 2f64 6976 3e5c 6e20 2020  _on"></div>\n   
-0016ed30: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-0016ed40: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
-0016ed50: 2d63 6f6e 7465 6e74 223e 5c6e 2020 2020  -content">\n    
-0016ed60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016ed70: 3c68 363e 4465 7065 6e64 7320 4f6e 3c2f  <h6>Depends On</
-0016ed80: 6836 3e5c 6e20 2020 2020 2020 2020 2020  h6>\n           
-0016ed90: 2020 2020 2020 2020 203c 7265 6665 7265           <refere
-0016eda0: 6e63 652d 6c69 7374 2072 6566 6572 656e  nce-list referen
-0016edb0: 6365 733d 2270 6172 656e 7473 2220 6e6f  ces="parents" no
-0016edc0: 6465 3d22 6d65 7472 6963 2220 2f3e 5c6e  de="metric" />\n
-0016edd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016ede0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-0016edf0: 2020 2020 3c2f 7365 6374 696f 6e3e 5c6e      </section>\n
-0016ee00: 5c6e 2020 2020 2020 2020 3c2f 6469 763e  \n        </div>
-0016ee10: 5c6e 2020 2020 3c2f 6469 763e 5c6e 3c2f  \n    </div>\n</
-0016ee20: 6469 763e 5c6e 2729 7d5d 292c 652e 6578  div>\n')}]),e.ex
-0016ee30: 706f 7274 733d 6e7d 2c66 756e 6374 696f  ports=n},functio
-0016ee40: 6e28 652c 7429 7b76 6172 206e 3d22 2f64  n(e,t){var n="/d
-0016ee50: 6f63 732f 7365 6d61 6e74 6963 5f6d 6f64  ocs/semantic_mod
-0016ee60: 656c 2e68 746d 6c22 3b77 696e 646f 772e  el.html";window.
-0016ee70: 616e 6775 6c61 722e 6d6f 6475 6c65 2822  angular.module("
-0016ee80: 6e67 2229 2e72 756e 285b 2224 7465 6d70  ng").run(["$temp
-0016ee90: 6c61 7465 4361 6368 6522 2c66 756e 6374  lateCache",funct
-0016eea0: 696f 6e28 6529 7b65 2e70 7574 286e 2c27  ion(e){e.put(n,'
-0016eeb0: 3c73 7479 6c65 3e5c 6e2f 2a20 544f 444f  <style>\n/* TODO
-0016eec0: 202a 2f5c 6e2e 7365 6374 696f 6e2d 7461   */\n.section-ta
-0016eed0: 7267 6574 207b 5c6e 2020 2020 746f 703a  rget {\n    top:
-0016eee0: 202d 3865 6d3b 5c6e 7d5c 6e5c 6e2e 6e6f   -8em;\n}\n\n.no
-0016eef0: 666c 6578 207b 5c6e 2020 2020 666c 6578  flex {\n    flex
-0016ef00: 3a20 3020 3020 3136 3070 7820 2169 6d70  : 0 0 160px !imp
-0016ef10: 6f72 7461 6e74 3b5c 6e7d 5c6e 5c6e 2e68  ortant;\n}\n\n.h
-0016ef20: 6967 686c 6967 6874 207b 5c6e 2020 2020  ighlight {\n    
-0016ef30: 636f 6c6f 723a 2023 3234 3239 3265 3b5c  color: #24292e;\
-0016ef40: 6e20 2020 2062 6163 6b67 726f 756e 642d  n    background-
-0016ef50: 636f 6c6f 723a 2077 6869 7465 3b5c 6e7d  color: white;\n}
-0016ef60: 5c6e 5c6e 3c2f 7374 796c 653e 5c6e 5c6e  \n\n</style>\n\n
-0016ef70: 3c64 6976 2063 6c61 7373 3d5c 2761 7070  <div class=\'app
-0016ef80: 2d73 6372 6f6c 6c5c 273e 5c6e 2020 2020  -scroll\'>\n    
-0016ef90: 3c64 6976 2063 6c61 7373 3d22 6170 702d  <div class="app-
-0016efa0: 6c69 6e6b 7320 6170 702d 7374 6963 6b79  links app-sticky
-0016efb0: 223e 5c6e 2020 2020 2020 2020 3c64 6976  ">\n        <div
-0016efc0: 2063 6c61 7373 3d22 6170 702d 7469 746c   class="app-titl
-0016efd0: 6522 3e5c 6e20 2020 2020 2020 2020 2020  e">\n           
-0016efe0: 203c 6469 7620 636c 6173 733d 2261 7070   <div class="app
-0016eff0: 2d66 7261 6d65 2061 7070 2d70 6164 2061  -frame app-pad a
-0016f000: 7070 2d66 6c75 7368 2d62 6f74 746f 6d22  pp-flush-bottom"
-0016f010: 3e5c 6e5c 6e20 2020 2020 2020 2020 2020  >\n\n           
-0016f020: 2020 2020 203c 6831 3e5c 6e20 2020 2020       <h1>\n     
-0016f030: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016f040: 7370 616e 2063 6c61 7373 3d22 6272 6561  span class="brea
-0016f050: 6b22 3e7b 7b20 7365 6d61 6e74 6963 5f6d  k">{{ semantic_m
-0016f060: 6f64 656c 2e6e 616d 6520 7d7d 3c2f 7370  odel.name }}</sp
-0016f070: 616e 3e5c 6e20 2020 2020 2020 2020 2020  an>\n           
-0016f080: 2020 2020 2020 2020 203c 736d 616c 6c3e           <small>
-0016f090: 7365 6d61 6e74 6963 5f6d 6f64 656c 3c2f  semantic_model</
-0016f0a0: 736d 616c 6c3e 5c6e 5c6e 2020 2020 2020  small>\n\n      
-0016f0b0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0016f0c0: 6976 2063 6c61 7373 3d5c 2763 6c65 6172  iv class=\'clear
-0016f0d0: 6669 785c 273e 3c2f 6469 763e 5c6e 2020  fix\'></div>\n  
-0016f0e0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-0016f0f0: 6831 3e5c 6e5c 6e20 2020 2020 2020 2020  h1>\n\n         
-0016f100: 2020 203c 2f64 6976 3e5c 6e20 2020 2020     </div>\n     
-0016f110: 2020 203c 2f64 6976 3e5c 6e20 2020 2020     </div>\n     
-0016f120: 2020 203c 6469 7620 636c 6173 733d 2261     <div class="a
-0016f130: 7070 2d66 7261 6d65 2061 7070 2d70 6164  pp-frame app-pad
-0016f140: 2d68 223e 5c6e 2020 2020 2020 2020 2020  -h">\n          
-0016f150: 2020 3c75 6c20 636c 6173 733d 226e 6176    <ul class="nav
-0016f160: 206e 6176 2d74 6162 7322 3e5c 6e20 2020   nav-tabs">\n   
-0016f170: 2020 2020 2020 2020 2020 2020 203c 6c69               <li
-0016f180: 2075 692d 7372 6566 2d61 6374 6976 653d   ui-sref-active=
-0016f190: 5c27 6163 7469 7665 5c27 3e3c 6120 7569  \'active\'><a ui
-0016f1a0: 2d73 7265 663d 2264 6274 2e73 656d 616e  -sref="dbt.seman
-0016f1b0: 7469 635f 6d6f 6465 6c28 7b5c 2723 5c27  tic_model({\'#\'
-0016f1c0: 3a20 5c27 6465 7461 696c 735c 277d 2922  : \'details\'})"
-0016f1d0: 3e44 6574 6169 6c73 3c2f 613e 3c2f 6c69  >Details</a></li
-0016f1e0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016f1f0: 2020 203c 6c69 2075 692d 7372 6566 2d61     <li ui-sref-a
-0016f200: 6374 6976 653d 5c27 6163 7469 7665 5c27  ctive=\'active\'
-0016f210: 3e3c 6120 7569 2d73 7265 663d 2264 6274  ><a ui-sref="dbt
-0016f220: 2e73 656d 616e 7469 635f 6d6f 6465 6c28  .semantic_model(
-0016f230: 7b5c 2723 5c27 3a20 5c27 6465 7363 7269  {\'#\': \'descri
-0016f240: 7074 696f 6e5c 277d 2922 3e44 6573 6372  ption\'})">Descr
-0016f250: 6970 7469 6f6e 3c2f 613e 3c2f 6c69 3e5c  iption</a></li>\
-0016f260: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-0016f270: 203c 6c69 2075 692d 7372 6566 2d61 6374   <li ui-sref-act
-0016f280: 6976 653d 5c27 6163 7469 7665 5c27 206e  ive=\'active\' n
-0016f290: 672d 7368 6f77 203d 2022 7061 7265 6e74  g-show = "parent
-0016f2a0: 734c 656e 6774 6820 213d 2030 223e 3c61  sLength != 0"><a
-0016f2b0: 2075 692d 7372 6566 3d22 6462 742e 7365   ui-sref="dbt.se
-0016f2c0: 6d61 6e74 6963 5f6d 6f64 656c 287b 5c27  mantic_model({\'
-0016f2d0: 235c 273a 205c 2764 6570 656e 6473 5f6f  #\': \'depends_o
-0016f2e0: 6e5c 277d 2922 3e44 6570 656e 6473 204f  n\'})">Depends O
-0016f2f0: 6e3c 2f61 3e3c 2f6c 693e 5c6e 2020 2020  n</a></li>\n    
-0016f300: 2020 2020 2020 2020 3c2f 756c 3e5c 6e20          </ul>\n 
-0016f310: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
-0016f320: 2020 203c 2f64 6976 3e5c 6e20 2020 203c     </div>\n    <
-0016f330: 6469 7620 636c 6173 733d 2261 7070 2d64  div class="app-d
-0016f340: 6574 6169 6c73 223e 5c6e 2020 2020 2020  etails">\n      
-0016f350: 2020 3c64 6976 2063 6c61 7373 3d22 6170    <div class="ap
-0016f360: 702d 6672 616d 6520 6170 702d 7061 6422  p-frame app-pad"
-0016f370: 3e5c 6e5c 6e20 2020 2020 2020 2020 2020  >\n\n           
-0016f380: 203c 7365 6374 696f 6e20 636c 6173 733d   <section class=
-0016f390: 2273 6563 7469 6f6e 223e 5c6e 2020 2020  "section">\n    
-0016f3a0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-0016f3b0: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
-0016f3c0: 7461 7267 6574 2220 6964 3d22 6465 7461  target" id="deta
-0016f3d0: 696c 7322 3e3c 2f64 6976 3e5c 6e20 2020  ils"></div>\n   
-0016f3e0: 2020 2020 2020 2020 2020 2020 203c 7461               <ta
-0016f3f0: 626c 652d 6465 7461 696c 7320 6d6f 6465  ble-details mode
-0016f400: 6c3d 2273 656d 616e 7469 635f 6d6f 6465  l="semantic_mode
-0016f410: 6c22 2065 7874 7261 733d 2265 7874 7261  l" extras="extra
-0016f420: 5f74 6162 6c65 5f66 6965 6c64 7322 202f  _table_fields" /
-0016f430: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
-0016f440: 2f73 6563 7469 6f6e 3e5c 6e5c 6e20 2020  /section>\n\n   
-0016f450: 2020 2020 2020 2020 203c 7365 6374 696f           <sectio
-0016f460: 6e20 636c 6173 733d 2273 6563 7469 6f6e  n class="section
-0016f470: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
-0016f480: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-0016f490: 7365 6374 696f 6e2d 7461 7267 6574 2220  section-target" 
-0016f4a0: 6964 3d22 6465 7363 7269 7074 696f 6e22  id="description"
-0016f4b0: 3e3c 2f64 6976 3e5c 6e20 2020 2020 2020  ></div>\n       
-0016f4c0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0016f4d0: 6173 733d 2273 6563 7469 6f6e 2d63 6f6e  ass="section-con
-0016f4e0: 7465 6e74 223e 5c6e 2020 2020 2020 2020  tent">\n        
-0016f4f0: 2020 2020 2020 2020 2020 2020 3c68 363e              <h6>
-0016f500: 4465 7363 7269 7074 696f 6e3c 2f68 363e  Description</h6>
-0016f510: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0016f520: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-0016f530: 3d22 7061 6e65 6c22 3e5c 6e20 2020 2020  ="panel">\n     
-0016f540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016f550: 2020 203c 6469 7620 636c 6173 733d 2270     <div class="p
-0016f560: 616e 656c 2d62 6f64 7922 3e5c 6e20 2020  anel-body">\n   
-0016f570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016f580: 2020 2020 2020 2020 203c 6469 7620 6e67           <div ng
-0016f590: 2d69 663d 2273 656d 616e 7469 635f 6d6f  -if="semantic_mo
-0016f5a0: 6465 6c2e 6465 7363 7269 7074 696f 6e22  del.description"
-0016f5b0: 2063 6c61 7373 3d22 6d6f 6465 6c2d 6d61   class="model-ma
-0016f5c0: 726b 646f 776e 2220 6d61 726b 6564 3d22  rkdown" marked="
-0016f5d0: 7365 6d61 6e74 6963 5f6d 6f64 656c 2e64  semantic_model.d
-0016f5e0: 6573 6372 6970 7469 6f6e 223e 3c2f 6469  escription"></di
-0016f5f0: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
-0016f600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016f610: 3c64 6976 206e 672d 6966 3d22 2173 656d  <div ng-if="!sem
-0016f620: 616e 7469 635f 6d6f 6465 6c2e 6465 7363  antic_model.desc
-0016f630: 7269 7074 696f 6e22 3e54 6869 7320 7b7b  ription">This {{
-0016f640: 2073 656d 616e 7469 635f 6d6f 6465 6c2e   semantic_model.
-0016f650: 7265 736f 7572 6365 5f74 7970 6520 7d7d  resource_type }}
-0016f660: 2069 7320 6e6f 7420 6375 7272 656e 746c   is not currentl
-0016f670: 7920 646f 6375 6d65 6e74 6564 3c2f 6469  y documented</di
-0016f680: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
-0016f690: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-0016f6a0: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
-0016f6b0: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
-0016f6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016f6d0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-0016f6e0: 2020 2020 3c2f 7365 6374 696f 6e3e 5c6e      </section>\n
-0016f6f0: 5c6e 2020 2020 2020 2020 2020 2020 3c73  \n            <s
-0016f700: 6563 7469 6f6e 2063 6c61 7373 3d22 7365  ection class="se
-0016f710: 6374 696f 6e22 206e 672d 7368 6f77 203d  ction" ng-show =
-0016f720: 2022 7365 6d61 6e74 6963 5f6d 6f64 656c   "semantic_model
-0016f730: 2e65 6e74 6974 6965 732e 6c65 6e67 7468  .entities.length
-0016f740: 2021 3d20 3022 3e5c 6e20 2020 2020 2020   != 0">\n       
-0016f750: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-0016f760: 6173 733d 2273 6563 7469 6f6e 2d74 6172  ass="section-tar
-0016f770: 6765 7422 2069 643d 2265 6e74 6974 6965  get" id="entitie
-0016f780: 7322 3e3c 2f64 6976 3e5c 6e20 2020 2020  s"></div>\n     
-0016f790: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-0016f7a0: 636c 6173 733d 2273 6563 7469 6f6e 2d63  class="section-c
-0016f7b0: 6f6e 7465 6e74 223e 5c6e 2020 2020 2020  ontent">\n      
-0016f7c0: 2020 2020 2020 2020 2020 2020 2020 3c68                <h
-0016f7d0: 363e 456e 7469 7469 6573 3c2f 6836 3e5c  6>Entities</h6>\
-0016f7e0: 6e5c 6e20 2020 2020 2020 2020 2020 2020  n\n             
-0016f7f0: 2020 203c 6469 7620 636c 6173 733d 2270     <div class="p
-0016f800: 616e 656c 223e 5c6e 2020 2020 2020 2020  anel">\n        
-0016f810: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-0016f820: 2063 6c61 7373 3d22 6465 7461 696c 2d67   class="detail-g
-0016f830: 726f 7570 2220 7374 796c 653d 2270 6164  roup" style="pad
-0016f840: 6469 6e67 2d62 6f74 746f 6d3a 2030 223e  ding-bottom: 0">
-0016f850: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0016f860: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0016f870: 6c61 7373 3d22 6465 7461 696c 2d62 6f64  lass="detail-bod
-0016f880: 7922 2073 7479 6c65 3d22 7061 6464 696e  y" style="paddin
-0016f890: 672d 6c65 6674 3a20 3022 3e5c 6e20 2020  g-left: 0">\n   
-0016f8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016f8b0: 2020 2020 2020 2020 203c 646c 2063 6c61           <dl cla
-0016f8c0: 7373 3d22 6465 7461 696c 2220 6e67 2d73  ss="detail" ng-s
-0016f8d0: 7479 6c65 3d22 7b5c 2770 6164 6469 6e67  tyle="{\'padding
-0016f8e0: 2d6c 6566 745c 273a 2024 696e 6465 7820  -left\': $index 
-0016f8f0: 3d3d 2030 203f 2030 203a 205c 2761 7574  == 0 ? 0 : \'aut
-0016f900: 6f5c 277d 225c 6e20 2020 2020 2020 2020  o\'}"\n         
-0016f910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016f920: 2020 2020 2020 206e 672d 7265 7065 6174         ng-repeat
-0016f930: 3d22 656e 7469 7479 2069 6e20 7365 6d61  ="entity in sema
-0016f940: 6e74 6963 5f6d 6f64 656c 2e65 6e74 6974  ntic_model.entit
-0016f950: 6965 7322 3e5c 6e20 2020 2020 2020 2020  ies">\n         
-0016f960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016f970: 2020 2020 2020 203c 6474 2063 6c61 7373         <dt class
-0016f980: 3d22 6465 7461 696c 2d6c 6162 656c 223e  ="detail-label">
-0016f990: 4e61 6d65 3c2f 6474 3e5c 6e20 2020 2020  Name</dt>\n     
-0016f9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016f9b0: 2020 2020 2020 2020 2020 203c 6464 2063             <dd c
-0016f9c0: 6c61 7373 3d22 6465 7461 696c 2d76 616c  lass="detail-val
-0016f9d0: 7565 2220 6e67 2d69 663d 2265 6e74 6974  ue" ng-if="entit
-0016f9e0: 792e 6e61 6d65 223e 7b7b 2065 6e74 6974  y.name">{{ entit
-0016f9f0: 792e 6e61 6d65 207d 7d3c 2f64 643e 5c6e  y.name }}</dd>\n
-0016fa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016fa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016fa20: 3c64 6420 636c 6173 733d 2264 6574 6169  <dd class="detai
-0016fa30: 6c2d 7661 6c75 6522 206e 672d 6966 3d22  l-value" ng-if="
-0016fa40: 2165 6e74 6974 792e 6e61 6d65 223e 4e6f  !entity.name">No
-0016fa50: 6e65 3c2f 6464 3e5c 6e20 2020 2020 2020  ne</dd>\n       
-0016fa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016fa70: 2020 2020 2020 2020 203c 6474 2063 6c61           <dt cla
-0016fa80: 7373 3d22 6465 7461 696c 2d6c 6162 656c  ss="detail-label
-0016fa90: 223e 5479 7065 3c2f 6474 3e5c 6e20 2020  ">Type</dt>\n   
-0016faa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016fab0: 2020 2020 2020 2020 2020 2020 203c 6464               <dd
-0016fac0: 2063 6c61 7373 3d22 6465 7461 696c 2d76   class="detail-v
-0016fad0: 616c 7565 2220 6e67 2d69 663d 2265 6e74  alue" ng-if="ent
-0016fae0: 6974 792e 7479 7065 223e 7b7b 2065 6e74  ity.type">{{ ent
-0016faf0: 6974 792e 7479 7065 207d 7d3c 2f64 643e  ity.type }}</dd>
-0016fb00: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0016fb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016fb20: 2020 3c64 6420 636c 6173 733d 2264 6574    <dd class="det
-0016fb30: 6169 6c2d 7661 6c75 6522 206e 672d 6966  ail-value" ng-if
-0016fb40: 3d22 2165 6e74 6974 792e 7479 7065 223e  ="!entity.type">
-0016fb50: 4e6f 6e65 3c2f 6464 3e5c 6e20 2020 2020  None</dd>\n     
-0016fb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016fb70: 2020 2020 2020 2020 2020 203c 6474 2063             <dt c
-0016fb80: 6c61 7373 3d22 6465 7461 696c 2d6c 6162  lass="detail-lab
-0016fb90: 656c 223e 4578 7072 6573 7369 6f6e 3c2f  el">Expression</
-0016fba0: 6474 3e5c 6e20 2020 2020 2020 2020 2020  dt>\n           
-0016fbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016fbc0: 2020 2020 203c 6464 2063 6c61 7373 3d22       <dd class="
-0016fbd0: 6465 7461 696c 2d76 616c 7565 2220 6e67  detail-value" ng
-0016fbe0: 2d69 663d 2265 6e74 6974 792e 6578 7072  -if="entity.expr
-0016fbf0: 223e 7b7b 2065 6e74 6974 792e 6578 7072  ">{{ entity.expr
-0016fc00: 207d 7d3c 2f64 643e 5c6e 2020 2020 2020   }}</dd>\n      
-0016fc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016fc20: 2020 2020 2020 2020 2020 3c64 6420 636c            <dd cl
-0016fc30: 6173 733d 2264 6574 6169 6c2d 7661 6c75  ass="detail-valu
-0016fc40: 6522 206e 672d 6966 3d22 2165 6e74 6974  e" ng-if="!entit
-0016fc50: 792e 6578 7072 223e 4e6f 6e65 3c2f 6464  y.expr">None</dd
-0016fc60: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-0016fc70: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0016fc80: 2f64 6c3e 5c6e 2020 2020 2020 2020 2020  /dl>\n          
-0016fc90: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-0016fca0: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
-0016fcb0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-0016fcc0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-0016fcd0: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
-0016fce0: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
-0016fcf0: 2020 2020 2020 3c2f 7365 6374 696f 6e3e        </section>
-0016fd00: 5c6e 5c6e 2020 2020 2020 2020 2020 2020  \n\n            
-0016fd10: 3c73 6563 7469 6f6e 2063 6c61 7373 3d22  <section class="
-0016fd20: 7365 6374 696f 6e22 206e 672d 7368 6f77  section" ng-show
-0016fd30: 203d 2022 7061 7265 6e74 734c 656e 6774   = "parentsLengt
-0016fd40: 6820 213d 2030 223e 5c6e 2020 2020 2020  h != 0">\n      
-0016fd50: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-0016fd60: 6c61 7373 3d22 7365 6374 696f 6e2d 7461  lass="section-ta
-0016fd70: 7267 6574 2220 6964 3d22 6465 7065 6e64  rget" id="depend
-0016fd80: 735f 6f6e 223e 3c2f 6469 763e 5c6e 2020  s_on"></div>\n  
-0016fd90: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-0016fda0: 6976 2063 6c61 7373 3d22 7365 6374 696f  iv class="sectio
-0016fdb0: 6e2d 636f 6e74 656e 7422 3e5c 6e20 2020  n-content">\n   
-0016fdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0016fdd0: 203c 6836 3e44 6570 656e 6473 204f 6e3c   <h6>Depends On<
-0016fde0: 2f68 363e 5c6e 2020 2020 2020 2020 2020  /h6>\n          
-0016fdf0: 2020 2020 2020 2020 2020 3c72 6566 6572            <refer
-0016fe00: 656e 6365 2d6c 6973 7420 7265 6665 7265  ence-list refere
-0016fe10: 6e63 6573 3d22 7061 7265 6e74 7322 206e  nces="parents" n
-0016fe20: 6f64 653d 2273 656d 616e 7469 635f 6d6f  ode="semantic_mo
-0016fe30: 6465 6c22 202f 3e5c 6e20 2020 2020 2020  del" />\n       
-0016fe40: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
-0016fe50: 6e20 2020 2020 2020 2020 2020 203c 2f73  n            </s
-0016fe60: 6563 7469 6f6e 3e5c 6e5c 6e20 2020 2020  ection>\n\n     
-0016fe70: 2020 203c 2f64 6976 3e5c 6e20 2020 203c     </div>\n    <
-0016fe80: 2f64 6976 3e5c 6e3c 2f64 6976 3e5c 6e27  /div>\n</div>\n'
-0016fe90: 297d 5d29 2c65 2e65 7870 6f72 7473 3d6e  )}]),e.exports=n
-0016fea0: 7d2c 6675 6e63 7469 6f6e 2865 2c74 297b  },function(e,t){
-0016feb0: 7661 7220 6e3d 222f 646f 6373 2f6f 7065  var n="/docs/ope
-0016fec0: 7261 7469 6f6e 2e68 746d 6c22 3b77 696e  ration.html";win
-0016fed0: 646f 772e 616e 6775 6c61 722e 6d6f 6475  dow.angular.modu
-0016fee0: 6c65 2822 6e67 2229 2e72 756e 285b 2224  le("ng").run(["$
-0016fef0: 7465 6d70 6c61 7465 4361 6368 6522 2c66  templateCache",f
-0016ff00: 756e 6374 696f 6e28 6529 7b65 2e70 7574  unction(e){e.put
-0016ff10: 286e 2c27 3c73 7479 6c65 3e5c 6e2f 2a20  (n,'<style>\n/* 
-0016ff20: 544f 444f 202a 2f5c 6e2e 7365 6374 696f  TODO */\n.sectio
-0016ff30: 6e2d 7461 7267 6574 207b 5c6e 2020 2020  n-target {\n    
-0016ff40: 746f 703a 202d 3865 6d3b 5c6e 7d5c 6e5c  top: -8em;\n}\n\
-0016ff50: 6e2e 6e6f 666c 6578 207b 5c6e 2020 2020  n.noflex {\n    
-0016ff60: 666c 6578 3a20 3020 3020 3136 3070 7820  flex: 0 0 160px 
-0016ff70: 2169 6d70 6f72 7461 6e74 3b5c 6e7d 5c6e  !important;\n}\n
-0016ff80: 5c6e 2e68 6967 686c 6967 6874 207b 5c6e  \n.highlight {\n
-0016ff90: 2020 2020 636f 6c6f 723a 2023 3234 3239      color: #2429
-0016ffa0: 3265 3b5c 6e20 2020 2062 6163 6b67 726f  2e;\n    backgro
-0016ffb0: 756e 642d 636f 6c6f 723a 2077 6869 7465  und-color: white
-0016ffc0: 3b5c 6e7d 5c6e 5c6e 3c2f 7374 796c 653e  ;\n}\n\n</style>
-0016ffd0: 5c6e 5c6e 3c64 6976 2063 6c61 7373 3d5c  \n\n<div class=\
-0016ffe0: 2761 7070 2d73 6372 6f6c 6c5c 273e 5c6e  'app-scroll\'>\n
-0016fff0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00170000: 6170 702d 6c69 6e6b 7320 6170 702d 7374  app-links app-st
-00170010: 6963 6b79 223e 5c6e 2020 2020 2020 2020  icky">\n        
-00170020: 3c64 6976 2063 6c61 7373 3d22 6170 702d  <div class="app-
-00170030: 7469 746c 6522 3e5c 6e20 2020 2020 2020  title">\n       
-00170040: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00170050: 2261 7070 2d66 7261 6d65 2061 7070 2d70  "app-frame app-p
-00170060: 6164 2061 7070 2d66 6c75 7368 2d62 6f74  ad app-flush-bot
-00170070: 746f 6d22 3e5c 6e20 2020 2020 2020 2020  tom">\n         
-00170080: 2020 2020 2020 203c 6831 3e5c 6e20 2020         <h1>\n   
-00170090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001700a0: 203c 7370 616e 2063 6c61 7373 3d22 6272   <span class="br
-001700b0: 6561 6b22 3e7b 7b20 6d6f 6465 6c2e 6e61  eak">{{ model.na
-001700c0: 6d65 207d 7d3c 2f73 7061 6e3e 5c6e 2020  me }}</span>\n  
-001700d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001700e0: 2020 3c73 6d61 6c6c 3e6f 7065 7261 7469    <small>operati
-001700f0: 6f6e 3c2f 736d 616c 6c3e 5c6e 2020 2020  on</small>\n    
-00170100: 2020 2020 2020 2020 2020 2020 3c2f 6831              </h1
-00170110: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
-00170120: 2f64 6976 3e5c 6e20 2020 2020 2020 203c  /div>\n        <
-00170130: 2f64 6976 3e5c 6e20 2020 2020 2020 203c  /div>\n        <
-00170140: 6469 7620 636c 6173 733d 2261 7070 2d66  div class="app-f
-00170150: 7261 6d65 2061 7070 2d70 6164 2d68 223e  rame app-pad-h">
-00170160: 5c6e 2020 2020 2020 2020 2020 2020 3c75  \n            <u
-00170170: 6c20 636c 6173 733d 226e 6176 206e 6176  l class="nav nav
-00170180: 2d74 6162 7322 3e5c 6e20 2020 2020 2020  -tabs">\n       
-00170190: 2020 2020 2020 2020 203c 6c69 2075 692d           <li ui-
-001701a0: 7372 6566 2d61 6374 6976 653d 5c27 6163  sref-active=\'ac
-001701b0: 7469 7665 5c27 3e3c 6120 7569 2d73 7265  tive\'><a ui-sre
-001701c0: 663d 2264 6274 2e6f 7065 7261 7469 6f6e  f="dbt.operation
-001701d0: 287b 5c27 235c 273a 205c 2764 6573 6372  ({\'#\': \'descr
-001701e0: 6970 7469 6f6e 5c27 7d29 223e 4465 7363  iption\'})">Desc
-001701f0: 7269 7074 696f 6e3c 2f61 3e3c 2f6c 693e  ription</a></li>
-00170200: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
-00170210: 2020 3c6c 6920 7569 2d73 7265 662d 6163    <li ui-sref-ac
-00170220: 7469 7665 3d5c 2761 6374 6976 655c 2720  tive=\'active\' 
-00170230: 6e67 2d73 686f 7720 3d20 2270 6172 656e  ng-show = "paren
-00170240: 7473 4c65 6e67 7468 2021 3d20 3022 3e3c  tsLength != 0"><
-00170250: 6120 7569 2d73 7265 663d 2264 6274 2e6f  a ui-sref="dbt.o
-00170260: 7065 7261 7469 6f6e 287b 5c27 235c 273a  peration({\'#\':
-00170270: 205c 2764 6570 656e 6473 5f6f 6e5c 277d   \'depends_on\'}
-00170280: 2922 3e44 6570 656e 6473 204f 6e3c 2f61  )">Depends On</a
-00170290: 3e3c 2f6c 693e 5c6e 2020 2020 2020 2020  ></li>\n        
-001702a0: 2020 2020 2020 2020 3c6c 6920 7569 2d73          <li ui-s
-001702b0: 7265 662d 6163 7469 7665 3d5c 2761 6374  ref-active=\'act
-001702c0: 6976 655c 273e 3c61 2075 692d 7372 6566  ive\'><a ui-sref
-001702d0: 3d22 6462 742e 6f70 6572 6174 696f 6e28  ="dbt.operation(
-001702e0: 7b5c 2723 5c27 3a20 5c27 636f 6465 5c27  {\'#\': \'code\'
-001702f0: 7d29 223e 5351 4c3c 2f61 3e3c 2f6c 693e  })">SQL</a></li>
-00170300: 5c6e 2020 2020 2020 2020 2020 2020 3c2f  \n            </
-00170310: 756c 3e5c 6e20 2020 2020 2020 203c 2f64  ul>\n        </d
-00170320: 6976 3e5c 6e20 2020 203c 2f64 6976 3e5c  iv>\n    </div>\
-00170330: 6e20 2020 203c 6469 7620 636c 6173 733d  n    <div class=
-00170340: 2261 7070 2d64 6574 6169 6c73 223e 5c6e  "app-details">\n
-00170350: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-00170360: 7373 3d22 6170 702d 6672 616d 6520 6170  ss="app-frame ap
-00170370: 702d 7061 6422 3e5c 6e20 2020 2020 2020  p-pad">\n       
-00170380: 2020 2020 203c 7365 6374 696f 6e20 636c       <section cl
-00170390: 6173 733d 2273 6563 7469 6f6e 223e 5c6e  ass="section">\n
-001703a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001703b0: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
-001703c0: 696f 6e2d 7461 7267 6574 2220 6964 3d22  ion-target" id="
-001703d0: 6465 7363 7269 7074 696f 6e22 3e3c 2f64  description"></d
-001703e0: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
-001703f0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00170400: 2273 6563 7469 6f6e 2d63 6f6e 7465 6e74  "section-content
-00170410: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
-00170420: 2020 2020 2020 2020 3c68 363e 4465 7363          <h6>Desc
-00170430: 7269 7074 696f 6e3c 2f68 363e 5c6e 2020  ription</h6>\n  
-00170440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00170450: 2020 3c64 6976 2063 6c61 7373 3d22 7061    <div class="pa
-00170460: 6e65 6c22 3e5c 6e20 2020 2020 2020 2020  nel">\n         
-00170470: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00170480: 6469 7620 636c 6173 733d 2270 616e 656c  div class="panel
-00170490: 2d62 6f64 7922 3e5c 6e20 2020 2020 2020  -body">\n       
-001704a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001704b0: 2020 2020 203c 6469 7620 6e67 2d69 663d       <div ng-if=
-001704c0: 226d 6f64 656c 2e64 6573 6372 6970 7469  "model.descripti
-001704d0: 6f6e 2220 636c 6173 733d 226d 6f64 656c  on" class="model
-001704e0: 2d6d 6172 6b64 6f77 6e22 206d 6172 6b65  -markdown" marke
-001704f0: 643d 226d 6f64 656c 2e64 6573 6372 6970  d="model.descrip
-00170500: 7469 6f6e 223e 3c2f 6469 763e 5c6e 2020  tion"></div>\n  
-00170510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00170520: 2020 2020 2020 2020 2020 3c64 6976 206e            <div n
-00170530: 672d 6966 3d22 216d 6f64 656c 2e64 6573  g-if="!model.des
-00170540: 6372 6970 7469 6f6e 223e 5468 6973 207b  cription">This {
-00170550: 7b20 6d6f 6465 6c2e 7265 736f 7572 6365  { model.resource
-00170560: 5f74 7970 6520 7d7d 2069 7320 6e6f 7420  _type }} is not 
-00170570: 6375 7272 656e 746c 7920 646f 6375 6d65  currently docume
-00170580: 6e74 6564 3c2f 6469 763e 5c6e 2020 2020  nted</div>\n    
-00170590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001705a0: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
+00167c90: 2020 2020 2020 2020 2020 3c2f 7461 626c            </tabl
+00167ca0: 653e 5c6e 2020 2020 2020 2020 2020 2020  e>\n            
+00167cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167cc0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
+00167cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167ce0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
+00167cf0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00167d00: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
+00167d10: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
+00167d20: 2020 2020 2020 2020 3c2f 7365 6374 696f          </sectio
+00167d30: 6e3e 5c6e 2020 2020 2020 2020 3c2f 6469  n>\n        </di
+00167d40: 763e 5c6e 2020 2020 3c2f 6469 763e 5c6e  v>\n    </div>\n
+00167d50: 3c2f 6469 763e 5c6e 2729 7d5d 292c 652e  </div>\n')}]),e.
+00167d60: 6578 706f 7274 733d 6e7d 2c66 756e 6374  exports=n},funct
+00167d70: 696f 6e28 652c 7429 7b76 6172 206e 3d22  ion(e,t){var n="
+00167d80: 2f64 6f63 732f 6d6f 6465 6c2e 6874 6d6c  /docs/model.html
+00167d90: 223b 7769 6e64 6f77 2e61 6e67 756c 6172  ";window.angular
+00167da0: 2e6d 6f64 756c 6528 226e 6722 292e 7275  .module("ng").ru
+00167db0: 6e28 5b22 2474 656d 706c 6174 6543 6163  n(["$templateCac
+00167dc0: 6865 222c 6675 6e63 7469 6f6e 2865 297b  he",function(e){
+00167dd0: 652e 7075 7428 6e2c 273c 7374 796c 653e  e.put(n,'<style>
+00167de0: 5c6e 2f2a 2054 4f44 4f20 2a2f 5c6e 2e73  \n/* TODO */\n.s
+00167df0: 6563 7469 6f6e 2d74 6172 6765 7420 7b5c  ection-target {\
+00167e00: 6e20 2020 2074 6f70 3a20 2d38 656d 3b5c  n    top: -8em;\
+00167e10: 6e7d 5c6e 5c6e 2e6e 6f66 6c65 7820 7b5c  n}\n\n.noflex {\
+00167e20: 6e20 2020 2066 6c65 783a 2030 2030 2031  n    flex: 0 0 1
+00167e30: 3630 7078 2021 696d 706f 7274 616e 743b  60px !important;
+00167e40: 5c6e 7d5c 6e5c 6e2e 6869 6768 6c69 6768  \n}\n\n.highligh
+00167e50: 7420 7b5c 6e20 2020 2063 6f6c 6f72 3a20  t {\n    color: 
+00167e60: 2332 3432 3932 653b 5c6e 2020 2020 6261  #24292e;\n    ba
+00167e70: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a20  ckground-color: 
+00167e80: 7768 6974 653b 5c6e 7d5c 6e5c 6e3c 2f73  white;\n}\n\n</s
+00167e90: 7479 6c65 3e5c 6e5c 6e3c 6469 7620 636c  tyle>\n\n<div cl
+00167ea0: 6173 733d 5c27 6170 702d 7363 726f 6c6c  ass=\'app-scroll
+00167eb0: 5c27 3e5c 6e20 2020 203c 6469 7620 636c  \'>\n    <div cl
+00167ec0: 6173 733d 2261 7070 2d6c 696e 6b73 2061  ass="app-links a
+00167ed0: 7070 2d73 7469 636b 7922 3e5c 6e20 2020  pp-sticky">\n   
+00167ee0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00167ef0: 2261 7070 2d74 6974 6c65 223e 5c6e 2020  "app-title">\n  
+00167f00: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00167f10: 6c61 7373 3d22 6170 702d 6672 616d 6520  lass="app-frame 
+00167f20: 6170 702d 7061 6420 6170 702d 666c 7573  app-pad app-flus
+00167f30: 682d 626f 7474 6f6d 223e 5c6e 2020 2020  h-bottom">\n    
+00167f40: 2020 2020 2020 2020 2020 2020 3c68 3120              <h1 
+00167f50: 6e67 2d69 663d 226d 6f64 656c 2e64 6f63  ng-if="model.doc
+00167f60: 732e 7368 6f77 203d 3d3d 2066 616c 7365  s.show === false
+00167f70: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
+00167f80: 2020 2020 2020 2020 3c73 6d61 6c6c 2063          <small c
+00167f90: 6c61 7373 3d5c 2774 6578 742d 626f 6c64  lass=\'text-bold
+00167fa0: 2074 6578 742d 7269 6768 745c 273e 5c6e   text-right\'>\n
+00167fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00167fc0: 2020 2020 2020 2020 3c69 2064 6174 612d          <i data-
+00167fd0: 6963 6f6e 3d22 6579 6522 3e3c 2f69 3e5c  icon="eye"></i>\
+00167fe0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00167ff0: 2020 2020 2020 2020 2054 6869 7320 6d6f           This mo
+00168000: 6465 6c20 6973 2068 6964 6465 6e5c 6e20  del is hidden\n 
+00168010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00168020: 2020 203c 2f73 6d61 6c6c 3e5c 6e20 2020     </small>\n   
+00168030: 2020 2020 2020 2020 2020 2020 203c 2f68               </h
+00168040: 313e 5c6e 2020 2020 2020 2020 2020 2020  1>\n            
+00168050: 2020 2020 3c68 313e 5c6e 2020 2020 2020      <h1>\n      
+00168060: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+00168070: 7061 6e20 636c 6173 733d 2262 7265 616b  pan class="break
+00168080: 223e 7b7b 206d 6f64 656c 2e6e 616d 6520  ">{{ model.name 
+00168090: 7d7d 3c2f 7370 616e 3e5c 6e20 2020 2020  }}</span>\n     
+001680a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+001680b0: 736d 616c 6c3e 7b7b 206d 6f64 656c 2e63  small>{{ model.c
+001680c0: 6f6e 6669 672e 6d61 7465 7269 616c 697a  onfig.materializ
+001680d0: 6564 207d 7d3c 2f73 6d61 6c6c 3e5c 6e20  ed }}</small>\n 
+001680e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+001680f0: 2f68 313e 5c6e 2020 2020 2020 2020 2020  /h1>\n          
+00168100: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
+00168110: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
+00168120: 2020 3c64 6976 2063 6c61 7373 3d22 6170    <div class="ap
+00168130: 702d 6672 616d 6520 6170 702d 7061 642d  p-frame app-pad-
+00168140: 6822 3e5c 6e20 2020 2020 2020 2020 2020  h">\n           
+00168150: 203c 756c 2063 6c61 7373 3d22 6e61 7620   <ul class="nav 
+00168160: 6e61 762d 7461 6273 223e 5c6e 2020 2020  nav-tabs">\n    
+00168170: 2020 2020 2020 2020 2020 2020 3c6c 6920              <li 
+00168180: 7569 2d73 7265 662d 6163 7469 7665 3d5c  ui-sref-active=\
+00168190: 2761 6374 6976 655c 273e 3c61 2075 692d  'active\'><a ui-
+001681a0: 7372 6566 3d22 6462 742e 6d6f 6465 6c28  sref="dbt.model(
+001681b0: 7b5c 2723 5c27 3a20 5c27 6465 7461 696c  {\'#\': \'detail
+001681c0: 735c 277d 2922 3e44 6574 6169 6c73 3c2f  s\'})">Details</
+001681d0: 613e 3c2f 6c69 3e5c 6e20 2020 2020 2020  a></li>\n       
+001681e0: 2020 2020 2020 2020 203c 6c69 2075 692d           <li ui-
+001681f0: 7372 6566 2d61 6374 6976 653d 5c27 6163  sref-active=\'ac
+00168200: 7469 7665 5c27 3e3c 6120 7569 2d73 7265  tive\'><a ui-sre
+00168210: 663d 2264 6274 2e6d 6f64 656c 287b 5c27  f="dbt.model({\'
+00168220: 235c 273a 205c 2764 6573 6372 6970 7469  #\': \'descripti
+00168230: 6f6e 5c27 7d29 223e 4465 7363 7269 7074  on\'})">Descript
+00168240: 696f 6e3c 2f61 3e3c 2f6c 693e 5c6e 2020  ion</a></li>\n  
+00168250: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
+00168260: 6920 7569 2d73 7265 662d 6163 7469 7665  i ui-sref-active
+00168270: 3d5c 2761 6374 6976 655c 273e 3c61 2075  =\'active\'><a u
+00168280: 692d 7372 6566 3d22 6462 742e 6d6f 6465  i-sref="dbt.mode
+00168290: 6c28 7b5c 2723 5c27 3a20 5c27 636f 6c75  l({\'#\': \'colu
+001682a0: 6d6e 735c 277d 2922 3e43 6f6c 756d 6e73  mns\'})">Columns
+001682b0: 3c2f 613e 3c2f 6c69 3e5c 6e20 2020 2020  </a></li>\n     
+001682c0: 2020 2020 2020 2020 2020 203c 6c69 2075             <li u
+001682d0: 692d 7372 6566 2d61 6374 6976 653d 5c27  i-sref-active=\'
+001682e0: 6163 7469 7665 5c27 206e 672d 7368 6f77  active\' ng-show
+001682f0: 203d 2022 7265 6665 7265 6e63 6573 4c65   = "referencesLe
+00168300: 6e67 7468 2021 3d20 3022 3e3c 6120 7569  ngth != 0"><a ui
+00168310: 2d73 7265 663d 2264 6274 2e6d 6f64 656c  -sref="dbt.model
+00168320: 287b 5c27 235c 273a 205c 2772 6566 6572  ({\'#\': \'refer
+00168330: 656e 6365 645f 6279 5c27 7d29 223e 5265  enced_by\'})">Re
+00168340: 6665 7265 6e63 6564 2042 793c 2f61 3e3c  ferenced By</a><
+00168350: 2f6c 693e 5c6e 2020 2020 2020 2020 2020  /li>\n          
+00168360: 2020 2020 2020 3c6c 6920 7569 2d73 7265        <li ui-sre
+00168370: 662d 6163 7469 7665 3d5c 2761 6374 6976  f-active=\'activ
+00168380: 655c 2720 6e67 2d73 686f 7720 3d20 2270  e\' ng-show = "p
+00168390: 6172 656e 7473 4c65 6e67 7468 2021 3d20  arentsLength != 
+001683a0: 3022 3e3c 6120 7569 2d73 7265 663d 2264  0"><a ui-sref="d
+001683b0: 6274 2e6d 6f64 656c 287b 5c27 235c 273a  bt.model({\'#\':
+001683c0: 205c 2764 6570 656e 6473 5f6f 6e5c 277d   \'depends_on\'}
+001683d0: 2922 3e44 6570 656e 6473 204f 6e3c 2f61  )">Depends On</a
+001683e0: 3e3c 2f6c 693e 5c6e 2020 2020 2020 2020  ></li>\n        
+001683f0: 2020 2020 2020 2020 3c6c 6920 7569 2d73          <li ui-s
+00168400: 7265 662d 6163 7469 7665 3d5c 2761 6374  ref-active=\'act
+00168410: 6976 655c 273e 3c61 2075 692d 7372 6566  ive\'><a ui-sref
+00168420: 3d22 6462 742e 6d6f 6465 6c28 7b5c 2723  ="dbt.model({\'#
+00168430: 5c27 3a20 5c27 636f 6465 5c27 7d29 223e  \': \'code\'})">
+00168440: 436f 6465 3c2f 613e 3c2f 6c69 3e5c 6e20  Code</a></li>\n 
+00168450: 2020 2020 2020 2020 2020 203c 2f75 6c3e             </ul>
+00168460: 5c6e 2020 2020 2020 2020 3c2f 6469 763e  \n        </div>
+00168470: 5c6e 2020 2020 3c2f 6469 763e 5c6e 2020  \n    </div>\n  
+00168480: 2020 3c64 6976 2063 6c61 7373 3d22 6170    <div class="ap
+00168490: 702d 6465 7461 696c 7322 3e5c 6e20 2020  p-details">\n   
+001684a0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+001684b0: 2261 7070 2d66 7261 6d65 2061 7070 2d70  "app-frame app-p
+001684c0: 6164 223e 5c6e 2020 2020 2020 2020 2020  ad">\n          
+001684d0: 2020 3c73 6563 7469 6f6e 2063 6c61 7373    <section class
+001684e0: 3d22 7365 6374 696f 6e22 3e5c 6e20 2020  ="section">\n   
+001684f0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00168500: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
+00168510: 2d74 6172 6765 7422 2069 643d 2264 6574  -target" id="det
+00168520: 6169 6c73 223e 3c2f 6469 763e 5c6e 2020  ails"></div>\n  
+00168530: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
+00168540: 6162 6c65 2d64 6574 6169 6c73 206d 6f64  able-details mod
+00168550: 656c 3d22 6d6f 6465 6c22 3e3c 2f74 6162  el="model"></tab
+00168560: 6c65 2d64 6574 6169 6c73 3e5c 6e20 2020  le-details>\n   
+00168570: 2020 2020 2020 2020 203c 2f73 6563 7469           </secti
+00168580: 6f6e 3e5c 6e5c 6e20 2020 2020 2020 2020  on>\n\n         
+00168590: 2020 203c 7365 6374 696f 6e20 636c 6173     <section clas
+001685a0: 733d 2273 6563 7469 6f6e 223e 5c6e 2020  s="section">\n  
+001685b0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+001685c0: 6976 2063 6c61 7373 3d22 7365 6374 696f  iv class="sectio
+001685d0: 6e2d 7461 7267 6574 2220 6964 3d22 6465  n-target" id="de
+001685e0: 7363 7269 7074 696f 6e22 3e3c 2f64 6976  scription"></div
+001685f0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+00168600: 2020 203c 6469 7620 636c 6173 733d 2273     <div class="s
+00168610: 6563 7469 6f6e 2d63 6f6e 7465 6e74 223e  ection-content">
+00168620: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00168630: 2020 2020 2020 3c68 363e 4465 7363 7269        <h6>Descri
+00168640: 7074 696f 6e3c 2f68 363e 5c6e 2020 2020  ption</h6>\n    
+00168650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00168660: 3c64 6976 2063 6c61 7373 3d22 7061 6e65  <div class="pane
+00168670: 6c22 3e5c 6e20 2020 2020 2020 2020 2020  l">\n           
+00168680: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00168690: 7620 636c 6173 733d 2270 616e 656c 2d62  v class="panel-b
+001686a0: 6f64 7922 3e5c 6e20 2020 2020 2020 2020  ody">\n         
+001686b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001686c0: 2020 203c 6469 7620 6e67 2d69 663d 226d     <div ng-if="m
+001686d0: 6f64 656c 2e64 6573 6372 6970 7469 6f6e  odel.description
+001686e0: 2220 636c 6173 733d 226d 6f64 656c 2d6d  " class="model-m
+001686f0: 6172 6b64 6f77 6e22 206d 6172 6b65 643d  arkdown" marked=
+00168700: 226d 6f64 656c 2e64 6573 6372 6970 7469  "model.descripti
+00168710: 6f6e 223e 3c2f 6469 763e 5c6e 2020 2020  on"></div>\n    
+00168720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00168730: 2020 2020 2020 2020 3c64 6976 206e 672d          <div ng-
+00168740: 6966 3d22 216d 6f64 656c 2e64 6573 6372  if="!model.descr
+00168750: 6970 7469 6f6e 223e 5468 6973 207b 7b20  iption">This {{ 
+00168760: 6d6f 6465 6c2e 7265 736f 7572 6365 5f74  model.resource_t
+00168770: 7970 6520 7d7d 2069 7320 6e6f 7420 6375  ype }} is not cu
+00168780: 7272 656e 746c 7920 646f 6375 6d65 6e74  rrently document
+00168790: 6564 3c2f 6469 763e 5c6e 2020 2020 2020  ed</div>\n      
+001687a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001687b0: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
+001687c0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+001687d0: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
+001687e0: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
+001687f0: 2020 2020 2020 2020 2020 3c2f 7365 6374            </sect
+00168800: 696f 6e3e 5c6e 5c6e 2020 2020 2020 2020  ion>\n\n        
+00168810: 2020 2020 3c73 6563 7469 6f6e 2063 6c61      <section cla
+00168820: 7373 3d22 7365 6374 696f 6e22 3e5c 6e20  ss="section">\n 
+00168830: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00168840: 6469 7620 636c 6173 733d 2273 6563 7469  div class="secti
+00168850: 6f6e 2d74 6172 6765 7422 2069 643d 2263  on-target" id="c
+00168860: 6f6c 756d 6e73 223e 3c2f 6469 763e 5c6e  olumns"></div>\n
+00168870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00168880: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
+00168890: 696f 6e2d 636f 6e74 656e 7422 3e5c 6e20  ion-content">\n 
+001688a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001688b0: 2020 203c 6836 3e43 6f6c 756d 6e73 3c2f     <h6>Columns</
+001688c0: 6836 3e5c 6e20 2020 2020 2020 2020 2020  h6>\n           
+001688d0: 2020 2020 2020 2020 203c 636f 6c75 6d6e           <column
+001688e0: 2d64 6574 6169 6c73 206d 6f64 656c 3d22  -details model="
+001688f0: 6d6f 6465 6c22 202f 3e5c 6e20 2020 2020  model" />\n     
+00168900: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00168910: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
+00168920: 2f73 6563 7469 6f6e 3e5c 6e5c 6e20 2020  /section>\n\n   
+00168930: 2020 2020 2020 2020 203c 7365 6374 696f           <sectio
+00168940: 6e20 636c 6173 733d 2273 6563 7469 6f6e  n class="section
+00168950: 2220 6e67 2d73 686f 7720 3d20 2272 6566  " ng-show = "ref
+00168960: 6572 656e 6365 734c 656e 6774 6820 213d  erencesLength !=
+00168970: 2030 223e 5c6e 2020 2020 2020 2020 2020   0">\n          
+00168980: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00168990: 3d22 7365 6374 696f 6e2d 7461 7267 6574  ="section-target
+001689a0: 2220 6964 3d22 7265 6665 7265 6e63 6564  " id="referenced
+001689b0: 5f62 7922 3e3c 2f64 6976 3e5c 6e20 2020  _by"></div>\n   
+001689c0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+001689d0: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
+001689e0: 2d63 6f6e 7465 6e74 223e 5c6e 2020 2020  -content">\n    
+001689f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00168a00: 3c68 363e 5265 6665 7265 6e63 6564 2042  <h6>Referenced B
+00168a10: 793c 2f68 363e 5c6e 2020 2020 2020 2020  y</h6>\n        
+00168a20: 2020 2020 2020 2020 2020 2020 3c72 6566              <ref
+00168a30: 6572 656e 6365 2d6c 6973 7420 7265 6665  erence-list refe
+00168a40: 7265 6e63 6573 3d22 7265 6665 7265 6e63  rences="referenc
+00168a50: 6573 2220 6e6f 6465 3d22 6d6f 6465 6c22  es" node="model"
+00168a60: 202f 3e5c 6e20 2020 2020 2020 2020 2020   />\n           
+00168a70: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
+00168a80: 2020 2020 2020 2020 203c 2f73 6563 7469           </secti
+00168a90: 6f6e 3e5c 6e5c 6e20 2020 2020 2020 2020  on>\n\n         
+00168aa0: 2020 203c 7365 6374 696f 6e20 636c 6173     <section clas
+00168ab0: 733d 2273 6563 7469 6f6e 2220 6e67 2d73  s="section" ng-s
+00168ac0: 686f 7720 3d20 2270 6172 656e 7473 4c65  how = "parentsLe
+00168ad0: 6e67 7468 2021 3d20 3022 3e5c 6e20 2020  ngth != 0">\n   
+00168ae0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00168af0: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
+00168b00: 2d74 6172 6765 7422 2069 643d 2264 6570  -target" id="dep
+00168b10: 656e 6473 5f6f 6e22 3e3c 2f64 6976 3e5c  ends_on"></div>\
+00168b20: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00168b30: 203c 6469 7620 636c 6173 733d 2273 6563   <div class="sec
+00168b40: 7469 6f6e 2d63 6f6e 7465 6e74 223e 5c6e  tion-content">\n
+00168b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00168b60: 2020 2020 3c68 363e 4465 7065 6e64 7320      <h6>Depends 
+00168b70: 4f6e 3c2f 6836 3e5c 6e20 2020 2020 2020  On</h6>\n       
+00168b80: 2020 2020 2020 2020 2020 2020 203c 7265               <re
+00168b90: 6665 7265 6e63 652d 6c69 7374 2072 6566  ference-list ref
+00168ba0: 6572 656e 6365 733d 2270 6172 656e 7473  erences="parents
+00168bb0: 2220 6e6f 6465 3d22 6d6f 6465 6c22 202f  " node="model" /
+00168bc0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+00168bd0: 2020 203c 2f64 6976 3e5c 6e20 2020 2020     </div>\n     
+00168be0: 2020 2020 2020 203c 2f73 6563 7469 6f6e         </section
+00168bf0: 3e5c 6e5c 6e20 2020 2020 2020 2020 2020  >\n\n           
+00168c00: 203c 7365 6374 696f 6e20 636c 6173 733d   <section class=
+00168c10: 2273 6563 7469 6f6e 223e 5c6e 2020 2020  "section">\n    
+00168c20: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00168c30: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
+00168c40: 7461 7267 6574 2220 6964 3d22 636f 6465  target" id="code
+00168c50: 223e 3c2f 6469 763e 5c6e 2020 2020 2020  "></div>\n      
+00168c60: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00168c70: 6c61 7373 3d22 7365 6374 696f 6e2d 636f  lass="section-co
+00168c80: 6e74 656e 7422 3e5c 6e20 2020 2020 2020  ntent">\n       
+00168c90: 2020 2020 2020 2020 2020 2020 203c 636f               <co
+00168ca0: 6465 2d62 6c6f 636b 2076 6572 7369 6f6e  de-block version
+00168cb0: 733d 2276 6572 7369 6f6e 7322 2064 6566  s="versions" def
+00168cc0: 6175 6c74 3d22 6465 6661 756c 745f 7665  ault="default_ve
+00168cd0: 7273 696f 6e22 206c 616e 6775 6167 653d  rsion" language=
+00168ce0: 226c 616e 6775 6167 6522 3e3c 2f63 6f64  "language"></cod
+00168cf0: 652d 626c 6f63 6b3e 5c6e 2020 2020 2020  e-block>\n      
+00168d00: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00168d10: 5c6e 2020 2020 2020 2020 2020 2020 3c2f  \n            </
+00168d20: 7365 6374 696f 6e3e 5c6e 2020 2020 2020  section>\n      
+00168d30: 2020 3c2f 6469 763e 5c6e 2020 2020 3c2f    </div>\n    </
+00168d40: 6469 763e 5c6e 3c2f 6469 763e 5c6e 2729  div>\n</div>\n')
+00168d50: 7d5d 292c 652e 6578 706f 7274 733d 6e7d  }]),e.exports=n}
+00168d60: 2c66 756e 6374 696f 6e28 652c 7429 7b76  ,function(e,t){v
+00168d70: 6172 206e 3d22 2f64 6f63 732f 736e 6170  ar n="/docs/snap
+00168d80: 7368 6f74 2e68 746d 6c22 3b77 696e 646f  shot.html";windo
+00168d90: 772e 616e 6775 6c61 722e 6d6f 6475 6c65  w.angular.module
+00168da0: 2822 6e67 2229 2e72 756e 285b 2224 7465  ("ng").run(["$te
+00168db0: 6d70 6c61 7465 4361 6368 6522 2c66 756e  mplateCache",fun
+00168dc0: 6374 696f 6e28 6529 7b65 2e70 7574 286e  ction(e){e.put(n
+00168dd0: 2c27 3c73 7479 6c65 3e5c 6e2f 2a20 544f  ,'<style>\n/* TO
+00168de0: 444f 202a 2f5c 6e2e 7365 6374 696f 6e2d  DO */\n.section-
+00168df0: 7461 7267 6574 207b 5c6e 2020 2020 746f  target {\n    to
+00168e00: 703a 202d 3865 6d3b 5c6e 7d5c 6e5c 6e2e  p: -8em;\n}\n\n.
+00168e10: 6e6f 666c 6578 207b 5c6e 2020 2020 666c  noflex {\n    fl
+00168e20: 6578 3a20 3020 3020 3136 3070 7820 2169  ex: 0 0 160px !i
+00168e30: 6d70 6f72 7461 6e74 3b5c 6e7d 5c6e 5c6e  mportant;\n}\n\n
+00168e40: 2e68 6967 686c 6967 6874 207b 5c6e 2020  .highlight {\n  
+00168e50: 2020 636f 6c6f 723a 2023 3234 3239 3265    color: #24292e
+00168e60: 3b5c 6e20 2020 2062 6163 6b67 726f 756e  ;\n    backgroun
+00168e70: 642d 636f 6c6f 723a 2077 6869 7465 3b5c  d-color: white;\
+00168e80: 6e7d 5c6e 5c6e 3c2f 7374 796c 653e 5c6e  n}\n\n</style>\n
+00168e90: 5c6e 3c64 6976 2063 6c61 7373 3d5c 2761  \n<div class=\'a
+00168ea0: 7070 2d73 6372 6f6c 6c5c 273e 5c6e 2020  pp-scroll\'>\n  
+00168eb0: 2020 3c64 6976 2063 6c61 7373 3d22 6170    <div class="ap
+00168ec0: 702d 6c69 6e6b 7320 6170 702d 7374 6963  p-links app-stic
+00168ed0: 6b79 223e 5c6e 2020 2020 2020 2020 3c64  ky">\n        <d
+00168ee0: 6976 2063 6c61 7373 3d22 6170 702d 7469  iv class="app-ti
+00168ef0: 746c 6522 3e5c 6e20 2020 2020 2020 2020  tle">\n         
+00168f00: 2020 203c 6469 7620 636c 6173 733d 2261     <div class="a
+00168f10: 7070 2d66 7261 6d65 2061 7070 2d70 6164  pp-frame app-pad
+00168f20: 2061 7070 2d66 6c75 7368 2d62 6f74 746f   app-flush-botto
+00168f30: 6d22 3e5c 6e20 2020 2020 2020 2020 2020  m">\n           
+00168f40: 2020 2020 203c 6831 206e 672d 6966 3d22       <h1 ng-if="
+00168f50: 6d6f 6465 6c2e 646f 6373 2e73 686f 7720  model.docs.show 
+00168f60: 3d3d 3d20 6661 6c73 6522 3e5c 6e20 2020  === false">\n   
+00168f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00168f80: 203c 736d 616c 6c20 636c 6173 733d 5c27   <small class=\'
+00168f90: 7465 7874 2d62 6f6c 6420 7465 7874 2d72  text-bold text-r
+00168fa0: 6967 6874 5c27 3e5c 6e20 2020 2020 2020  ight\'>\n       
+00168fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00168fc0: 203c 6920 6461 7461 2d69 636f 6e3d 2265   <i data-icon="e
+00168fd0: 7965 223e 3c2f 693e 5c6e 2020 2020 2020  ye"></i>\n      
+00168fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00168ff0: 2020 5468 6973 207b 7b20 6d6f 6465 6c2e    This {{ model.
+00169000: 7265 736f 7572 6365 5f74 7970 6520 7d7d  resource_type }}
+00169010: 2069 7320 6869 6464 656e 5c6e 2020 2020   is hidden\n    
+00169020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00169030: 3c2f 736d 616c 6c3e 5c6e 2020 2020 2020  </small>\n      
+00169040: 2020 2020 2020 2020 2020 3c2f 6831 3e5c            </h1>\
+00169050: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00169060: 203c 6831 3e5c 6e20 2020 2020 2020 2020   <h1>\n         
+00169070: 2020 2020 2020 2020 2020 203c 7370 616e             <span
+00169080: 2063 6c61 7373 3d22 6272 6561 6b22 3e7b   class="break">{
+00169090: 7b20 6d6f 6465 6c2e 6e61 6d65 207d 7d3c  { model.name }}<
+001690a0: 2f73 7061 6e3e 5c6e 2020 2020 2020 2020  /span>\n        
+001690b0: 2020 2020 2020 2020 2020 2020 3c73 6d61              <sma
+001690c0: 6c6c 3e7b 7b20 6d6f 6465 6c2e 636f 6e66  ll>{{ model.conf
+001690d0: 6967 2e6d 6174 6572 6961 6c69 7a65 6420  ig.materialized 
+001690e0: 7d7d 3c2f 736d 616c 6c3e 5c6e 2020 2020  }}</small>\n    
+001690f0: 2020 2020 2020 2020 2020 2020 3c2f 6831              </h1
+00169100: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
+00169110: 2f64 6976 3e5c 6e20 2020 2020 2020 203c  /div>\n        <
+00169120: 2f64 6976 3e5c 6e20 2020 2020 2020 203c  /div>\n        <
+00169130: 6469 7620 636c 6173 733d 2261 7070 2d66  div class="app-f
+00169140: 7261 6d65 2061 7070 2d70 6164 2d68 223e  rame app-pad-h">
+00169150: 5c6e 2020 2020 2020 2020 2020 2020 3c75  \n            <u
+00169160: 6c20 636c 6173 733d 226e 6176 206e 6176  l class="nav nav
+00169170: 2d74 6162 7322 3e5c 6e20 2020 2020 2020  -tabs">\n       
+00169180: 2020 2020 2020 2020 203c 6c69 2075 692d           <li ui-
+00169190: 7372 6566 2d61 6374 6976 653d 5c27 6163  sref-active=\'ac
+001691a0: 7469 7665 5c27 3e3c 6120 7569 2d73 7265  tive\'><a ui-sre
+001691b0: 663d 2264 6274 2e73 6e61 7073 686f 7428  f="dbt.snapshot(
+001691c0: 7b5c 2723 5c27 3a20 5c27 6465 7461 696c  {\'#\': \'detail
+001691d0: 735c 277d 2922 3e44 6574 6169 6c73 3c2f  s\'})">Details</
+001691e0: 613e 3c2f 6c69 3e5c 6e20 2020 2020 2020  a></li>\n       
+001691f0: 2020 2020 2020 2020 203c 6c69 2075 692d           <li ui-
+00169200: 7372 6566 2d61 6374 6976 653d 5c27 6163  sref-active=\'ac
+00169210: 7469 7665 5c27 3e3c 6120 7569 2d73 7265  tive\'><a ui-sre
+00169220: 663d 2264 6274 2e73 6e61 7073 686f 7428  f="dbt.snapshot(
+00169230: 7b5c 2723 5c27 3a20 5c27 6465 7363 7269  {\'#\': \'descri
+00169240: 7074 696f 6e5c 277d 2922 3e44 6573 6372  ption\'})">Descr
+00169250: 6970 7469 6f6e 3c2f 613e 3c2f 6c69 3e5c  iption</a></li>\
+00169260: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00169270: 203c 6c69 2075 692d 7372 6566 2d61 6374   <li ui-sref-act
+00169280: 6976 653d 5c27 6163 7469 7665 5c27 3e3c  ive=\'active\'><
+00169290: 6120 7569 2d73 7265 663d 2264 6274 2e73  a ui-sref="dbt.s
+001692a0: 6e61 7073 686f 7428 7b5c 2723 5c27 3a20  napshot({\'#\': 
+001692b0: 5c27 636f 6c75 6d6e 735c 277d 2922 3e43  \'columns\'})">C
+001692c0: 6f6c 756d 6e73 3c2f 613e 3c2f 6c69 3e5c  olumns</a></li>\
+001692d0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+001692e0: 203c 6c69 2075 692d 7372 6566 2d61 6374   <li ui-sref-act
+001692f0: 6976 653d 5c27 6163 7469 7665 5c27 206e  ive=\'active\' n
+00169300: 672d 7368 6f77 203d 2022 7265 6665 7265  g-show = "refere
+00169310: 6e63 6573 4c65 6e67 7468 2021 3d20 3022  ncesLength != 0"
+00169320: 3e3c 6120 7569 2d73 7265 663d 2264 6274  ><a ui-sref="dbt
+00169330: 2e73 6e61 7073 686f 7428 7b5c 2723 5c27  .snapshot({\'#\'
+00169340: 3a20 5c27 7265 6665 7265 6e63 6564 5f62  : \'referenced_b
+00169350: 795c 277d 2922 3e52 6566 6572 656e 6365  y\'})">Reference
+00169360: 6420 4279 3c2f 613e 3c2f 6c69 3e5c 6e20  d By</a></li>\n 
+00169370: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00169380: 6c69 2075 692d 7372 6566 2d61 6374 6976  li ui-sref-activ
+00169390: 653d 5c27 6163 7469 7665 5c27 206e 672d  e=\'active\' ng-
+001693a0: 7368 6f77 203d 2022 7061 7265 6e74 734c  show = "parentsL
+001693b0: 656e 6774 6820 213d 2030 223e 3c61 2075  ength != 0"><a u
+001693c0: 692d 7372 6566 3d22 6462 742e 736e 6170  i-sref="dbt.snap
+001693d0: 7368 6f74 287b 5c27 235c 273a 205c 2764  shot({\'#\': \'d
+001693e0: 6570 656e 6473 5f6f 6e5c 277d 2922 3e44  epends_on\'})">D
+001693f0: 6570 656e 6473 204f 6e3c 2f61 3e3c 2f6c  epends On</a></l
+00169400: 693e 5c6e 2020 2020 2020 2020 2020 2020  i>\n            
+00169410: 2020 2020 3c6c 6920 7569 2d73 7265 662d      <li ui-sref-
+00169420: 6163 7469 7665 3d5c 2761 6374 6976 655c  active=\'active\
+00169430: 273e 3c61 2075 692d 7372 6566 3d22 6462  '><a ui-sref="db
+00169440: 742e 736e 6170 7368 6f74 287b 5c27 235c  t.snapshot({\'#\
+00169450: 273a 205c 2763 6f64 655c 277d 2922 3e53  ': \'code\'})">S
+00169460: 514c 3c2f 613e 3c2f 6c69 3e5c 6e20 2020  QL</a></li>\n   
+00169470: 2020 2020 2020 2020 203c 2f75 6c3e 5c6e           </ul>\n
+00169480: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
+00169490: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
+001694a0: 3c64 6976 2063 6c61 7373 3d22 6170 702d  <div class="app-
+001694b0: 6465 7461 696c 7322 3e5c 6e20 2020 2020  details">\n     
+001694c0: 2020 203c 6469 7620 636c 6173 733d 2261     <div class="a
+001694d0: 7070 2d66 7261 6d65 2061 7070 2d70 6164  pp-frame app-pad
+001694e0: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
+001694f0: 3c73 6563 7469 6f6e 2063 6c61 7373 3d22  <section class="
+00169500: 7365 6374 696f 6e22 3e5c 6e20 2020 2020  section">\n     
+00169510: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+00169520: 636c 6173 733d 2273 6563 7469 6f6e 2d74  class="section-t
+00169530: 6172 6765 7422 2069 643d 2264 6574 6169  arget" id="detai
+00169540: 6c73 223e 3c2f 6469 763e 5c6e 2020 2020  ls"></div>\n    
+00169550: 2020 2020 2020 2020 2020 2020 3c74 6162              <tab
+00169560: 6c65 2d64 6574 6169 6c73 206d 6f64 656c  le-details model
+00169570: 3d22 6d6f 6465 6c22 202f 3e5c 6e20 2020  ="model" />\n   
+00169580: 2020 2020 2020 2020 203c 2f73 6563 7469           </secti
+00169590: 6f6e 3e5c 6e5c 6e20 2020 2020 2020 2020  on>\n\n         
+001695a0: 2020 203c 7365 6374 696f 6e20 636c 6173     <section clas
+001695b0: 733d 2273 6563 7469 6f6e 223e 5c6e 2020  s="section">\n  
+001695c0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+001695d0: 6976 2063 6c61 7373 3d22 7365 6374 696f  iv class="sectio
+001695e0: 6e2d 7461 7267 6574 2220 6964 3d22 6465  n-target" id="de
+001695f0: 7363 7269 7074 696f 6e22 3e3c 2f64 6976  scription"></div
+00169600: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+00169610: 2020 203c 6469 7620 636c 6173 733d 2273     <div class="s
+00169620: 6563 7469 6f6e 2d63 6f6e 7465 6e74 223e  ection-content">
+00169630: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00169640: 2020 2020 2020 3c68 363e 4465 7363 7269        <h6>Descri
+00169650: 7074 696f 6e3c 2f68 363e 5c6e 2020 2020  ption</h6>\n    
+00169660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00169670: 3c64 6976 2063 6c61 7373 3d22 7061 6e65  <div class="pane
+00169680: 6c22 3e5c 6e20 2020 2020 2020 2020 2020  l">\n           
+00169690: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+001696a0: 7620 636c 6173 733d 2270 616e 656c 2d62  v class="panel-b
+001696b0: 6f64 7922 3e5c 6e20 2020 2020 2020 2020  ody">\n         
+001696c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001696d0: 2020 203c 6469 7620 6e67 2d69 663d 226d     <div ng-if="m
+001696e0: 6f64 656c 2e64 6573 6372 6970 7469 6f6e  odel.description
+001696f0: 2220 636c 6173 733d 226d 6f64 656c 2d6d  " class="model-m
+00169700: 6172 6b64 6f77 6e22 206d 6172 6b65 643d  arkdown" marked=
+00169710: 226d 6f64 656c 2e64 6573 6372 6970 7469  "model.descripti
+00169720: 6f6e 223e 3c2f 6469 763e 5c6e 2020 2020  on"></div>\n    
+00169730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00169740: 2020 2020 2020 2020 3c64 6976 206e 672d          <div ng-
+00169750: 6966 3d22 216d 6f64 656c 2e64 6573 6372  if="!model.descr
+00169760: 6970 7469 6f6e 223e 5468 6973 207b 7b20  iption">This {{ 
+00169770: 6d6f 6465 6c2e 7265 736f 7572 6365 5f74  model.resource_t
+00169780: 7970 6520 7d7d 2069 7320 6e6f 7420 6375  ype }} is not cu
+00169790: 7272 656e 746c 7920 646f 6375 6d65 6e74  rrently document
+001697a0: 6564 3c2f 6469 763e 5c6e 2020 2020 2020  ed</div>\n      
+001697b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001697c0: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
+001697d0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+001697e0: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
+001697f0: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
+00169800: 2020 2020 2020 2020 2020 3c2f 7365 6374            </sect
+00169810: 696f 6e3e 5c6e 5c6e 2020 2020 2020 2020  ion>\n\n        
+00169820: 2020 2020 3c73 6563 7469 6f6e 2063 6c61      <section cla
+00169830: 7373 3d22 7365 6374 696f 6e22 3e5c 6e20  ss="section">\n 
+00169840: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00169850: 6469 7620 636c 6173 733d 2273 6563 7469  div class="secti
+00169860: 6f6e 2d74 6172 6765 7422 2069 643d 2263  on-target" id="c
+00169870: 6f6c 756d 6e73 223e 3c2f 6469 763e 5c6e  olumns"></div>\n
+00169880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00169890: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
+001698a0: 696f 6e2d 636f 6e74 656e 7422 3e5c 6e20  ion-content">\n 
+001698b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001698c0: 2020 203c 6836 3e43 6f6c 756d 6e73 3c2f     <h6>Columns</
+001698d0: 6836 3e5c 6e20 2020 2020 2020 2020 2020  h6>\n           
+001698e0: 2020 2020 2020 2020 203c 636f 6c75 6d6e           <column
+001698f0: 2d64 6574 6169 6c73 206d 6f64 656c 3d22  -details model="
+00169900: 6d6f 6465 6c22 202f 3e5c 6e20 2020 2020  model" />\n     
+00169910: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00169920: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
+00169930: 2f73 6563 7469 6f6e 3e5c 6e5c 6e20 2020  /section>\n\n   
+00169940: 2020 2020 2020 2020 203c 7365 6374 696f           <sectio
+00169950: 6e20 636c 6173 733d 2273 6563 7469 6f6e  n class="section
+00169960: 2220 6e67 2d73 686f 7720 3d20 2272 6566  " ng-show = "ref
+00169970: 6572 656e 6365 734c 656e 6774 6820 213d  erencesLength !=
+00169980: 2030 223e 5c6e 2020 2020 2020 2020 2020   0">\n          
+00169990: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+001699a0: 3d22 7365 6374 696f 6e2d 7461 7267 6574  ="section-target
+001699b0: 2220 6964 3d22 7265 6665 7265 6e63 6564  " id="referenced
+001699c0: 5f62 7922 3e3c 2f64 6976 3e5c 6e20 2020  _by"></div>\n   
+001699d0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+001699e0: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
+001699f0: 2d63 6f6e 7465 6e74 223e 5c6e 2020 2020  -content">\n    
+00169a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00169a10: 3c68 363e 5265 6665 7265 6e63 6564 2042  <h6>Referenced B
+00169a20: 793c 2f68 363e 5c6e 2020 2020 2020 2020  y</h6>\n        
+00169a30: 2020 2020 2020 2020 2020 2020 3c72 6566              <ref
+00169a40: 6572 656e 6365 2d6c 6973 7420 7265 6665  erence-list refe
+00169a50: 7265 6e63 6573 3d22 7265 6665 7265 6e63  rences="referenc
+00169a60: 6573 2220 6e6f 6465 3d22 6d6f 6465 6c22  es" node="model"
+00169a70: 202f 3e5c 6e20 2020 2020 2020 2020 2020   />\n           
+00169a80: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
+00169a90: 2020 2020 2020 2020 203c 2f73 6563 7469           </secti
+00169aa0: 6f6e 3e5c 6e5c 6e20 2020 2020 2020 2020  on>\n\n         
+00169ab0: 2020 203c 7365 6374 696f 6e20 636c 6173     <section clas
+00169ac0: 733d 2273 6563 7469 6f6e 2220 6e67 2d73  s="section" ng-s
+00169ad0: 686f 7720 3d20 2270 6172 656e 7473 4c65  how = "parentsLe
+00169ae0: 6e67 7468 2021 3d20 3022 3e5c 6e20 2020  ngth != 0">\n   
+00169af0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00169b00: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
+00169b10: 2d74 6172 6765 7422 2069 643d 2264 6570  -target" id="dep
+00169b20: 656e 6473 5f6f 6e22 3e3c 2f64 6976 3e5c  ends_on"></div>\
+00169b30: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00169b40: 203c 6469 7620 636c 6173 733d 2273 6563   <div class="sec
+00169b50: 7469 6f6e 2d63 6f6e 7465 6e74 223e 5c6e  tion-content">\n
+00169b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00169b70: 2020 2020 3c68 363e 4465 7065 6e64 7320      <h6>Depends 
+00169b80: 4f6e 3c2f 6836 3e5c 6e20 2020 2020 2020  On</h6>\n       
+00169b90: 2020 2020 2020 2020 2020 2020 203c 7265               <re
+00169ba0: 6665 7265 6e63 652d 6c69 7374 2072 6566  ference-list ref
+00169bb0: 6572 656e 6365 733d 2270 6172 656e 7473  erences="parents
+00169bc0: 2220 6e6f 6465 3d22 6d6f 6465 6c22 202f  " node="model" /
+00169bd0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+00169be0: 2020 203c 2f64 6976 3e5c 6e20 2020 2020     </div>\n     
+00169bf0: 2020 2020 2020 203c 2f73 6563 7469 6f6e         </section
+00169c00: 3e5c 6e5c 6e20 2020 2020 2020 2020 2020  >\n\n           
+00169c10: 203c 7365 6374 696f 6e20 636c 6173 733d   <section class=
+00169c20: 2273 6563 7469 6f6e 223e 5c6e 2020 2020  "section">\n    
+00169c30: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00169c40: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
+00169c50: 7461 7267 6574 2220 6964 3d22 636f 6465  target" id="code
+00169c60: 223e 3c2f 6469 763e 5c6e 2020 2020 2020  "></div>\n      
+00169c70: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00169c80: 6c61 7373 3d22 7365 6374 696f 6e2d 636f  lass="section-co
+00169c90: 6e74 656e 7422 3e5c 6e20 2020 2020 2020  ntent">\n       
+00169ca0: 2020 2020 2020 2020 2020 2020 203c 636f               <co
+00169cb0: 6465 2d62 6c6f 636b 2076 6572 7369 6f6e  de-block version
+00169cc0: 733d 2276 6572 7369 6f6e 7322 2064 6566  s="versions" def
+00169cd0: 6175 6c74 3d22 6465 6661 756c 745f 7665  ault="default_ve
+00169ce0: 7273 696f 6e22 206c 616e 6775 6167 653d  rsion" language=
+00169cf0: 226c 616e 6775 6167 6522 3e3c 2f63 6f64  "language"></cod
+00169d00: 652d 626c 6f63 6b3e 5c6e 2020 2020 2020  e-block>\n      
+00169d10: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00169d20: 5c6e 2020 2020 2020 2020 2020 2020 3c2f  \n            </
+00169d30: 7365 6374 696f 6e3e 5c6e 2020 2020 2020  section>\n      
+00169d40: 2020 3c2f 6469 763e 5c6e 2020 2020 3c2f    </div>\n    </
+00169d50: 6469 763e 5c6e 3c2f 6469 763e 5c6e 2729  div>\n</div>\n')
+00169d60: 7d5d 292c 652e 6578 706f 7274 733d 6e7d  }]),e.exports=n}
+00169d70: 2c66 756e 6374 696f 6e28 652c 7429 7b76  ,function(e,t){v
+00169d80: 6172 206e 3d22 2f64 6f63 732f 7365 6564  ar n="/docs/seed
+00169d90: 2e68 746d 6c22 3b77 696e 646f 772e 616e  .html";window.an
+00169da0: 6775 6c61 722e 6d6f 6475 6c65 2822 6e67  gular.module("ng
+00169db0: 2229 2e72 756e 285b 2224 7465 6d70 6c61  ").run(["$templa
+00169dc0: 7465 4361 6368 6522 2c66 756e 6374 696f  teCache",functio
+00169dd0: 6e28 6529 7b65 2e70 7574 286e 2c27 3c73  n(e){e.put(n,'<s
+00169de0: 7479 6c65 3e5c 6e2f 2a20 544f 444f 202a  tyle>\n/* TODO *
+00169df0: 2f5c 6e2e 7365 6374 696f 6e2d 7461 7267  /\n.section-targ
+00169e00: 6574 207b 5c6e 2020 2020 746f 703a 202d  et {\n    top: -
+00169e10: 3865 6d3b 5c6e 7d5c 6e5c 6e2e 6e6f 666c  8em;\n}\n\n.nofl
+00169e20: 6578 207b 5c6e 2020 2020 666c 6578 3a20  ex {\n    flex: 
+00169e30: 3020 3020 3136 3070 7820 2169 6d70 6f72  0 0 160px !impor
+00169e40: 7461 6e74 3b5c 6e7d 5c6e 5c6e 2e68 6967  tant;\n}\n\n.hig
+00169e50: 686c 6967 6874 207b 5c6e 2020 2020 636f  hlight {\n    co
+00169e60: 6c6f 723a 2023 3234 3239 3265 3b5c 6e20  lor: #24292e;\n 
+00169e70: 2020 2062 6163 6b67 726f 756e 642d 636f     background-co
+00169e80: 6c6f 723a 2077 6869 7465 3b5c 6e7d 5c6e  lor: white;\n}\n
+00169e90: 5c6e 3c2f 7374 796c 653e 5c6e 5c6e 3c64  \n</style>\n\n<d
+00169ea0: 6976 2063 6c61 7373 3d5c 2761 7070 2d73  iv class=\'app-s
+00169eb0: 6372 6f6c 6c5c 273e 5c6e 2020 2020 3c64  croll\'>\n    <d
+00169ec0: 6976 2063 6c61 7373 3d22 6170 702d 6c69  iv class="app-li
+00169ed0: 6e6b 7320 6170 702d 7374 6963 6b79 223e  nks app-sticky">
+00169ee0: 5c6e 2020 2020 2020 2020 3c64 6976 2063  \n        <div c
+00169ef0: 6c61 7373 3d22 6170 702d 7469 746c 6522  lass="app-title"
+00169f00: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
+00169f10: 6469 7620 636c 6173 733d 2261 7070 2d66  div class="app-f
+00169f20: 7261 6d65 2061 7070 2d70 6164 2061 7070  rame app-pad app
+00169f30: 2d66 6c75 7368 2d62 6f74 746f 6d22 3e5c  -flush-bottom">\
+00169f40: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00169f50: 203c 6831 206e 672d 6966 3d22 6d6f 6465   <h1 ng-if="mode
+00169f60: 6c2e 646f 6373 2e73 686f 7720 3d3d 3d20  l.docs.show === 
+00169f70: 6661 6c73 6522 3e5c 6e20 2020 2020 2020  false">\n       
+00169f80: 2020 2020 2020 2020 2020 2020 203c 736d               <sm
+00169f90: 616c 6c20 636c 6173 733d 5c27 7465 7874  all class=\'text
+00169fa0: 2d62 6f6c 6420 7465 7874 2d72 6967 6874  -bold text-right
+00169fb0: 5c27 3e5c 6e20 2020 2020 2020 2020 2020  \'>\n           
+00169fc0: 2020 2020 2020 2020 2020 2020 203c 6920               <i 
+00169fd0: 6461 7461 2d69 636f 6e3d 2265 7965 223e  data-icon="eye">
+00169fe0: 3c2f 693e 5c6e 2020 2020 2020 2020 2020  </i>\n          
+00169ff0: 2020 2020 2020 2020 2020 2020 2020 5468                Th
+0016a000: 6973 207b 7b20 6d6f 6465 6c2e 7265 736f  is {{ model.reso
+0016a010: 7572 6365 5f74 7970 6520 7d7d 2069 7320  urce_type }} is 
+0016a020: 6869 6464 656e 5c6e 2020 2020 2020 2020  hidden\n        
+0016a030: 2020 2020 2020 2020 2020 2020 3c2f 736d              </sm
+0016a040: 616c 6c3e 5c6e 2020 2020 2020 2020 2020  all>\n          
+0016a050: 2020 2020 2020 3c2f 6831 3e5c 6e20 2020        </h1>\n   
+0016a060: 2020 2020 2020 2020 2020 2020 203c 6831               <h1
+0016a070: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016a080: 2020 2020 2020 203c 7370 616e 2063 6c61         <span cla
+0016a090: 7373 3d22 6272 6561 6b22 3e7b 7b20 6d6f  ss="break">{{ mo
+0016a0a0: 6465 6c2e 6e61 6d65 207d 7d3c 2f73 7061  del.name }}</spa
+0016a0b0: 6e3e 5c6e 2020 2020 2020 2020 2020 2020  n>\n            
+0016a0c0: 2020 2020 2020 2020 3c73 6d61 6c6c 3e7b          <small>{
+0016a0d0: 7b20 6d6f 6465 6c2e 636f 6e66 6967 2e6d  { model.config.m
+0016a0e0: 6174 6572 6961 6c69 7a65 6420 7d7d 3c2f  aterialized }}</
+0016a0f0: 736d 616c 6c3e 5c6e 2020 2020 2020 2020  small>\n        
+0016a100: 2020 2020 2020 2020 3c2f 6831 3e5c 6e20          </h1>\n 
+0016a110: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+0016a120: 3e5c 6e20 2020 2020 2020 203c 2f64 6976  >\n        </div
+0016a130: 3e5c 6e20 2020 2020 2020 203c 6469 7620  >\n        <div 
+0016a140: 636c 6173 733d 2261 7070 2d66 7261 6d65  class="app-frame
+0016a150: 2061 7070 2d70 6164 2d68 223e 5c6e 2020   app-pad-h">\n  
+0016a160: 2020 2020 2020 2020 2020 3c75 6c20 636c            <ul cl
+0016a170: 6173 733d 226e 6176 206e 6176 2d74 6162  ass="nav nav-tab
+0016a180: 7322 3e5c 6e20 2020 2020 2020 2020 2020  s">\n           
+0016a190: 2020 2020 203c 6c69 2075 692d 7372 6566       <li ui-sref
+0016a1a0: 2d61 6374 6976 653d 5c27 6163 7469 7665  -active=\'active
+0016a1b0: 5c27 3e3c 6120 7569 2d73 7265 663d 2264  \'><a ui-sref="d
+0016a1c0: 6274 2e73 6565 6428 7b5c 2723 5c27 3a20  bt.seed({\'#\': 
+0016a1d0: 5c27 6465 7461 696c 735c 277d 2922 3e44  \'details\'})">D
+0016a1e0: 6574 6169 6c73 3c2f 613e 3c2f 6c69 3e5c  etails</a></li>\
+0016a1f0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016a200: 203c 6c69 2075 692d 7372 6566 2d61 6374   <li ui-sref-act
+0016a210: 6976 653d 5c27 6163 7469 7665 5c27 3e3c  ive=\'active\'><
+0016a220: 6120 7569 2d73 7265 663d 2264 6274 2e73  a ui-sref="dbt.s
+0016a230: 6565 6428 7b5c 2723 5c27 3a20 5c27 6465  eed({\'#\': \'de
+0016a240: 7363 7269 7074 696f 6e5c 277d 2922 3e44  scription\'})">D
+0016a250: 6573 6372 6970 7469 6f6e 3c2f 613e 3c2f  escription</a></
+0016a260: 6c69 3e5c 6e20 2020 2020 2020 2020 2020  li>\n           
+0016a270: 2020 2020 203c 6c69 2075 692d 7372 6566       <li ui-sref
+0016a280: 2d61 6374 6976 653d 5c27 6163 7469 7665  -active=\'active
+0016a290: 5c27 3e3c 6120 7569 2d73 7265 663d 2264  \'><a ui-sref="d
+0016a2a0: 6274 2e73 6565 6428 7b5c 2723 5c27 3a20  bt.seed({\'#\': 
+0016a2b0: 5c27 636f 6c75 6d6e 735c 277d 2922 3e43  \'columns\'})">C
+0016a2c0: 6f6c 756d 6e73 3c2f 613e 3c2f 6c69 3e5c  olumns</a></li>\
+0016a2d0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016a2e0: 203c 6c69 2075 692d 7372 6566 2d61 6374   <li ui-sref-act
+0016a2f0: 6976 653d 5c27 6163 7469 7665 5c27 206e  ive=\'active\' n
+0016a300: 672d 7368 6f77 203d 2022 7265 6665 7265  g-show = "refere
+0016a310: 6e63 6573 4c65 6e67 7468 2021 3d20 3022  ncesLength != 0"
+0016a320: 3e3c 6120 7569 2d73 7265 663d 2264 6274  ><a ui-sref="dbt
+0016a330: 2e73 6565 6428 7b5c 2723 5c27 3a20 5c27  .seed({\'#\': \'
+0016a340: 7265 6665 7265 6e63 6564 5f62 795c 277d  referenced_by\'}
+0016a350: 2922 3e52 6566 6572 656e 6365 6420 4279  )">Referenced By
+0016a360: 3c2f 613e 3c2f 6c69 3e5c 6e20 2020 2020  </a></li>\n     
+0016a370: 2020 2020 2020 2020 2020 203c 6c69 2075             <li u
+0016a380: 692d 7372 6566 2d61 6374 6976 653d 5c27  i-sref-active=\'
+0016a390: 6163 7469 7665 5c27 206e 672d 7368 6f77  active\' ng-show
+0016a3a0: 203d 2022 7061 7265 6e74 734c 656e 6774   = "parentsLengt
+0016a3b0: 6820 213d 2030 223e 3c61 2075 692d 7372  h != 0"><a ui-sr
+0016a3c0: 6566 3d22 6462 742e 7365 6564 287b 5c27  ef="dbt.seed({\'
+0016a3d0: 235c 273a 205c 2764 6570 656e 6473 5f6f  #\': \'depends_o
+0016a3e0: 6e5c 277d 2922 3e44 6570 656e 6473 204f  n\'})">Depends O
+0016a3f0: 6e3c 2f61 3e3c 2f6c 693e 5c6e 2020 2020  n</a></li>\n    
+0016a400: 2020 2020 2020 2020 2020 2020 3c6c 6920              <li 
+0016a410: 7569 2d73 7265 662d 6163 7469 7665 3d5c  ui-sref-active=\
+0016a420: 2761 6374 6976 655c 273e 3c61 2075 692d  'active\'><a ui-
+0016a430: 7372 6566 3d22 6462 742e 7365 6564 287b  sref="dbt.seed({
+0016a440: 5c27 235c 273a 205c 2763 6f64 655c 277d  \'#\': \'code\'}
+0016a450: 2922 3e53 514c 3c2f 613e 3c2f 6c69 3e5c  )">SQL</a></li>\
+0016a460: 6e20 2020 2020 2020 2020 2020 203c 2f75  n            </u
+0016a470: 6c3e 5c6e 2020 2020 2020 2020 3c2f 6469  l>\n        </di
+0016a480: 763e 5c6e 2020 2020 3c2f 6469 763e 5c6e  v>\n    </div>\n
+0016a490: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0016a4a0: 6170 702d 6465 7461 696c 7322 3e5c 6e20  app-details">\n 
+0016a4b0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0016a4c0: 733d 2261 7070 2d66 7261 6d65 2061 7070  s="app-frame app
+0016a4d0: 2d70 6164 223e 5c6e 2020 2020 2020 2020  -pad">\n        
+0016a4e0: 2020 2020 3c73 6563 7469 6f6e 2063 6c61      <section cla
+0016a4f0: 7373 3d22 7365 6374 696f 6e22 3e5c 6e20  ss="section">\n 
+0016a500: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016a510: 6469 7620 636c 6173 733d 2273 6563 7469  div class="secti
+0016a520: 6f6e 2d74 6172 6765 7422 2069 643d 2264  on-target" id="d
+0016a530: 6574 6169 6c73 223e 3c2f 6469 763e 5c6e  etails"></div>\n
+0016a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016a550: 3c74 6162 6c65 2d64 6574 6169 6c73 206d  <table-details m
+0016a560: 6f64 656c 3d22 6d6f 6465 6c22 202f 3e5c  odel="model" />\
+0016a570: 6e20 2020 2020 2020 2020 2020 203c 2f73  n            </s
+0016a580: 6563 7469 6f6e 3e5c 6e5c 6e20 2020 2020  ection>\n\n     
+0016a590: 2020 2020 2020 203c 7365 6374 696f 6e20         <section 
+0016a5a0: 636c 6173 733d 2273 6563 7469 6f6e 223e  class="section">
+0016a5b0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+0016a5c0: 2020 3c64 6976 2063 6c61 7373 3d22 7365    <div class="se
+0016a5d0: 6374 696f 6e2d 7461 7267 6574 2220 6964  ction-target" id
+0016a5e0: 3d22 6465 7363 7269 7074 696f 6e22 3e3c  ="description"><
+0016a5f0: 2f64 6976 3e5c 6e20 2020 2020 2020 2020  /div>\n         
+0016a600: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0016a610: 733d 2273 6563 7469 6f6e 2d63 6f6e 7465  s="section-conte
+0016a620: 6e74 223e 5c6e 2020 2020 2020 2020 2020  nt">\n          
+0016a630: 2020 2020 2020 2020 2020 3c68 363e 4465            <h6>De
+0016a640: 7363 7269 7074 696f 6e3c 2f68 363e 5c6e  scription</h6>\n
+0016a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016a660: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0016a670: 7061 6e65 6c22 3e5c 6e20 2020 2020 2020  panel">\n       
+0016a680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016a690: 203c 6469 7620 636c 6173 733d 2270 616e   <div class="pan
+0016a6a0: 656c 2d62 6f64 7922 3e5c 6e20 2020 2020  el-body">\n     
+0016a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016a6c0: 2020 2020 2020 203c 6469 7620 6e67 2d69         <div ng-i
+0016a6d0: 663d 226d 6f64 656c 2e64 6573 6372 6970  f="model.descrip
+0016a6e0: 7469 6f6e 2220 636c 6173 733d 226d 6f64  tion" class="mod
+0016a6f0: 656c 2d6d 6172 6b64 6f77 6e22 206d 6172  el-markdown" mar
+0016a700: 6b65 643d 226d 6f64 656c 2e64 6573 6372  ked="model.descr
+0016a710: 6970 7469 6f6e 223e 3c2f 6469 763e 5c6e  iption"></div>\n
+0016a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016a730: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0016a740: 206e 672d 6966 3d22 216d 6f64 656c 2e64   ng-if="!model.d
+0016a750: 6573 6372 6970 7469 6f6e 223e 5468 6973  escription">This
+0016a760: 207b 7b20 6d6f 6465 6c2e 7265 736f 7572   {{ model.resour
+0016a770: 6365 5f74 7970 6520 7d7d 2069 7320 6e6f  ce_type }} is no
+0016a780: 7420 6375 7272 656e 746c 7920 646f 6375  t currently docu
+0016a790: 6d65 6e74 6564 3c2f 6469 763e 5c6e 2020  mented</div>\n  
+0016a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016a7b0: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
+0016a7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016a7d0: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
+0016a7e0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+0016a7f0: 5c6e 2020 2020 2020 2020 2020 2020 3c2f  \n            </
+0016a800: 7365 6374 696f 6e3e 5c6e 2020 2020 2020  section>\n      
+0016a810: 2020 2020 2020 3c73 6563 7469 6f6e 2063        <section c
+0016a820: 6c61 7373 3d22 7365 6374 696f 6e22 3e5c  lass="section">\
+0016a830: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016a840: 203c 6469 7620 636c 6173 733d 2273 6563   <div class="sec
+0016a850: 7469 6f6e 2d74 6172 6765 7422 2069 643d  tion-target" id=
+0016a860: 2263 6f6c 756d 6e73 223e 3c2f 6469 763e  "columns"></div>
+0016a870: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+0016a880: 2020 3c64 6976 2063 6c61 7373 3d22 7365    <div class="se
+0016a890: 6374 696f 6e2d 636f 6e74 656e 7422 3e5c  ction-content">\
+0016a8a0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016a8b0: 2020 2020 203c 6836 3e43 6f6c 756d 6e73       <h6>Columns
+0016a8c0: 3c2f 6836 3e5c 6e20 2020 2020 2020 2020  </h6>\n         
+0016a8d0: 2020 2020 2020 2020 2020 203c 636f 6c75             <colu
+0016a8e0: 6d6e 2d64 6574 6169 6c73 206d 6f64 656c  mn-details model
+0016a8f0: 3d22 6d6f 6465 6c22 202f 3e5c 6e20 2020  ="model" />\n   
+0016a900: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+0016a910: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
+0016a920: 203c 2f73 6563 7469 6f6e 3e5c 6e5c 6e20   </section>\n\n 
+0016a930: 2020 2020 2020 2020 2020 203c 7365 6374             <sect
+0016a940: 696f 6e20 636c 6173 733d 2273 6563 7469  ion class="secti
+0016a950: 6f6e 2220 6e67 2d73 686f 7720 3d20 2272  on" ng-show = "r
+0016a960: 6566 6572 656e 6365 734c 656e 6774 6820  eferencesLength 
+0016a970: 213d 2030 223e 5c6e 2020 2020 2020 2020  != 0">\n        
+0016a980: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0016a990: 7373 3d22 7365 6374 696f 6e2d 7461 7267  ss="section-targ
+0016a9a0: 6574 2220 6964 3d22 7265 6665 7265 6e63  et" id="referenc
+0016a9b0: 6564 5f62 7922 3e3c 2f64 6976 3e5c 6e20  ed_by"></div>\n 
+0016a9c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016a9d0: 6469 7620 636c 6173 733d 2273 6563 7469  div class="secti
+0016a9e0: 6f6e 2d63 6f6e 7465 6e74 223e 5c6e 2020  on-content">\n  
+0016a9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016aa00: 2020 3c68 363e 5265 6665 7265 6e63 6564    <h6>Referenced
+0016aa10: 2042 793c 2f68 363e 5c6e 2020 2020 2020   By</h6>\n      
+0016aa20: 2020 2020 2020 2020 2020 2020 2020 3c72                <r
+0016aa30: 6566 6572 656e 6365 2d6c 6973 7420 7265  eference-list re
+0016aa40: 6665 7265 6e63 6573 3d22 7265 6665 7265  ferences="refere
+0016aa50: 6e63 6573 2220 6e6f 6465 3d22 6d6f 6465  nces" node="mode
+0016aa60: 6c22 202f 3e5c 6e20 2020 2020 2020 2020  l" />\n         
+0016aa70: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
+0016aa80: 2020 2020 2020 2020 2020 203c 2f73 6563             </sec
+0016aa90: 7469 6f6e 3e5c 6e5c 6e20 2020 2020 2020  tion>\n\n       
+0016aaa0: 2020 2020 203c 7365 6374 696f 6e20 636c       <section cl
+0016aab0: 6173 733d 2273 6563 7469 6f6e 2220 6e67  ass="section" ng
+0016aac0: 2d73 686f 7720 3d20 2270 6172 656e 7473  -show = "parents
+0016aad0: 4c65 6e67 7468 2021 3d20 3022 3e5c 6e20  Length != 0">\n 
+0016aae0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016aaf0: 6469 7620 636c 6173 733d 2273 6563 7469  div class="secti
+0016ab00: 6f6e 2d74 6172 6765 7422 2069 643d 2264  on-target" id="d
+0016ab10: 6570 656e 6473 5f6f 6e22 3e3c 2f64 6976  epends_on"></div
+0016ab20: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016ab30: 2020 203c 6469 7620 636c 6173 733d 2273     <div class="s
+0016ab40: 6563 7469 6f6e 2d63 6f6e 7465 6e74 223e  ection-content">
+0016ab50: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+0016ab60: 2020 2020 2020 3c68 363e 4465 7065 6e64        <h6>Depend
+0016ab70: 7320 4f6e 3c2f 6836 3e5c 6e20 2020 2020  s On</h6>\n     
+0016ab80: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016ab90: 7265 6665 7265 6e63 652d 6c69 7374 2072  reference-list r
+0016aba0: 6566 6572 656e 6365 733d 2270 6172 656e  eferences="paren
+0016abb0: 7473 2220 6e6f 6465 3d22 6d6f 6465 6c22  ts" node="model"
+0016abc0: 202f 3e5c 6e20 2020 2020 2020 2020 2020   />\n           
+0016abd0: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
+0016abe0: 2020 2020 2020 2020 203c 2f73 6563 7469           </secti
+0016abf0: 6f6e 3e5c 6e5c 6e20 2020 2020 2020 2020  on>\n\n         
+0016ac00: 2020 203c 7365 6374 696f 6e20 636c 6173     <section clas
+0016ac10: 733d 2273 6563 7469 6f6e 223e 5c6e 2020  s="section">\n  
+0016ac20: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+0016ac30: 6976 2063 6c61 7373 3d22 7365 6374 696f  iv class="sectio
+0016ac40: 6e2d 7461 7267 6574 2220 6964 3d22 636f  n-target" id="co
+0016ac50: 6465 223e 3c2f 6469 763e 5c6e 2020 2020  de"></div>\n    
+0016ac60: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0016ac70: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
+0016ac80: 636f 6e74 656e 7422 3e5c 6e20 2020 2020  content">\n     
+0016ac90: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016aca0: 636f 6465 2d62 6c6f 636b 2076 6572 7369  code-block versi
+0016acb0: 6f6e 733d 2276 6572 7369 6f6e 7322 2064  ons="versions" d
+0016acc0: 6566 6175 6c74 3d22 6465 6661 756c 745f  efault="default_
+0016acd0: 7665 7273 696f 6e22 206c 616e 6775 6167  version" languag
+0016ace0: 653d 226c 616e 6775 6167 6522 3e3c 2f63  e="language"></c
+0016acf0: 6f64 652d 626c 6f63 6b3e 5c6e 2020 2020  ode-block>\n    
+0016ad00: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+0016ad10: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
+0016ad20: 3c2f 7365 6374 696f 6e3e 5c6e 2020 2020  </section>\n    
+0016ad30: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
+0016ad40: 3c2f 6469 763e 5c6e 3c2f 6469 763e 5c6e  </div>\n</div>\n
+0016ad50: 2729 7d5d 292c 652e 6578 706f 7274 733d  ')}]),e.exports=
+0016ad60: 6e7d 2c66 756e 6374 696f 6e28 652c 7429  n},function(e,t)
+0016ad70: 7b76 6172 206e 3d22 2f64 6f63 732f 756e  {var n="/docs/un
+0016ad80: 6974 5f74 6573 742e 6874 6d6c 223b 7769  it_test.html";wi
+0016ad90: 6e64 6f77 2e61 6e67 756c 6172 2e6d 6f64  ndow.angular.mod
+0016ada0: 756c 6528 226e 6722 292e 7275 6e28 5b22  ule("ng").run(["
+0016adb0: 2474 656d 706c 6174 6543 6163 6865 222c  $templateCache",
+0016adc0: 6675 6e63 7469 6f6e 2865 297b 652e 7075  function(e){e.pu
+0016add0: 7428 6e2c 273c 7374 796c 653e 5c6e 2f2a  t(n,'<style>\n/*
+0016ade0: 2054 4f44 4f20 2a2f 5c6e 2e73 6563 7469   TODO */\n.secti
+0016adf0: 6f6e 2d74 6172 6765 7420 7b5c 6e20 2020  on-target {\n   
+0016ae00: 2074 6f70 3a20 2d38 656d 3b5c 6e7d 5c6e   top: -8em;\n}\n
+0016ae10: 5c6e 2e6e 6f66 6c65 7820 7b5c 6e20 2020  \n.noflex {\n   
+0016ae20: 2066 6c65 783a 2030 2030 2031 3630 7078   flex: 0 0 160px
+0016ae30: 2021 696d 706f 7274 616e 743b 5c6e 7d5c   !important;\n}\
+0016ae40: 6e5c 6e2e 6869 6768 6c69 6768 7420 7b5c  n\n.highlight {\
+0016ae50: 6e20 2020 2063 6f6c 6f72 3a20 2332 3432  n    color: #242
+0016ae60: 3932 653b 5c6e 2020 2020 6261 636b 6772  92e;\n    backgr
+0016ae70: 6f75 6e64 2d63 6f6c 6f72 3a20 7768 6974  ound-color: whit
+0016ae80: 653b 5c6e 7d5c 6e5c 6e3c 2f73 7479 6c65  e;\n}\n\n</style
+0016ae90: 3e5c 6e5c 6e3c 6469 7620 636c 6173 733d  >\n\n<div class=
+0016aea0: 5c27 6170 702d 7363 726f 6c6c 5c27 3e5c  \'app-scroll\'>\
+0016aeb0: 6e20 2020 203c 6469 7620 636c 6173 733d  n    <div class=
+0016aec0: 2261 7070 2d6c 696e 6b73 2061 7070 2d73  "app-links app-s
+0016aed0: 7469 636b 7922 3e5c 6e20 2020 2020 2020  ticky">\n       
+0016aee0: 203c 6469 7620 636c 6173 733d 2261 7070   <div class="app
+0016aef0: 2d74 6974 6c65 223e 5c6e 2020 2020 2020  -title">\n      
+0016af00: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0016af10: 3d22 6170 702d 6672 616d 6520 6170 702d  ="app-frame app-
+0016af20: 7061 6420 6170 702d 666c 7573 682d 626f  pad app-flush-bo
+0016af30: 7474 6f6d 223e 5c6e 2020 2020 2020 2020  ttom">\n        
+0016af40: 2020 2020 2020 2020 3c68 313e 5c6e 2020          <h1>\n  
+0016af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016af60: 2020 3c73 7061 6e20 636c 6173 733d 2262    <span class="b
+0016af70: 7265 616b 223e 7b7b 206d 6f64 656c 2e6e  reak">{{ model.n
+0016af80: 616d 6520 7d7d 3c2f 7370 616e 3e5c 6e20  ame }}</span>\n 
+0016af90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016afa0: 2020 203c 736d 616c 6c3e 756e 6974 2074     <small>unit t
+0016afb0: 6573 743c 2f73 6d61 6c6c 3e5c 6e20 2020  est</small>\n   
+0016afc0: 2020 2020 2020 2020 2020 2020 203c 2f68               </h
+0016afd0: 313e 5c6e 2020 2020 2020 2020 2020 2020  1>\n            
+0016afe0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
+0016aff0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
+0016b000: 3c64 6976 2063 6c61 7373 3d22 6170 702d  <div class="app-
+0016b010: 6672 616d 6520 6170 702d 7061 642d 6822  frame app-pad-h"
+0016b020: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
+0016b030: 756c 2063 6c61 7373 3d22 6e61 7620 6e61  ul class="nav na
+0016b040: 762d 7461 6273 223e 5c6e 2020 2020 2020  v-tabs">\n      
+0016b050: 2020 2020 2020 2020 2020 3c6c 6920 7569            <li ui
+0016b060: 2d73 7265 662d 6163 7469 7665 3d5c 2761  -sref-active=\'a
+0016b070: 6374 6976 655c 273e 3c61 2075 692d 7372  ctive\'><a ui-sr
+0016b080: 6566 3d22 6462 742e 756e 6974 5f74 6573  ef="dbt.unit_tes
+0016b090: 7428 7b5c 2723 5c27 3a20 5c27 6465 7363  t({\'#\': \'desc
+0016b0a0: 7269 7074 696f 6e5c 277d 2922 3e44 6573  ription\'})">Des
+0016b0b0: 6372 6970 7469 6f6e 3c2f 613e 3c2f 6c69  cription</a></li
+0016b0c0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016b0d0: 2020 203c 6c69 2075 692d 7372 6566 2d61     <li ui-sref-a
+0016b0e0: 6374 6976 653d 5c27 6163 7469 7665 5c27  ctive=\'active\'
+0016b0f0: 206e 672d 7368 6f77 203d 2022 7061 7265   ng-show = "pare
+0016b100: 6e74 734c 656e 6774 6820 213d 2030 223e  ntsLength != 0">
+0016b110: 3c61 2075 692d 7372 6566 3d22 6462 742e  <a ui-sref="dbt.
+0016b120: 756e 6974 5f74 6573 7428 7b5c 2723 5c27  unit_test({\'#\'
+0016b130: 3a20 5c27 6465 7065 6e64 735f 6f6e 5c27  : \'depends_on\'
+0016b140: 7d29 223e 4465 7065 6e64 7320 4f6e 3c2f  })">Depends On</
+0016b150: 613e 3c2f 6c69 3e5c 6e20 2020 2020 2020  a></li>\n       
+0016b160: 2020 2020 203c 2f75 6c3e 5c6e 2020 2020       </ul>\n    
+0016b170: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
+0016b180: 3c2f 6469 763e 5c6e 2020 2020 3c64 6976  </div>\n    <div
+0016b190: 2063 6c61 7373 3d22 6170 702d 6465 7461   class="app-deta
+0016b1a0: 696c 7322 3e5c 6e20 2020 2020 2020 203c  ils">\n        <
+0016b1b0: 6469 7620 636c 6173 733d 2261 7070 2d66  div class="app-f
+0016b1c0: 7261 6d65 2061 7070 2d70 6164 223e 5c6e  rame app-pad">\n
+0016b1d0: 2020 2020 2020 2020 2020 2020 3c73 6563              <sec
+0016b1e0: 7469 6f6e 2063 6c61 7373 3d22 7365 6374  tion class="sect
+0016b1f0: 696f 6e22 3e5c 6e20 2020 2020 2020 2020  ion">\n         
+0016b200: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0016b210: 733d 2273 6563 7469 6f6e 2d74 6172 6765  s="section-targe
+0016b220: 7422 2069 643d 2264 6573 6372 6970 7469  t" id="descripti
+0016b230: 6f6e 223e 3c2f 6469 763e 5c6e 2020 2020  on"></div>\n    
+0016b240: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0016b250: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
+0016b260: 636f 6e74 656e 7422 3e5c 6e20 2020 2020  content">\n     
+0016b270: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016b280: 6836 3e44 6573 6372 6970 7469 6f6e 3c2f  h6>Description</
+0016b290: 6836 3e5c 6e20 2020 2020 2020 2020 2020  h6>\n           
+0016b2a0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0016b2b0: 6173 733d 2270 616e 656c 223e 5c6e 2020  ass="panel">\n  
+0016b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016b2d0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0016b2e0: 3d22 7061 6e65 6c2d 626f 6479 223e 5c6e  ="panel-body">\n
+0016b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016b300: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0016b310: 206e 672d 6966 3d22 6d6f 6465 6c2e 6465   ng-if="model.de
+0016b320: 7363 7269 7074 696f 6e22 2063 6c61 7373  scription" class
+0016b330: 3d22 6d6f 6465 6c2d 6d61 726b 646f 776e  ="model-markdown
+0016b340: 2220 6d61 726b 6564 3d22 6d6f 6465 6c2e  " marked="model.
+0016b350: 6465 7363 7269 7074 696f 6e22 3e3c 2f64  description"></d
+0016b360: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
+0016b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016b380: 203c 6469 7620 6e67 2d69 663d 2221 6d6f   <div ng-if="!mo
+0016b390: 6465 6c2e 6465 7363 7269 7074 696f 6e22  del.description"
+0016b3a0: 3e54 6869 7320 7b7b 206d 6f64 656c 2e72  >This {{ model.r
+0016b3b0: 6573 6f75 7263 655f 7479 7065 207d 7d20  esource_type }} 
+0016b3c0: 6973 206e 6f74 2063 7572 7265 6e74 6c79  is not currently
+0016b3d0: 2064 6f63 756d 656e 7465 643c 2f64 6976   documented</div
+0016b3e0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016b3f0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+0016b400: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016b410: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
+0016b420: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016b430: 2f64 6976 3e5c 6e20 2020 2020 2020 2020  /div>\n         
+0016b440: 2020 203c 2f73 6563 7469 6f6e 3e5c 6e5c     </section>\n\
+0016b450: 6e20 2020 2020 2020 2020 2020 203c 7365  n            <se
+0016b460: 6374 696f 6e20 636c 6173 733d 2273 6563  ction class="sec
+0016b470: 7469 6f6e 2220 6e67 2d73 686f 7720 3d20  tion" ng-show = 
+0016b480: 2270 6172 656e 7473 4c65 6e67 7468 2021  "parentsLength !
+0016b490: 3d20 3022 3e5c 6e20 2020 2020 2020 2020  = 0">\n         
+0016b4a0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0016b4b0: 733d 2273 6563 7469 6f6e 2d74 6172 6765  s="section-targe
+0016b4c0: 7422 2069 643d 2264 6570 656e 6473 5f6f  t" id="depends_o
+0016b4d0: 6e22 3e3c 2f64 6976 3e5c 6e20 2020 2020  n"></div>\n     
+0016b4e0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0016b4f0: 636c 6173 733d 2273 6563 7469 6f6e 2d63  class="section-c
+0016b500: 6f6e 7465 6e74 223e 5c6e 2020 2020 2020  ontent">\n      
+0016b510: 2020 2020 2020 2020 2020 2020 2020 3c68                <h
+0016b520: 363e 4465 7065 6e64 7320 4f6e 3c2f 6836  6>Depends On</h6
+0016b530: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016b540: 2020 2020 2020 203c 7265 6665 7265 6e63         <referenc
+0016b550: 652d 6c69 7374 2072 6566 6572 656e 6365  e-list reference
+0016b560: 733d 2270 6172 656e 7473 2220 6e6f 6465  s="parents" node
+0016b570: 3d22 6d6f 6465 6c22 202f 3e5c 6e20 2020  ="model" />\n   
+0016b580: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+0016b590: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
+0016b5a0: 203c 2f73 6563 7469 6f6e 3e5c 6e5c 6e20   </section>\n\n 
+0016b5b0: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
+0016b5c0: 2020 203c 2f64 6976 3e5c 6e3c 2f64 6976     </div>\n</div
+0016b5d0: 3e5c 6e27 297d 5d29 2c65 2e65 7870 6f72  >\n')}]),e.expor
+0016b5e0: 7473 3d6e 7d2c 6675 6e63 7469 6f6e 2865  ts=n},function(e
+0016b5f0: 2c74 297b 7661 7220 6e3d 222f 646f 6373  ,t){var n="/docs
+0016b600: 2f74 6573 742e 6874 6d6c 223b 7769 6e64  /test.html";wind
+0016b610: 6f77 2e61 6e67 756c 6172 2e6d 6f64 756c  ow.angular.modul
+0016b620: 6528 226e 6722 292e 7275 6e28 5b22 2474  e("ng").run(["$t
+0016b630: 656d 706c 6174 6543 6163 6865 222c 6675  emplateCache",fu
+0016b640: 6e63 7469 6f6e 2865 297b 652e 7075 7428  nction(e){e.put(
+0016b650: 6e2c 273c 7374 796c 653e 5c6e 2f2a 2054  n,'<style>\n/* T
+0016b660: 4f44 4f20 2a2f 5c6e 2e73 6563 7469 6f6e  ODO */\n.section
+0016b670: 2d74 6172 6765 7420 7b5c 6e20 2020 2074  -target {\n    t
+0016b680: 6f70 3a20 2d38 656d 3b5c 6e7d 5c6e 5c6e  op: -8em;\n}\n\n
+0016b690: 2e6e 6f66 6c65 7820 7b5c 6e20 2020 2066  .noflex {\n    f
+0016b6a0: 6c65 783a 2030 2030 2031 3630 7078 2021  lex: 0 0 160px !
+0016b6b0: 696d 706f 7274 616e 743b 5c6e 7d5c 6e5c  important;\n}\n\
+0016b6c0: 6e2e 6869 6768 6c69 6768 7420 7b5c 6e20  n.highlight {\n 
+0016b6d0: 2020 2063 6f6c 6f72 3a20 2332 3432 3932     color: #24292
+0016b6e0: 653b 5c6e 2020 2020 6261 636b 6772 6f75  e;\n    backgrou
+0016b6f0: 6e64 2d63 6f6c 6f72 3a20 7768 6974 653b  nd-color: white;
+0016b700: 5c6e 7d5c 6e5c 6e3c 2f73 7479 6c65 3e5c  \n}\n\n</style>\
+0016b710: 6e5c 6e3c 6469 7620 636c 6173 733d 5c27  n\n<div class=\'
+0016b720: 6170 702d 7363 726f 6c6c 5c27 3e5c 6e20  app-scroll\'>\n 
+0016b730: 2020 203c 6469 7620 636c 6173 733d 2261     <div class="a
+0016b740: 7070 2d6c 696e 6b73 2061 7070 2d73 7469  pp-links app-sti
+0016b750: 636b 7922 3e5c 6e20 2020 2020 2020 203c  cky">\n        <
+0016b760: 6469 7620 636c 6173 733d 2261 7070 2d74  div class="app-t
+0016b770: 6974 6c65 223e 5c6e 2020 2020 2020 2020  itle">\n        
+0016b780: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0016b790: 6170 702d 6672 616d 6520 6170 702d 7061  app-frame app-pa
+0016b7a0: 6420 6170 702d 666c 7573 682d 626f 7474  d app-flush-bott
+0016b7b0: 6f6d 223e 5c6e 2020 2020 2020 2020 2020  om">\n          
+0016b7c0: 2020 2020 2020 3c68 313e 5c6e 2020 2020        <h1>\n    
+0016b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016b7e0: 3c73 7061 6e20 636c 6173 733d 2262 7265  <span class="bre
+0016b7f0: 616b 223e 7b7b 206d 6f64 656c 2e6e 616d  ak">{{ model.nam
+0016b800: 6520 7d7d 3c2f 7370 616e 3e5c 6e20 2020  e }}</span>\n   
+0016b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016b820: 203c 736d 616c 6c3e 7465 7374 3c2f 736d   <small>test</sm
+0016b830: 616c 6c3e 5c6e 2020 2020 2020 2020 2020  all>\n          
+0016b840: 2020 2020 2020 3c2f 6831 3e5c 6e20 2020        </h1>\n   
+0016b850: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
+0016b860: 6e20 2020 2020 2020 203c 2f64 6976 3e5c  n        </div>\
+0016b870: 6e20 2020 2020 2020 203c 6469 7620 636c  n        <div cl
+0016b880: 6173 733d 2261 7070 2d66 7261 6d65 2061  ass="app-frame a
+0016b890: 7070 2d70 6164 2d68 223e 5c6e 2020 2020  pp-pad-h">\n    
+0016b8a0: 2020 2020 2020 2020 3c75 6c20 636c 6173          <ul clas
+0016b8b0: 733d 226e 6176 206e 6176 2d74 6162 7322  s="nav nav-tabs"
+0016b8c0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016b8d0: 2020 203c 6c69 2075 692d 7372 6566 2d61     <li ui-sref-a
+0016b8e0: 6374 6976 653d 5c27 6163 7469 7665 5c27  ctive=\'active\'
+0016b8f0: 3e3c 6120 7569 2d73 7265 663d 2264 6274  ><a ui-sref="dbt
+0016b900: 2e74 6573 7428 7b5c 2723 5c27 3a20 5c27  .test({\'#\': \'
+0016b910: 6465 7363 7269 7074 696f 6e5c 277d 2922  description\'})"
+0016b920: 3e44 6573 6372 6970 7469 6f6e 3c2f 613e  >Description</a>
+0016b930: 3c2f 6c69 3e5c 6e20 2020 2020 2020 2020  </li>\n         
+0016b940: 2020 2020 2020 203c 6c69 2075 692d 7372         <li ui-sr
+0016b950: 6566 2d61 6374 6976 653d 5c27 6163 7469  ef-active=\'acti
+0016b960: 7665 5c27 206e 672d 7368 6f77 203d 2022  ve\' ng-show = "
+0016b970: 7061 7265 6e74 734c 656e 6774 6820 213d  parentsLength !=
+0016b980: 2030 223e 3c61 2075 692d 7372 6566 3d22   0"><a ui-sref="
+0016b990: 6462 742e 7465 7374 287b 5c27 235c 273a  dbt.test({\'#\':
+0016b9a0: 205c 2764 6570 656e 6473 5f6f 6e5c 277d   \'depends_on\'}
+0016b9b0: 2922 3e44 6570 656e 6473 204f 6e3c 2f61  )">Depends On</a
+0016b9c0: 3e3c 2f6c 693e 5c6e 2020 2020 2020 2020  ></li>\n        
+0016b9d0: 2020 2020 2020 2020 3c6c 6920 7569 2d73          <li ui-s
+0016b9e0: 7265 662d 6163 7469 7665 3d5c 2761 6374  ref-active=\'act
+0016b9f0: 6976 655c 273e 3c61 2075 692d 7372 6566  ive\'><a ui-sref
+0016ba00: 3d22 6462 742e 7465 7374 287b 5c27 235c  ="dbt.test({\'#\
+0016ba10: 273a 205c 2763 6f64 655c 277d 2922 3e53  ': \'code\'})">S
+0016ba20: 514c 3c2f 613e 3c2f 6c69 3e5c 6e20 2020  QL</a></li>\n   
+0016ba30: 2020 2020 2020 2020 203c 2f75 6c3e 5c6e           </ul>\n
+0016ba40: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
+0016ba50: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
+0016ba60: 3c64 6976 2063 6c61 7373 3d22 6170 702d  <div class="app-
+0016ba70: 6465 7461 696c 7322 3e5c 6e20 2020 2020  details">\n     
+0016ba80: 2020 203c 6469 7620 636c 6173 733d 2261     <div class="a
+0016ba90: 7070 2d66 7261 6d65 2061 7070 2d70 6164  pp-frame app-pad
+0016baa0: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
+0016bab0: 3c73 6563 7469 6f6e 2063 6c61 7373 3d22  <section class="
+0016bac0: 7365 6374 696f 6e22 3e5c 6e20 2020 2020  section">\n     
+0016bad0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0016bae0: 636c 6173 733d 2273 6563 7469 6f6e 2d74  class="section-t
+0016baf0: 6172 6765 7422 2069 643d 2264 6573 6372  arget" id="descr
+0016bb00: 6970 7469 6f6e 223e 3c2f 6469 763e 5c6e  iption"></div>\n
+0016bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016bb20: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
+0016bb30: 696f 6e2d 636f 6e74 656e 7422 3e5c 6e20  ion-content">\n 
+0016bb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016bb50: 2020 203c 6836 3e44 6573 6372 6970 7469     <h6>Descripti
+0016bb60: 6f6e 3c2f 6836 3e5c 6e20 2020 2020 2020  on</h6>\n       
+0016bb70: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0016bb80: 7620 636c 6173 733d 2270 616e 656c 223e  v class="panel">
+0016bb90: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+0016bba0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0016bbb0: 6c61 7373 3d22 7061 6e65 6c2d 626f 6479  lass="panel-body
+0016bbc0: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
+0016bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016bbe0: 3c64 6976 206e 672d 6966 3d22 6d6f 6465  <div ng-if="mode
+0016bbf0: 6c2e 6465 7363 7269 7074 696f 6e22 2063  l.description" c
+0016bc00: 6c61 7373 3d22 6d6f 6465 6c2d 6d61 726b  lass="model-mark
+0016bc10: 646f 776e 2220 6d61 726b 6564 3d22 6d6f  down" marked="mo
+0016bc20: 6465 6c2e 6465 7363 7269 7074 696f 6e22  del.description"
+0016bc30: 3e3c 2f64 6976 3e5c 6e20 2020 2020 2020  ></div>\n       
+0016bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016bc50: 2020 2020 203c 6469 7620 6e67 2d69 663d       <div ng-if=
+0016bc60: 2221 6d6f 6465 6c2e 6465 7363 7269 7074  "!model.descript
+0016bc70: 696f 6e22 3e54 6869 7320 7b7b 206d 6f64  ion">This {{ mod
+0016bc80: 656c 2e72 6573 6f75 7263 655f 7479 7065  el.resource_type
+0016bc90: 207d 7d20 6973 206e 6f74 2063 7572 7265   }} is not curre
+0016bca0: 6e74 6c79 2064 6f63 756d 656e 7465 643c  ntly documented<
+0016bcb0: 2f64 6976 3e5c 6e20 2020 2020 2020 2020  /div>\n         
+0016bcc0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016bcd0: 2f64 6976 3e5c 6e20 2020 2020 2020 2020  /div>\n         
+0016bce0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+0016bcf0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016bd00: 2020 203c 2f64 6976 3e5c 6e20 2020 2020     </div>\n     
+0016bd10: 2020 2020 2020 203c 2f73 6563 7469 6f6e         </section
+0016bd20: 3e5c 6e5c 6e20 2020 2020 2020 2020 2020  >\n\n           
+0016bd30: 203c 7365 6374 696f 6e20 636c 6173 733d   <section class=
+0016bd40: 2273 6563 7469 6f6e 2220 6e67 2d73 686f  "section" ng-sho
+0016bd50: 7720 3d20 2270 6172 656e 7473 4c65 6e67  w = "parentsLeng
+0016bd60: 7468 2021 3d20 3022 3e5c 6e20 2020 2020  th != 0">\n     
+0016bd70: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0016bd80: 636c 6173 733d 2273 6563 7469 6f6e 2d74  class="section-t
+0016bd90: 6172 6765 7422 2069 643d 2264 6570 656e  arget" id="depen
+0016bda0: 6473 5f6f 6e22 3e3c 2f64 6976 3e5c 6e20  ds_on"></div>\n 
+0016bdb0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016bdc0: 6469 7620 636c 6173 733d 2273 6563 7469  div class="secti
+0016bdd0: 6f6e 2d63 6f6e 7465 6e74 223e 5c6e 2020  on-content">\n  
+0016bde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016bdf0: 2020 3c68 363e 4465 7065 6e64 7320 4f6e    <h6>Depends On
+0016be00: 3c2f 6836 3e5c 6e20 2020 2020 2020 2020  </h6>\n         
+0016be10: 2020 2020 2020 2020 2020 203c 7265 6665             <refe
+0016be20: 7265 6e63 652d 6c69 7374 2072 6566 6572  rence-list refer
+0016be30: 656e 6365 733d 2270 6172 656e 7473 2220  ences="parents" 
+0016be40: 6e6f 6465 3d22 6d6f 6465 6c22 202f 3e5c  node="model" />\
+0016be50: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016be60: 203c 2f64 6976 3e5c 6e20 2020 2020 2020   </div>\n       
+0016be70: 2020 2020 203c 2f73 6563 7469 6f6e 3e5c       </section>\
+0016be80: 6e5c 6e20 2020 2020 2020 2020 2020 203c  n\n            <
+0016be90: 7365 6374 696f 6e20 636c 6173 733d 2273  section class="s
+0016bea0: 6563 7469 6f6e 223e 5c6e 2020 2020 2020  ection">\n      
+0016beb0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0016bec0: 6c61 7373 3d22 7365 6374 696f 6e2d 7461  lass="section-ta
+0016bed0: 7267 6574 2220 6964 3d22 636f 6465 223e  rget" id="code">
+0016bee0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
+0016bef0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0016bf00: 7373 3d22 7365 6374 696f 6e2d 636f 6e74  ss="section-cont
+0016bf10: 656e 7422 3e5c 6e20 2020 2020 2020 2020  ent">\n         
+0016bf20: 2020 2020 2020 2020 2020 203c 636f 6465             <code
+0016bf30: 2d62 6c6f 636b 2076 6572 7369 6f6e 733d  -block versions=
+0016bf40: 2276 6572 7369 6f6e 7322 2064 6566 6175  "versions" defau
+0016bf50: 6c74 3d22 6465 6661 756c 745f 7665 7273  lt="default_vers
+0016bf60: 696f 6e22 206c 616e 6775 6167 653d 226c  ion" language="l
+0016bf70: 616e 6775 6167 6522 3e3c 2f63 6f64 652d  anguage"></code-
+0016bf80: 626c 6f63 6b3e 5c6e 2020 2020 2020 2020  block>\n        
+0016bf90: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
+0016bfa0: 2020 2020 2020 2020 2020 2020 3c2f 7365              </se
+0016bfb0: 6374 696f 6e3e 5c6e 2020 2020 2020 2020  ction>\n        
+0016bfc0: 3c2f 6469 763e 5c6e 2020 2020 3c2f 6469  </div>\n    </di
+0016bfd0: 763e 5c6e 3c2f 6469 763e 5c6e 2729 7d5d  v>\n</div>\n')}]
+0016bfe0: 292c 652e 6578 706f 7274 733d 6e7d 2c66  ),e.exports=n},f
+0016bff0: 756e 6374 696f 6e28 652c 7429 7b76 6172  unction(e,t){var
+0016c000: 206e 3d22 2f64 6f63 732f 616e 616c 7973   n="/docs/analys
+0016c010: 6973 2e68 746d 6c22 3b77 696e 646f 772e  is.html";window.
+0016c020: 616e 6775 6c61 722e 6d6f 6475 6c65 2822  angular.module("
+0016c030: 6e67 2229 2e72 756e 285b 2224 7465 6d70  ng").run(["$temp
+0016c040: 6c61 7465 4361 6368 6522 2c66 756e 6374  lateCache",funct
+0016c050: 696f 6e28 6529 7b65 2e70 7574 286e 2c27  ion(e){e.put(n,'
+0016c060: 3c73 7479 6c65 3e5c 6e2f 2a20 544f 444f  <style>\n/* TODO
+0016c070: 202a 2f5c 6e2e 7365 6374 696f 6e2d 7461   */\n.section-ta
+0016c080: 7267 6574 207b 5c6e 2020 2020 746f 703a  rget {\n    top:
+0016c090: 202d 3865 6d3b 5c6e 7d5c 6e5c 6e2e 6e6f   -8em;\n}\n\n.no
+0016c0a0: 666c 6578 207b 5c6e 2020 2020 666c 6578  flex {\n    flex
+0016c0b0: 3a20 3020 3020 3136 3070 7820 2169 6d70  : 0 0 160px !imp
+0016c0c0: 6f72 7461 6e74 3b5c 6e7d 5c6e 5c6e 2e68  ortant;\n}\n\n.h
+0016c0d0: 6967 686c 6967 6874 207b 5c6e 2020 2020  ighlight {\n    
+0016c0e0: 636f 6c6f 723a 2023 3234 3239 3265 3b5c  color: #24292e;\
+0016c0f0: 6e20 2020 2062 6163 6b67 726f 756e 642d  n    background-
+0016c100: 636f 6c6f 723a 2077 6869 7465 3b5c 6e7d  color: white;\n}
+0016c110: 5c6e 5c6e 3c2f 7374 796c 653e 5c6e 5c6e  \n\n</style>\n\n
+0016c120: 3c64 6976 2063 6c61 7373 3d5c 2761 7070  <div class=\'app
+0016c130: 2d73 6372 6f6c 6c5c 273e 5c6e 2020 2020  -scroll\'>\n    
+0016c140: 3c64 6976 2063 6c61 7373 3d22 6170 702d  <div class="app-
+0016c150: 6c69 6e6b 7320 6170 702d 7374 6963 6b79  links app-sticky
+0016c160: 223e 5c6e 2020 2020 2020 2020 3c64 6976  ">\n        <div
+0016c170: 2063 6c61 7373 3d22 6170 702d 7469 746c   class="app-titl
+0016c180: 6522 3e5c 6e20 2020 2020 2020 2020 2020  e">\n           
+0016c190: 203c 6469 7620 636c 6173 733d 2261 7070   <div class="app
+0016c1a0: 2d66 7261 6d65 2061 7070 2d70 6164 2061  -frame app-pad a
+0016c1b0: 7070 2d66 6c75 7368 2d62 6f74 746f 6d22  pp-flush-bottom"
+0016c1c0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016c1d0: 2020 203c 6831 206e 672d 6966 3d22 6d6f     <h1 ng-if="mo
+0016c1e0: 6465 6c2e 646f 6373 2e73 686f 7720 3d3d  del.docs.show ==
+0016c1f0: 3d20 6661 6c73 6522 3e5c 6e20 2020 2020  = false">\n     
+0016c200: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016c210: 736d 616c 6c20 636c 6173 733d 5c27 7465  small class=\'te
+0016c220: 7874 2d62 6f6c 6420 7465 7874 2d72 6967  xt-bold text-rig
+0016c230: 6874 5c27 3e5c 6e20 2020 2020 2020 2020  ht\'>\n         
+0016c240: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016c250: 6920 6461 7461 2d69 636f 6e3d 2265 7965  i data-icon="eye
+0016c260: 223e 3c2f 693e 5c6e 2020 2020 2020 2020  "></i>\n        
+0016c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016c280: 5468 6973 207b 7b20 6d6f 6465 6c2e 7265  This {{ model.re
+0016c290: 736f 7572 6365 5f74 7970 6520 7d7d 2069  source_type }} i
+0016c2a0: 7320 6869 6464 656e 5c6e 2020 2020 2020  s hidden\n      
+0016c2b0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+0016c2c0: 736d 616c 6c3e 5c6e 2020 2020 2020 2020  small>\n        
+0016c2d0: 2020 2020 2020 2020 3c2f 6831 3e5c 6e20          </h1>\n 
+0016c2e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016c2f0: 6831 3e5c 6e20 2020 2020 2020 2020 2020  h1>\n           
+0016c300: 2020 2020 2020 2020 203c 7370 616e 2063           <span c
+0016c310: 6c61 7373 3d22 6272 6561 6b22 3e7b 7b20  lass="break">{{ 
+0016c320: 6d6f 6465 6c2e 6e61 6d65 207d 7d3c 2f73  model.name }}</s
+0016c330: 7061 6e3e 5c6e 2020 2020 2020 2020 2020  pan>\n          
+0016c340: 2020 2020 2020 2020 2020 3c73 6d61 6c6c            <small
+0016c350: 3e41 6e61 6c79 7369 733c 2f73 6d61 6c6c  >Analysis</small
+0016c360: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016c370: 2020 203c 2f68 313e 5c6e 2020 2020 2020     </h1>\n      
+0016c380: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
+0016c390: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
+0016c3a0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0016c3b0: 3d22 6170 702d 6672 616d 6520 6170 702d  ="app-frame app-
+0016c3c0: 7061 642d 6822 3e5c 6e20 2020 2020 2020  pad-h">\n       
+0016c3d0: 2020 2020 203c 756c 2063 6c61 7373 3d22       <ul class="
+0016c3e0: 6e61 7620 6e61 762d 7461 6273 223e 5c6e  nav nav-tabs">\n
+0016c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016c400: 3c6c 6920 7569 2d73 7265 662d 6163 7469  <li ui-sref-acti
+0016c410: 7665 3d5c 2761 6374 6976 655c 273e 3c61  ve=\'active\'><a
+0016c420: 2075 692d 7372 6566 3d22 6462 742e 616e   ui-sref="dbt.an
+0016c430: 616c 7973 6973 287b 5c27 235c 273a 205c  alysis({\'#\': \
+0016c440: 2764 6573 6372 6970 7469 6f6e 5c27 7d29  'description\'})
+0016c450: 223e 4465 7363 7269 7074 696f 6e3c 2f61  ">Description</a
+0016c460: 3e3c 2f6c 693e 5c6e 2020 2020 2020 2020  ></li>\n        
+0016c470: 2020 2020 2020 2020 3c6c 6920 7569 2d73          <li ui-s
+0016c480: 7265 662d 6163 7469 7665 3d5c 2761 6374  ref-active=\'act
+0016c490: 6976 655c 2720 6e67 2d73 686f 7720 3d20  ive\' ng-show = 
+0016c4a0: 2270 6172 656e 7473 4c65 6e67 7468 2021  "parentsLength !
+0016c4b0: 3d20 3022 3e3c 6120 7569 2d73 7265 663d  = 0"><a ui-sref=
+0016c4c0: 2264 6274 2e61 6e61 6c79 7369 7328 7b5c  "dbt.analysis({\
+0016c4d0: 2723 5c27 3a20 5c27 6465 7065 6e64 735f  '#\': \'depends_
+0016c4e0: 6f6e 5c27 7d29 223e 4465 7065 6e64 7320  on\'})">Depends 
+0016c4f0: 4f6e 3c2f 613e 3c2f 6c69 3e5c 6e20 2020  On</a></li>\n   
+0016c500: 2020 2020 2020 2020 2020 2020 203c 6c69               <li
+0016c510: 2075 692d 7372 6566 2d61 6374 6976 653d   ui-sref-active=
+0016c520: 5c27 6163 7469 7665 5c27 3e3c 6120 7569  \'active\'><a ui
+0016c530: 2d73 7265 663d 2264 6274 2e61 6e61 6c79  -sref="dbt.analy
+0016c540: 7369 7328 7b5c 2723 5c27 3a20 5c27 7371  sis({\'#\': \'sq
+0016c550: 6c5c 277d 2922 3e53 514c 3c2f 613e 3c2f  l\'})">SQL</a></
+0016c560: 6c69 3e5c 6e20 2020 2020 2020 2020 2020  li>\n           
+0016c570: 203c 2f75 6c3e 5c6e 2020 2020 2020 2020   </ul>\n        
+0016c580: 3c2f 6469 763e 5c6e 2020 2020 3c2f 6469  </div>\n    </di
+0016c590: 763e 5c6e 2020 2020 3c64 6976 2063 6c61  v>\n    <div cla
+0016c5a0: 7373 3d22 6170 702d 6465 7461 696c 7322  ss="app-details"
+0016c5b0: 3e5c 6e20 2020 2020 2020 203c 6469 7620  >\n        <div 
+0016c5c0: 636c 6173 733d 2261 7070 2d66 7261 6d65  class="app-frame
+0016c5d0: 2061 7070 2d70 6164 223e 5c6e 5c6e 2020   app-pad">\n\n  
+0016c5e0: 2020 2020 2020 2020 2020 3c73 6563 7469            <secti
+0016c5f0: 6f6e 2063 6c61 7373 3d22 7365 6374 696f  on class="sectio
+0016c600: 6e22 3e5c 6e20 2020 2020 2020 2020 2020  n">\n           
+0016c610: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0016c620: 2273 6563 7469 6f6e 2d74 6172 6765 7422  "section-target"
+0016c630: 2069 643d 2264 6573 6372 6970 7469 6f6e   id="description
+0016c640: 223e 3c2f 6469 763e 5c6e 2020 2020 2020  "></div>\n      
+0016c650: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0016c660: 6c61 7373 3d22 7365 6374 696f 6e2d 636f  lass="section-co
+0016c670: 6e74 656e 7422 3e5c 6e20 2020 2020 2020  ntent">\n       
+0016c680: 2020 2020 2020 2020 2020 2020 203c 6836               <h6
+0016c690: 3e44 6573 6372 6970 7469 6f6e 3c2f 6836  >Description</h6
+0016c6a0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016c6b0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0016c6c0: 733d 2270 616e 656c 223e 5c6e 2020 2020  s="panel">\n    
+0016c6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016c6e0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0016c6f0: 7061 6e65 6c2d 626f 6479 223e 5c6e 2020  panel-body">\n  
+0016c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016c710: 2020 2020 2020 2020 2020 3c64 6976 206e            <div n
+0016c720: 672d 6966 3d22 6d6f 6465 6c2e 6465 7363  g-if="model.desc
+0016c730: 7269 7074 696f 6e22 2063 6c61 7373 3d22  ription" class="
+0016c740: 6d6f 6465 6c2d 6d61 726b 646f 776e 2220  model-markdown" 
+0016c750: 6d61 726b 6564 3d22 6d6f 6465 6c2e 6465  marked="model.de
+0016c760: 7363 7269 7074 696f 6e22 3e3c 2f64 6976  scription"></div
+0016c770: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016c780: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016c790: 6469 7620 6e67 2d69 663d 2221 6d6f 6465  div ng-if="!mode
+0016c7a0: 6c2e 6465 7363 7269 7074 696f 6e22 3e54  l.description">T
+0016c7b0: 6869 7320 7b7b 206d 6f64 656c 2e72 6573  his {{ model.res
+0016c7c0: 6f75 7263 655f 7479 7065 207d 7d20 6973  ource_type }} is
+0016c7d0: 206e 6f74 2063 7572 7265 6e74 6c79 2064   not currently d
+0016c7e0: 6f63 756d 656e 7465 643c 2f64 6976 3e5c  ocumented</div>\
+0016c7f0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016c800: 2020 2020 2020 2020 203c 2f64 6976 3e5c           </div>\
+0016c810: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016c820: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
+0016c830: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+0016c840: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
+0016c850: 203c 2f73 6563 7469 6f6e 3e5c 6e5c 6e20   </section>\n\n 
+0016c860: 2020 2020 2020 2020 2020 203c 7365 6374             <sect
+0016c870: 696f 6e20 636c 6173 733d 2273 6563 7469  ion class="secti
+0016c880: 6f6e 2220 6e67 2d73 686f 7720 3d20 2270  on" ng-show = "p
+0016c890: 6172 656e 7473 4c65 6e67 7468 2021 3d20  arentsLength != 
+0016c8a0: 3022 3e5c 6e20 2020 2020 2020 2020 2020  0">\n           
+0016c8b0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0016c8c0: 2273 6563 7469 6f6e 2d74 6172 6765 7422  "section-target"
+0016c8d0: 2069 643d 2264 6570 656e 6473 5f6f 6e22   id="depends_on"
+0016c8e0: 3e3c 2f64 6976 3e5c 6e20 2020 2020 2020  ></div>\n       
+0016c8f0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0016c900: 6173 733d 2273 6563 7469 6f6e 2d63 6f6e  ass="section-con
+0016c910: 7465 6e74 223e 5c6e 2020 2020 2020 2020  tent">\n        
+0016c920: 2020 2020 2020 2020 2020 2020 3c68 363e              <h6>
+0016c930: 4465 7065 6e64 7320 4f6e 3c2f 6836 3e5c  Depends On</h6>\
+0016c940: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016c950: 2020 2020 203c 7265 6665 7265 6e63 652d       <reference-
+0016c960: 6c69 7374 2072 6566 6572 656e 6365 733d  list references=
+0016c970: 2270 6172 656e 7473 2220 2f3e 5c6e 2020  "parents" />\n  
+0016c980: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+0016c990: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
+0016c9a0: 2020 3c2f 7365 6374 696f 6e3e 5c6e 5c6e    </section>\n\n
+0016c9b0: 2020 2020 2020 2020 2020 2020 3c73 6563              <sec
+0016c9c0: 7469 6f6e 2063 6c61 7373 3d22 7365 6374  tion class="sect
+0016c9d0: 696f 6e22 3e5c 6e20 2020 2020 2020 2020  ion">\n         
+0016c9e0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0016c9f0: 733d 2273 6563 7469 6f6e 2d74 6172 6765  s="section-targe
+0016ca00: 7422 2069 643d 2273 716c 223e 3c2f 6469  t" id="sql"></di
+0016ca10: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
+0016ca20: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0016ca30: 7365 6374 696f 6e2d 636f 6e74 656e 7422  section-content"
+0016ca40: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016ca50: 2020 2020 2020 203c 636f 6465 2d62 6c6f         <code-blo
+0016ca60: 636b 2076 6572 7369 6f6e 733d 2276 6572  ck versions="ver
+0016ca70: 7369 6f6e 7322 2064 6566 6175 6c74 3d22  sions" default="
+0016ca80: 6465 6661 756c 745f 7665 7273 696f 6e22  default_version"
+0016ca90: 206c 616e 6775 6167 653d 226c 616e 6775   language="langu
+0016caa0: 6167 6522 3e3c 2f63 6f64 652d 626c 6f63  age"></code-bloc
+0016cab0: 6b3e 5c6e 2020 2020 2020 2020 2020 2020  k>\n            
+0016cac0: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
+0016cad0: 2020 2020 2020 2020 3c2f 7365 6374 696f          </sectio
+0016cae0: 6e3e 5c6e 2020 2020 2020 2020 3c2f 6469  n>\n        </di
+0016caf0: 763e 5c6e 2020 2020 3c2f 6469 763e 5c6e  v>\n    </div>\n
+0016cb00: 3c2f 6469 763e 5c6e 2729 7d5d 292c 652e  </div>\n')}]),e.
+0016cb10: 6578 706f 7274 733d 6e7d 2c66 756e 6374  exports=n},funct
+0016cb20: 696f 6e28 652c 7429 7b76 6172 206e 3d22  ion(e,t){var n="
+0016cb30: 2f64 6f63 732f 6d61 6372 6f2e 6874 6d6c  /docs/macro.html
+0016cb40: 223b 7769 6e64 6f77 2e61 6e67 756c 6172  ";window.angular
+0016cb50: 2e6d 6f64 756c 6528 226e 6722 292e 7275  .module("ng").ru
+0016cb60: 6e28 5b22 2474 656d 706c 6174 6543 6163  n(["$templateCac
+0016cb70: 6865 222c 6675 6e63 7469 6f6e 2865 297b  he",function(e){
+0016cb80: 652e 7075 7428 6e2c 273c 7374 796c 653e  e.put(n,'<style>
+0016cb90: 5c6e 2f2a 2054 4f44 4f20 2a2f 5c6e 2e73  \n/* TODO */\n.s
+0016cba0: 6563 7469 6f6e 2d74 6172 6765 7420 7b5c  ection-target {\
+0016cbb0: 6e20 2020 2074 6f70 3a20 2d38 656d 3b5c  n    top: -8em;\
+0016cbc0: 6e7d 5c6e 5c6e 2e6e 6f66 6c65 7820 7b5c  n}\n\n.noflex {\
+0016cbd0: 6e20 2020 2066 6c65 783a 2030 2030 2031  n    flex: 0 0 1
+0016cbe0: 3630 7078 2021 696d 706f 7274 616e 743b  60px !important;
+0016cbf0: 5c6e 7d5c 6e5c 6e2e 6869 6768 6c69 6768  \n}\n\n.highligh
+0016cc00: 7420 7b5c 6e20 2020 2063 6f6c 6f72 3a20  t {\n    color: 
+0016cc10: 2332 3432 3932 653b 5c6e 2020 2020 6261  #24292e;\n    ba
+0016cc20: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a20  ckground-color: 
+0016cc30: 7768 6974 653b 5c6e 7d5c 6e5c 6e3c 2f73  white;\n}\n\n</s
+0016cc40: 7479 6c65 3e5c 6e5c 6e3c 6469 7620 636c  tyle>\n\n<div cl
+0016cc50: 6173 733d 5c27 6170 702d 7363 726f 6c6c  ass=\'app-scroll
+0016cc60: 5c27 3e5c 6e20 2020 203c 6469 7620 636c  \'>\n    <div cl
+0016cc70: 6173 733d 2261 7070 2d6c 696e 6b73 2061  ass="app-links a
+0016cc80: 7070 2d73 7469 636b 7922 3e5c 6e20 2020  pp-sticky">\n   
+0016cc90: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0016cca0: 2261 7070 2d74 6974 6c65 223e 5c6e 2020  "app-title">\n  
+0016ccb0: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0016ccc0: 6c61 7373 3d22 6170 702d 6672 616d 6520  lass="app-frame 
+0016ccd0: 6170 702d 7061 6420 6170 702d 666c 7573  app-pad app-flus
+0016cce0: 682d 626f 7474 6f6d 223e 5c6e 2020 2020  h-bottom">\n    
+0016ccf0: 2020 2020 2020 2020 2020 2020 3c68 313e              <h1>
+0016cd00: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+0016cd10: 2020 2020 2020 3c73 7061 6e20 636c 6173        <span clas
+0016cd20: 733d 2262 7265 616b 223e 7b7b 206d 6163  s="break">{{ mac
+0016cd30: 726f 2e70 6163 6b61 6765 5f6e 616d 6520  ro.package_name 
+0016cd40: 7d7d 2e7b 7b20 6d61 6372 6f2e 6e61 6d65  }}.{{ macro.name
+0016cd50: 207d 7d3c 2f73 7061 6e3e 5c6e 2020 2020   }}</span>\n    
+0016cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016cd70: 3c73 6d61 6c6c 206e 672d 6966 3d22 6d61  <small ng-if="ma
+0016cd80: 6372 6f2e 6973 5f61 6461 7074 6572 5f6d  cro.is_adapter_m
+0016cd90: 6163 726f 223e 6164 6170 7465 7220 6d61  acro">adapter ma
+0016cda0: 6372 6f3c 2f73 6d61 6c6c 3e5c 6e20 2020  cro</small>\n   
+0016cdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016cdc0: 203c 736d 616c 6c20 6e67 2d69 663d 2221   <small ng-if="!
+0016cdd0: 6d61 6372 6f2e 6973 5f61 6461 7074 6572  macro.is_adapter
+0016cde0: 5f6d 6163 726f 223e 6d61 6372 6f3c 2f73  _macro">macro</s
+0016cdf0: 6d61 6c6c 3e5c 6e20 2020 2020 2020 2020  mall>\n         
+0016ce00: 2020 2020 2020 203c 2f68 313e 5c6e 2020         </h1>\n  
+0016ce10: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+0016ce20: 5c6e 2020 2020 2020 2020 3c2f 6469 763e  \n        </div>
+0016ce30: 5c6e 2020 2020 2020 2020 3c64 6976 2063  \n        <div c
+0016ce40: 6c61 7373 3d22 6170 702d 6672 616d 6520  lass="app-frame 
+0016ce50: 6170 702d 7061 642d 6822 3e5c 6e20 2020  app-pad-h">\n   
+0016ce60: 2020 2020 2020 2020 203c 756c 2063 6c61           <ul cla
+0016ce70: 7373 3d22 6e61 7620 6e61 762d 7461 6273  ss="nav nav-tabs
+0016ce80: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
+0016ce90: 2020 2020 3c6c 6920 7569 2d73 7265 662d      <li ui-sref-
+0016cea0: 6163 7469 7665 3d5c 2761 6374 6976 655c  active=\'active\
+0016ceb0: 273e 3c61 2075 692d 7372 6566 3d22 6462  '><a ui-sref="db
+0016cec0: 742e 6d61 6372 6f28 7b5c 2723 5c27 3a20  t.macro({\'#\': 
+0016ced0: 5c27 6465 7363 7269 7074 696f 6e5c 277d  \'description\'}
+0016cee0: 2922 3e44 6573 6372 6970 7469 6f6e 3c2f  )">Description</
+0016cef0: 613e 3c2f 6c69 3e5c 6e20 2020 2020 2020  a></li>\n       
+0016cf00: 2020 2020 2020 2020 203c 6c69 2075 692d           <li ui-
+0016cf10: 7372 6566 2d61 6374 6976 653d 5c27 6163  sref-active=\'ac
+0016cf20: 7469 7665 5c27 3e3c 6120 7569 2d73 7265  tive\'><a ui-sre
+0016cf30: 663d 2264 6274 2e6d 6163 726f 287b 5c27  f="dbt.macro({\'
+0016cf40: 235c 273a 205c 2761 7267 756d 656e 7473  #\': \'arguments
+0016cf50: 5c27 7d29 223e 4172 6775 6d65 6e74 733c  \'})">Arguments<
+0016cf60: 2f61 3e3c 2f6c 693e 5c6e 2020 2020 2020  /a></li>\n      
+0016cf70: 2020 2020 2020 2020 2020 3c6c 6920 7569            <li ui
+0016cf80: 2d73 7265 662d 6163 7469 7665 3d5c 2761  -sref-active=\'a
+0016cf90: 6374 6976 655c 2720 6e67 2d73 686f 7720  ctive\' ng-show 
+0016cfa0: 3d20 2272 6566 6572 656e 6365 734c 656e  = "referencesLen
+0016cfb0: 6774 6820 213d 2030 223e 3c61 2075 692d  gth != 0"><a ui-
+0016cfc0: 7372 6566 3d22 6462 742e 6d61 6372 6f28  sref="dbt.macro(
+0016cfd0: 7b5c 2723 5c27 3a20 5c27 7265 6665 7265  {\'#\': \'refere
+0016cfe0: 6e63 6564 5f62 795c 277d 2922 3e52 6566  nced_by\'})">Ref
+0016cff0: 6572 656e 6365 6420 4279 3c2f 613e 3c2f  erenced By</a></
+0016d000: 6c69 3e5c 6e20 2020 2020 2020 2020 2020  li>\n           
+0016d010: 2020 2020 203c 6c69 2075 692d 7372 6566       <li ui-sref
+0016d020: 2d61 6374 6976 653d 5c27 6163 7469 7665  -active=\'active
+0016d030: 5c27 206e 672d 7368 6f77 203d 2022 7061  \' ng-show = "pa
+0016d040: 7265 6e74 734c 656e 6774 6820 213d 2030  rentsLength != 0
+0016d050: 223e 3c61 2075 692d 7372 6566 3d22 6462  "><a ui-sref="db
+0016d060: 742e 6d61 6372 6f28 7b5c 2723 5c27 3a20  t.macro({\'#\': 
+0016d070: 5c27 6465 7065 6e64 735f 6f6e 5c27 7d29  \'depends_on\'})
+0016d080: 223e 4465 7065 6e64 7320 4f6e 3c2f 613e  ">Depends On</a>
+0016d090: 3c2f 6c69 3e5c 6e20 2020 2020 2020 2020  </li>\n         
+0016d0a0: 2020 2020 2020 203c 6c69 2075 692d 7372         <li ui-sr
+0016d0b0: 6566 2d61 6374 6976 653d 5c27 6163 7469  ef-active=\'acti
+0016d0c0: 7665 5c27 3e3c 6120 7569 2d73 7265 663d  ve\'><a ui-sref=
+0016d0d0: 2264 6274 2e6d 6163 726f 287b 5c27 235c  "dbt.macro({\'#\
+0016d0e0: 273a 205c 2763 6f64 655c 277d 2922 3e43  ': \'code\'})">C
+0016d0f0: 6f64 653c 2f61 3e3c 2f6c 693e 5c6e 2020  ode</a></li>\n  
+0016d100: 2020 2020 2020 2020 2020 3c2f 756c 3e5c            </ul>\
+0016d110: 6e20 2020 2020 2020 203c 2f64 6976 3e5c  n        </div>\
+0016d120: 6e20 2020 203c 2f64 6976 3e5c 6e20 2020  n    </div>\n   
+0016d130: 203c 6469 7620 636c 6173 733d 2261 7070   <div class="app
+0016d140: 2d64 6574 6169 6c73 223e 5c6e 2020 2020  -details">\n    
+0016d150: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0016d160: 6170 702d 6672 616d 6520 6170 702d 7061  app-frame app-pa
+0016d170: 6422 3e5c 6e20 2020 2020 2020 2020 2020  d">\n           
+0016d180: 203c 7365 6374 696f 6e20 636c 6173 733d   <section class=
+0016d190: 2273 6563 7469 6f6e 223e 5c6e 2020 2020  "section">\n    
+0016d1a0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0016d1b0: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
+0016d1c0: 7461 7267 6574 2220 6964 3d22 6465 7363  target" id="desc
+0016d1d0: 7269 7074 696f 6e22 3e3c 2f64 6976 3e5c  ription"></div>\
+0016d1e0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016d1f0: 203c 6469 7620 636c 6173 733d 2273 6563   <div class="sec
+0016d200: 7469 6f6e 2d63 6f6e 7465 6e74 223e 5c6e  tion-content">\n
+0016d210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d220: 2020 2020 3c68 363e 4465 7363 7269 7074      <h6>Descript
+0016d230: 696f 6e3c 2f68 363e 5c6e 2020 2020 2020  ion</h6>\n      
+0016d240: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+0016d250: 6976 2063 6c61 7373 3d22 7061 6e65 6c22  iv class="panel"
+0016d260: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016d270: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0016d280: 636c 6173 733d 2270 616e 656c 2d62 6f64  class="panel-bod
+0016d290: 7922 3e5c 6e20 2020 2020 2020 2020 2020  y">\n           
+0016d2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d2b0: 203c 6469 7620 6e67 2d69 663d 226d 6163   <div ng-if="mac
+0016d2c0: 726f 2e64 6573 6372 6970 7469 6f6e 2220  ro.description" 
+0016d2d0: 636c 6173 733d 226d 6f64 656c 2d6d 6172  class="model-mar
+0016d2e0: 6b64 6f77 6e22 206d 6172 6b65 643d 226d  kdown" marked="m
+0016d2f0: 6163 726f 2e64 6573 6372 6970 7469 6f6e  acro.description
+0016d300: 223e 3c2f 6469 763e 5c6e 2020 2020 2020  "></div>\n      
+0016d310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d320: 2020 2020 2020 3c64 6976 206e 672d 6966        <div ng-if
+0016d330: 3d22 216d 6163 726f 2e64 6573 6372 6970  ="!macro.descrip
+0016d340: 7469 6f6e 223e 5468 6973 207b 7b20 6d61  tion">This {{ ma
+0016d350: 6372 6f2e 7265 736f 7572 6365 5f74 7970  cro.resource_typ
+0016d360: 6520 7d7d 2069 7320 6e6f 7420 6375 7272  e }} is not curr
+0016d370: 656e 746c 7920 646f 6375 6d65 6e74 6564  ently documented
+0016d380: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
+0016d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d3a0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
+0016d3b0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+0016d3c0: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
+0016d3d0: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
+0016d3e0: 2020 2020 2020 2020 3c2f 7365 6374 696f          </sectio
+0016d3f0: 6e3e 5c6e 5c6e 2020 2020 2020 2020 2020  n>\n\n          
+0016d400: 2020 3c73 6563 7469 6f6e 2063 6c61 7373    <section class
+0016d410: 3d22 7365 6374 696f 6e22 3e5c 6e20 2020  ="section">\n   
+0016d420: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0016d430: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
+0016d440: 2d74 6172 6765 7422 2069 643d 2261 7267  -target" id="arg
+0016d450: 756d 656e 7473 223e 3c2f 6469 763e 5c6e  uments"></div>\n
+0016d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d470: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
+0016d480: 696f 6e2d 636f 6e74 656e 7422 3e5c 6e20  ion-content">\n 
+0016d490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d4a0: 2020 203c 6836 3e41 7267 756d 656e 7473     <h6>Arguments
+0016d4b0: 3c2f 6836 3e5c 6e20 2020 2020 2020 2020  </h6>\n         
+0016d4c0: 2020 2020 2020 2020 2020 203c 6d61 6372             <macr
+0016d4d0: 6f2d 6172 6775 6d65 6e74 7320 6d61 6372  o-arguments macr
+0016d4e0: 6f3d 226d 6163 726f 223e 3c2f 6d61 6372  o="macro"></macr
+0016d4f0: 6f2d 6172 6775 6d65 6e74 733e 5c6e 2020  o-arguments>\n  
+0016d500: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+0016d510: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
+0016d520: 2020 3c2f 7365 6374 696f 6e3e 5c6e 5c6e    </section>\n\n
+0016d530: 2020 2020 2020 2020 2020 2020 3c73 6563              <sec
+0016d540: 7469 6f6e 2063 6c61 7373 3d22 7365 6374  tion class="sect
+0016d550: 696f 6e22 206e 672d 7368 6f77 203d 2022  ion" ng-show = "
+0016d560: 7265 6665 7265 6e63 6573 4c65 6e67 7468  referencesLength
+0016d570: 2021 3d20 3022 3e5c 6e20 2020 2020 2020   != 0">\n       
+0016d580: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0016d590: 6173 733d 2273 6563 7469 6f6e 2d74 6172  ass="section-tar
+0016d5a0: 6765 7422 2069 643d 2272 6566 6572 656e  get" id="referen
+0016d5b0: 6365 645f 6279 223e 3c2f 6469 763e 5c6e  ced_by"></div>\n
+0016d5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d5d0: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
+0016d5e0: 696f 6e2d 636f 6e74 656e 7422 3e5c 6e20  ion-content">\n 
+0016d5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d600: 2020 203c 6836 3e52 6566 6572 656e 6365     <h6>Reference
+0016d610: 6420 4279 3c2f 6836 3e5c 6e20 2020 2020  d By</h6>\n     
+0016d620: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016d630: 7265 6665 7265 6e63 652d 6c69 7374 2072  reference-list r
+0016d640: 6566 6572 656e 6365 733d 2272 6566 6572  eferences="refer
+0016d650: 656e 6365 7322 206e 6f64 653d 226d 6163  ences" node="mac
+0016d660: 726f 2220 2f3e 5c6e 2020 2020 2020 2020  ro" />\n        
+0016d670: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
+0016d680: 2020 2020 2020 2020 2020 2020 3c2f 7365              </se
+0016d690: 6374 696f 6e3e 5c6e 5c6e 2020 2020 2020  ction>\n\n      
+0016d6a0: 2020 2020 2020 3c73 6563 7469 6f6e 2063        <section c
+0016d6b0: 6c61 7373 3d22 7365 6374 696f 6e22 206e  lass="section" n
+0016d6c0: 672d 7368 6f77 203d 2022 7061 7265 6e74  g-show = "parent
+0016d6d0: 734c 656e 6774 6820 213d 2030 223e 5c6e  sLength != 0">\n
+0016d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d6f0: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
+0016d700: 696f 6e2d 7461 7267 6574 2220 6964 3d22  ion-target" id="
+0016d710: 6465 7065 6e64 735f 6f6e 223e 3c2f 6469  depends_on"></di
+0016d720: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
+0016d730: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0016d740: 7365 6374 696f 6e2d 636f 6e74 656e 7422  section-content"
+0016d750: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016d760: 2020 2020 2020 203c 6836 3e44 6570 656e         <h6>Depen
+0016d770: 6473 204f 6e3c 2f68 363e 5c6e 2020 2020  ds On</h6>\n    
+0016d780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d790: 3c72 6566 6572 656e 6365 2d6c 6973 7420  <reference-list 
+0016d7a0: 7265 6665 7265 6e63 6573 3d22 7061 7265  references="pare
+0016d7b0: 6e74 7322 206e 6f64 653d 226d 6163 726f  nts" node="macro
+0016d7c0: 2220 2f3e 5c6e 2020 2020 2020 2020 2020  " />\n          
+0016d7d0: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
+0016d7e0: 2020 2020 2020 2020 2020 3c2f 7365 6374            </sect
+0016d7f0: 696f 6e3e 5c6e 5c6e 2020 2020 2020 2020  ion>\n\n        
+0016d800: 2020 2020 3c73 6563 7469 6f6e 2063 6c61      <section cla
+0016d810: 7373 3d22 7365 6374 696f 6e22 3e5c 6e20  ss="section">\n 
+0016d820: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016d830: 6469 7620 636c 6173 733d 2273 6563 7469  div class="secti
+0016d840: 6f6e 2d74 6172 6765 7422 2069 643d 2263  on-target" id="c
+0016d850: 6f64 6522 3e3c 2f64 6976 3e5c 6e20 2020  ode"></div>\n   
+0016d860: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0016d870: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
+0016d880: 2d63 6f6e 7465 6e74 223e 5c6e 2020 2020  -content">\n    
+0016d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016d8a0: 3c63 6f64 652d 626c 6f63 6b20 7665 7273  <code-block vers
+0016d8b0: 696f 6e73 3d22 7665 7273 696f 6e73 2220  ions="versions" 
+0016d8c0: 6465 6661 756c 743d 2264 6566 6175 6c74  default="default
+0016d8d0: 5f76 6572 7369 6f6e 2220 6c61 6e67 7561  _version" langua
+0016d8e0: 6765 3d22 6c61 6e67 7561 6765 223e 3c2f  ge="language"></
+0016d8f0: 636f 6465 2d62 6c6f 636b 3e5c 6e20 2020  code-block>\n   
+0016d900: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+0016d910: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
+0016d920: 203c 2f73 6563 7469 6f6e 3e5c 6e20 2020   </section>\n   
+0016d930: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
+0016d940: 203c 2f64 6976 3e5c 6e3c 2f64 6976 3e5c   </div>\n</div>\
+0016d950: 6e27 297d 5d29 2c65 2e65 7870 6f72 7473  n')}]),e.exports
+0016d960: 3d6e 7d2c 6675 6e63 7469 6f6e 2865 2c74  =n},function(e,t
+0016d970: 297b 7661 7220 6e3d 222f 646f 6373 2f65  ){var n="/docs/e
+0016d980: 7870 6f73 7572 652e 6874 6d6c 223b 7769  xposure.html";wi
+0016d990: 6e64 6f77 2e61 6e67 756c 6172 2e6d 6f64  ndow.angular.mod
+0016d9a0: 756c 6528 226e 6722 292e 7275 6e28 5b22  ule("ng").run(["
+0016d9b0: 2474 656d 706c 6174 6543 6163 6865 222c  $templateCache",
+0016d9c0: 6675 6e63 7469 6f6e 2865 297b 652e 7075  function(e){e.pu
+0016d9d0: 7428 6e2c 273c 7374 796c 653e 5c6e 2f2a  t(n,'<style>\n/*
+0016d9e0: 2054 4f44 4f20 2a2f 5c6e 2e73 6563 7469   TODO */\n.secti
+0016d9f0: 6f6e 2d74 6172 6765 7420 7b5c 6e20 2020  on-target {\n   
+0016da00: 2074 6f70 3a20 2d38 656d 3b5c 6e7d 5c6e   top: -8em;\n}\n
+0016da10: 5c6e 2e6e 6f66 6c65 7820 7b5c 6e20 2020  \n.noflex {\n   
+0016da20: 2066 6c65 783a 2030 2030 2031 3630 7078   flex: 0 0 160px
+0016da30: 2021 696d 706f 7274 616e 743b 5c6e 7d5c   !important;\n}\
+0016da40: 6e5c 6e2e 6869 6768 6c69 6768 7420 7b5c  n\n.highlight {\
+0016da50: 6e20 2020 2063 6f6c 6f72 3a20 2332 3432  n    color: #242
+0016da60: 3932 653b 5c6e 2020 2020 6261 636b 6772  92e;\n    backgr
+0016da70: 6f75 6e64 2d63 6f6c 6f72 3a20 7768 6974  ound-color: whit
+0016da80: 653b 5c6e 7d5c 6e5c 6e3c 2f73 7479 6c65  e;\n}\n\n</style
+0016da90: 3e5c 6e5c 6e3c 6469 7620 636c 6173 733d  >\n\n<div class=
+0016daa0: 5c27 6170 702d 7363 726f 6c6c 5c27 3e5c  \'app-scroll\'>\
+0016dab0: 6e20 2020 203c 6469 7620 636c 6173 733d  n    <div class=
+0016dac0: 2261 7070 2d6c 696e 6b73 2061 7070 2d73  "app-links app-s
+0016dad0: 7469 636b 7922 3e5c 6e20 2020 2020 2020  ticky">\n       
+0016dae0: 203c 6469 7620 636c 6173 733d 2261 7070   <div class="app
+0016daf0: 2d74 6974 6c65 223e 5c6e 2020 2020 2020  -title">\n      
+0016db00: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0016db10: 3d22 6170 702d 6672 616d 6520 6170 702d  ="app-frame app-
+0016db20: 7061 6420 6170 702d 666c 7573 682d 626f  pad app-flush-bo
+0016db30: 7474 6f6d 223e 5c6e 5c6e 2020 2020 2020  ttom">\n\n      
+0016db40: 2020 2020 2020 2020 2020 3c68 313e 5c6e            <h1>\n
+0016db50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016db60: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
+0016db70: 2262 7265 616b 223e 7b7b 2065 7870 6f73  "break">{{ expos
+0016db80: 7572 652e 6c61 6265 6c20 7d7d 3c2f 7370  ure.label }}</sp
+0016db90: 616e 3e5c 6e20 2020 2020 2020 2020 2020  an>\n           
+0016dba0: 2020 2020 2020 2020 203c 736d 616c 6c3e           <small>
+0016dbb0: 6578 706f 7375 7265 3c2f 736d 616c 6c3e  exposure</small>
+0016dbc0: 5c6e 5c6e 2020 2020 2020 2020 2020 2020  \n\n            
+0016dbd0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0016dbe0: 7373 3d5c 2770 756c 6c2d 7269 6768 745c  ss=\'pull-right\
+0016dbf0: 2720 6e67 2d73 686f 773d 2265 7870 6f73  ' ng-show="expos
+0016dc00: 7572 652e 7572 6c22 3e5c 6e20 2020 2020  ure.url">\n     
+0016dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016dc20: 2020 203c 6120 636c 6173 733d 5c27 6274     <a class=\'bt
+0016dc30: 6e20 7465 7874 2d77 6869 7465 2062 746e  n text-white btn
+0016dc40: 2d70 7269 6d61 7279 2062 746e 2d73 6d5c  -primary btn-sm\
+0016dc50: 2720 6e67 2d68 7265 663d 227b 7b20 6578  ' ng-href="{{ ex
+0016dc60: 706f 7375 7265 2e75 726c 207d 7d22 2074  posure.url }}" t
+0016dc70: 6172 6765 743d 225f 626c 616e 6b22 3e56  arget="_blank">V
+0016dc80: 6965 7720 7468 6973 2065 7870 6f73 7572  iew this exposur
+0016dc90: 653c 2f61 3e5c 6e20 2020 2020 2020 2020  e</a>\n         
+0016dca0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+0016dcb0: 3e5c 6e5c 6e20 2020 2020 2020 2020 2020  >\n\n           
+0016dcc0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0016dcd0: 6173 733d 5c27 636c 6561 7266 6978 5c27  ass=\'clearfix\'
+0016dce0: 3e3c 2f64 6976 3e5c 6e20 2020 2020 2020  ></div>\n       
+0016dcf0: 2020 2020 2020 2020 203c 2f68 313e 5c6e           </h1>\n
+0016dd00: 5c6e 2020 2020 2020 2020 2020 2020 3c2f  \n            </
+0016dd10: 6469 763e 5c6e 2020 2020 2020 2020 3c2f  div>\n        </
+0016dd20: 6469 763e 5c6e 2020 2020 2020 2020 3c64  div>\n        <d
+0016dd30: 6976 2063 6c61 7373 3d22 6170 702d 6672  iv class="app-fr
+0016dd40: 616d 6520 6170 702d 7061 642d 6822 3e5c  ame app-pad-h">\
+0016dd50: 6e20 2020 2020 2020 2020 2020 203c 756c  n            <ul
+0016dd60: 2063 6c61 7373 3d22 6e61 7620 6e61 762d   class="nav nav-
+0016dd70: 7461 6273 223e 5c6e 2020 2020 2020 2020  tabs">\n        
+0016dd80: 2020 2020 2020 2020 3c6c 6920 7569 2d73          <li ui-s
+0016dd90: 7265 662d 6163 7469 7665 3d5c 2761 6374  ref-active=\'act
+0016dda0: 6976 655c 273e 3c61 2075 692d 7372 6566  ive\'><a ui-sref
+0016ddb0: 3d22 6462 742e 6578 706f 7375 7265 287b  ="dbt.exposure({
+0016ddc0: 5c27 235c 273a 205c 2764 6574 6169 6c73  \'#\': \'details
+0016ddd0: 5c27 7d29 223e 4465 7461 696c 733c 2f61  \'})">Details</a
+0016dde0: 3e3c 2f6c 693e 5c6e 2020 2020 2020 2020  ></li>\n        
+0016ddf0: 2020 2020 2020 2020 3c6c 6920 7569 2d73          <li ui-s
+0016de00: 7265 662d 6163 7469 7665 3d5c 2761 6374  ref-active=\'act
+0016de10: 6976 655c 273e 3c61 2075 692d 7372 6566  ive\'><a ui-sref
+0016de20: 3d22 6462 742e 6578 706f 7375 7265 287b  ="dbt.exposure({
+0016de30: 5c27 235c 273a 205c 2764 6573 6372 6970  \'#\': \'descrip
+0016de40: 7469 6f6e 5c27 7d29 223e 4465 7363 7269  tion\'})">Descri
+0016de50: 7074 696f 6e3c 2f61 3e3c 2f6c 693e 5c6e  ption</a></li>\n
+0016de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016de70: 3c6c 6920 7569 2d73 7265 662d 6163 7469  <li ui-sref-acti
+0016de80: 7665 3d5c 2761 6374 6976 655c 2720 6e67  ve=\'active\' ng
+0016de90: 2d73 686f 7720 3d20 2270 6172 656e 7473  -show = "parents
+0016dea0: 4c65 6e67 7468 2021 3d20 3022 3e3c 6120  Length != 0"><a 
+0016deb0: 7569 2d73 7265 663d 2264 6274 2e65 7870  ui-sref="dbt.exp
+0016dec0: 6f73 7572 6528 7b5c 2723 5c27 3a20 5c27  osure({\'#\': \'
+0016ded0: 6465 7065 6e64 735f 6f6e 5c27 7d29 223e  depends_on\'})">
+0016dee0: 4465 7065 6e64 7320 4f6e 3c2f 613e 3c2f  Depends On</a></
+0016def0: 6c69 3e5c 6e20 2020 2020 2020 2020 2020  li>\n           
+0016df00: 203c 2f75 6c3e 5c6e 2020 2020 2020 2020   </ul>\n        
+0016df10: 3c2f 6469 763e 5c6e 2020 2020 3c2f 6469  </div>\n    </di
+0016df20: 763e 5c6e 2020 2020 3c64 6976 2063 6c61  v>\n    <div cla
+0016df30: 7373 3d22 6170 702d 6465 7461 696c 7322  ss="app-details"
+0016df40: 3e5c 6e20 2020 2020 2020 203c 6469 7620  >\n        <div 
+0016df50: 636c 6173 733d 2261 7070 2d66 7261 6d65  class="app-frame
+0016df60: 2061 7070 2d70 6164 223e 5c6e 5c6e 2020   app-pad">\n\n  
+0016df70: 2020 2020 2020 2020 2020 3c73 6563 7469            <secti
+0016df80: 6f6e 2063 6c61 7373 3d22 7365 6374 696f  on class="sectio
+0016df90: 6e22 3e5c 6e20 2020 2020 2020 2020 2020  n">\n           
+0016dfa0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0016dfb0: 2273 6563 7469 6f6e 2d74 6172 6765 7422  "section-target"
+0016dfc0: 2069 643d 2264 6574 6169 6c73 223e 3c2f   id="details"></
+0016dfd0: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
+0016dfe0: 2020 2020 2020 3c74 6162 6c65 2d64 6574        <table-det
+0016dff0: 6169 6c73 206d 6f64 656c 3d22 6578 706f  ails model="expo
+0016e000: 7375 7265 2220 6578 7472 6173 3d22 6578  sure" extras="ex
+0016e010: 7472 615f 7461 626c 655f 6669 656c 6473  tra_table_fields
+0016e020: 2220 2f3e 5c6e 2020 2020 2020 2020 2020  " />\n          
+0016e030: 2020 3c2f 7365 6374 696f 6e3e 5c6e 5c6e    </section>\n\n
+0016e040: 2020 2020 2020 2020 2020 2020 3c73 6563              <sec
+0016e050: 7469 6f6e 2063 6c61 7373 3d22 7365 6374  tion class="sect
+0016e060: 696f 6e22 3e5c 6e20 2020 2020 2020 2020  ion">\n         
+0016e070: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0016e080: 733d 2273 6563 7469 6f6e 2d74 6172 6765  s="section-targe
+0016e090: 7422 2069 643d 2264 6573 6372 6970 7469  t" id="descripti
+0016e0a0: 6f6e 223e 3c2f 6469 763e 5c6e 2020 2020  on"></div>\n    
+0016e0b0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0016e0c0: 2063 6c61 7373 3d22 7365 6374 696f 6e2d   class="section-
+0016e0d0: 636f 6e74 656e 7422 3e5c 6e20 2020 2020  content">\n     
+0016e0e0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016e0f0: 6836 3e44 6573 6372 6970 7469 6f6e 3c2f  h6>Description</
+0016e100: 6836 3e5c 6e20 2020 2020 2020 2020 2020  h6>\n           
+0016e110: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0016e120: 6173 733d 2270 616e 656c 223e 5c6e 2020  ass="panel">\n  
+0016e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016e140: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0016e150: 3d22 7061 6e65 6c2d 626f 6479 223e 5c6e  ="panel-body">\n
+0016e160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016e170: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+0016e180: 206e 672d 6966 3d22 6578 706f 7375 7265   ng-if="exposure
+0016e190: 2e64 6573 6372 6970 7469 6f6e 2220 636c  .description" cl
+0016e1a0: 6173 733d 226d 6f64 656c 2d6d 6172 6b64  ass="model-markd
+0016e1b0: 6f77 6e22 206d 6172 6b65 643d 2265 7870  own" marked="exp
+0016e1c0: 6f73 7572 652e 6465 7363 7269 7074 696f  osure.descriptio
+0016e1d0: 6e22 3e3c 2f64 6976 3e5c 6e20 2020 2020  n"></div>\n     
+0016e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016e1f0: 2020 2020 2020 203c 6469 7620 6e67 2d69         <div ng-i
+0016e200: 663d 2221 6578 706f 7375 7265 2e64 6573  f="!exposure.des
+0016e210: 6372 6970 7469 6f6e 223e 5468 6973 207b  cription">This {
+0016e220: 7b20 6578 706f 7375 7265 2e72 6573 6f75  { exposure.resou
+0016e230: 7263 655f 7479 7065 207d 7d20 6973 206e  rce_type }} is n
+0016e240: 6f74 2063 7572 7265 6e74 6c79 2064 6f63  ot currently doc
+0016e250: 756d 656e 7465 643c 2f64 6976 3e5c 6e20  umented</div>\n 
+0016e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016e270: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
+0016e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016e290: 2020 203c 2f64 6976 3e5c 6e20 2020 2020     </div>\n     
+0016e2a0: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+0016e2b0: 3e5c 6e20 2020 2020 2020 2020 2020 203c  >\n            <
+0016e2c0: 2f73 6563 7469 6f6e 3e5c 6e5c 6e20 2020  /section>\n\n   
+0016e2d0: 2020 2020 2020 2020 203c 7365 6374 696f           <sectio
+0016e2e0: 6e20 636c 6173 733d 2273 6563 7469 6f6e  n class="section
+0016e2f0: 2220 6e67 2d73 686f 7720 3d20 2270 6172  " ng-show = "par
+0016e300: 656e 7473 4c65 6e67 7468 2021 3d20 3022  entsLength != 0"
+0016e310: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016e320: 2020 203c 6469 7620 636c 6173 733d 2273     <div class="s
+0016e330: 6563 7469 6f6e 2d74 6172 6765 7422 2069  ection-target" i
+0016e340: 643d 2264 6570 656e 6473 5f6f 6e22 3e3c  d="depends_on"><
+0016e350: 2f64 6976 3e5c 6e20 2020 2020 2020 2020  /div>\n         
+0016e360: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0016e370: 733d 2273 6563 7469 6f6e 2d63 6f6e 7465  s="section-conte
+0016e380: 6e74 223e 5c6e 2020 2020 2020 2020 2020  nt">\n          
+0016e390: 2020 2020 2020 2020 2020 3c68 363e 4465            <h6>De
+0016e3a0: 7065 6e64 7320 4f6e 3c2f 6836 3e5c 6e20  pends On</h6>\n 
+0016e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016e3c0: 2020 203c 7265 6665 7265 6e63 652d 6c69     <reference-li
+0016e3d0: 7374 2072 6566 6572 656e 6365 733d 2270  st references="p
+0016e3e0: 6172 656e 7473 2220 6e6f 6465 3d22 6578  arents" node="ex
+0016e3f0: 706f 7375 7265 2220 2f3e 5c6e 2020 2020  posure" />\n    
+0016e400: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+0016e410: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
+0016e420: 3c2f 7365 6374 696f 6e3e 5c6e 5c6e 2020  </section>\n\n  
+0016e430: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
+0016e440: 2020 3c2f 6469 763e 5c6e 3c2f 6469 763e    </div>\n</div>
+0016e450: 5c6e 2729 7d5d 292c 652e 6578 706f 7274  \n')}]),e.export
+0016e460: 733d 6e7d 2c66 756e 6374 696f 6e28 652c  s=n},function(e,
+0016e470: 7429 7b76 6172 206e 3d22 2f64 6f63 732f  t){var n="/docs/
+0016e480: 6d65 7472 6963 2e68 746d 6c22 3b77 696e  metric.html";win
+0016e490: 646f 772e 616e 6775 6c61 722e 6d6f 6475  dow.angular.modu
+0016e4a0: 6c65 2822 6e67 2229 2e72 756e 285b 2224  le("ng").run(["$
+0016e4b0: 7465 6d70 6c61 7465 4361 6368 6522 2c66  templateCache",f
+0016e4c0: 756e 6374 696f 6e28 6529 7b65 2e70 7574  unction(e){e.put
+0016e4d0: 286e 2c27 3c73 7479 6c65 3e5c 6e2f 2a20  (n,'<style>\n/* 
+0016e4e0: 544f 444f 202a 2f5c 6e2e 7365 6374 696f  TODO */\n.sectio
+0016e4f0: 6e2d 7461 7267 6574 207b 5c6e 2020 2020  n-target {\n    
+0016e500: 746f 703a 202d 3865 6d3b 5c6e 7d5c 6e5c  top: -8em;\n}\n\
+0016e510: 6e2e 6e6f 666c 6578 207b 5c6e 2020 2020  n.noflex {\n    
+0016e520: 666c 6578 3a20 3020 3020 3136 3070 7820  flex: 0 0 160px 
+0016e530: 2169 6d70 6f72 7461 6e74 3b5c 6e7d 5c6e  !important;\n}\n
+0016e540: 5c6e 2e68 6967 686c 6967 6874 207b 5c6e  \n.highlight {\n
+0016e550: 2020 2020 636f 6c6f 723a 2023 3234 3239      color: #2429
+0016e560: 3265 3b5c 6e20 2020 2062 6163 6b67 726f  2e;\n    backgro
+0016e570: 756e 642d 636f 6c6f 723a 2077 6869 7465  und-color: white
+0016e580: 3b5c 6e7d 5c6e 5c6e 3c2f 7374 796c 653e  ;\n}\n\n</style>
+0016e590: 5c6e 5c6e 3c64 6976 2063 6c61 7373 3d5c  \n\n<div class=\
+0016e5a0: 2761 7070 2d73 6372 6f6c 6c5c 273e 5c6e  'app-scroll\'>\n
+0016e5b0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0016e5c0: 6170 702d 6c69 6e6b 7320 6170 702d 7374  app-links app-st
+0016e5d0: 6963 6b79 223e 5c6e 2020 2020 2020 2020  icky">\n        
+0016e5e0: 3c64 6976 2063 6c61 7373 3d22 6170 702d  <div class="app-
+0016e5f0: 7469 746c 6522 3e5c 6e20 2020 2020 2020  title">\n       
+0016e600: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0016e610: 2261 7070 2d66 7261 6d65 2061 7070 2d70  "app-frame app-p
+0016e620: 6164 2061 7070 2d66 6c75 7368 2d62 6f74  ad app-flush-bot
+0016e630: 746f 6d22 3e5c 6e5c 6e20 2020 2020 2020  tom">\n\n       
+0016e640: 2020 2020 2020 2020 203c 6831 3e5c 6e20           <h1>\n 
+0016e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016e660: 2020 203c 7370 616e 2063 6c61 7373 3d22     <span class="
+0016e670: 6272 6561 6b22 3e7b 7b20 6d65 7472 6963  break">{{ metric
+0016e680: 2e6c 6162 656c 207d 7d3c 2f73 7061 6e3e  .label }}</span>
+0016e690: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+0016e6a0: 2020 2020 2020 3c73 6d61 6c6c 3e6d 6574        <small>met
+0016e6b0: 7269 633c 2f73 6d61 6c6c 3e5c 6e5c 6e20  ric</small>\n\n 
+0016e6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016e6d0: 2020 203c 6469 7620 636c 6173 733d 5c27     <div class=\'
+0016e6e0: 636c 6561 7266 6978 5c27 3e3c 2f64 6976  clearfix\'></div
+0016e6f0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+0016e700: 2020 203c 2f68 313e 5c6e 5c6e 2020 2020     </h1>\n\n    
+0016e710: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
+0016e720: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
+0016e730: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0016e740: 7373 3d22 6170 702d 6672 616d 6520 6170  ss="app-frame ap
+0016e750: 702d 7061 642d 6822 3e5c 6e20 2020 2020  p-pad-h">\n     
+0016e760: 2020 2020 2020 203c 756c 2063 6c61 7373         <ul class
+0016e770: 3d22 6e61 7620 6e61 762d 7461 6273 223e  ="nav nav-tabs">
+0016e780: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+0016e790: 2020 3c6c 6920 7569 2d73 7265 662d 6163    <li ui-sref-ac
+0016e7a0: 7469 7665 3d5c 2761 6374 6976 655c 273e  tive=\'active\'>
+0016e7b0: 3c61 2075 692d 7372 6566 3d22 6462 742e  <a ui-sref="dbt.
+0016e7c0: 6d65 7472 6963 287b 5c27 235c 273a 205c  metric({\'#\': \
+0016e7d0: 2764 6574 6169 6c73 5c27 7d29 223e 4465  'details\'})">De
+0016e7e0: 7461 696c 733c 2f61 3e3c 2f6c 693e 5c6e  tails</a></li>\n
+0016e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016e800: 3c6c 6920 7569 2d73 7265 662d 6163 7469  <li ui-sref-acti
+0016e810: 7665 3d5c 2761 6374 6976 655c 273e 3c61  ve=\'active\'><a
+0016e820: 2075 692d 7372 6566 3d22 6462 742e 6d65   ui-sref="dbt.me
+0016e830: 7472 6963 287b 5c27 235c 273a 205c 2764  tric({\'#\': \'d
+0016e840: 6573 6372 6970 7469 6f6e 5c27 7d29 223e  escription\'})">
+0016e850: 4465 7363 7269 7074 696f 6e3c 2f61 3e3c  Description</a><
+0016e860: 2f6c 693e 5c6e 2020 2020 2020 2020 2020  /li>\n          
+0016e870: 2020 2020 2020 3c6c 6920 7569 2d73 7265        <li ui-sre
+0016e880: 662d 6163 7469 7665 3d5c 2761 6374 6976  f-active=\'activ
+0016e890: 655c 2720 6e67 2d73 686f 7720 3d20 2270  e\' ng-show = "p
+0016e8a0: 6172 656e 7473 4c65 6e67 7468 2021 3d20  arentsLength != 
+0016e8b0: 3022 3e3c 6120 7569 2d73 7265 663d 2264  0"><a ui-sref="d
+0016e8c0: 6274 2e6d 6574 7269 6328 7b5c 2723 5c27  bt.metric({\'#\'
+0016e8d0: 3a20 5c27 6465 7065 6e64 735f 6f6e 5c27  : \'depends_on\'
+0016e8e0: 7d29 223e 4465 7065 6e64 7320 4f6e 3c2f  })">Depends On</
+0016e8f0: 613e 3c2f 6c69 3e5c 6e20 2020 2020 2020  a></li>\n       
+0016e900: 2020 2020 203c 2f75 6c3e 5c6e 2020 2020       </ul>\n    
+0016e910: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
+0016e920: 3c2f 6469 763e 5c6e 2020 2020 3c64 6976  </div>\n    <div
+0016e930: 2063 6c61 7373 3d22 6170 702d 6465 7461   class="app-deta
+0016e940: 696c 7322 3e5c 6e20 2020 2020 2020 203c  ils">\n        <
+0016e950: 6469 7620 636c 6173 733d 2261 7070 2d66  div class="app-f
+0016e960: 7261 6d65 2061 7070 2d70 6164 223e 5c6e  rame app-pad">\n
+0016e970: 5c6e 2020 2020 2020 2020 2020 2020 3c73  \n            <s
+0016e980: 6563 7469 6f6e 2063 6c61 7373 3d22 7365  ection class="se
+0016e990: 6374 696f 6e22 3e5c 6e20 2020 2020 2020  ction">\n       
+0016e9a0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0016e9b0: 6173 733d 2273 6563 7469 6f6e 2d74 6172  ass="section-tar
+0016e9c0: 6765 7422 2069 643d 2264 6574 6169 6c73  get" id="details
+0016e9d0: 223e 3c2f 6469 763e 5c6e 2020 2020 2020  "></div>\n      
+0016e9e0: 2020 2020 2020 2020 2020 3c74 6162 6c65            <table
+0016e9f0: 2d64 6574 6169 6c73 206d 6f64 656c 3d22  -details model="
+0016ea00: 6d65 7472 6963 2220 6578 7472 6173 3d22  metric" extras="
+0016ea10: 6578 7472 615f 7461 626c 655f 6669 656c  extra_table_fiel
+0016ea20: 6473 2220 2f3e 5c6e 2020 2020 2020 2020  ds" />\n        
+0016ea30: 2020 2020 3c2f 7365 6374 696f 6e3e 5c6e      </section>\n
+0016ea40: 5c6e 2020 2020 2020 2020 2020 2020 3c73  \n            <s
+0016ea50: 6563 7469 6f6e 2063 6c61 7373 3d22 7365  ection class="se
+0016ea60: 6374 696f 6e22 3e5c 6e20 2020 2020 2020  ction">\n       
+0016ea70: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+0016ea80: 6173 733d 2273 6563 7469 6f6e 2d74 6172  ass="section-tar
+0016ea90: 6765 7422 2069 643d 2264 6573 6372 6970  get" id="descrip
+0016eaa0: 7469 6f6e 223e 3c2f 6469 763e 5c6e 2020  tion"></div>\n  
+0016eab0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+0016eac0: 6976 2063 6c61 7373 3d22 7365 6374 696f  iv class="sectio
+0016ead0: 6e2d 636f 6e74 656e 7422 3e5c 6e20 2020  n-content">\n   
+0016eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016eaf0: 203c 6836 3e44 6573 6372 6970 7469 6f6e   <h6>Description
+0016eb00: 3c2f 6836 3e5c 6e20 2020 2020 2020 2020  </h6>\n         
+0016eb10: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+0016eb20: 636c 6173 733d 2270 616e 656c 223e 5c6e  class="panel">\n
+0016eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016eb40: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0016eb50: 7373 3d22 7061 6e65 6c2d 626f 6479 223e  ss="panel-body">
+0016eb60: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+0016eb70: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+0016eb80: 6976 206e 672d 6966 3d22 6d65 7472 6963  iv ng-if="metric
+0016eb90: 2e64 6573 6372 6970 7469 6f6e 2220 636c  .description" cl
+0016eba0: 6173 733d 226d 6f64 656c 2d6d 6172 6b64  ass="model-markd
+0016ebb0: 6f77 6e22 206d 6172 6b65 643d 226d 6574  own" marked="met
+0016ebc0: 7269 632e 6465 7363 7269 7074 696f 6e22  ric.description"
+0016ebd0: 3e3c 2f64 6976 3e5c 6e20 2020 2020 2020  ></div>\n       
+0016ebe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016ebf0: 2020 2020 203c 6469 7620 6e67 2d69 663d       <div ng-if=
+0016ec00: 2221 6d65 7472 6963 2e64 6573 6372 6970  "!metric.descrip
+0016ec10: 7469 6f6e 223e 5468 6973 207b 7b20 6d65  tion">This {{ me
+0016ec20: 7472 6963 2e72 6573 6f75 7263 655f 7479  tric.resource_ty
+0016ec30: 7065 207d 7d20 6973 206e 6f74 2063 7572  pe }} is not cur
+0016ec40: 7265 6e74 6c79 2064 6f63 756d 656e 7465  rently documente
+0016ec50: 643c 2f64 6976 3e5c 6e20 2020 2020 2020  d</div>\n       
+0016ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016ec70: 203c 2f64 6976 3e5c 6e20 2020 2020 2020   </div>\n       
+0016ec80: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+0016ec90: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
+0016eca0: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
+0016ecb0: 2020 2020 2020 2020 203c 2f73 6563 7469           </secti
+0016ecc0: 6f6e 3e5c 6e5c 6e20 2020 2020 2020 2020  on>\n\n         
+0016ecd0: 2020 203c 7365 6374 696f 6e20 636c 6173     <section clas
+0016ece0: 733d 2273 6563 7469 6f6e 2220 6e67 2d73  s="section" ng-s
+0016ecf0: 686f 7720 3d20 2270 6172 656e 7473 4c65  how = "parentsLe
+0016ed00: 6e67 7468 2021 3d20 3022 3e5c 6e20 2020  ngth != 0">\n   
+0016ed10: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0016ed20: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
+0016ed30: 2d74 6172 6765 7422 2069 643d 2264 6570  -target" id="dep
+0016ed40: 656e 6473 5f6f 6e22 3e3c 2f64 6976 3e5c  ends_on"></div>\
+0016ed50: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016ed60: 203c 6469 7620 636c 6173 733d 2273 6563   <div class="sec
+0016ed70: 7469 6f6e 2d63 6f6e 7465 6e74 223e 5c6e  tion-content">\n
+0016ed80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016ed90: 2020 2020 3c68 363e 4465 7065 6e64 7320      <h6>Depends 
+0016eda0: 4f6e 3c2f 6836 3e5c 6e20 2020 2020 2020  On</h6>\n       
+0016edb0: 2020 2020 2020 2020 2020 2020 203c 7265               <re
+0016edc0: 6665 7265 6e63 652d 6c69 7374 2072 6566  ference-list ref
+0016edd0: 6572 656e 6365 733d 2270 6172 656e 7473  erences="parents
+0016ede0: 2220 6e6f 6465 3d22 6d65 7472 6963 2220  " node="metric" 
+0016edf0: 2f3e 5c6e 2020 2020 2020 2020 2020 2020  />\n            
+0016ee00: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
+0016ee10: 2020 2020 2020 2020 3c2f 7365 6374 696f          </sectio
+0016ee20: 6e3e 5c6e 5c6e 2020 2020 2020 2020 3c2f  n>\n\n        </
+0016ee30: 6469 763e 5c6e 2020 2020 3c2f 6469 763e  div>\n    </div>
+0016ee40: 5c6e 3c2f 6469 763e 5c6e 2729 7d5d 292c  \n</div>\n')}]),
+0016ee50: 652e 6578 706f 7274 733d 6e7d 2c66 756e  e.exports=n},fun
+0016ee60: 6374 696f 6e28 652c 7429 7b76 6172 206e  ction(e,t){var n
+0016ee70: 3d22 2f64 6f63 732f 7365 6d61 6e74 6963  ="/docs/semantic
+0016ee80: 5f6d 6f64 656c 2e68 746d 6c22 3b77 696e  _model.html";win
+0016ee90: 646f 772e 616e 6775 6c61 722e 6d6f 6475  dow.angular.modu
+0016eea0: 6c65 2822 6e67 2229 2e72 756e 285b 2224  le("ng").run(["$
+0016eeb0: 7465 6d70 6c61 7465 4361 6368 6522 2c66  templateCache",f
+0016eec0: 756e 6374 696f 6e28 6529 7b65 2e70 7574  unction(e){e.put
+0016eed0: 286e 2c27 3c73 7479 6c65 3e5c 6e2f 2a20  (n,'<style>\n/* 
+0016eee0: 544f 444f 202a 2f5c 6e2e 7365 6374 696f  TODO */\n.sectio
+0016eef0: 6e2d 7461 7267 6574 207b 5c6e 2020 2020  n-target {\n    
+0016ef00: 746f 703a 202d 3865 6d3b 5c6e 7d5c 6e5c  top: -8em;\n}\n\
+0016ef10: 6e2e 6e6f 666c 6578 207b 5c6e 2020 2020  n.noflex {\n    
+0016ef20: 666c 6578 3a20 3020 3020 3136 3070 7820  flex: 0 0 160px 
+0016ef30: 2169 6d70 6f72 7461 6e74 3b5c 6e7d 5c6e  !important;\n}\n
+0016ef40: 5c6e 2e68 6967 686c 6967 6874 207b 5c6e  \n.highlight {\n
+0016ef50: 2020 2020 636f 6c6f 723a 2023 3234 3239      color: #2429
+0016ef60: 3265 3b5c 6e20 2020 2062 6163 6b67 726f  2e;\n    backgro
+0016ef70: 756e 642d 636f 6c6f 723a 2077 6869 7465  und-color: white
+0016ef80: 3b5c 6e7d 5c6e 5c6e 3c2f 7374 796c 653e  ;\n}\n\n</style>
+0016ef90: 5c6e 5c6e 3c64 6976 2063 6c61 7373 3d5c  \n\n<div class=\
+0016efa0: 2761 7070 2d73 6372 6f6c 6c5c 273e 5c6e  'app-scroll\'>\n
+0016efb0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+0016efc0: 6170 702d 6c69 6e6b 7320 6170 702d 7374  app-links app-st
+0016efd0: 6963 6b79 223e 5c6e 2020 2020 2020 2020  icky">\n        
+0016efe0: 3c64 6976 2063 6c61 7373 3d22 6170 702d  <div class="app-
+0016eff0: 7469 746c 6522 3e5c 6e20 2020 2020 2020  title">\n       
+0016f000: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+0016f010: 2261 7070 2d66 7261 6d65 2061 7070 2d70  "app-frame app-p
+0016f020: 6164 2061 7070 2d66 6c75 7368 2d62 6f74  ad app-flush-bot
+0016f030: 746f 6d22 3e5c 6e5c 6e20 2020 2020 2020  tom">\n\n       
+0016f040: 2020 2020 2020 2020 203c 6831 3e5c 6e20           <h1>\n 
+0016f050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016f060: 2020 203c 7370 616e 2063 6c61 7373 3d22     <span class="
+0016f070: 6272 6561 6b22 3e7b 7b20 7365 6d61 6e74  break">{{ semant
+0016f080: 6963 5f6d 6f64 656c 2e6e 616d 6520 7d7d  ic_model.name }}
+0016f090: 3c2f 7370 616e 3e5c 6e20 2020 2020 2020  </span>\n       
+0016f0a0: 2020 2020 2020 2020 2020 2020 203c 736d               <sm
+0016f0b0: 616c 6c3e 7365 6d61 6e74 6963 5f6d 6f64  all>semantic_mod
+0016f0c0: 656c 3c2f 736d 616c 6c3e 5c6e 5c6e 2020  el</small>\n\n  
+0016f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016f0e0: 2020 3c64 6976 2063 6c61 7373 3d5c 2763    <div class=\'c
+0016f0f0: 6c65 6172 6669 785c 273e 3c2f 6469 763e  learfix\'></div>
+0016f100: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+0016f110: 2020 3c2f 6831 3e5c 6e5c 6e20 2020 2020    </h1>\n\n     
+0016f120: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
+0016f130: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
+0016f140: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0016f150: 733d 2261 7070 2d66 7261 6d65 2061 7070  s="app-frame app
+0016f160: 2d70 6164 2d68 223e 5c6e 2020 2020 2020  -pad-h">\n      
+0016f170: 2020 2020 2020 3c75 6c20 636c 6173 733d        <ul class=
+0016f180: 226e 6176 206e 6176 2d74 6162 7322 3e5c  "nav nav-tabs">\
+0016f190: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016f1a0: 203c 6c69 2075 692d 7372 6566 2d61 6374   <li ui-sref-act
+0016f1b0: 6976 653d 5c27 6163 7469 7665 5c27 3e3c  ive=\'active\'><
+0016f1c0: 6120 7569 2d73 7265 663d 2264 6274 2e73  a ui-sref="dbt.s
+0016f1d0: 656d 616e 7469 635f 6d6f 6465 6c28 7b5c  emantic_model({\
+0016f1e0: 2723 5c27 3a20 5c27 6465 7461 696c 735c  '#\': \'details\
+0016f1f0: 277d 2922 3e44 6574 6169 6c73 3c2f 613e  '})">Details</a>
+0016f200: 3c2f 6c69 3e5c 6e20 2020 2020 2020 2020  </li>\n         
+0016f210: 2020 2020 2020 203c 6c69 2075 692d 7372         <li ui-sr
+0016f220: 6566 2d61 6374 6976 653d 5c27 6163 7469  ef-active=\'acti
+0016f230: 7665 5c27 3e3c 6120 7569 2d73 7265 663d  ve\'><a ui-sref=
+0016f240: 2264 6274 2e73 656d 616e 7469 635f 6d6f  "dbt.semantic_mo
+0016f250: 6465 6c28 7b5c 2723 5c27 3a20 5c27 6465  del({\'#\': \'de
+0016f260: 7363 7269 7074 696f 6e5c 277d 2922 3e44  scription\'})">D
+0016f270: 6573 6372 6970 7469 6f6e 3c2f 613e 3c2f  escription</a></
+0016f280: 6c69 3e5c 6e20 2020 2020 2020 2020 2020  li>\n           
+0016f290: 2020 2020 203c 6c69 2075 692d 7372 6566       <li ui-sref
+0016f2a0: 2d61 6374 6976 653d 5c27 6163 7469 7665  -active=\'active
+0016f2b0: 5c27 206e 672d 7368 6f77 203d 2022 7061  \' ng-show = "pa
+0016f2c0: 7265 6e74 734c 656e 6774 6820 213d 2030  rentsLength != 0
+0016f2d0: 223e 3c61 2075 692d 7372 6566 3d22 6462  "><a ui-sref="db
+0016f2e0: 742e 7365 6d61 6e74 6963 5f6d 6f64 656c  t.semantic_model
+0016f2f0: 287b 5c27 235c 273a 205c 2764 6570 656e  ({\'#\': \'depen
+0016f300: 6473 5f6f 6e5c 277d 2922 3e44 6570 656e  ds_on\'})">Depen
+0016f310: 6473 204f 6e3c 2f61 3e3c 2f6c 693e 5c6e  ds On</a></li>\n
+0016f320: 2020 2020 2020 2020 2020 2020 3c2f 756c              </ul
+0016f330: 3e5c 6e20 2020 2020 2020 203c 2f64 6976  >\n        </div
+0016f340: 3e5c 6e20 2020 203c 2f64 6976 3e5c 6e20  >\n    </div>\n 
+0016f350: 2020 203c 6469 7620 636c 6173 733d 2261     <div class="a
+0016f360: 7070 2d64 6574 6169 6c73 223e 5c6e 2020  pp-details">\n  
+0016f370: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+0016f380: 3d22 6170 702d 6672 616d 6520 6170 702d  ="app-frame app-
+0016f390: 7061 6422 3e5c 6e5c 6e20 2020 2020 2020  pad">\n\n       
+0016f3a0: 2020 2020 203c 7365 6374 696f 6e20 636c       <section cl
+0016f3b0: 6173 733d 2273 6563 7469 6f6e 223e 5c6e  ass="section">\n
+0016f3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016f3d0: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
+0016f3e0: 696f 6e2d 7461 7267 6574 2220 6964 3d22  ion-target" id="
+0016f3f0: 6465 7461 696c 7322 3e3c 2f64 6976 3e5c  details"></div>\
+0016f400: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016f410: 203c 7461 626c 652d 6465 7461 696c 7320   <table-details 
+0016f420: 6d6f 6465 6c3d 2273 656d 616e 7469 635f  model="semantic_
+0016f430: 6d6f 6465 6c22 2065 7874 7261 733d 2265  model" extras="e
+0016f440: 7874 7261 5f74 6162 6c65 5f66 6965 6c64  xtra_table_field
+0016f450: 7322 202f 3e5c 6e20 2020 2020 2020 2020  s" />\n         
+0016f460: 2020 203c 2f73 6563 7469 6f6e 3e5c 6e5c     </section>\n\
+0016f470: 6e20 2020 2020 2020 2020 2020 203c 7365  n            <se
+0016f480: 6374 696f 6e20 636c 6173 733d 2273 6563  ction class="sec
+0016f490: 7469 6f6e 223e 5c6e 2020 2020 2020 2020  tion">\n        
+0016f4a0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+0016f4b0: 7373 3d22 7365 6374 696f 6e2d 7461 7267  ss="section-targ
+0016f4c0: 6574 2220 6964 3d22 6465 7363 7269 7074  et" id="descript
+0016f4d0: 696f 6e22 3e3c 2f64 6976 3e5c 6e20 2020  ion"></div>\n   
+0016f4e0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0016f4f0: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
+0016f500: 2d63 6f6e 7465 6e74 223e 5c6e 2020 2020  -content">\n    
+0016f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016f520: 3c68 363e 4465 7363 7269 7074 696f 6e3c  <h6>Description<
+0016f530: 2f68 363e 5c6e 2020 2020 2020 2020 2020  /h6>\n          
+0016f540: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+0016f550: 6c61 7373 3d22 7061 6e65 6c22 3e5c 6e20  lass="panel">\n 
+0016f560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016f570: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0016f580: 733d 2270 616e 656c 2d62 6f64 7922 3e5c  s="panel-body">\
+0016f590: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016f5a0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0016f5b0: 7620 6e67 2d69 663d 2273 656d 616e 7469  v ng-if="semanti
+0016f5c0: 635f 6d6f 6465 6c2e 6465 7363 7269 7074  c_model.descript
+0016f5d0: 696f 6e22 2063 6c61 7373 3d22 6d6f 6465  ion" class="mode
+0016f5e0: 6c2d 6d61 726b 646f 776e 2220 6d61 726b  l-markdown" mark
+0016f5f0: 6564 3d22 7365 6d61 6e74 6963 5f6d 6f64  ed="semantic_mod
+0016f600: 656c 2e64 6573 6372 6970 7469 6f6e 223e  el.description">
+0016f610: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
+0016f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016f630: 2020 2020 3c64 6976 206e 672d 6966 3d22      <div ng-if="
+0016f640: 2173 656d 616e 7469 635f 6d6f 6465 6c2e  !semantic_model.
+0016f650: 6465 7363 7269 7074 696f 6e22 3e54 6869  description">Thi
+0016f660: 7320 7b7b 2073 656d 616e 7469 635f 6d6f  s {{ semantic_mo
+0016f670: 6465 6c2e 7265 736f 7572 6365 5f74 7970  del.resource_typ
+0016f680: 6520 7d7d 2069 7320 6e6f 7420 6375 7272  e }} is not curr
+0016f690: 656e 746c 7920 646f 6375 6d65 6e74 6564  ently documented
+0016f6a0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
+0016f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016f6c0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
+0016f6d0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+0016f6e0: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
+0016f6f0: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
+0016f700: 2020 2020 2020 2020 3c2f 7365 6374 696f          </sectio
+0016f710: 6e3e 5c6e 5c6e 2020 2020 2020 2020 2020  n>\n\n          
+0016f720: 2020 3c73 6563 7469 6f6e 2063 6c61 7373    <section class
+0016f730: 3d22 7365 6374 696f 6e22 206e 672d 7368  ="section" ng-sh
+0016f740: 6f77 203d 2022 7365 6d61 6e74 6963 5f6d  ow = "semantic_m
+0016f750: 6f64 656c 2e65 6e74 6974 6965 732e 6c65  odel.entities.le
+0016f760: 6e67 7468 2021 3d20 3022 3e5c 6e20 2020  ngth != 0">\n   
+0016f770: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+0016f780: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
+0016f790: 2d74 6172 6765 7422 2069 643d 2265 6e74  -target" id="ent
+0016f7a0: 6974 6965 7322 3e3c 2f64 6976 3e5c 6e20  ities"></div>\n 
+0016f7b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016f7c0: 6469 7620 636c 6173 733d 2273 6563 7469  div class="secti
+0016f7d0: 6f6e 2d63 6f6e 7465 6e74 223e 5c6e 2020  on-content">\n  
+0016f7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016f7f0: 2020 3c68 363e 456e 7469 7469 6573 3c2f    <h6>Entities</
+0016f800: 6836 3e5c 6e5c 6e20 2020 2020 2020 2020  h6>\n\n         
+0016f810: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+0016f820: 733d 2270 616e 656c 223e 5c6e 2020 2020  s="panel">\n    
+0016f830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016f840: 3c64 6976 2063 6c61 7373 3d22 6465 7461  <div class="deta
+0016f850: 696c 2d67 726f 7570 2220 7374 796c 653d  il-group" style=
+0016f860: 2270 6164 6469 6e67 2d62 6f74 746f 6d3a  "padding-bottom:
+0016f870: 2030 223e 5c6e 2020 2020 2020 2020 2020   0">\n          
+0016f880: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+0016f890: 6976 2063 6c61 7373 3d22 6465 7461 696c  iv class="detail
+0016f8a0: 2d62 6f64 7922 2073 7479 6c65 3d22 7061  -body" style="pa
+0016f8b0: 6464 696e 672d 6c65 6674 3a20 3022 3e5c  dding-left: 0">\
+0016f8c0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016f8d0: 2020 2020 2020 2020 2020 2020 203c 646c               <dl
+0016f8e0: 2063 6c61 7373 3d22 6465 7461 696c 2220   class="detail" 
+0016f8f0: 6e67 2d73 7479 6c65 3d22 7b5c 2770 6164  ng-style="{\'pad
+0016f900: 6469 6e67 2d6c 6566 745c 273a 2024 696e  ding-left\': $in
+0016f910: 6465 7820 3d3d 2030 203f 2030 203a 205c  dex == 0 ? 0 : \
+0016f920: 2761 7574 6f5c 277d 225c 6e20 2020 2020  'auto\'}"\n     
+0016f930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016f940: 2020 2020 2020 2020 2020 206e 672d 7265             ng-re
+0016f950: 7065 6174 3d22 656e 7469 7479 2069 6e20  peat="entity in 
+0016f960: 7365 6d61 6e74 6963 5f6d 6f64 656c 2e65  semantic_model.e
+0016f970: 6e74 6974 6965 7322 3e5c 6e20 2020 2020  ntities">\n     
+0016f980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016f990: 2020 2020 2020 2020 2020 203c 6474 2063             <dt c
+0016f9a0: 6c61 7373 3d22 6465 7461 696c 2d6c 6162  lass="detail-lab
+0016f9b0: 656c 223e 4e61 6d65 3c2f 6474 3e5c 6e20  el">Name</dt>\n 
+0016f9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016f9d0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016f9e0: 6464 2063 6c61 7373 3d22 6465 7461 696c  dd class="detail
+0016f9f0: 2d76 616c 7565 2220 6e67 2d69 663d 2265  -value" ng-if="e
+0016fa00: 6e74 6974 792e 6e61 6d65 223e 7b7b 2065  ntity.name">{{ e
+0016fa10: 6e74 6974 792e 6e61 6d65 207d 7d3c 2f64  ntity.name }}</d
+0016fa20: 643e 5c6e 2020 2020 2020 2020 2020 2020  d>\n            
+0016fa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016fa40: 2020 2020 3c64 6420 636c 6173 733d 2264      <dd class="d
+0016fa50: 6574 6169 6c2d 7661 6c75 6522 206e 672d  etail-value" ng-
+0016fa60: 6966 3d22 2165 6e74 6974 792e 6e61 6d65  if="!entity.name
+0016fa70: 223e 4e6f 6e65 3c2f 6464 3e5c 6e20 2020  ">None</dd>\n   
+0016fa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016fa90: 2020 2020 2020 2020 2020 2020 203c 6474               <dt
+0016faa0: 2063 6c61 7373 3d22 6465 7461 696c 2d6c   class="detail-l
+0016fab0: 6162 656c 223e 5479 7065 3c2f 6474 3e5c  abel">Type</dt>\
+0016fac0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016fad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016fae0: 203c 6464 2063 6c61 7373 3d22 6465 7461   <dd class="deta
+0016faf0: 696c 2d76 616c 7565 2220 6e67 2d69 663d  il-value" ng-if=
+0016fb00: 2265 6e74 6974 792e 7479 7065 223e 7b7b  "entity.type">{{
+0016fb10: 2065 6e74 6974 792e 7479 7065 207d 7d3c   entity.type }}<
+0016fb20: 2f64 643e 5c6e 2020 2020 2020 2020 2020  /dd>\n          
+0016fb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016fb40: 2020 2020 2020 3c64 6420 636c 6173 733d        <dd class=
+0016fb50: 2264 6574 6169 6c2d 7661 6c75 6522 206e  "detail-value" n
+0016fb60: 672d 6966 3d22 2165 6e74 6974 792e 7479  g-if="!entity.ty
+0016fb70: 7065 223e 4e6f 6e65 3c2f 6464 3e5c 6e20  pe">None</dd>\n 
+0016fb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016fb90: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0016fba0: 6474 2063 6c61 7373 3d22 6465 7461 696c  dt class="detail
+0016fbb0: 2d6c 6162 656c 223e 4578 7072 6573 7369  -label">Expressi
+0016fbc0: 6f6e 3c2f 6474 3e5c 6e20 2020 2020 2020  on</dt>\n       
+0016fbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016fbe0: 2020 2020 2020 2020 203c 6464 2063 6c61           <dd cla
+0016fbf0: 7373 3d22 6465 7461 696c 2d76 616c 7565  ss="detail-value
+0016fc00: 2220 6e67 2d69 663d 2265 6e74 6974 792e  " ng-if="entity.
+0016fc10: 6578 7072 223e 7b7b 2065 6e74 6974 792e  expr">{{ entity.
+0016fc20: 6578 7072 207d 7d3c 2f64 643e 5c6e 2020  expr }}</dd>\n  
+0016fc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016fc40: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+0016fc50: 6420 636c 6173 733d 2264 6574 6169 6c2d  d class="detail-
+0016fc60: 7661 6c75 6522 206e 672d 6966 3d22 2165  value" ng-if="!e
+0016fc70: 6e74 6974 792e 6578 7072 223e 4e6f 6e65  ntity.expr">None
+0016fc80: 3c2f 6464 3e5c 6e20 2020 2020 2020 2020  </dd>\n         
+0016fc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016fca0: 2020 203c 2f64 6c3e 5c6e 2020 2020 2020     </dl>\n      
+0016fcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0016fcc0: 2020 3c2f 6469 763e 5c6e 2020 2020 2020    </div>\n      
+0016fcd0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+0016fce0: 6469 763e 5c6e 2020 2020 2020 2020 2020  div>\n          
+0016fcf0: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
+0016fd00: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+0016fd10: 5c6e 2020 2020 2020 2020 3c2f 7365 6374  \n        </sect
+0016fd20: 696f 6e3e 5c6e 5c6e 2020 2020 2020 2020  ion>\n\n        
+0016fd30: 2020 2020 3c73 6563 7469 6f6e 2063 6c61      <section cla
+0016fd40: 7373 3d22 7365 6374 696f 6e22 206e 672d  ss="section" ng-
+0016fd50: 7368 6f77 203d 2022 7061 7265 6e74 734c  show = "parentsL
+0016fd60: 656e 6774 6820 213d 2030 223e 5c6e 2020  ength != 0">\n  
+0016fd70: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+0016fd80: 6976 2063 6c61 7373 3d22 7365 6374 696f  iv class="sectio
+0016fd90: 6e2d 7461 7267 6574 2220 6964 3d22 6465  n-target" id="de
+0016fda0: 7065 6e64 735f 6f6e 223e 3c2f 6469 763e  pends_on"></div>
+0016fdb0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+0016fdc0: 2020 3c64 6976 2063 6c61 7373 3d22 7365    <div class="se
+0016fdd0: 6374 696f 6e2d 636f 6e74 656e 7422 3e5c  ction-content">\
+0016fde0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+0016fdf0: 2020 2020 203c 6836 3e44 6570 656e 6473       <h6>Depends
+0016fe00: 204f 6e3c 2f68 363e 5c6e 2020 2020 2020   On</h6>\n      
+0016fe10: 2020 2020 2020 2020 2020 2020 2020 3c72                <r
+0016fe20: 6566 6572 656e 6365 2d6c 6973 7420 7265  eference-list re
+0016fe30: 6665 7265 6e63 6573 3d22 7061 7265 6e74  ferences="parent
+0016fe40: 7322 206e 6f64 653d 2273 656d 616e 7469  s" node="semanti
+0016fe50: 635f 6d6f 6465 6c22 202f 3e5c 6e20 2020  c_model" />\n   
+0016fe60: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+0016fe70: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
+0016fe80: 203c 2f73 6563 7469 6f6e 3e5c 6e5c 6e20   </section>\n\n 
+0016fe90: 2020 2020 2020 203c 2f64 6976 3e5c 6e20         </div>\n 
+0016fea0: 2020 203c 2f64 6976 3e5c 6e3c 2f64 6976     </div>\n</div
+0016feb0: 3e5c 6e27 297d 5d29 2c65 2e65 7870 6f72  >\n')}]),e.expor
+0016fec0: 7473 3d6e 7d2c 6675 6e63 7469 6f6e 2865  ts=n},function(e
+0016fed0: 2c74 297b 7661 7220 6e3d 222f 646f 6373  ,t){var n="/docs
+0016fee0: 2f6f 7065 7261 7469 6f6e 2e68 746d 6c22  /operation.html"
+0016fef0: 3b77 696e 646f 772e 616e 6775 6c61 722e  ;window.angular.
+0016ff00: 6d6f 6475 6c65 2822 6e67 2229 2e72 756e  module("ng").run
+0016ff10: 285b 2224 7465 6d70 6c61 7465 4361 6368  (["$templateCach
+0016ff20: 6522 2c66 756e 6374 696f 6e28 6529 7b65  e",function(e){e
+0016ff30: 2e70 7574 286e 2c27 3c73 7479 6c65 3e5c  .put(n,'<style>\
+0016ff40: 6e2f 2a20 544f 444f 202a 2f5c 6e2e 7365  n/* TODO */\n.se
+0016ff50: 6374 696f 6e2d 7461 7267 6574 207b 5c6e  ction-target {\n
+0016ff60: 2020 2020 746f 703a 202d 3865 6d3b 5c6e      top: -8em;\n
+0016ff70: 7d5c 6e5c 6e2e 6e6f 666c 6578 207b 5c6e  }\n\n.noflex {\n
+0016ff80: 2020 2020 666c 6578 3a20 3020 3020 3136      flex: 0 0 16
+0016ff90: 3070 7820 2169 6d70 6f72 7461 6e74 3b5c  0px !important;\
+0016ffa0: 6e7d 5c6e 5c6e 2e68 6967 686c 6967 6874  n}\n\n.highlight
+0016ffb0: 207b 5c6e 2020 2020 636f 6c6f 723a 2023   {\n    color: #
+0016ffc0: 3234 3239 3265 3b5c 6e20 2020 2062 6163  24292e;\n    bac
+0016ffd0: 6b67 726f 756e 642d 636f 6c6f 723a 2077  kground-color: w
+0016ffe0: 6869 7465 3b5c 6e7d 5c6e 5c6e 3c2f 7374  hite;\n}\n\n</st
+0016fff0: 796c 653e 5c6e 5c6e 3c64 6976 2063 6c61  yle>\n\n<div cla
+00170000: 7373 3d5c 2761 7070 2d73 6372 6f6c 6c5c  ss=\'app-scroll\
+00170010: 273e 5c6e 2020 2020 3c64 6976 2063 6c61  '>\n    <div cla
+00170020: 7373 3d22 6170 702d 6c69 6e6b 7320 6170  ss="app-links ap
+00170030: 702d 7374 6963 6b79 223e 5c6e 2020 2020  p-sticky">\n    
+00170040: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00170050: 6170 702d 7469 746c 6522 3e5c 6e20 2020  app-title">\n   
+00170060: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00170070: 6173 733d 2261 7070 2d66 7261 6d65 2061  ass="app-frame a
+00170080: 7070 2d70 6164 2061 7070 2d66 6c75 7368  pp-pad app-flush
+00170090: 2d62 6f74 746f 6d22 3e5c 6e20 2020 2020  -bottom">\n     
+001700a0: 2020 2020 2020 2020 2020 203c 6831 3e5c             <h1>\
+001700b0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+001700c0: 2020 2020 203c 7370 616e 2063 6c61 7373       <span class
+001700d0: 3d22 6272 6561 6b22 3e7b 7b20 6d6f 6465  ="break">{{ mode
+001700e0: 6c2e 6e61 6d65 207d 7d3c 2f73 7061 6e3e  l.name }}</span>
+001700f0: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00170100: 2020 2020 2020 3c73 6d61 6c6c 3e6f 7065        <small>ope
+00170110: 7261 7469 6f6e 3c2f 736d 616c 6c3e 5c6e  ration</small>\n
+00170120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00170130: 3c2f 6831 3e5c 6e20 2020 2020 2020 2020  </h1>\n         
+00170140: 2020 203c 2f64 6976 3e5c 6e20 2020 2020     </div>\n     
+00170150: 2020 203c 2f64 6976 3e5c 6e20 2020 2020     </div>\n     
+00170160: 2020 203c 6469 7620 636c 6173 733d 2261     <div class="a
+00170170: 7070 2d66 7261 6d65 2061 7070 2d70 6164  pp-frame app-pad
+00170180: 2d68 223e 5c6e 2020 2020 2020 2020 2020  -h">\n          
+00170190: 2020 3c75 6c20 636c 6173 733d 226e 6176    <ul class="nav
+001701a0: 206e 6176 2d74 6162 7322 3e5c 6e20 2020   nav-tabs">\n   
+001701b0: 2020 2020 2020 2020 2020 2020 203c 6c69               <li
+001701c0: 2075 692d 7372 6566 2d61 6374 6976 653d   ui-sref-active=
+001701d0: 5c27 6163 7469 7665 5c27 3e3c 6120 7569  \'active\'><a ui
+001701e0: 2d73 7265 663d 2264 6274 2e6f 7065 7261  -sref="dbt.opera
+001701f0: 7469 6f6e 287b 5c27 235c 273a 205c 2764  tion({\'#\': \'d
+00170200: 6573 6372 6970 7469 6f6e 5c27 7d29 223e  escription\'})">
+00170210: 4465 7363 7269 7074 696f 6e3c 2f61 3e3c  Description</a><
+00170220: 2f6c 693e 5c6e 2020 2020 2020 2020 2020  /li>\n          
+00170230: 2020 2020 2020 3c6c 6920 7569 2d73 7265        <li ui-sre
+00170240: 662d 6163 7469 7665 3d5c 2761 6374 6976  f-active=\'activ
+00170250: 655c 2720 6e67 2d73 686f 7720 3d20 2270  e\' ng-show = "p
+00170260: 6172 656e 7473 4c65 6e67 7468 2021 3d20  arentsLength != 
+00170270: 3022 3e3c 6120 7569 2d73 7265 663d 2264  0"><a ui-sref="d
+00170280: 6274 2e6f 7065 7261 7469 6f6e 287b 5c27  bt.operation({\'
+00170290: 235c 273a 205c 2764 6570 656e 6473 5f6f  #\': \'depends_o
+001702a0: 6e5c 277d 2922 3e44 6570 656e 6473 204f  n\'})">Depends O
+001702b0: 6e3c 2f61 3e3c 2f6c 693e 5c6e 2020 2020  n</a></li>\n    
+001702c0: 2020 2020 2020 2020 2020 2020 3c6c 6920              <li 
+001702d0: 7569 2d73 7265 662d 6163 7469 7665 3d5c  ui-sref-active=\
+001702e0: 2761 6374 6976 655c 273e 3c61 2075 692d  'active\'><a ui-
+001702f0: 7372 6566 3d22 6462 742e 6f70 6572 6174  sref="dbt.operat
+00170300: 696f 6e28 7b5c 2723 5c27 3a20 5c27 636f  ion({\'#\': \'co
+00170310: 6465 5c27 7d29 223e 5351 4c3c 2f61 3e3c  de\'})">SQL</a><
+00170320: 2f6c 693e 5c6e 2020 2020 2020 2020 2020  /li>\n          
+00170330: 2020 3c2f 756c 3e5c 6e20 2020 2020 2020    </ul>\n       
+00170340: 203c 2f64 6976 3e5c 6e20 2020 203c 2f64   </div>\n    </d
+00170350: 6976 3e5c 6e20 2020 203c 6469 7620 636c  iv>\n    <div cl
+00170360: 6173 733d 2261 7070 2d64 6574 6169 6c73  ass="app-details
+00170370: 223e 5c6e 2020 2020 2020 2020 3c64 6976  ">\n        <div
+00170380: 2063 6c61 7373 3d22 6170 702d 6672 616d   class="app-fram
+00170390: 6520 6170 702d 7061 6422 3e5c 6e20 2020  e app-pad">\n   
+001703a0: 2020 2020 2020 2020 203c 7365 6374 696f           <sectio
+001703b0: 6e20 636c 6173 733d 2273 6563 7469 6f6e  n class="section
+001703c0: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
+001703d0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+001703e0: 7365 6374 696f 6e2d 7461 7267 6574 2220  section-target" 
+001703f0: 6964 3d22 6465 7363 7269 7074 696f 6e22  id="description"
+00170400: 3e3c 2f64 6976 3e5c 6e20 2020 2020 2020  ></div>\n       
+00170410: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00170420: 6173 733d 2273 6563 7469 6f6e 2d63 6f6e  ass="section-con
+00170430: 7465 6e74 223e 5c6e 2020 2020 2020 2020  tent">\n        
+00170440: 2020 2020 2020 2020 2020 2020 3c68 363e              <h6>
+00170450: 4465 7363 7269 7074 696f 6e3c 2f68 363e  Description</h6>
+00170460: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00170470: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00170480: 3d22 7061 6e65 6c22 3e5c 6e20 2020 2020  ="panel">\n     
+00170490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001704a0: 2020 203c 6469 7620 636c 6173 733d 2270     <div class="p
+001704b0: 616e 656c 2d62 6f64 7922 3e5c 6e20 2020  anel-body">\n   
+001704c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001704d0: 2020 2020 2020 2020 203c 6469 7620 6e67           <div ng
+001704e0: 2d69 663d 226d 6f64 656c 2e64 6573 6372  -if="model.descr
+001704f0: 6970 7469 6f6e 2220 636c 6173 733d 226d  iption" class="m
+00170500: 6f64 656c 2d6d 6172 6b64 6f77 6e22 206d  odel-markdown" m
+00170510: 6172 6b65 643d 226d 6f64 656c 2e64 6573  arked="model.des
+00170520: 6372 6970 7469 6f6e 223e 3c2f 6469 763e  cription"></div>
+00170530: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00170540: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00170550: 6976 206e 672d 6966 3d22 216d 6f64 656c  iv ng-if="!model
+00170560: 2e64 6573 6372 6970 7469 6f6e 223e 5468  .description">Th
+00170570: 6973 207b 7b20 6d6f 6465 6c2e 7265 736f  is {{ model.reso
+00170580: 7572 6365 5f74 7970 6520 7d7d 2069 7320  urce_type }} is 
+00170590: 6e6f 7420 6375 7272 656e 746c 7920 646f  not currently do
+001705a0: 6375 6d65 6e74 6564 3c2f 6469 763e 5c6e  cumented</div>\n
 001705b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001705c0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
-001705d0: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
-001705e0: 2020 2020 2020 2020 2020 2020 3c2f 7365              </se
-001705f0: 6374 696f 6e3e 5c6e 5c6e 2020 2020 2020  ction>\n\n      
-00170600: 2020 2020 2020 3c73 6563 7469 6f6e 2063        <section c
-00170610: 6c61 7373 3d22 7365 6374 696f 6e22 206e  lass="section" n
-00170620: 672d 7368 6f77 203d 2022 7061 7265 6e74  g-show = "parent
-00170630: 734c 656e 6774 6820 213d 2030 223e 5c6e  sLength != 0">\n
-00170640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00170650: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
-00170660: 696f 6e2d 7461 7267 6574 2220 6964 3d22  ion-target" id="
-00170670: 6465 7065 6e64 735f 6f6e 223e 3c2f 6469  depends_on"></di
-00170680: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
-00170690: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-001706a0: 7365 6374 696f 6e2d 636f 6e74 656e 7422  section-content"
-001706b0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
-001706c0: 2020 2020 2020 203c 6836 3e44 6570 656e         <h6>Depen
-001706d0: 6473 204f 6e3c 2f68 363e 5c6e 2020 2020  ds On</h6>\n    
-001706e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-001706f0: 3c72 6566 6572 656e 6365 2d6c 6973 7420  <reference-list 
-00170700: 7265 6665 7265 6e63 6573 3d22 7061 7265  references="pare
-00170710: 6e74 7322 206e 6f64 653d 226d 6f64 656c  nts" node="model
-00170720: 2220 2f3e 5c6e 2020 2020 2020 2020 2020  " />\n          
-00170730: 2020 2020 2020 3c2f 6469 763e 5c6e 2020        </div>\n  
-00170740: 2020 2020 2020 2020 2020 3c2f 7365 6374            </sect
-00170750: 696f 6e3e 5c6e 5c6e 2020 2020 2020 2020  ion>\n\n        
-00170760: 2020 2020 3c73 6563 7469 6f6e 2063 6c61      <section cla
-00170770: 7373 3d22 7365 6374 696f 6e22 3e5c 6e20  ss="section">\n 
-00170780: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00170790: 6469 7620 636c 6173 733d 2273 6563 7469  div class="secti
-001707a0: 6f6e 2d74 6172 6765 7422 2069 643d 2263  on-target" id="c
-001707b0: 6f64 6522 3e3c 2f64 6976 3e5c 6e20 2020  ode"></div>\n   
-001707c0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-001707d0: 7620 636c 6173 733d 2273 6563 7469 6f6e  v class="section
-001707e0: 2d63 6f6e 7465 6e74 223e 5c6e 2020 2020  -content">\n    
-001707f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00170800: 3c63 6f64 652d 626c 6f63 6b20 7665 7273  <code-block vers
-00170810: 696f 6e73 3d22 7665 7273 696f 6e73 2220  ions="versions" 
-00170820: 6465 6661 756c 743d 2264 6566 6175 6c74  default="default
-00170830: 5f76 6572 7369 6f6e 2220 6c61 6e67 7561  _version" langua
-00170840: 6765 3d22 6c61 6e67 7561 6765 223e 3c2f  ge="language"></
-00170850: 636f 6465 2d62 6c6f 636b 3e5c 6e20 2020  code-block>\n   
-00170860: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00170870: 6976 3e5c 6e20 2020 2020 2020 2020 2020  iv>\n           
-00170880: 203c 2f73 6563 7469 6f6e 3e5c 6e20 2020   </section>\n   
-00170890: 2020 2020 203c 2f64 6976 3e5c 6e20 2020       </div>\n   
-001708a0: 203c 2f64 6976 3e5c 6e3c 2f64 6976 3e5c   </div>\n</div>\
-001708b0: 6e27 297d 5d29 2c65 2e65 7870 6f72 7473  n')}]),e.exports
-001708c0: 3d6e 7d5d 293b 0a2f 2f23 2073 6f75 7263  =n}]);.//# sourc
-001708d0: 654d 6170 7069 6e67 5552 4c3d 6d61 696e  eMappingURL=main
-001708e0: 2e6a 732e 6d61 703c 2f73 6372 6970 743e  .js.map</script>
-001708f0: 3c2f 626f 6479 3e0a 3c2f 6874 6d6c 3e0a  </body>.</html>.
+001705c0: 2020 2020 2020 2020 3c2f 6469 763e 5c6e          </div>\n
+001705d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+001705e0: 2020 2020 3c2f 6469 763e 5c6e 2020 2020      </div>\n    
+001705f0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00170600: 763e 5c6e 2020 2020 2020 2020 2020 2020  v>\n            
+00170610: 3c2f 7365 6374 696f 6e3e 5c6e 5c6e 2020  </section>\n\n  
+00170620: 2020 2020 2020 2020 2020 3c73 6563 7469            <secti
+00170630: 6f6e 2063 6c61 7373 3d22 7365 6374 696f  on class="sectio
+00170640: 6e22 206e 672d 7368 6f77 203d 2022 7061  n" ng-show = "pa
+00170650: 7265 6e74 734c 656e 6774 6820 213d 2030  rentsLength != 0
+00170660: 223e 5c6e 2020 2020 2020 2020 2020 2020  ">\n            
+00170670: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00170680: 7365 6374 696f 6e2d 7461 7267 6574 2220  section-target" 
+00170690: 6964 3d22 6465 7065 6e64 735f 6f6e 223e  id="depends_on">
+001706a0: 3c2f 6469 763e 5c6e 2020 2020 2020 2020  </div>\n        
+001706b0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+001706c0: 7373 3d22 7365 6374 696f 6e2d 636f 6e74  ss="section-cont
+001706d0: 656e 7422 3e5c 6e20 2020 2020 2020 2020  ent">\n         
+001706e0: 2020 2020 2020 2020 2020 203c 6836 3e44             <h6>D
+001706f0: 6570 656e 6473 204f 6e3c 2f68 363e 5c6e  epends On</h6>\n
+00170700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00170710: 2020 2020 3c72 6566 6572 656e 6365 2d6c      <reference-l
+00170720: 6973 7420 7265 6665 7265 6e63 6573 3d22  ist references="
+00170730: 7061 7265 6e74 7322 206e 6f64 653d 226d  parents" node="m
+00170740: 6f64 656c 2220 2f3e 5c6e 2020 2020 2020  odel" />\n      
+00170750: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00170760: 5c6e 2020 2020 2020 2020 2020 2020 3c2f  \n            </
+00170770: 7365 6374 696f 6e3e 5c6e 5c6e 2020 2020  section>\n\n    
+00170780: 2020 2020 2020 2020 3c73 6563 7469 6f6e          <section
+00170790: 2063 6c61 7373 3d22 7365 6374 696f 6e22   class="section"
+001707a0: 3e5c 6e20 2020 2020 2020 2020 2020 2020  >\n             
+001707b0: 2020 203c 6469 7620 636c 6173 733d 2273     <div class="s
+001707c0: 6563 7469 6f6e 2d74 6172 6765 7422 2069  ection-target" i
+001707d0: 643d 2263 6f64 6522 3e3c 2f64 6976 3e5c  d="code"></div>\
+001707e0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+001707f0: 203c 6469 7620 636c 6173 733d 2273 6563   <div class="sec
+00170800: 7469 6f6e 2d63 6f6e 7465 6e74 223e 5c6e  tion-content">\n
+00170810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00170820: 2020 2020 3c63 6f64 652d 626c 6f63 6b20      <code-block 
+00170830: 7665 7273 696f 6e73 3d22 7665 7273 696f  versions="versio
+00170840: 6e73 2220 6465 6661 756c 743d 2264 6566  ns" default="def
+00170850: 6175 6c74 5f76 6572 7369 6f6e 2220 6c61  ault_version" la
+00170860: 6e67 7561 6765 3d22 6c61 6e67 7561 6765  nguage="language
+00170870: 223e 3c2f 636f 6465 2d62 6c6f 636b 3e5c  "></code-block>\
+00170880: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
+00170890: 203c 2f64 6976 3e5c 6e20 2020 2020 2020   </div>\n       
+001708a0: 2020 2020 203c 2f73 6563 7469 6f6e 3e5c       </section>\
+001708b0: 6e20 2020 2020 2020 203c 2f64 6976 3e5c  n        </div>\
+001708c0: 6e20 2020 203c 2f64 6976 3e5c 6e3c 2f64  n    </div>\n</d
+001708d0: 6976 3e5c 6e27 297d 5d29 2c65 2e65 7870  iv>\n')}]),e.exp
+001708e0: 6f72 7473 3d6e 7d5d 293b 0a2f 2f23 2073  orts=n}]);.//# s
+001708f0: 6f75 7263 654d 6170 7069 6e67 5552 4c3d  ourceMappingURL=
+00170900: 6d61 696e 2e6a 732e 6d61 703c 2f73 6372  main.js.map</scr
+00170910: 6970 743e 3c2f 626f 6479 3e0a 3c2f 6874  ipt></body>.</ht
+00170920: 6d6c 3e0a                                ml>.
```

### Comparing `dbt_core-1.8.0b3/dbt/task/docs/serve.py` & `dbt_core-1.8.0rc1/dbt/task/docs/serve.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/freshness.py` & `dbt_core-1.8.0rc1/dbt/task/freshness.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     PartialSourceFreshnessResult,
     SourceFreshnessResult,
     FreshnessStatus,
 )
 from dbt_common.exceptions import DbtRuntimeError, DbtInternalError
 from dbt_common.events.functions import fire_event
 from dbt_common.events.types import Note
+from dbt import deprecations
 from dbt.events.types import (
     FreshnessCheckComplete,
     LogStartLine,
     LogFreshnessResult,
 )
 from dbt.contracts.results import RunStatus
 from dbt.node_types import NodeType, RunHookType
@@ -236,17 +237,20 @@
                 RunStatus.Error,
             ):
                 print_run_result_error(result)
 
         fire_event(FreshnessCheckComplete())
 
     def get_hooks_by_type(self, hook_type: RunHookType) -> List[HookNode]:
+        hooks = super().get_hooks_by_type(hook_type)
         if self.args.source_freshness_run_project_hooks:
-            return super().get_hooks_by_type(hook_type)
+            return hooks
         else:
+            if hooks:
+                deprecations.warn("source-freshness-project-hooks")
             return []
 
     def populate_metadata_freshness_cache(self, adapter, selected_uids: AbstractSet[str]) -> None:
         if self.manifest is None:
             raise DbtInternalError("Manifest must be set to populate metadata freshness cache")
 
         batch_metadata_sources: List[BaseRelation] = []
```

### Comparing `dbt_core-1.8.0b3/dbt/task/init.py` & `dbt_core-1.8.0rc1/dbt/task/init.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/list.py` & `dbt_core-1.8.0rc1/dbt/task/list.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/printer.py` & `dbt_core-1.8.0rc1/dbt/task/printer.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/retry.py` & `dbt_core-1.8.0rc1/dbt/task/retry.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/run.py` & `dbt_core-1.8.0rc1/dbt/task/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -450,18 +450,18 @@
             FinishedRunningStats(
                 stat_line=stat_line, execution=execution, execution_time=execution_time
             )
         )
 
     def before_run(self, adapter, selected_uids: AbstractSet[str]) -> None:
         with adapter.connection_named("master"):
+            self.defer_to_manifest()
             required_schemas = self.get_model_schemas(adapter, selected_uids)
             self.create_schemas(adapter, required_schemas)
             self.populate_adapter_cache(adapter, required_schemas)
-            self.defer_to_manifest(adapter, selected_uids)
             self.safe_run_hooks(adapter, RunHookType.Start, {})
 
     def after_run(self, adapter, results) -> None:
         # in on-run-end hooks, provide the value 'database_schemas', which is a
         # list of unique (database, schema) pairs that successfully executed
         # models were in. For backwards compatibility, include the old
         # 'schemas', which did not include database information.
```

### Comparing `dbt_core-1.8.0b3/dbt/task/run_operation.py` & `dbt_core-1.8.0rc1/dbt/task/run_operation.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/runnable.py` & `dbt_core-1.8.0rc1/dbt/task/runnable.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,58 +104,42 @@
 
     @property
     def exclusion_arg(self):
         return self.args.exclude
 
     def get_selection_spec(self) -> SelectionSpec:
         default_selector_name = self.config.get_default_selector_name()
-        # TODO:  The "eager" string below needs to be replaced with programatic access
-        #  to the default value for the indirect selection parameter in
-        # dbt.cli.params.indirect_selection
-        #
-        # Doing that is actually a little tricky, so I'm punting it to a new ticket GH #6397
-        indirect_selection = getattr(self.args, "INDIRECT_SELECTION", "eager")
-
         if self.args.selector:
             # use pre-defined selector (--selector)
             spec = self.config.get_selector(self.args.selector)
         elif not (self.selection_arg or self.exclusion_arg) and default_selector_name:
             # use pre-defined selector (--selector) with default: true
             fire_event(DefaultSelector(name=default_selector_name))
             spec = self.config.get_selector(default_selector_name)
         else:
             # This is what's used with no default selector and no selection
             # use --select and --exclude args
-            spec = parse_difference(self.selection_arg, self.exclusion_arg, indirect_selection)
+            spec = parse_difference(self.selection_arg, self.exclusion_arg)
         # mypy complains because the return values of get_selector and parse_difference
         # are different
         return spec  # type: ignore
 
     @abstractmethod
     def get_node_selector(self) -> NodeSelector:
         raise NotImplementedError(f"get_node_selector not implemented for task {type(self)}")
 
-    def defer_to_manifest(self, adapter, selected_uids: AbstractSet[str]):
+    def defer_to_manifest(self):
         deferred_manifest = self._get_deferred_manifest()
         if deferred_manifest is None:
             return
         if self.manifest is None:
             raise DbtInternalError(
                 "Expected to defer to manifest, but there is no runtime manifest to defer from!"
             )
-        self.manifest.merge_from_artifact(
-            adapter=adapter,
-            other=deferred_manifest,
-            selected=selected_uids,
-            favor_state=bool(self.args.favor_state),
-        )
-        # We're rewriting the manifest because it's been mutated during merge_from_artifact.
-        # This is to reflect which nodes had been deferred to (= replaced with) their counterparts.
-        if self.args.write_json:
-            write_manifest(self.manifest, self.config.project_target_path)
+        self.manifest.merge_from_artifact(other=deferred_manifest)
 
     def get_graph_queue(self) -> GraphQueue:
         selector = self.get_node_selector()
         # Following uses self.selection_arg and self.exclusion_arg
         spec = self.get_selection_spec()
         return selector.get_graph_queue(spec)
 
@@ -482,16 +466,16 @@
         if dbt.tracking.active_user is not None:
             dbt.tracking.track_runnable_timing(
                 {"adapter_cache_construction_elapsed": cache_populate_time}
             )
 
     def before_run(self, adapter, selected_uids: AbstractSet[str]):
         with adapter.connection_named("master"):
+            self.defer_to_manifest()
             self.populate_adapter_cache(adapter)
-            self.defer_to_manifest(adapter, selected_uids)
 
     def after_run(self, adapter, results):
         pass
 
     def print_results_line(self, node_results, elapsed):
         pass
```

### Comparing `dbt_core-1.8.0b3/dbt/task/seed.py` & `dbt_core-1.8.0rc1/dbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/show.py` & `dbt_core-1.8.0rc1/dbt/task/show.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/snapshot.py` & `dbt_core-1.8.0rc1/dbt/task/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/sql.py` & `dbt_core-1.8.0rc1/dbt/task/sql.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/task/test.py` & `dbt_core-1.8.0rc1/dbt/task/test.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/tests/fixtures/project.py` & `dbt_core-1.8.0rc1/dbt/tests/fixtures/project.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/tests/util.py` & `dbt_core-1.8.0rc1/dbt/tests/util.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/tracking.py` & `dbt_core-1.8.0rc1/dbt/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/utils.py` & `dbt_core-1.8.0rc1/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/dbt/version.py` & `dbt_core-1.8.0rc1/dbt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,9 +225,9 @@
             # the path is like .../dbt/adapters/{plugin_name}/__version__.py
             # except it could be \\ on windows!
             plugin_root, _ = os.path.split(version_path)
             _, plugin_name = os.path.split(plugin_root)
             yield plugin_name
 
 
-__version__ = "1.8.0b3"
+__version__ = "1.8.0rc1"
 installed = get_installed_version()
```

### Comparing `dbt_core-1.8.0b3/dbt_core.egg-info/PKG-INFO` & `dbt_core-1.8.0rc1/dbt_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.8.0b3
+Version: 1.8.0rc1
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -13,28 +13,28 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: agate<1.8,>=1.7.0
+Requires-Dist: agate<1.10,>=1.7.0
 Requires-Dist: Jinja2<4,>=3.1.3
 Requires-Dist: mashumaro[msgpack]<4.0,>=3.9
 Requires-Dist: logbook<1.6,>=1.5
 Requires-Dist: click<9.0,>=8.0.2
 Requires-Dist: networkx<4.0,>=2.3
 Requires-Dist: protobuf<5,>=4.0.0
 Requires-Dist: requests<3.0.0
 Requires-Dist: pathspec<0.13,>=0.9
 Requires-Dist: sqlparse<0.6.0,>=0.5.0
 Requires-Dist: dbt-extractor<=0.6,>=0.5.0
 Requires-Dist: minimal-snowplow-tracker<0.1,>=0.0.2
 Requires-Dist: dbt-semantic-interfaces<0.6,>=0.5.1
-Requires-Dist: dbt-common<2.0,>=1.0.1
+Requires-Dist: dbt-common<2.0,>=1.0.2
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2
 Requires-Dist: packaging>20.9
 Requires-Dist: pytz>=2015.7
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: daff>=1.3.46
 Requires-Dist: typing-extensions>=4.4
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0b3 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0rc1 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Python: >=3.8 Description-Content-Type:
-text/markdown Requires-Dist: agate<1.8,>=1.7.0 Requires-Dist: Jinja2<4,>=3.1.3
+text/markdown Requires-Dist: agate<1.10,>=1.7.0 Requires-Dist: Jinja2<4,>=3.1.3
 Requires-Dist: mashumaro[msgpack]<4.0,>=3.9 Requires-Dist: logbook<1.6,>=1.5
 Requires-Dist: click<9.0,>=8.0.2 Requires-Dist: networkx<4.0,>=2.3 Requires-
 Dist: protobuf<5,>=4.0.0 Requires-Dist: requests<3.0.0 Requires-Dist:
 pathspec<0.13,>=0.9 Requires-Dist: sqlparse<0.6.0,>=0.5.0 Requires-Dist: dbt-
 extractor<=0.6,>=0.5.0 Requires-Dist: minimal-snowplow-tracker<0.1,>=0.0.2
 Requires-Dist: dbt-semantic-interfaces<0.6,>=0.5.1 Requires-Dist: dbt-
-common<2.0,>=1.0.1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2 Requires-Dist:
+common<2.0,>=1.0.2 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2 Requires-Dist:
 packaging>20.9 Requires-Dist: pytz>=2015.7 Requires-Dist: pyyaml>=6.0 Requires-
 Dist: daff>=1.3.46 Requires-Dist: typing-extensions>=4.4
                                   [dbt logo]
                                   _[_C_I_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. ![architecture](https://raw.githubusercontent.com/dbt-labs/
```

### Comparing `dbt_core-1.8.0b3/dbt_core.egg-info/SOURCES.txt` & `dbt_core-1.8.0rc1/dbt_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt_core-1.8.0b3/setup.py` & `dbt_core-1.8.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 package_name = "dbt-core"
-package_version = "1.8.0b3"
+package_version = "1.8.0rc1"
 description = """With dbt, data analysts and engineers can build analytics \
 the way engineers build applications."""
 
 
 setup(
     name=package_name,
     version=package_version,
@@ -45,15 +45,15 @@
     entry_points={
         "console_scripts": ["dbt = dbt.cli.main:cli"],
     },
     install_requires=[
         # ----
         # dbt-core uses these packages deeply, throughout the codebase, and there have been breaking changes in past patch releases (even though these are major-version-one).
         # Pin to the patch or minor version, and bump in each new minor version of dbt-core.
-        "agate>=1.7.0,<1.8",
+        "agate>=1.7.0,<1.10",
         "Jinja2>=3.1.3,<4",
         "mashumaro[msgpack]>=3.9,<4.0",
         # ----
         # Legacy: This package has not been updated since 2019, and it is unused in dbt's logging system (since v1.0)
         # The dependency here will be removed along with the removal of 'legacy logging', in a future release of dbt-core
         "logbook>=1.5,<1.6",
         # ----
@@ -71,15 +71,15 @@
         # ----
         # These are major-version-0 packages also maintained by dbt-labs.
         # Accept patches but avoid automatically updating past a set minor version range.
         "dbt-extractor>=0.5.0,<=0.6",
         "minimal-snowplow-tracker>=0.0.2,<0.1",
         "dbt-semantic-interfaces>=0.5.1,<0.6",
         # Minor versions for these are expected to be backwards-compatible
-        "dbt-common>=1.0.1,<2.0",
+        "dbt-common>=1.0.2,<2.0",
         "dbt-adapters>=0.1.0a2,<2.0",
         # ----
         # Expect compatibility with all new versions of these packages, so lower bounds only.
         "packaging>20.9",
         "pytz>=2015.7",
         "pyyaml>=6.0",
         "daff>=1.3.46",
```

