# Comparing `tmp/viewser-6.5.0.tar.gz` & `tmp/viewser-6.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viewser-6.5.0.tar", max compression
+gzip compressed data, was "viewser-6.5.1.tar", max compression
```

## Comparing `viewser-6.5.0.tar` & `viewser-6.5.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    19916 2024-04-29 13:44:58.806424 viewser-6.5.0/LICENSE
--rw-r--r--   0        0        0    22367 2024-04-29 13:44:58.806424 viewser-6.5.0/README.md
--rw-r--r--   0        0        0      878 2024-04-29 13:44:58.806424 viewser-6.5.0/pyproject.toml
--rw-r--r--   0        0        0       79 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/__init__.py
--rw-r--r--   0        0        0     1779 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/cli.py
--rw-r--r--   0        0        0        0 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/__init__.py
--rw-r--r--   0        0        0       22 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/config/__init__.py
--rw-r--r--   0        0        0     3184 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/config/cli.py
--rw-r--r--   0        0        0       61 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/documentation/__init__.py
--rw-r--r--   0        0        0     3733 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/documentation/cli.py
--rw-r--r--   0        0        0     3484 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/documentation/formatting.py
--rw-r--r--   0        0        0     2070 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/documentation/operations.py
--rw-r--r--   0        0        0      909 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/documentation/wrapped_views_doc.py
--rw-r--r--   0        0        0       21 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/help/__init__.py
--rw-r--r--   0        0        0      790 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/help/cli.py
--rw-r--r--   0        0        0      242 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/help/operations.py
--rw-r--r--   0        0        0       22 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/logs/__init__.py
--rw-r--r--   0        0        0      393 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/logs/cli.py
--rw-r--r--   0        0        0       22 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/model/__init__.py
--rw-r--r--   0        0        0     3531 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/model/cli.py
--rw-r--r--   0        0        0      731 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/model/formatting.py
--rw-r--r--   0        0        0        1 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/model/models.py
--rw-r--r--   0        0        0       22 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/notebooks/__init__.py
--rw-r--r--   0        0        0     1766 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/notebooks/cli.py
--rw-r--r--   0        0        0     6167 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/notebooks/operations.py
--rw-r--r--   0        0        0       60 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/queryset/__init__.py
--rw-r--r--   0        0        0     2245 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/queryset/cli.py
--rw-r--r--   0        0        0     2529 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/queryset/config_drift.py
--rw-r--r--   0        0        0     6209 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/drift_detection.py
--rw-r--r--   0        0        0     1269 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/formatting.py
--rw-r--r--   0        0        0    12542 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/integrity_checks.py
--rw-r--r--   0        0        0      133 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/models/__init__.py
--rw-r--r--   0        0        0     3059 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/models/column.py
--rw-r--r--   0        0        0     7755 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/models/queryset.py
--rw-r--r--   0        0        0     2285 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/models/transform.py
--rw-r--r--   0        0        0      313 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/models/util.py
--rw-r--r--   0        0        0     9112 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/operations.py
--rw-r--r--   0        0        0      231 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/queryset_list.py
--rw-r--r--   0        0        0       22 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/system/__init__.py
--rw-r--r--   0        0        0     1816 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/system/cli.py
--rw-r--r--   0        0        0     1371 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/system/formatting.py
--rw-r--r--   0        0        0      481 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/system/models.py
--rw-r--r--   0        0        0       73 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/error_handling/__init__.py
--rw-r--r--   0        0        0     3929 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/error_handling/checks.py
--rw-r--r--   0        0        0     2164 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/error_handling/error_handling.py
--rw-r--r--   0        0        0     7304 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/error_handling/errors.py
--rw-r--r--   0        0        0     6252 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/error_handling/exceptions.py
--rw-r--r--   0        0        0      205 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/hirearchical_dict.py
--rw-r--r--   0        0        0      706 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/operations.py
--rw-r--r--   0        0        0     5859 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/remotes.py
--rw-r--r--   0        0        0      868 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/__init__.py
--rw-r--r--   0        0        0     4168 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/config_resolver.py
--rw-r--r--   0        0        0      182 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/db.py
--rw-r--r--   0        0        0      295 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/defaults.py
--rw-r--r--   0        0        0       47 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/exceptions.py
--rw-r--r--   0        0        0        1 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/interactive.py
--rw-r--r--   0        0        0      389 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/models.py
--rw-r--r--   0        0        0     1401 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/static.py
--rw-r--r--   0        0        0      181 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/validation.py
--rw-r--r--   0        0        0      387 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/storage/azure.py
--rw-r--r--   0        0        0     2443 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/storage/db.py
--rw-r--r--   0        0        0     1462 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/storage/metadata_storage_serializer.py
--rw-r--r--   0        0        0     1175 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/storage/model_object.py
--rw-r--r--   0        0        0        0 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/__init__.py
--rw-r--r--   0        0        0      842 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/animations.py
--rw-r--r--   0        0        0      322 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/ascii_art.py
--rw-r--r--   0        0        0        0 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/__init__.py
--rw-r--r--   0        0        0     3186 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/abc.py
--rw-r--r--   0        0        0      144 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/conventions.py
--rw-r--r--   0        0        0      830 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/errors.py
--rw-r--r--   0        0        0      291 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/formatters.py
--rw-r--r--   0        0        0      177 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/generic_models.py
--rw-r--r--   0        0        0      196 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/json_formatter.py
--rw-r--r--   0        0        0      443 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/sections.py
--rw-r--r--   0        0        0      103 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/styles.py
--rw-r--r--   0        0        0       32 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/models.py
--rw-r--r--   0        0        0       82 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/utils.py
--rw-r--r--   0        0        0    23702 1970-01-01 00:00:00.000000 viewser-6.5.0/PKG-INFO
+-rw-r--r--   0        0        0    19916 2024-05-02 10:16:36.359939 viewser-6.5.1/LICENSE
+-rw-r--r--   0        0        0    22367 2024-05-02 10:16:36.359939 viewser-6.5.1/README.md
+-rw-r--r--   0        0        0      912 2024-05-02 10:16:36.359939 viewser-6.5.1/pyproject.toml
+-rw-r--r--   0        0        0       79 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/__init__.py
+-rw-r--r--   0        0        0     1779 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/cli.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/config/__init__.py
+-rw-r--r--   0        0        0     3184 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/config/cli.py
+-rw-r--r--   0        0        0       61 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/documentation/__init__.py
+-rw-r--r--   0        0        0     3733 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/documentation/cli.py
+-rw-r--r--   0        0        0     3484 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/documentation/formatting.py
+-rw-r--r--   0        0        0     2070 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/documentation/operations.py
+-rw-r--r--   0        0        0      909 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/documentation/wrapped_views_doc.py
+-rw-r--r--   0        0        0       21 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/help/__init__.py
+-rw-r--r--   0        0        0      790 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/help/cli.py
+-rw-r--r--   0        0        0      242 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/help/operations.py
+-rw-r--r--   0        0        0       22 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/logs/__init__.py
+-rw-r--r--   0        0        0      393 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/logs/cli.py
+-rw-r--r--   0        0        0       22 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/model/__init__.py
+-rw-r--r--   0        0        0     3531 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/model/cli.py
+-rw-r--r--   0        0        0      731 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/model/formatting.py
+-rw-r--r--   0        0        0        1 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/model/models.py
+-rw-r--r--   0        0        0       22 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/notebooks/__init__.py
+-rw-r--r--   0        0        0     1766 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/notebooks/cli.py
+-rw-r--r--   0        0        0     6167 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/notebooks/operations.py
+-rw-r--r--   0        0        0       60 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/queryset/__init__.py
+-rw-r--r--   0        0        0     2245 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/queryset/cli.py
+-rw-r--r--   0        0        0     2529 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/queryset/config_drift.py
+-rw-r--r--   0        0        0     6209 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/queryset/drift_detection.py
+-rw-r--r--   0        0        0     1269 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/queryset/formatting.py
+-rw-r--r--   0        0        0    12542 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/queryset/integrity_checks.py
+-rw-r--r--   0        0        0      133 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/queryset/models/__init__.py
+-rw-r--r--   0        0        0     3059 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/queryset/models/column.py
+-rw-r--r--   0        0        0     7755 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/queryset/models/queryset.py
+-rw-r--r--   0        0        0     2285 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/queryset/models/transform.py
+-rw-r--r--   0        0        0      313 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/queryset/models/util.py
+-rw-r--r--   0        0        0     9112 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/queryset/operations.py
+-rw-r--r--   0        0        0      231 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/queryset/queryset_list.py
+-rw-r--r--   0        0        0       22 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/system/__init__.py
+-rw-r--r--   0        0        0     1816 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/system/cli.py
+-rw-r--r--   0        0        0     1371 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/system/formatting.py
+-rw-r--r--   0        0        0      481 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/commands/system/models.py
+-rw-r--r--   0        0        0       73 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/error_handling/__init__.py
+-rw-r--r--   0        0        0     3929 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/error_handling/checks.py
+-rw-r--r--   0        0        0     2164 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/error_handling/error_handling.py
+-rw-r--r--   0        0        0     7304 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/error_handling/errors.py
+-rw-r--r--   0        0        0     6252 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/error_handling/exceptions.py
+-rw-r--r--   0        0        0      205 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/hirearchical_dict.py
+-rw-r--r--   0        0        0      706 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/operations.py
+-rw-r--r--   0        0        0     5859 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/remotes.py
+-rw-r--r--   0        0        0      868 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/settings/__init__.py
+-rw-r--r--   0        0        0     4168 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/settings/config_resolver.py
+-rw-r--r--   0        0        0      182 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/settings/db.py
+-rw-r--r--   0        0        0      295 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/settings/defaults.py
+-rw-r--r--   0        0        0       47 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/settings/exceptions.py
+-rw-r--r--   0        0        0        1 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/settings/interactive.py
+-rw-r--r--   0        0        0      389 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/settings/models.py
+-rw-r--r--   0        0        0     1401 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/settings/static.py
+-rw-r--r--   0        0        0      181 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/settings/validation.py
+-rw-r--r--   0        0        0      387 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/storage/azure.py
+-rw-r--r--   0        0        0     2443 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/storage/db.py
+-rw-r--r--   0        0        0     1462 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/storage/metadata_storage_serializer.py
+-rw-r--r--   0        0        0     1175 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/storage/model_object.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/tui/__init__.py
+-rw-r--r--   0        0        0      842 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/tui/animations.py
+-rw-r--r--   0        0        0      322 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/tui/ascii_art.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/tui/formatting/__init__.py
+-rw-r--r--   0        0        0     3186 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/tui/formatting/abc.py
+-rw-r--r--   0        0        0      144 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/tui/formatting/conventions.py
+-rw-r--r--   0        0        0      830 2024-05-02 10:16:36.359939 viewser-6.5.1/viewser/tui/formatting/errors.py
+-rw-r--r--   0        0        0      291 2024-05-02 10:16:36.363939 viewser-6.5.1/viewser/tui/formatting/formatters.py
+-rw-r--r--   0        0        0      177 2024-05-02 10:16:36.363939 viewser-6.5.1/viewser/tui/formatting/generic_models.py
+-rw-r--r--   0        0        0      196 2024-05-02 10:16:36.363939 viewser-6.5.1/viewser/tui/formatting/json_formatter.py
+-rw-r--r--   0        0        0      443 2024-05-02 10:16:36.363939 viewser-6.5.1/viewser/tui/formatting/sections.py
+-rw-r--r--   0        0        0      103 2024-05-02 10:16:36.363939 viewser-6.5.1/viewser/tui/formatting/styles.py
+-rw-r--r--   0        0        0       32 2024-05-02 10:16:36.363939 viewser-6.5.1/viewser/tui/models.py
+-rw-r--r--   0        0        0       82 2024-05-02 10:16:36.363939 viewser-6.5.1/viewser/tui/utils.py
+-rw-r--r--   0        0        0    23749 1970-01-01 00:00:00.000000 viewser-6.5.1/PKG-INFO
```

### Comparing `viewser-6.5.0/LICENSE` & `viewser-6.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/README.md` & `viewser-6.5.1/README.md`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/pyproject.toml` & `viewser-6.5.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "viewser"
-version = "6.5.0"
+version = "6.5.1"
 description = "The Views 3 CLI tool"
 authors = ["peder2911 <pglandsverk@gmail.com>"]
 readme = "README.md"
 homepage = "https://www.github.com/prio-data/viewser"
 license = "CC-BY-NC"
 
 [tool.poetry.dependencies]
@@ -24,14 +24,15 @@
 PyMonad = "^2.4.0"
 docker = "^5.0.0"
 psutil = "^5.8.0"
 strconv = "^0.4.2"
 pyarrow = ">9.0.0"
 views-storage = "^1.1.0"
 tqdm = "^4.66.0"
+views_tensor_utilities = "<1.0.0"
 
 [tool.poetry.scripts]
 viewser = "viewser.cli:viewser"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 httpretty = "^1.1.3"
```

### Comparing `viewser-6.5.0/viewser/cli.py` & `viewser-6.5.1/viewser/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/config/cli.py` & `viewser-6.5.1/viewser/commands/config/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/documentation/cli.py` & `viewser-6.5.1/viewser/commands/documentation/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/documentation/formatting.py` & `viewser-6.5.1/viewser/commands/documentation/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/documentation/operations.py` & `viewser-6.5.1/viewser/commands/documentation/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/documentation/wrapped_views_doc.py` & `viewser-6.5.1/viewser/commands/documentation/wrapped_views_doc.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/help/cli.py` & `viewser-6.5.1/viewser/commands/help/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/model/cli.py` & `viewser-6.5.1/viewser/commands/model/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/model/formatting.py` & `viewser-6.5.1/viewser/commands/model/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/notebooks/cli.py` & `viewser-6.5.1/viewser/commands/notebooks/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/notebooks/operations.py` & `viewser-6.5.1/viewser/commands/notebooks/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/queryset/cli.py` & `viewser-6.5.1/viewser/commands/queryset/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/queryset/config_drift.py` & `viewser-6.5.1/viewser/commands/queryset/config_drift.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/queryset/drift_detection.py` & `viewser-6.5.1/viewser/commands/queryset/drift_detection.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/queryset/formatting.py` & `viewser-6.5.1/viewser/commands/queryset/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/queryset/integrity_checks.py` & `viewser-6.5.1/viewser/commands/queryset/integrity_checks.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/queryset/models/column.py` & `viewser-6.5.1/viewser/commands/queryset/models/column.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/queryset/models/queryset.py` & `viewser-6.5.1/viewser/commands/queryset/models/queryset.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/queryset/models/transform.py` & `viewser-6.5.1/viewser/commands/queryset/models/transform.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/queryset/operations.py` & `viewser-6.5.1/viewser/commands/queryset/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/system/cli.py` & `viewser-6.5.1/viewser/commands/system/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/commands/system/formatting.py` & `viewser-6.5.1/viewser/commands/system/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/error_handling/checks.py` & `viewser-6.5.1/viewser/error_handling/checks.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/error_handling/error_handling.py` & `viewser-6.5.1/viewser/error_handling/error_handling.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/error_handling/errors.py` & `viewser-6.5.1/viewser/error_handling/errors.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/error_handling/exceptions.py` & `viewser-6.5.1/viewser/error_handling/exceptions.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/operations.py` & `viewser-6.5.1/viewser/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/remotes.py` & `viewser-6.5.1/viewser/remotes.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/settings/__init__.py` & `viewser-6.5.1/viewser/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/settings/config_resolver.py` & `viewser-6.5.1/viewser/settings/config_resolver.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/settings/static.py` & `viewser-6.5.1/viewser/settings/static.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/storage/db.py` & `viewser-6.5.1/viewser/storage/db.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/storage/metadata_storage_serializer.py` & `viewser-6.5.1/viewser/storage/metadata_storage_serializer.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/storage/model_object.py` & `viewser-6.5.1/viewser/storage/model_object.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/tui/animations.py` & `viewser-6.5.1/viewser/tui/animations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/tui/formatting/abc.py` & `viewser-6.5.1/viewser/tui/formatting/abc.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/viewser/tui/formatting/errors.py` & `viewser-6.5.1/viewser/tui/formatting/errors.py`

 * *Files identical despite different names*

### Comparing `viewser-6.5.0/PKG-INFO` & `viewser-6.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viewser
-Version: 6.5.0
+Version: 6.5.1
 Summary: The Views 3 CLI tool
 Home-page: https://www.github.com/prio-data/viewser
 License: CC-BY-NC
 Author: peder2911
 Author-email: pglandsverk@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -28,14 +28,15 @@
 Requires-Dist: strconv (>=0.4.2,<0.5.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: toolz (>=0.11.1,<0.12.0)
 Requires-Dist: tqdm (>=4.66.0,<5.0.0)
 Requires-Dist: views-schema (>=2.3.0,<3.0.0)
 Requires-Dist: views-storage (>=1.1.0,<2.0.0)
+Requires-Dist: views_tensor_utilities (<1.0.0)
 Description-Content-Type: text/markdown
 
 
 # viewser
 
 Viewser is a software package allowing any user to fetch raw data from the VIEWS database, apply a wide range 
 of transforms to the raw data, and download the resulting dataset as a single pandas dataframe.
```

