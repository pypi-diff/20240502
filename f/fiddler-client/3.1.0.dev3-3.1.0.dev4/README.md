# Comparing `tmp/fiddler-client-3.1.0.dev3.tar.gz` & `tmp/fiddler_client-3.1.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-client-3.1.0.dev3.tar", last modified: Tue Apr 30 14:58:00 2024, max compression
+gzip compressed data, was "fiddler_client-3.1.0.dev4.tar", last modified: Thu May  2 12:40:41 2024, max compression
```

## Comparing `fiddler-client-3.1.0.dev3.tar` & `fiddler_client-3.1.0.dev4.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.413544 fiddler-client-3.1.0.dev3/
--rw-r--r--   0 runner    (1001) runner    (1001)      559 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/LICENSE.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       42 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) runner    (1001)     1589 2024-04-30 14:58:00.413544 fiddler-client-3.1.0.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      855 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/PUBLIC.md
--rw-r--r--   0 runner    (1001) runner    (1001)     2165 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.393543 fiddler-client-3.1.0.dev3/fiddler/
--rw-r--r--   0 runner    (1001) runner    (1001)       11 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/VERSION
--rw-r--r--   0 runner    (1001) runner    (1001)     3824 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      217 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/configs.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5677 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/connection.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.393543 fiddler-client-3.1.0.dev3/fiddler/constants/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)      400 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/common.py
--rw-r--r--   0 runner    (1001) runner    (1001)      126 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)      114 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1706 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)      278 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)      214 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/constants/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1820 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/decorators.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.393543 fiddler-client-3.1.0.dev3/fiddler/entities/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3564 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11800 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2106 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/base.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7907 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6568 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/custom_expression.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4399 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5383 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/file.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5220 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)    19206 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5520 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/model_artifact.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3769 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1074 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/organization.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4631 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3077 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/surrogate.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1243 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/user.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4514 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)    20250 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/entities/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2221 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/exceptions.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.393543 fiddler-client-3.1.0.dev3/fiddler/libs/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/libs/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6027 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/libs/http_client.py
--rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/libs/json_encoder.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15995 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/libs/semver.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.393543 fiddler-client-3.1.0.dev3/fiddler/packtools/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/packtools/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4637 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/packtools/gem.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7941 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/packtools/keras_ig_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15799 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/packtools/project_attributions_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10467 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/packtools/template_model.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.403543 fiddler-client-3.1.0.dev3/fiddler/schemas/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      668 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1328 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)      189 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/base.py
--rw-r--r--   0 runner    (1001) runner    (1001)      933 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)      953 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/custom_expression.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5531 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/custom_features.py
--rw-r--r--   0 runner    (1001) runner    (1001)      657 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)      409 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/file.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1325 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/filter_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)      354 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1405 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1128 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1914 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/model_schema.py
--rw-r--r--   0 runner    (1001) runner    (1001)      941 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/model_spec.py
--rw-r--r--   0 runner    (1001) runner    (1001)      691 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/model_task_params.py
--rw-r--r--   0 runner    (1001) runner    (1001)      281 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/organization.py
--rw-r--r--   0 runner    (1001) runner    (1001)      379 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1166 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/response.py
--rw-r--r--   0 runner    (1001) runner    (1001)      500 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/server_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/user.py
--rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)      739 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/schemas/xai_params.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.403543 fiddler-client-3.1.0.dev3/fiddler/tests/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.403543 fiddler-client-3.1.0.dev3/fiddler/tests/apis/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3118 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11593 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7494 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8208 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_custom_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4636 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5134 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_events.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4501 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_files.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5089 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_generate_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1891 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2517 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_mixin.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18551 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5635 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model_artifact.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2441 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4443 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model_surrogate.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6015 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7804 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_segment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8099 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)    28590 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)      840 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/conftest.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/constants.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1865 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/test_connection.py
--rw-r--r--   0 runner    (1001) runner    (1001)      783 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/test_json_encoder.py
--rw-r--r--   0 runner    (1001) runner    (1001)      312 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/test_logger.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3333 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/test_utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)      335 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/tests/utils.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.413544 fiddler-client-3.1.0.dev3/fiddler/utils/
--rw-r--r--   0 runner    (1001) runner    (1001)       53 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2908 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/utils/helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/utils/logger.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2203 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/utils/model_generator.py
--rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/utils/validations.py
--rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/utils/version.py
--rw-r--r--   0 runner    (1001) runner    (1001)      140 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/fiddler/version.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 14:58:00.413544 fiddler-client-3.1.0.dev3/fiddler_client.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     1589 2024-04-30 14:58:00.000000 fiddler-client-3.1.0.dev3/fiddler_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)     3321 2024-04-30 14:58:00.000000 fiddler-client-3.1.0.dev3/fiddler_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-30 14:58:00.000000 fiddler-client-3.1.0.dev3/fiddler_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)      162 2024-04-30 14:58:00.000000 fiddler-client-3.1.0.dev3/fiddler_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        8 2024-04-30 14:58:00.000000 fiddler-client-3.1.0.dev3/fiddler_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-30 14:58:00.413544 fiddler-client-3.1.0.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)     1138 2024-04-30 14:57:54.000000 fiddler-client-3.1.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:41.132803 fiddler_client-3.1.0.dev4/
+-rw-r--r--   0 runner    (1001) runner    (1001)      559 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       42 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) runner    (1001)     1589 2024-05-02 12:40:41.122803 fiddler_client-3.1.0.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      855 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/PUBLIC.md
+-rw-r--r--   0 runner    (1001) runner    (1001)     2165 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:41.122803 fiddler_client-3.1.0.dev4/fiddler/
+-rw-r--r--   0 runner    (1001) runner    (1001)       11 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/VERSION
+-rw-r--r--   0 runner    (1001) runner    (1001)     3824 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      217 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/configs.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5677 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/connection.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:41.122803 fiddler_client-3.1.0.dev4/fiddler/constants/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/constants/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/constants/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/constants/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      400 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/constants/common.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      126 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/constants/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      114 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/constants/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/constants/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1706 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/constants/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      278 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/constants/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      214 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/constants/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1820 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/decorators.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:41.122803 fiddler_client-3.1.0.dev4/fiddler/entities/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3564 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11744 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2106 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7907 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6568 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/custom_expression.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4399 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5383 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5220 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    19271 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5520 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/model_artifact.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3966 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1074 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4631 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3077 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/surrogate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1243 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4514 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    20250 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/entities/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2221 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/exceptions.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:41.122803 fiddler_client-3.1.0.dev4/fiddler/libs/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/libs/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6027 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/libs/http_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/libs/json_encoder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15995 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/libs/semver.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:41.122803 fiddler_client-3.1.0.dev4/fiddler/packtools/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/packtools/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4637 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/packtools/gem.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7941 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/packtools/keras_ig_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15799 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/packtools/project_attributions_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10484 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/packtools/template_model.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:41.122803 fiddler_client-3.1.0.dev4/fiddler/schemas/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      668 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1387 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      189 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      933 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      953 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/custom_expression.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5531 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/custom_features.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      657 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      409 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1325 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/filter_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      354 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1405 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1128 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1914 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/model_schema.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      941 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/model_spec.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      691 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/model_task_params.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      281 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      379 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1166 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      500 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/server_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      739 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/schemas/xai_params.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:41.122803 fiddler_client-3.1.0.dev4/fiddler/tests/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:41.122803 fiddler_client-3.1.0.dev4/fiddler/tests/apis/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3118 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13196 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7494 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8208 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_custom_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4636 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5134 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4501 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_files.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5089 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_generate_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1891 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2517 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_mixin.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18779 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5635 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_model_artifact.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3350 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4443 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_model_surrogate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6015 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7804 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_segment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8099 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    28590 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      840 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/conftest.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/constants.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1865 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      783 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/test_json_encoder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      312 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3333 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      335 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/tests/utils.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:41.122803 fiddler_client-3.1.0.dev4/fiddler/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)       53 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2908 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/utils/helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/utils/logger.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2203 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/utils/model_generator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/utils/validations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/utils/version.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      140 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/fiddler/version.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-05-02 12:40:41.122803 fiddler_client-3.1.0.dev4/fiddler_client.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1589 2024-05-02 12:40:41.000000 fiddler_client-3.1.0.dev4/fiddler_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     3321 2024-05-02 12:40:41.000000 fiddler_client-3.1.0.dev4/fiddler_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-05-02 12:40:41.000000 fiddler_client-3.1.0.dev4/fiddler_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)      162 2024-05-02 12:40:41.000000 fiddler_client-3.1.0.dev4/fiddler_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        8 2024-05-02 12:40:41.000000 fiddler_client-3.1.0.dev4/fiddler_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-05-02 12:40:41.132803 fiddler_client-3.1.0.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)     1138 2024-05-02 12:40:35.000000 fiddler_client-3.1.0.dev4/setup.py
```

### Comparing `fiddler-client-3.1.0.dev3/LICENSE.txt` & `fiddler_client-3.1.0.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/PKG-INFO` & `fiddler_client-3.1.0.dev4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 3.1.0.dev3
+Version: 3.1.0.dev4
 Summary: Python client for Fiddler Platform
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8.0
```

### Comparing `fiddler-client-3.1.0.dev3/PUBLIC.md` & `fiddler_client-3.1.0.dev4/PUBLIC.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/README.md` & `fiddler_client-3.1.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/__init__.py` & `fiddler_client-3.1.0.dev4/fiddler/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/connection.py` & `fiddler_client-3.1.0.dev4/fiddler/connection.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/constants/alert_rule.py` & `fiddler_client-3.1.0.dev4/fiddler/constants/alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/constants/model.py` & `fiddler_client-3.1.0.dev4/fiddler/constants/model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/decorators.py` & `fiddler_client-3.1.0.dev4/fiddler/decorators.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/alert_record.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/alert_rule.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/alert_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from datetime import datetime
 from typing import Any, Iterator
 from uuid import UUID
 
 from fiddler.constants.alert_rule import AlertCondition, BinSize, CompareTo, Priority
 from fiddler.decorators import handle_api_error
 from fiddler.entities.base import BaseEntity
-from fiddler.entities.baseline import Baseline, BaselineCompactMixin
-from fiddler.entities.model import Model, ModelCompactMixin
+from fiddler.entities.baseline import BaselineCompactMixin
+from fiddler.entities.model import ModelCompactMixin
 from fiddler.entities.project import ProjectCompactMixin
 from fiddler.schemas.alert_rule import AlertRuleResp, NotificationConfig
 from fiddler.schemas.filter_query import OperatorType, QueryCondition, QueryRule
 from fiddler.utils.logger import get_logger
 
 logger = get_logger(__name__)
 
@@ -60,29 +60,35 @@
 
         # Deserialized response object
         self._resp: AlertRuleResp | None = None
 
     @staticmethod
     def _get_url(id_: UUID | str | None = None) -> str:
         """Get model resource/item url."""
+        url = '/v3/alert-rules'
+        return url if not id_ else f'{url}/{id_}'
+
+    @staticmethod
+    def _get_url_v2(id_: UUID | str | None = None) -> str:
+        """Get model resource/item url."""
         url = '/v2/alert-configs'
         return url if not id_ else f'{url}/{id_}'
 
     @classmethod
     def _from_dict(cls, data: dict) -> AlertRule:
         """Build entity object from the given dictionary."""
 
         # Deserialize the response
         resp_obj = AlertRuleResp(**data)
 
         # Initialize
         instance = cls(
             name=resp_obj.name,
             model_id=resp_obj.model.id,
-            metric_id=resp_obj.metric_id,
+            metric_id=resp_obj.metric.id,
             priority=resp_obj.priority,
             compare_to=resp_obj.compare_to,
             condition=resp_obj.condition,
             bin_size=resp_obj.bin_size,
             critical_threshold=resp_obj.critical_threshold,
             warning_threshold=resp_obj.warning_threshold,
             columns=resp_obj.columns,
@@ -109,19 +115,19 @@
         """Refresh the fields of this instance from the given response dictionary"""
         # Deserialize the response
         resp_obj = AlertRuleResp(**data)
 
         # Reset properties
         self.model_id = resp_obj.model.id
         self.project_id = resp_obj.project.id
+        self.metric_id = resp_obj.metric.id
 
         # Add remaining fields
         fields = [
             'id',
-            'metric_id',
             'created_at',
             'updated_at',
         ]
         for field in fields:
             setattr(self, field, getattr(resp_obj, field, None))
 
         self._resp = resp_obj
@@ -175,82 +181,78 @@
                 QueryRule(
                     field='metric_id', operator=OperatorType.EQUAL, value=metric_id
                 )
             )
         if columns:
             for column in columns:
                 rules.append(
-                    QueryRule(field='columns', operator=OperatorType.ANY, value=column)
+                    QueryRule(
+                        field='feature_names', operator=OperatorType.ANY, value=column
+                    )
                 )
 
         _filter = QueryCondition(rules=rules)
         params: dict[str, Any] = {'filter': _filter.json()}
 
         if ordering:
             params['ordering'] = ','.join(ordering)
 
-        params['organization_name'] = cls.get_organization_name()
         for rule in cls._paginate(url=cls._get_url(), params=params):
             yield cls._from_dict(data=rule)
 
     @handle_api_error
     def delete(self) -> None:
         """Delete an alert rule."""
         assert self.id is not None
 
         self._client().delete(url=self._get_url(id_=self.id))
 
     @handle_api_error
     def create(self) -> AlertRule:
         """Create a new alert rule."""
-        model = Model.get(self.model_id)
         payload: dict[str, Any] = {
             'name': self.name,
-            'organization_name': self.organization_name,
-            'model_name': model.name,
-            'project_name': model.project.name,
+            'model_id': self.model_id,
             'metric_id': self.metric_id,
             'priority': self.priority,
             'compare_to': self.compare_to,
             'condition': self.condition,
             'bin_size': self.bin_size,
             'segment_id': self.segment_id,
             'critical_threshold': self.critical_threshold,
             'warning_threshold': self.warning_threshold,
             'feature_names': self.columns,
             'compare_bin_delta': self.compare_bin_delta,
-            'notifications': self._get_notifications_dict(),
         }
         if self.baseline_id:
-            baseline = Baseline.get(self.baseline_id)
-            payload['baseline_name'] = baseline.name
+            payload['baseline_id'] = self.baseline_id
 
         response = self._client().post(
             url=self._get_url(),
             data=payload,
         )
 
         self._refresh_from_response(response=response)
         return self
 
     @handle_api_error
     def enable_notifications(self) -> None:
         """Enable notifications for an alert rule"""
         self._client().patch(
-            url=self._get_url(id_=self.id), data={'enable_notification': True}
+            url=self._get_url_v2(id_=self.id), data={'enable_notification': True}
         )
         logger.info(
             'Notifications have been enabled for alert rule with id: %s', self.id
         )
 
     @handle_api_error
     def disable_notifications(self) -> None:
         """Disable notifications for an alert rule"""
         self._client().patch(
-            url=self._get_url(id_=self.id), data={'enable_notification': False}
+            url=self._get_url_v2(id_=self.id), data={'enable_notification': False}
         )
         logger.info(
             'Notifications have been disabled for alert rule with id: %s', self.id
         )
 
     @handle_api_error
     def set_notification_config(
@@ -273,15 +275,15 @@
         notifications = self._get_notifications_dict(
             emails=emails,
             pagerduty_services=pagerduty_services,
             pagerduty_severity=pagerduty_severity,
             webhooks=webhooks,
         )
         response = self._client().patch(
-            url=self._get_url(id_=self.id),
+            url=self._get_url_v2(id_=self.id),
             data={'notifications': notifications},
         )
 
         return self._get_notifications_from_dict(
             response.json()['data']['notifications']
         )
 
@@ -289,15 +291,15 @@
     def get_notification_config(self) -> NotificationConfig:
         """
         Get notifications config for an alert rule
 
         :return: NotificationConfig object
         """
 
-        response = self._client().get(url=self._get_url(id_=self.id))
+        response = self._client().get(url=self._get_url_v2(id_=self.id))
 
         return self._get_notifications_from_dict(
             response.json()['data']['notifications']
         )
 
     @staticmethod
     def _get_notifications_from_dict(notif_dict: dict) -> NotificationConfig:
```

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/base.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/base.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/baseline.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/baseline.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/custom_expression.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/custom_expression.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/dataset.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/events.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/events.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/file.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/file.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/job.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/job.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/model.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import builtins
 import typing
+from copy import deepcopy
 from dataclasses import dataclass
 from datetime import datetime
 from functools import cached_property
 from pathlib import Path
 from typing import Any, Iterator
 from uuid import UUID
 
@@ -35,15 +36,14 @@
 from fiddler.utils.logger import get_logger
 from fiddler.utils.model_generator import ModelGenerator
 
 if typing.TYPE_CHECKING:
     from fiddler.entities.baseline import Baseline
     from fiddler.entities.dataset import Dataset
 
-
 logger = get_logger(__name__)
 
 
 class Model(
     BaseEntity,
     CreatedByMixin,
     ProjectCompactMixin,
@@ -323,25 +323,25 @@
 
         :param version: Version name for the new instance
         :return: Model instance
         """
         return Model(
             name=self.name,
             project_id=self.project_id,
-            schema=self.schema,
-            spec=self.spec,
+            schema=deepcopy(self.schema),
+            spec=deepcopy(self.spec),
             version=version if version else self.version,
             input_type=self.input_type,
             task=self.task,
-            task_params=self.task_params,
+            task_params=deepcopy(self.task_params),
             description=self.description,
             event_id_col=self.event_id_col,
             event_ts_col=self.event_ts_col,
             event_ts_format=self.event_ts_format,
-            xai_params=self.xai_params,
+            xai_params=deepcopy(self.xai_params),
         )
 
     @property
     def datasets(self) -> Iterator[Dataset]:
         """Fetch all the datasets of this model"""
         from fiddler.entities.dataset import (  # pylint: disable=import-outside-toplevel
             Dataset,
```

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/model_artifact.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/model_artifact.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/model_deployment.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/model_deployment.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 from datetime import datetime
 from typing import Any
 from uuid import UUID
 
 from fiddler.decorators import handle_api_error
 from fiddler.entities.base import BaseEntity
+from fiddler.entities.job import Job
 from fiddler.entities.project import ProjectCompactMixin
+from fiddler.schemas.job import JobCompactResp
 from fiddler.schemas.model_deployment import ModelDeploymentResponse
 from fiddler.utils.logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class ModelDeployment(
@@ -90,28 +92,30 @@
         ]
         for field in fields:
             setattr(self, field, getattr(resp_obj, field, None))
 
         self._resp = resp_obj
 
     @handle_api_error
-    def update(self) -> None:
+    def update(self) -> Job:
         """Update an existing model deployment."""
         payload: dict[str, Any] = {'active': self.active}
         if self.replicas is not None:
             payload['replicas'] = self.replicas
         if self.cpu is not None:
             payload['cpu'] = self.cpu
         if self.memory is not None:
             payload['memory'] = self.memory
 
         response = self._client().patch(
             url=self._get_url(model_id=self.model_id), data=payload
         )
         self._refresh_from_response(response=response)
+        job_compact = JobCompactResp(**response.json()['data']['job'])
+        return Job.get(id_=job_compact.id)
 
     @classmethod
     def of(cls, model_id: UUID | str) -> ModelDeployment:
         """
         Get model deployment instance of the given model
 
         :param model_id: Model identifier
```

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/organization.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/organization.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/project.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/project.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/surrogate.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/surrogate.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/user.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/user.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/webhook.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/webhook.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/entities/xai.py` & `fiddler_client-3.1.0.dev4/fiddler/entities/xai.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/exceptions.py` & `fiddler_client-3.1.0.dev4/fiddler/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/libs/http_client.py` & `fiddler_client-3.1.0.dev4/fiddler/libs/http_client.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/libs/json_encoder.py` & `fiddler_client-3.1.0.dev4/fiddler/libs/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/libs/semver.py` & `fiddler_client-3.1.0.dev4/fiddler/libs/semver.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/packtools/gem.py` & `fiddler_client-3.1.0.dev4/fiddler/packtools/gem.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/packtools/keras_ig_helpers.py` & `fiddler_client-3.1.0.dev4/fiddler/packtools/keras_ig_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/packtools/project_attributions_helpers.py` & `fiddler_client-3.1.0.dev4/fiddler/packtools/project_attributions_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/packtools/template_model.py` & `fiddler_client-3.1.0.dev4/fiddler/packtools/template_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
                defined in model info.
         :param embedding_names: List. Name(s) the embedding layer(s) of the model.
         :param batch_input_shape_list: List of tuples corresponding to the output shape of the embedding layer(s)
                of the model. For example if the model has two embeddings, the list should have two tuples.
         :param hybrid: Boolean value for hybrid data type (for example matrices). Default to False.
         """
         import tensorflow as tf
-        from packtools.keras_ig_helpers import ComputeGradientsKerasTF2
+
+        from fiddler.packtools.keras_ig_helpers import ComputeGradientsKerasTF2
 
         embedding_names = embedding_names or []
         batch_input_shape_list = batch_input_shape_list or []
 
         self.output_col = output_col
         self.embedding_names = embedding_names
         self.hybrid = hybrid
@@ -193,15 +194,15 @@
 
         :param explanation_name: parameter used in Fiddler BE code to get explanation for a given explanation method.
                This allows users to define multiple custom explanations methods.
         :param input_df: a pandas DataFrame of input features
         :return: explanations_by_output and extras_by_output: two dictionaries with keys the output columns and values
                  the corresponding explanations and extra information necessary
         """
-        from packtools.project_attributions_helpers import TreeShapAttributions
+        from fiddler.packtools.project_attributions_helpers import TreeShapAttributions
 
         if explanation_name != self.tree_shap_explanations:
             raise NotImplementedError(
                 f'Please implement {explanation_name} in package.py with explain_custom method'
             )
 
         predictions = self.predict(input_df).iloc[0].to_dict()  # type: ignore
```

### Comparing `fiddler-client-3.1.0.dev3/fiddler/schemas/alert_record.py` & `fiddler_client-3.1.0.dev4/fiddler/schemas/alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/schemas/alert_rule.py` & `fiddler_client-3.1.0.dev4/fiddler/schemas/alert_rule.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,33 +8,41 @@
 from fiddler.schemas.base import BaseModel
 from fiddler.schemas.baseline import BaselineCompactResp
 from fiddler.schemas.custom_expression import SegmentCompactResp
 from fiddler.schemas.model import ModelCompactResp
 from fiddler.schemas.project import ProjectCompactResp
 
 
+class MetricResp(BaseModel):
+    id: Union[str, UUID]
+    display_name: str
+    type: str
+    type_display_name: str
+
+
 class AlertRuleResp(BaseModel):
-    id: UUID = Field(alias='uuid')
+    id: UUID
     name: str
-    model: ModelCompactResp
-    project: ProjectCompactResp
-    baseline: Optional[BaselineCompactResp]
-    segment: Optional[SegmentCompactResp]
     priority: Union[str, Priority]
     compare_to: Union[str, CompareTo]
-    metric_id: Union[str, UUID]
-    critical_threshold: float
     condition: Union[str, AlertCondition]
+    compare_bin_delta: Optional[int]
     bin_size: Union[str, BinSize]
     columns: Optional[List[str]] = Field(alias='feature_names')
-    compare_bin_delta: Optional[int]
+    critical_threshold: float
     warning_threshold: Optional[float]
 
     created_at: datetime
-    updated_at: datetime = Field(alias='last_updated')
+    updated_at: datetime
+
+    metric: MetricResp
+    model: ModelCompactResp
+    project: ProjectCompactResp
+    baseline: Optional[BaselineCompactResp]
+    segment: Optional[SegmentCompactResp]
 
 
 class NotificationConfig(BaseModel):
     emails: Optional[List[str]]
     pagerduty_services: Optional[List[str]]
     pagerduty_severity: Optional[str]
     webhooks: Optional[List[UUID]]
```

### Comparing `fiddler-client-3.1.0.dev3/fiddler/schemas/baseline.py` & `fiddler_client-3.1.0.dev4/fiddler/schemas/baseline.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/schemas/custom_expression.py` & `fiddler_client-3.1.0.dev4/fiddler/schemas/custom_expression.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/schemas/custom_features.py` & `fiddler_client-3.1.0.dev4/fiddler/schemas/custom_features.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/schemas/dataset.py` & `fiddler_client-3.1.0.dev4/fiddler/schemas/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/schemas/filter_query.py` & `fiddler_client-3.1.0.dev4/fiddler/schemas/filter_query.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/schemas/model.py` & `fiddler_client-3.1.0.dev4/fiddler/schemas/model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/schemas/model_deployment.py` & `fiddler_client-3.1.0.dev4/fiddler/schemas/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/schemas/model_schema.py` & `fiddler_client-3.1.0.dev4/fiddler/schemas/model_schema.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/schemas/model_spec.py` & `fiddler_client-3.1.0.dev4/fiddler/schemas/model_spec.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/schemas/model_task_params.py` & `fiddler_client-3.1.0.dev4/fiddler/schemas/model_task_params.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/schemas/response.py` & `fiddler_client-3.1.0.dev4/fiddler/schemas/response.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/schemas/xai.py` & `fiddler_client-3.1.0.dev4/fiddler/schemas/xai.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_alert_record.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_baseline.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_baseline.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_custom_metric.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_custom_metric.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_dataset.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_events.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_events.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_files.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_files.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_generate_model.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_generate_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_job.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_job.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_mixin.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -668,7 +668,13 @@
         _ = model_copy._event_publisher
 
     # With version parameter
     new_version = 'v2'
     model_copy = model.duplicate(version=new_version)
     assert model_copy.id is None
     assert model_copy.version == new_version
+
+    # Update new version
+    assert model.schema['CreditScore'].max == 850
+    model_copy.schema['CreditScore'].max = 900
+    assert model.schema['CreditScore'].max == 850
+    assert model_copy.schema['CreditScore'].max == 900
```

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model_artifact.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_model_artifact.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_model_surrogate.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_model_surrogate.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_project.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_project.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_segment.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_segment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_webhook.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_webhook.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/apis/test_xai.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/apis/test_xai.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/conftest.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/constants.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/constants.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/test_connection.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/test_json_encoder.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/tests/test_utils.py` & `fiddler_client-3.1.0.dev4/fiddler/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/utils/helpers.py` & `fiddler_client-3.1.0.dev4/fiddler/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/utils/logger.py` & `fiddler_client-3.1.0.dev4/fiddler/utils/logger.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/utils/model_generator.py` & `fiddler_client-3.1.0.dev4/fiddler/utils/model_generator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler/utils/version.py` & `fiddler_client-3.1.0.dev4/fiddler/utils/version.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/fiddler_client.egg-info/PKG-INFO` & `fiddler_client-3.1.0.dev4/fiddler_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 3.1.0.dev3
+Version: 3.1.0.dev4
 Summary: Python client for Fiddler Platform
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8.0
```

### Comparing `fiddler-client-3.1.0.dev3/fiddler_client.egg-info/SOURCES.txt` & `fiddler_client-3.1.0.dev4/fiddler_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.1.0.dev3/setup.py` & `fiddler_client-3.1.0.dev4/setup.py`

 * *Files identical despite different names*

