# Comparing `tmp/dagshub-0.3.8.post2.tar.gz` & `tmp/dagshub-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagshub-0.3.8.post2.tar", last modified: Thu Oct 19 12:47:31 2023, max compression
+gzip compressed data, was "dagshub-0.3.9.tar", last modified: Wed Nov  8 10:21:15 2023, max compression
```

## Comparing `dagshub-0.3.8.post2.tar` & `dagshub-0.3.9.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.297091 dagshub-0.3.8.post2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10578 2023-10-19 12:47:31.297091 dagshub-0.3.8.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9714 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.285091 dagshub-0.3.8.post2/dagshub/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.289091 dagshub-0.3.8.post2/dagshub/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/auth/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/auth/token_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    13971 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/auth/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.289091 dagshub-0.3.8.post2/dagshub/common/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/common/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.289091 dagshub-0.3.8.post2/dagshub/common/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/common/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/common/api/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/common/api/responses.py
--rw-r--r--   0 runner    (1001) docker     (127)     9573 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/common/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/common/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/common/logging_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/common/rich_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/common/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.289091 dagshub-0.3.8.post2/dagshub/data_engine/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.289091 dagshub-0.3.8.post2/dagshub/data_engine/annotation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/annotation/voxel_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.289091 dagshub-0.3.8.post2/dagshub/data_engine/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/client/data_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/client/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/client/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.293091 dagshub-0.3.8.post2/dagshub/data_engine/client/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/client/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7710 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/client/loaders/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/client/loaders/tf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/client/loaders/torch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.293091 dagshub-0.3.8.post2/dagshub/data_engine/client/query_builder/
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/client/query_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/datasources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/dtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.293091 dagshub-0.3.8.post2/dagshub/data_engine/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7741 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/model/datapoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    29985 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/model/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/model/datasource_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/model/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/model/metadata_field_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/model/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    18765 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/model/query_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/model/schema_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.293091 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.285091 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.293091 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.293091 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    42241 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.293091 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/
--rw-r--r--   0 runner    (1001) docker     (127)   182256 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/fiftyone.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.293091 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/routes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/routes/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/routes/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/routes/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/routes/voxel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.293091 dagshub-0.3.8.post2/dagshub/fastai/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/fastai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/fastai/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.293091 dagshub-0.3.8.post2/dagshub/keras/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/keras/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/notebook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.293091 dagshub-0.3.8.post2/dagshub/pytorch_lightning/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/pytorch_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/pytorch_lightning/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/pytorch_lightning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.297091 dagshub-0.3.8.post2/dagshub/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/streaming/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/streaming/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    39648 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/streaming/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/streaming/mount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.297091 dagshub-0.3.8.post2/dagshub/upload/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/upload/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    27928 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/dagshub/upload/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.289091 dagshub-0.3.8.post2/dagshub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10578 2023-10-19 12:47:31.000000 dagshub-0.3.8.post2/dagshub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2023-10-19 12:47:31.000000 dagshub-0.3.8.post2/dagshub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 12:47:31.000000 dagshub-0.3.8.post2/dagshub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-10-19 12:47:31.000000 dagshub-0.3.8.post2/dagshub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      221 2023-10-19 12:47:31.000000 dagshub-0.3.8.post2/dagshub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-19 12:47:31.000000 dagshub-0.3.8.post2/dagshub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-19 12:47:31.297091 dagshub-0.3.8.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:47:31.297091 dagshub-0.3.8.post2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/tests/test_dagshub_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2023-10-19 12:47:21.000000 dagshub-0.3.8.post2/tests/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.577049 dagshub-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-08 10:21:03.000000 dagshub-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-08 10:21:03.000000 dagshub-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10563 2023-11-08 10:21:15.577049 dagshub-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9714 2023-11-08 10:21:03.000000 dagshub-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.561049 dagshub-0.3.9/dagshub/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.561049 dagshub-0.3.9/dagshub/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/auth/token_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13971 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/auth/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.565049 dagshub-0.3.9/dagshub/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/common/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.565049 dagshub-0.3.9/dagshub/common/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/common/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/common/api/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/common/api/responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9573 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/common/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/common/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/common/logging_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/common/rich_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/common/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.565049 dagshub-0.3.9/dagshub/data_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.565049 dagshub-0.3.9/dagshub/data_engine/annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/annotation/voxel_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.569049 dagshub-0.3.9/dagshub/data_engine/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/client/data_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/client/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/client/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.569049 dagshub-0.3.9/dagshub/data_engine/client/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/client/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7710 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/client/loaders/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/client/loaders/tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/client/loaders/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.569049 dagshub-0.3.9/dagshub/data_engine/client/query_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/client/query_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/datasources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.569049 dagshub-0.3.9/dagshub/data_engine/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/model/datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29985 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/model/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/model/datasource_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/model/metadata_field_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18765 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/model/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/model/schema_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.569049 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.557049 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.573049 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.573049 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    42241 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.573049 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)   182256 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/fiftyone.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.573049 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/routes/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/routes/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/routes/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/routes/voxel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.573049 dagshub-0.3.9/dagshub/fastai/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/fastai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/fastai/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.573049 dagshub-0.3.9/dagshub/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/keras/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.573049 dagshub-0.3.9/dagshub/pytorch_lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/pytorch_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/pytorch_lightning/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/pytorch_lightning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.577049 dagshub-0.3.9/dagshub/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/streaming/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/streaming/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39648 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/streaming/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/streaming/mount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.577049 dagshub-0.3.9/dagshub/upload/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/upload/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27928 2023-11-08 10:21:03.000000 dagshub-0.3.9/dagshub/upload/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.561049 dagshub-0.3.9/dagshub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10563 2023-11-08 10:21:15.000000 dagshub-0.3.9/dagshub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2023-11-08 10:21:15.000000 dagshub-0.3.9/dagshub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 10:21:15.000000 dagshub-0.3.9/dagshub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-08 10:21:15.000000 dagshub-0.3.9/dagshub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-11-08 10:21:15.000000 dagshub-0.3.9/dagshub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-08 10:21:15.000000 dagshub-0.3.9/dagshub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-11-08 10:21:03.000000 dagshub-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-08 10:21:15.577049 dagshub-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2023-11-08 10:21:03.000000 dagshub-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 10:21:15.577049 dagshub-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2023-11-08 10:21:03.000000 dagshub-0.3.9/tests/test_dagshub_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2023-11-08 10:21:03.000000 dagshub-0.3.9/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2023-11-08 10:21:03.000000 dagshub-0.3.9/tests/test_misc.py
```

### Comparing `dagshub-0.3.8.post2/LICENSE` & `dagshub-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/PKG-INFO` & `dagshub-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagshub
-Version: 0.3.8.post2
+Version: 0.3.9
 Summary: DagsHub client libraries
 Home-page: https://github.com/DagsHub/client
 Author: DagsHub
 Author-email: contact@dagshub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 License-File: LICENSE
 Requires-Dist: PyYAML>=5
 Requires-Dist: fusepy>=3
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: click>=8.0.4
 Requires-Dist: httpx~=0.23.0
 Requires-Dist: GitPython>=3.1.29
-Requires-Dist: rich[jupyter]~=13.1.0
+Requires-Dist: rich~=13.1.0
 Requires-Dist: dacite~=1.6.0
 Requires-Dist: tenacity~=8.2.2
 Requires-Dist: gql[requests]
 Requires-Dist: dataclasses-json
 Requires-Dist: pandas
 Requires-Dist: treelib~=1.6.4
 Requires-Dist: pathvalidate~=3.0.0
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: dagshub Version: 0.3.8.post2 Summary: DagsHub
-client libraries Home-page: https://github.com/DagsHub/client Author: DagsHub
-Author-email: contact@dagshub.com Classifier: Programming Language :: Python ::
-3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
+Metadata-Version: 2.1 Name: dagshub Version: 0.3.9 Summary: DagsHub client
+libraries Home-page: https://github.com/DagsHub/client Author: DagsHub Author-
+email: contact@dagshub.com Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: PyYAML>=5 Requires-Dist:
 fusepy>=3 Requires-Dist: appdirs>=1.4.4 Requires-Dist: click>=8.0.4 Requires-
-Dist: httpx~=0.23.0 Requires-Dist: GitPython>=3.1.29 Requires-Dist: rich
-[jupyter]~=13.1.0 Requires-Dist: dacite~=1.6.0 Requires-Dist: tenacity~=8.2.2
+Dist: httpx~=0.23.0 Requires-Dist: GitPython>=3.1.29 Requires-Dist:
+rich~=13.1.0 Requires-Dist: dacite~=1.6.0 Requires-Dist: tenacity~=8.2.2
 Requires-Dist: gql[requests] Requires-Dist: dataclasses-json Requires-Dist:
 pandas Requires-Dist: treelib~=1.6.4 Requires-Dist: pathvalidate~=3.0.0
 Requires-Dist: python-dateutil [![DagsHub Client](https://github.com/DagsHub/
 client/raw/master/dagshub_github.png)](https://dagshub.com)
   ******** ?ð??? LLaauunncchhiinngg _DD_aa_tt_aa_ _EE_nn_gg_ii_nn_ee ffoorr ppoowweerrffuull ppaannddaass--lliikkee mmaannaaggeemmeenntt ooff ffiillee
                               ddaattaasseettss!! ?ð??? ********
```

### Comparing `dagshub-0.3.8.post2/README.md` & `dagshub-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/auth/oauth.py` & `dagshub-0.3.9/dagshub/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/auth/token_auth.py` & `dagshub-0.3.9/dagshub/auth/token_auth.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/auth/tokens.py` & `dagshub-0.3.9/dagshub/auth/tokens.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/common/analytics.py` & `dagshub-0.3.9/dagshub/common/analytics.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/common/api/repo.py` & `dagshub-0.3.9/dagshub/common/api/repo.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/common/api/responses.py` & `dagshub-0.3.9/dagshub/common/api/responses.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/common/cli.py` & `dagshub-0.3.9/dagshub/common/cli.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/common/config.py` & `dagshub-0.3.9/dagshub/common/config.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/common/download.py` & `dagshub-0.3.9/dagshub/common/download.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/common/helpers.py` & `dagshub-0.3.9/dagshub/common/helpers.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/common/init.py` & `dagshub-0.3.9/dagshub/common/init.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/common/logging_util.py` & `dagshub-0.3.9/dagshub/common/logging_util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/common/util.py` & `dagshub-0.3.9/dagshub/common/util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/annotation/voxel_conversion.py` & `dagshub-0.3.9/dagshub/data_engine/annotation/voxel_conversion.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/client/data_client.py` & `dagshub-0.3.9/dagshub/data_engine/client/data_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Any, Optional, List, Dict, Union, TYPE_CHECKING
+from typing import Any, Optional, List, Dict, Union, TYPE_CHECKING, Set
 
 import dacite
 import gql
 import rich.progress
 from gql.transport.requests import RequestsHTTPTransport
 
 import dagshub.auth
@@ -27,15 +27,15 @@
 from dagshub.data_engine.model.query_result import QueryResult
 
 if TYPE_CHECKING:
     from dagshub.data_engine.datasources import DatasourceState
 
 logger = logging.getLogger(__name__)
 
-dacite_config = dacite.Config(cast=[IntegrationStatus, DatasourceType, PreprocessingStatus, MetadataFieldType])
+dacite_config = dacite.Config(cast=[IntegrationStatus, DatasourceType, PreprocessingStatus, MetadataFieldType, Set])
 
 
 class DataClient:
     HEAD_QUERY_SIZE = 100
     FULL_LIST_PAGE_SIZE = 5000
 
     def __init__(self, repo: str):
```

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/client/gql_mutations.py` & `dagshub-0.3.9/dagshub/data_engine/client/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/client/gql_queries.py` & `dagshub-0.3.9/dagshub/data_engine/client/gql_queries.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/client/loaders/base.py` & `dagshub-0.3.9/dagshub/data_engine/client/loaders/base.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/client/loaders/tf.py` & `dagshub-0.3.9/dagshub/data_engine/client/loaders/tf.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/client/loaders/torch.py` & `dagshub-0.3.9/dagshub/data_engine/client/loaders/torch.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/client/models.py` & `dagshub-0.3.9/dagshub/data_engine/client/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import enum
 import logging
 from dataclasses import dataclass, field
-from typing import Any, List, Union, Optional
+from typing import Any, List, Union, Optional, Set
 
 from dataclasses_json import dataclass_json, config
 from dagshub.data_engine.dtypes import MetadataFieldType, ReservedTags
 
 logger = logging.getLogger(__name__)
 
 
@@ -48,15 +48,15 @@
 @dataclass_json
 @dataclass
 class MetadataFieldSchema:
     # This should match the GraphQL schema: MetadataFieldProps
     name: str
     valueType: MetadataFieldType = field(metadata=config(encoder=lambda val: val.value))
     multiple: bool
-    tags: Optional[List[str]]
+    tags: Optional[Set[str]]
 
     def __repr__(self):
         res = f"{self.name} ({self.valueType.value})"
         if self.tags is not None and len(self.tags) > 0:
             res += f" with tags: {self.tags}"
         return res
```

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/client/query_builder/__init__.py` & `dagshub-0.3.9/dagshub/data_engine/client/query_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/datasets.py` & `dagshub-0.3.9/dagshub/data_engine/datasets.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/datasources.py` & `dagshub-0.3.9/dagshub/data_engine/datasources.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/dtypes.py` & `dagshub-0.3.9/dagshub/data_engine/dtypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import enum
 from abc import ABCMeta
-from typing import List
+from typing import Set
 
 
 class ReservedTags(enum.Enum):
     ANNOTATION = "annotation"
 
 
 # These are the base primitives that the data engine database is capable of storing
@@ -22,15 +22,15 @@
     """
     Attributes:
         backing_field_type: primitive type in the data engine database
         custom_tags: additional tags applied to this type
     """
 
     backing_field_type: MetadataFieldType = None
-    custom_tags: List[str] = None
+    custom_tags: Set[str] = None
 
 
 class Int(DagshubDataType):
     backing_field_type = MetadataFieldType.INTEGER
 
 
 class String(DagshubDataType):
@@ -47,13 +47,13 @@
 
 class Bool(DagshubDataType):
     backing_field_type = MetadataFieldType.BOOLEAN
 
 
 class LabelStudioAnnotation(DagshubDataType):
     backing_field_type = MetadataFieldType.BLOB
-    custom_tags = [ReservedTags.ANNOTATION.value]
+    custom_tags = {ReservedTags.ANNOTATION.value}
 
 
 class Voxel51Annotation(DagshubDataType):
     backing_field_type = MetadataFieldType.BLOB
-    custom_tags = [ReservedTags.ANNOTATION.value]
+    custom_tags = {ReservedTags.ANNOTATION.value}
```

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/model/datapoint.py` & `dagshub-0.3.9/dagshub/data_engine/model/datapoint.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/model/datasource.py` & `dagshub-0.3.9/dagshub/data_engine/model/datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/model/datasource_state.py` & `dagshub-0.3.9/dagshub/data_engine/model/datasource_state.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/model/errors.py` & `dagshub-0.3.9/dagshub/data_engine/model/errors.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/model/metadata_field_builder.py` & `dagshub-0.3.9/dagshub/data_engine/model/metadata_field_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses
 import logging
-from typing import TYPE_CHECKING, Type, Union, List
+from typing import TYPE_CHECKING, Type, Union, Set
 
 from dagshub.data_engine.client.models import MetadataFieldSchema
 from dagshub.data_engine.dtypes import DagshubDataType, MetadataFieldType, ReservedTags
 from dagshub.data_engine.model.schema_util import metadataTypeLookup
 
 if TYPE_CHECKING:
     from dagshub.data_engine.model.datasource import Datasource
@@ -49,15 +49,17 @@
         The type can be either a Python primitive supported by the Data Engine (str, bool, int, float, bytes)
         Or it can be a DagshubDataType inheritor (found in dagshub.data_engine.dtypes)
             The DataType inheritors can define additional tags on top of just the basic backing type
         """
         backing_type = self._get_backing_type(t)
 
         if self._schema is None:
-            self._schema = MetadataFieldSchema(name=self._field_name, valueType=backing_type, multiple=False, tags=[])
+            self._schema = MetadataFieldSchema(
+                name=self._field_name, valueType=backing_type, multiple=False, tags=set()
+            )
             if issubclass(t, DagshubDataType) and t.custom_tags is not None:
                 self._schema.tags = t.custom_tags.copy()
         else:
             if backing_type != self._schema.valueType:
                 raise ValueError(
                     "Can't change a type of an already existing field "
                     f"(changing from {self._schema.valueType.value} to {backing_type.value})"
@@ -72,22 +74,23 @@
         Mark or unmark the field as annotation field
         """
         self._set_or_unset(ReservedTags.ANNOTATION.value, is_annotation)
         return self
 
     def _set_or_unset(self, tag, is_set):
         if is_set:
-            self._add_tags([tag])
+            self._add_tags({tag})
         else:
             self._remove_tag(tag)
 
-    def _add_tags(self, tags: List[str]):
+    def _add_tags(self, tags: Set[str]):
         if self.schema.tags is None:
-            self.schema.tags = []
-        self.schema.tags.extend(tags)
+            self.schema.tags = set()
+        for t in tags:
+            self.schema.tags.add(t)
 
     def _remove_tag(self, tag: str):
         if self.schema.tags is None:
             return
         try:
             self.schema.tags.remove(tag)
         except ValueError:
```

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/model/query.py` & `dagshub-0.3.9/dagshub/data_engine/model/query.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/model/query_result.py` & `dagshub-0.3.9/dagshub/data_engine/model/query_result.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/app.py` & `dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/app.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/models.py` & `dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/models.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg` & `dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/assets/dagshub.svg`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js` & `dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/plugins/dagshub/dist/index.umd.js`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/routes/annotation.py` & `dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/routes/annotation.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/routes/datasource.py` & `dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/routes/datasource.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/routes/util.py` & `dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/routes/util.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/routes/voxel.py` & `dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/routes/voxel.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/server.py` & `dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/server.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/data_engine/voxel_plugin_server/utils.py` & `dagshub-0.3.9/dagshub/data_engine/voxel_plugin_server/utils.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/fastai/logger.py` & `dagshub-0.3.9/dagshub/fastai/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/keras/logger.py` & `dagshub-0.3.9/dagshub/keras/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/logger.py` & `dagshub-0.3.9/dagshub/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/notebook.py` & `dagshub-0.3.9/dagshub/notebook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import datetime
 import json
 import logging
 import tempfile
 from pathlib import Path, PurePosixPath
 from socket import gethostname, gethostbyname
+from typing import TYPE_CHECKING
 
 import httpx
 import urllib.parse
-from IPython import get_ipython
 
+from dagshub.common.util import lazy_load
 from dagshub.common.helpers import log_message
 from dagshub.upload import Repo
 
+if TYPE_CHECKING:
+    import IPython as IPy
+else:
+    IPy = lazy_load("IPython")
+
+
 logger = logging.getLogger(__name__)
 
 
 def _inside_notebook():
-    return get_ipython() is not None
+    return IPy.get_ipython() is not None
 
 
 def _inside_colab():
     try:
-        if get_ipython() and "google.colab" in get_ipython().extension_manager.loaded:
+        if IPy.get_ipython() and "google.colab" in IPy.get_ipython().extension_manager.loaded:
             return True
     except Exception:
         pass
     return False
 
 
 def _default_notebook_name():
@@ -85,15 +92,15 @@
             notebook_ipynb = _message.blocking_request("get_ipynb")
             if notebook_ipynb is None or "ipynb" not in notebook_ipynb:
                 raise RuntimeError("Couldn't get notebook data from colab.")
             with open(out_path, "w") as file:
                 file.write(json.dumps(notebook_ipynb["ipynb"], indent=4))
         else:
             log_message("Saving only the execution history for the notebook in Jupyter environments", logger)
-            get_ipython().run_line_magic("notebook", out_path)
+            IPy.get_ipython().run_line_magic("notebook", out_path)
 
         repo = Repo(owner, repo, branch=branch)
         repo.upload(
             out_path,
             remote_path=remote_path.as_posix(),
             commit_message=commit_message,
             versioning=versioning,
```

### Comparing `dagshub-0.3.8.post2/dagshub/pytorch_lightning/logger.py` & `dagshub-0.3.9/dagshub/pytorch_lightning/logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/streaming/dataclasses.py` & `dagshub-0.3.9/dagshub/streaming/dataclasses.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/streaming/filesystem.py` & `dagshub-0.3.9/dagshub/streaming/filesystem.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/streaming/mount.py` & `dagshub-0.3.9/dagshub/streaming/mount.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/upload/errors.py` & `dagshub-0.3.9/dagshub/upload/errors.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub/upload/wrapper.py` & `dagshub-0.3.9/dagshub/upload/wrapper.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/dagshub.egg-info/PKG-INFO` & `dagshub-0.3.9/dagshub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagshub
-Version: 0.3.8.post2
+Version: 0.3.9
 Summary: DagsHub client libraries
 Home-page: https://github.com/DagsHub/client
 Author: DagsHub
 Author-email: contact@dagshub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 License-File: LICENSE
 Requires-Dist: PyYAML>=5
 Requires-Dist: fusepy>=3
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: click>=8.0.4
 Requires-Dist: httpx~=0.23.0
 Requires-Dist: GitPython>=3.1.29
-Requires-Dist: rich[jupyter]~=13.1.0
+Requires-Dist: rich~=13.1.0
 Requires-Dist: dacite~=1.6.0
 Requires-Dist: tenacity~=8.2.2
 Requires-Dist: gql[requests]
 Requires-Dist: dataclasses-json
 Requires-Dist: pandas
 Requires-Dist: treelib~=1.6.4
 Requires-Dist: pathvalidate~=3.0.0
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: dagshub Version: 0.3.8.post2 Summary: DagsHub
-client libraries Home-page: https://github.com/DagsHub/client Author: DagsHub
-Author-email: contact@dagshub.com Classifier: Programming Language :: Python ::
-3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
-System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
+Metadata-Version: 2.1 Name: dagshub Version: 0.3.9 Summary: DagsHub client
+libraries Home-page: https://github.com/DagsHub/client Author: DagsHub Author-
+email: contact@dagshub.com Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: PyYAML>=5 Requires-Dist:
 fusepy>=3 Requires-Dist: appdirs>=1.4.4 Requires-Dist: click>=8.0.4 Requires-
-Dist: httpx~=0.23.0 Requires-Dist: GitPython>=3.1.29 Requires-Dist: rich
-[jupyter]~=13.1.0 Requires-Dist: dacite~=1.6.0 Requires-Dist: tenacity~=8.2.2
+Dist: httpx~=0.23.0 Requires-Dist: GitPython>=3.1.29 Requires-Dist:
+rich~=13.1.0 Requires-Dist: dacite~=1.6.0 Requires-Dist: tenacity~=8.2.2
 Requires-Dist: gql[requests] Requires-Dist: dataclasses-json Requires-Dist:
 pandas Requires-Dist: treelib~=1.6.4 Requires-Dist: pathvalidate~=3.0.0
 Requires-Dist: python-dateutil [![DagsHub Client](https://github.com/DagsHub/
 client/raw/master/dagshub_github.png)](https://dagshub.com)
   ******** ?ð??? LLaauunncchhiinngg _DD_aa_tt_aa_ _EE_nn_gg_ii_nn_ee ffoorr ppoowweerrffuull ppaannddaass--lliikkee mmaannaaggeemmeenntt ooff ffiillee
                               ddaattaasseettss!! ?ð??? ********
```

### Comparing `dagshub-0.3.8.post2/dagshub.egg-info/SOURCES.txt` & `dagshub-0.3.9/dagshub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/setup.py` & `dagshub-0.3.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,26 +27,31 @@
 install_requires = [
     "PyYAML>=5",
     "fusepy>=3",
     "appdirs>=1.4.4",
     "click>=8.0.4",
     "httpx~=0.23.0",
     "GitPython>=3.1.29",
-    "rich[jupyter]~=13.1.0",
+    "rich~=13.1.0",
     # Need to keep dacite version in lockstep with voxel, otherwise stuff breaks on their end
     "dacite~=1.6.0",
     "tenacity~=8.2.2",
     "gql[requests]",
     "dataclasses-json",
     "pandas",
     "treelib~=1.6.4",
     "pathvalidate~=3.0.0",
     "python-dateutil",
 ]
 
+extras_require = {
+    "jupyter": ["rich[jupyter]~=13.1.0"],
+    "fuse": ["fusepy>=3"],
+}
+
 # Polyfills for Python 3.7
 if sys.version_info.major == 3 and sys.version_info.minor == 7:
     install_requires += [
         "cached-property==1.5.2",
         "typing_extensions",
     ]
```

### Comparing `dagshub-0.3.8.post2/tests/test_dagshub_logger.py` & `dagshub-0.3.9/tests/test_dagshub_logger.py`

 * *Files identical despite different names*

### Comparing `dagshub-0.3.8.post2/tests/test_misc.py` & `dagshub-0.3.9/tests/test_misc.py`

 * *Files identical despite different names*

