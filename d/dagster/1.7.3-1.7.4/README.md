# Comparing `tmp/dagster-1.7.3.tar.gz` & `tmp/dagster-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.7.3.tar", last modified: Thu Apr 25 20:08:56 2024, max compression
+gzip compressed data, was "dagster-1.7.4.tar", last modified: Thu May  2 20:32:09 2024, max compression
```

## Comparing `dagster-1.7.3.tar` & `dagster-1.7.4.tar`

### file list

```diff
@@ -1,693 +1,695 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.772266 dagster-1.7.3/
--rw-r--r--   0 root         (0) root         (0)      553 2024-04-25 20:08:31.000000 dagster-1.7.3/COPYING
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-25 20:08:31.000000 dagster-1.7.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      533 2024-04-25 20:08:31.000000 dagster-1.7.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9867 2024-04-25 20:08:56.772266 dagster-1.7.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8153 2024-04-25 20:08:31.000000 dagster-1.7.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.688266 dagster-1.7.3/dagster/
--rw-r--r--   0 root         (0) root         (0)    29906 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)    20744 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.692266 dagster-1.7.3/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     3224 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5483 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3370 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.692266 dagster-1.7.3/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    52040 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.692266 dagster-1.7.3/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1182 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26898 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8030 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     8302 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/code_server.py
--rw-r--r--   0 root         (0) root         (0)     2374 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3513 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     8134 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     6651 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    30542 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     9114 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5120 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19351 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15461 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     4259 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.692266 dagster-1.7.3/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27910 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.696266 dagster-1.7.3/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15830 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18787 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    14918 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    19728 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9536 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.696266 dagster-1.7.3/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)     1394 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)    18116 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/config.py
--rw-r--r--   0 root         (0) root         (0)    11510 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    11583 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    41265 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/resource.py
--rw-r--r--   0 root         (0) root         (0)     1996 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/type_check_utils.py
--rw-r--r--   0 root         (0) root         (0)     8375 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)    12532 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3087 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    17137 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.700266 dagster-1.7.3/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.700266 dagster-1.7.3/dagster/_core/asset_graph_view/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/asset_graph_view/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21047 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/asset_graph_view/asset_graph_view.py
--rw-r--r--   0 root         (0) root         (0)      994 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13427 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.700266 dagster-1.7.3/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     9665 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.712266 dagster-1.7.3/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7827 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4506 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_check_evaluation.py
--rw-r--r--   0 root         (0) root         (0)     7052 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_check_result.py
--rw-r--r--   0 root         (0) root         (0)     5628 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_check_spec.py
--rw-r--r--   0 root         (0) root         (0)     6092 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.712266 dagster-1.7.3/dagster/_core/definitions/asset_condition/
--rw-r--r--   0 root         (0) root         (0)       62 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_condition/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21064 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_condition/asset_condition.py
--rw-r--r--   0 root         (0) root         (0)    16508 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py
--rw-r--r--   0 root         (0) root         (0)    26314 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_daemon_context.py
--rw-r--r--   0 root         (0) root         (0)    10648 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)     4628 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_dep.py
--rw-r--r--   0 root         (0) root         (0)    10133 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     7696 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_graph_differ.py
--rw-r--r--   0 root         (0) root         (0)    16636 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3644 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    29917 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_job.py
--rw-r--r--   0 root         (0) root         (0)     6060 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_key.py
--rw-r--r--   0 root         (0) root         (0)    30355 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     6945 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    39535 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7444 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     6764 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_spec.py
--rw-r--r--   0 root         (0) root         (0)    10723 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/asset_subset.py
--rw-r--r--   0 root         (0) root         (0)    79909 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    13905 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    54478 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/auto_materialize_rule.py
--rw-r--r--   0 root         (0) root         (0)    21726 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/auto_materialize_rule_evaluation.py
--rw-r--r--   0 root         (0) root         (0)     2768 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/auto_materialize_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     2939 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/backfill_policy.py
--rw-r--r--   0 root         (0) root         (0)    34666 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/base_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    16772 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    40623 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4278 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    14811 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    22990 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    30155 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.712266 dagster-1.7.3/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16572 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/asset_check_decorator.py
--rw-r--r--   0 root         (0) root         (0)    69618 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4907 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9077 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9353 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10815 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    19011 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    15668 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8718 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12463 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12664 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5267 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    23545 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    42243 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    26888 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21182 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)     9379 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/external_asset.py
--rw-r--r--   0 root         (0) root         (0)     9766 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_based_auto_materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.716266 dagster-1.7.3/dagster/_core/definitions/freshness_checks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5838 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_checks/last_update.py
--rw-r--r--   0 root         (0) root         (0)     7685 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_checks/sensor.py
--rw-r--r--   0 root         (0) root         (0)     9349 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_checks/shared_builder.py
--rw-r--r--   0 root         (0) root         (0)     4669 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_checks/time_partition.py
--rw-r--r--   0 root         (0) root         (0)    10409 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_checks/utils.py
--rw-r--r--   0 root         (0) root         (0)     8801 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16401 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    47569 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1524 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3537 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    21027 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     6410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2991 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    53689 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)     5693 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/load_asset_checks_from_modules.py
--rw-r--r--   0 root         (0) root         (0)    22306 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     7171 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.716266 dagster-1.7.3/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    42209 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    57203 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    22029 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)      197 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11892 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8016 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2892 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    23078 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    23141 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7551 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    19237 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    50520 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    47665 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    11087 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27733 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/reconstruct.py
--rw-r--r--   0 root         (0) root         (0)    21602 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/remote_asset_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.716266 dagster-1.7.3/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6024 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    21698 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    20892 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     8858 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1465 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    17900 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5382 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)    10320 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)     3383 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/result.py
--rw-r--r--   0 root         (0) root         (0)    23076 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    19555 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    44126 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    39363 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     6209 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/schema_change_checks.py
--rw-r--r--   0 root         (0) root         (0)     5134 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    14134 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    53797 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    19244 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)    21859 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)   102142 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15160 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)    11017 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     3982 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    26986 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)    17452 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.716266 dagster-1.7.3/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    71913 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8142 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.720266 dagster-1.7.3/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38363 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    64654 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    17100 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6296 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.720266 dagster-1.7.3/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79687 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    17598 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    29167 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    40124 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    37256 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    56002 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18837 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5135 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5897 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9633 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8602 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14247 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6723 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.724266 dagster-1.7.3/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26460 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     9850 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    17019 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16974 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    40691 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    11032 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    39260 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6251 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/instance_concurrency_context.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5706 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7326 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    61075 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    17174 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15985 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8230 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19141 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2100 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1564 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)     9950 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)    14043 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/submit_asset_runs.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.724266 dagster-1.7.3/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5989 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     3366 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15497 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.724266 dagster-1.7.3/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16894 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.724266 dagster-1.7.3/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.724266 dagster-1.7.3/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   132334 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15788 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24141 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     3899 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.724266 dagster-1.7.3/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3819 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6645 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1566 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    18041 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     6656 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/op_concurrency_limits_counter.py
--rw-r--r--   0 root         (0) root         (0)     3691 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.724266 dagster-1.7.3/dagster/_core/pipes/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/pipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8974 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/pipes/client.py
--rw-r--r--   0 root         (0) root         (0)    18318 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/pipes/context.py
--rw-r--r--   0 root         (0) root         (0)     5648 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/pipes/subprocess.py
--rw-r--r--   0 root         (0) root         (0)    25661 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/pipes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.728266 dagster-1.7.3/dagster/_core/remote_representation/
--rw-r--r--   0 root         (0) root         (0)     2793 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36695 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    37482 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    83582 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/feature_flags.py
--rw-r--r--   0 root         (0) root         (0)    12429 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4356 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    19669 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/remote_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.728266 dagster-1.7.3/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    13364 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.728266 dagster-1.7.3/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    28809 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)    10917 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.728266 dagster-1.7.3/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1801 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.728266 dagster-1.7.3/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18109 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.732266 dagster-1.7.3/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2842 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9302 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12155 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16934 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14185 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     3183 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.736266 dagster-1.7.3/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3058 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.736266 dagster-1.7.3/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6686 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.748266 dagster-1.7.3/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      312 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1486 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      599 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2729 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      635 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      958 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1537 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)     2062 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
--rw-r--r--   0 root         (0) root         (0)     2359 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
--rw-r--r--   0 root         (0) root         (0)     1322 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3887 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/asset_check_execution_record.py
--rw-r--r--   0 root         (0) root         (0)     7301 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1227 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.748266 dagster-1.7.3/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8725 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16223 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9557 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    25652 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11187 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.748266 dagster-1.7.3/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19078 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3801 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7289 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     8037 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     9250 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)   121159 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7508 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    22497 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10983 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13492 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8819 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10882 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    32629 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17558 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1167 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4355 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5964 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/migration/bigint_migration.py
--rw-r--r--   0 root         (0) root         (0)    15491 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3270 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    17398 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/root.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13903 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2452 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8716 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     6391 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    37611 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6310 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7236 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4133 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     4086 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    25146 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3684 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7691 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)     1391 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/sqlalchemy_compat.py
--rw-r--r--   0 root         (0) root         (0)      926 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4875 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1186 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    19215 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.752266 dagster-1.7.3/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13962 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    15178 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    29921 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    22361 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.756266 dagster-1.7.3/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3084 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7042 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    36504 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3571 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4764 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3620 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1441 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     6652 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.756266 dagster-1.7.3/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3160 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/batch_asset_record_loader.py
--rw-r--r--   0 root         (0) root         (0)     3422 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    29210 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11852 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4721 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     3463 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1971 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)    41795 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7402 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9036 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     2665 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     5118 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19590 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    12112 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      320 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1792 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/monitoring/concurrency.py
--rw-r--r--   0 root         (0) root         (0)     9904 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/monitoring/run_monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18725 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    39110 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)      678 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/utils.py
--rw-r--r--   0 root         (0) root         (0)     4114 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2997 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.688266 dagster-1.7.3/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.760266 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      279 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13462 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    27262 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/__generated__/api_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    43164 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2060 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    22739 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3584 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    23173 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5993 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    13431 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/proxy_server.py
--rw-r--r--   0 root         (0) root         (0)    60914 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5297 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    29291 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     3693 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_loggers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_model/
--rw-r--r--   0 root         (0) root         (0)     1373 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3897 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_model/pydantic_compat_layer.py
--rw-r--r--   0 root         (0) root         (0)     3269 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.764266 dagster-1.7.3/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41378 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1262 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.768266 dagster-1.7.3/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      701 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8916 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7292 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    43115 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.768266 dagster-1.7.3/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5455 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.768266 dagster-1.7.3/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.772266 dagster-1.7.3/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    24377 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9314 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     5404 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    42998 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     5865 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/concurrency.py
--rw-r--r--   0 root         (0) root         (0)    12887 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/container.py
--rw-r--r--   0 root         (0) root         (0)     2412 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/env.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      745 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)    11214 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    33445 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/security.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.772266 dagster-1.7.3/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    13678 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7790 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/data_versions.py
--rw-r--r--   0 root         (0) root         (0)      119 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    36138 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.772266 dagster-1.7.3/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/typed_dict.py
--rw-r--r--   0 root         (0) root         (0)      170 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4740 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/warnings.py
--rw-r--r--   0 root         (0) root         (0)     4902 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-25 20:08:31.000000 dagster-1.7.3/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 20:08:56.688266 dagster-1.7.3/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9867 2024-04-25 20:08:56.000000 dagster-1.7.3/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    28024 2024-04-25 20:08:56.000000 dagster-1.7.3/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 20:08:56.000000 dagster-1.7.3/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2024-04-25 20:08:56.000000 dagster-1.7.3/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1458 2024-04-25 20:08:56.000000 dagster-1.7.3/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-25 20:08:56.000000 dagster-1.7.3/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2024-04-25 20:08:56.772266 dagster-1.7.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6827 2024-04-25 20:08:31.000000 dagster-1.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.169218 dagster-1.7.4/
+-rw-r--r--   0 root         (0) root         (0)      553 2024-05-02 20:31:40.000000 dagster-1.7.4/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-02 20:31:40.000000 dagster-1.7.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      533 2024-05-02 20:31:40.000000 dagster-1.7.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9867 2024-05-02 20:32:09.169218 dagster-1.7.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8153 2024-05-02 20:31:40.000000 dagster-1.7.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.049219 dagster-1.7.4/dagster/
+-rw-r--r--   0 root         (0) root         (0)    29976 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    20744 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.053219 dagster-1.7.4/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     3224 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.053219 dagster-1.7.4/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    52040 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.053219 dagster-1.7.4/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1182 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26898 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8030 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     8302 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/code_server.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     8134 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     6651 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    30542 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     9114 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5120 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19351 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.057219 dagster-1.7.4/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27910 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.057219 dagster-1.7.4/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15830 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    18787 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    14918 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    19728 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9536 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.061219 dagster-1.7.4/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)     1394 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)    18114 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/config.py
+-rw-r--r--   0 root         (0) root         (0)    11510 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    11583 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    41265 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/type_check_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8375 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17137 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.061219 dagster-1.7.4/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.065219 dagster-1.7.4/dagster/_core/asset_graph_view/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/asset_graph_view/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21047 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/asset_graph_view/asset_graph_view.py
+-rw-r--r--   0 root         (0) root         (0)      994 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13427 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.065219 dagster-1.7.4/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     9665 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.081218 dagster-1.7.4/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7827 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_check_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)     7090 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_check_result.py
+-rw-r--r--   0 root         (0) root         (0)     5628 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_check_spec.py
+-rw-r--r--   0 root         (0) root         (0)     6113 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.081218 dagster-1.7.4/dagster/_core/definitions/asset_condition/
+-rw-r--r--   0 root         (0) root         (0)       62 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_condition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21109 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_condition/asset_condition.py
+-rw-r--r--   0 root         (0) root         (0)    16731 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py
+-rw-r--r--   0 root         (0) root         (0)    26314 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_daemon_context.py
+-rw-r--r--   0 root         (0) root         (0)    10654 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_dep.py
+-rw-r--r--   0 root         (0) root         (0)    10133 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     7696 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_graph_differ.py
+-rw-r--r--   0 root         (0) root         (0)    16636 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    30136 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_job.py
+-rw-r--r--   0 root         (0) root         (0)     6060 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)    30355 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     6945 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    39535 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7444 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6764 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_spec.py
+-rw-r--r--   0 root         (0) root         (0)    10723 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_subset.py
+-rw-r--r--   0 root         (0) root         (0)    80227 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13758 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    11477 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/auto_materialize_rule.py
+-rw-r--r--   0 root         (0) root         (0)    21722 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/auto_materialize_rule_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)    46525 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/auto_materialize_rule_impls.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/auto_materialize_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/backfill_policy.py
+-rw-r--r--   0 root         (0) root         (0)    34599 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/base_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    16772 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    40623 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4278 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    14811 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    22990 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    30155 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.085218 dagster-1.7.4/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16572 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/asset_check_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    70075 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4907 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9077 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9353 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10815 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    19011 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    15668 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8718 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12463 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12664 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5267 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    23545 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    42243 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    26888 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21182 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9379 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/external_asset.py
+-rw-r--r--   0 root         (0) root         (0)     9766 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_based_auto_materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.085218 dagster-1.7.4/dagster/_core/definitions/freshness_checks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5838 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_checks/last_update.py
+-rw-r--r--   0 root         (0) root         (0)     7685 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_checks/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     9349 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_checks/shared_builder.py
+-rw-r--r--   0 root         (0) root         (0)     4669 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_checks/time_partition.py
+-rw-r--r--   0 root         (0) root         (0)    10454 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_checks/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8801 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16401 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    47569 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    21027 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     6410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    53689 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5693 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/load_asset_checks_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)    22306 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     7171 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.085218 dagster-1.7.4/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    42277 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    57203 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    22029 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)      197 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11892 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8016 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    23078 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    23141 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7551 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    19237 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    50520 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    47665 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    11087 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27733 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/reconstruct.py
+-rw-r--r--   0 root         (0) root         (0)    21602 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/remote_asset_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.085218 dagster-1.7.4/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6024 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    21698 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    20892 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     8858 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    17900 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)    10320 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)     3383 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/result.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    19555 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    44126 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    39363 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6209 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/schema_change_checks.py
+-rw-r--r--   0 root         (0) root         (0)     5134 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    14134 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    53797 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19244 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)    22389 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)   102377 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15160 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    11017 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    26986 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    17452 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.085218 dagster-1.7.4/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    71913 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8142 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.093218 dagster-1.7.4/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38363 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    64654 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    17100 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.093218 dagster-1.7.4/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79687 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)     8657 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/data_version_cache.py
+-rw-r--r--   0 root         (0) root         (0)    17598 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    29167 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    40124 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    37256 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    49252 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18837 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14247 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6723 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.097218 dagster-1.7.4/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26460 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     9850 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    17019 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16974 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    40707 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    11032 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    39260 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/instance_concurrency_context.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    61075 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    17174 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15985 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8230 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19141 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)     9950 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)    14043 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/submit_asset_runs.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.097218 dagster-1.7.4/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15497 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.097218 dagster-1.7.4/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16894 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.097218 dagster-1.7.4/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.101218 dagster-1.7.4/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   132334 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15788 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24141 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.101218 dagster-1.7.4/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3819 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    18041 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     6656 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/op_concurrency_limits_counter.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.101218 dagster-1.7.4/dagster/_core/pipes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/pipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/pipes/client.py
+-rw-r--r--   0 root         (0) root         (0)    18318 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/pipes/context.py
+-rw-r--r--   0 root         (0) root         (0)     5648 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/pipes/subprocess.py
+-rw-r--r--   0 root         (0) root         (0)    25661 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/pipes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.105218 dagster-1.7.4/dagster/_core/remote_representation/
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36695 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    37482 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    83582 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/feature_flags.py
+-rw-r--r--   0 root         (0) root         (0)    12429 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    19669 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.105218 dagster-1.7.4/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    13364 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.105218 dagster-1.7.4/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    28809 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)    10917 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.105218 dagster-1.7.4/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.105218 dagster-1.7.4/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18109 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.109218 dagster-1.7.4/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9302 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12155 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16934 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14185 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.113218 dagster-1.7.4/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.113218 dagster-1.7.4/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6686 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.129218 dagster-1.7.4/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      312 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      599 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      635 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      958 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/asset_check_execution_record.py
+-rw-r--r--   0 root         (0) root         (0)     7301 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.129218 dagster-1.7.4/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8725 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16223 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9557 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    25652 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11187 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.129218 dagster-1.7.4/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19078 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7289 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     8037 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     9250 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)   121159 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.129218 dagster-1.7.4/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7508 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    22497 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13492 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8819 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10882 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    32629 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17558 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/migration/bigint_migration.py
+-rw-r--r--   0 root         (0) root         (0)    15491 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    17398 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/root.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13903 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     6391 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    37611 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6310 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7236 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     4086 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    25146 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3684 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7691 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/sqlalchemy_compat.py
+-rw-r--r--   0 root         (0) root         (0)      926 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4875 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    19138 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13962 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    29921 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    22361 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.137218 dagster-1.7.4/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7042 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    36504 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     6652 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.137218 dagster-1.7.4/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3160 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/batch_asset_record_loader.py
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    29210 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11852 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4721 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    42160 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9036 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     5118 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19590 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    12497 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/monitoring/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)     9904 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/monitoring/run_monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18725 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    39411 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.045219 dagster-1.7.4/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.145218 dagster-1.7.4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.145218 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.145218 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.145218 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.145218 dagster-1.7.4/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.149218 dagster-1.7.4/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13462 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    27262 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/__generated__/api_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    43164 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    22739 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    23173 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.149218 dagster-1.7.4/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5993 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    13431 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/proxy_server.py
+-rw-r--r--   0 root         (0) root         (0)    60914 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    29291 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.149218 dagster-1.7.4/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.149218 dagster-1.7.4/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_loggers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.149218 dagster-1.7.4/dagster/_model/
+-rw-r--r--   0 root         (0) root         (0)     1491 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_model/pydantic_compat_layer.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.149218 dagster-1.7.4/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42035 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.153218 dagster-1.7.4/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      701 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8916 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7292 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    43131 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.153218 dagster-1.7.4/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5455 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.153218 dagster-1.7.4/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.169218 dagster-1.7.4/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    26539 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9314 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     5536 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    42955 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     5865 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)    12887 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/container.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/env.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      745 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)    11214 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    33445 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/security.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.169218 dagster-1.7.4/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    13678 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7790 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/data_versions.py
+-rw-r--r--   0 root         (0) root         (0)      119 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    36138 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.169218 dagster-1.7.4/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/typed_dict.py
+-rw-r--r--   0 root         (0) root         (0)      170 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4740 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/warnings.py
+-rw-r--r--   0 root         (0) root         (0)     4902 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.049219 dagster-1.7.4/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9867 2024-05-02 20:32:08.000000 dagster-1.7.4/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    28135 2024-05-02 20:32:08.000000 dagster-1.7.4/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:32:08.000000 dagster-1.7.4/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2024-05-02 20:32:08.000000 dagster-1.7.4/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1467 2024-05-02 20:32:08.000000 dagster-1.7.4/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-02 20:32:08.000000 dagster-1.7.4/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2024-05-02 20:32:09.173218 dagster-1.7.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6847 2024-05-02 20:31:40.000000 dagster-1.7.4/setup.py
```

### Comparing `dagster-1.7.3/COPYING` & `dagster-1.7.4/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/LICENSE` & `dagster-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/MANIFEST.in` & `dagster-1.7.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/PKG-INFO` & `dagster-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.3
+Version: 1.7.4
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
```

### Comparing `dagster-1.7.3/README.md` & `dagster-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/__init__.py` & `dagster-1.7.4/dagster/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,17 +127,19 @@
 )
 from dagster._core.definitions.asset_spec import AssetSpec as AssetSpec
 from dagster._core.definitions.assets import AssetsDefinition as AssetsDefinition
 from dagster._core.definitions.auto_materialize_policy import (
     AutoMaterializePolicy as AutoMaterializePolicy,
 )
 from dagster._core.definitions.auto_materialize_rule import (
-    AutoMaterializeAssetPartitionsFilter as AutoMaterializeAssetPartitionsFilter,
     AutoMaterializeRule as AutoMaterializeRule,
 )
+from dagster._core.definitions.auto_materialize_rule_impls import (
+    AutoMaterializeAssetPartitionsFilter as AutoMaterializeAssetPartitionsFilter,
+)
 from dagster._core.definitions.auto_materialize_sensor_definition import (
     AutoMaterializeSensorDefinition as AutoMaterializeSensorDefinition,
 )
 from dagster._core.definitions.backfill_policy import BackfillPolicy as BackfillPolicy
 from dagster._core.definitions.composition import PendingNodeInvocation as PendingNodeInvocation
 from dagster._core.definitions.config import ConfigMapping as ConfigMapping
 from dagster._core.definitions.configurable import configured as configured
```

### Comparing `dagster-1.7.3/dagster/_annotations.py` & `dagster-1.7.4/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_api/get_server_id.py` & `dagster-1.7.4/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_api/list_repositories.py` & `dagster-1.7.4/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_api/notebook_data.py` & `dagster-1.7.4/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_api/snapshot_execution_plan.py` & `dagster-1.7.4/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_api/snapshot_job.py` & `dagster-1.7.4/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_api/snapshot_partition.py` & `dagster-1.7.4/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_api/snapshot_repository.py` & `dagster-1.7.4/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_api/snapshot_schedule.py` & `dagster-1.7.4/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_api/snapshot_sensor.py` & `dagster-1.7.4/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_check/README.md` & `dagster-1.7.4/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_check/__init__.py` & `dagster-1.7.4/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/__init__.py` & `dagster-1.7.4/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/api.py` & `dagster-1.7.4/dagster/_cli/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/asset.py` & `dagster-1.7.4/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/code_server.py` & `dagster-1.7.4/dagster/_cli/code_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/config_scaffolder.py` & `dagster-1.7.4/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/debug.py` & `dagster-1.7.4/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/dev.py` & `dagster-1.7.4/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/instance.py` & `dagster-1.7.4/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/job.py` & `dagster-1.7.4/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/load_handle.py` & `dagster-1.7.4/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/project.py` & `dagster-1.7.4/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/run.py` & `dagster-1.7.4/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/schedule.py` & `dagster-1.7.4/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/sensor.py` & `dagster-1.7.4/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/utils.py` & `dagster-1.7.4/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_cli/workspace/cli_target.py` & `dagster-1.7.4/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/__init__.py` & `dagster-1.7.4/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/config_schema.py` & `dagster-1.7.4/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/config_type.py` & `dagster-1.7.4/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/errors.py` & `dagster-1.7.4/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/evaluate_value_result.py` & `dagster-1.7.4/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/field.py` & `dagster-1.7.4/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/field_utils.py` & `dagster-1.7.4/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/post_process.py` & `dagster-1.7.4/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/primitive_mapping.py` & `dagster-1.7.4/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/pythonic_config/__init__.py` & `dagster-1.7.4/dagster/_config/pythonic_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.7.4/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/pythonic_config/config.py` & `dagster-1.7.4/dagster/_config/pythonic_config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from dagster._model.pydantic_compat_layer import (
     USING_PYDANTIC_2,
     ModelFieldCompat,
     PydanticUndefined,
     model_config,
     model_fields,
 )
-from dagster._utils.cached_method import CACHED_METHOD_FIELD_SUFFIX
+from dagster._utils.cached_method import CACHED_METHOD_CACHE_FIELD
 
 from .attach_other_object_to_context import (
     IAttachDifferentObjectToOpContext as IAttachDifferentObjectToOpContext,
 )
 from .conversion_utils import _convert_pydantic_field, safe_is_subclass
 from .type_check_utils import is_literal
 from .typing_utils import BaseConfigMeta
@@ -61,15 +61,15 @@
 
 
 def _is_field_internal(name: str) -> bool:
     return name.endswith(INTERNAL_MARKER)
 
 
 # ensure that this ends with the internal marker so we can do a single check
-assert CACHED_METHOD_FIELD_SUFFIX.endswith(INTERNAL_MARKER)
+assert CACHED_METHOD_CACHE_FIELD.endswith(INTERNAL_MARKER)
 
 
 def _is_frozen_pydantic_error(e: Exception) -> bool:
     """Parses an error to determine if it is a Pydantic error indicating that the instance
     is immutable. We use this to attach a more helpful error message.
     """
     return "Instance is frozen" in str(  # Pydantic 2.x error
```

### Comparing `dagster-1.7.3/dagster/_config/pythonic_config/conversion_utils.py` & `dagster-1.7.4/dagster/_config/pythonic_config/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/pythonic_config/io_manager.py` & `dagster-1.7.4/dagster/_config/pythonic_config/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/pythonic_config/resource.py` & `dagster-1.7.4/dagster/_config/pythonic_config/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/pythonic_config/type_check_utils.py` & `dagster-1.7.4/dagster/_config/pythonic_config/type_check_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.7.4/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/snap.py` & `dagster-1.7.4/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/source.py` & `dagster-1.7.4/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/stack.py` & `dagster-1.7.4/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/traversal_context.py` & `dagster-1.7.4/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/type_printer.py` & `dagster-1.7.4/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_config/validate.py` & `dagster-1.7.4/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/asset_graph_view/asset_graph_view.py` & `dagster-1.7.4/dagster/_core/asset_graph_view/asset_graph_view.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/assets.py` & `dagster-1.7.4/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/code_pointer.py` & `dagster-1.7.4/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/container_context/config.py` & `dagster-1.7.4/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/debug.py` & `dagster-1.7.4/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/decorator_utils.py` & `dagster-1.7.4/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/__init__.py` & `dagster-1.7.4/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_check_evaluation.py` & `dagster-1.7.4/dagster/_core/definitions/asset_check_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_check_result.py` & `dagster-1.7.4/dagster/_core/definitions/asset_check_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,17 @@
             step_context.job_def.asset_layer.check_names_by_asset_key_by_node_handle.get(
                 step_context.node_handle.root
             )
         )
 
         check_key = self.resolve_target_check_key(check_names_by_asset_key)
 
-        input_asset_info = step_context.get_input_asset_version_info(check_key.asset_key)
+        input_asset_info = step_context.maybe_fetch_and_get_input_asset_version_info(
+            check_key.asset_key
+        )
         from dagster._core.events import DagsterEventType
 
         if (
             input_asset_info is not None
             and input_asset_info.event_type == DagsterEventType.ASSET_MATERIALIZATION
         ):
             target_materialization_data = AssetCheckEvaluationTargetMaterializationData(
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_check_spec.py` & `dagster-1.7.4/dagster/_core/definitions/asset_check_spec.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_checks.py` & `dagster-1.7.4/dagster/_core/definitions/asset_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,12 +131,13 @@
         partitions_def=asset_def.partitions_def,
         check_specs=check_specs,
         description=asset_def.descriptions_by_key.get(asset_def.key),
         ins={name: AssetIn(key) for name, key in asset_def.keys_by_input_name.items()},
         resource_defs=asset_def.resource_defs,
         metadata=asset_def.metadata_by_key.get(asset_def.key),
         tags=None,
+        owners=None,
         freshness_policy=asset_def.freshness_policies_by_key.get(asset_def.key),
         auto_materialize_policy=asset_def.auto_materialize_policies_by_key.get(asset_def.key),
         backfill_policy=asset_def.backfill_policy,
         config=None,  # gets config from asset_def.op
     )
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_condition/asset_condition.py` & `dagster-1.7.4/dagster/_core/definitions/asset_condition/asset_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import functools
-import hashlib
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Dict,
     FrozenSet,
@@ -21,14 +20,15 @@
 
 from dagster._annotations import experimental
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.metadata import MetadataMapping, MetadataValue
 from dagster._core.definitions.partition import AllPartitionsSubset
 from dagster._model import DagsterModel
 from dagster._serdes.serdes import PackableValue, whitelist_for_serdes
+from dagster._utils.security import non_secure_md5_hash_str
 
 from ..asset_subset import AssetSubset, ValidAssetSubset
 from ..auto_materialize_rule import AutoMaterializeRule
 
 if TYPE_CHECKING:
     from .asset_condition_evaluation_context import AssetConditionEvaluationContext
 
@@ -281,15 +281,15 @@
 
     @property
     def unique_id(self) -> str:
         parts = [
             self.__class__.__name__,
             *[child.unique_id for child in self.children],
         ]
-        return hashlib.md5("".join(parts).encode()).hexdigest()
+        return non_secure_md5_hash_str("".join(parts).encode())
 
     @abstractmethod
     def evaluate(self, context: "AssetConditionEvaluationContext") -> "AssetConditionResult":
         raise NotImplementedError()
 
     @property
     @abstractmethod
@@ -405,15 +405,15 @@
     """This class represents the condition that a particular AutoMaterializeRule is satisfied."""
 
     rule: AutoMaterializeRule
 
     @property
     def unique_id(self) -> str:
         parts = [self.rule.__class__.__name__, self.description]
-        return hashlib.md5("".join(parts).encode()).hexdigest()
+        return non_secure_md5_hash_str("".join(parts).encode())
 
     @property
     def description(self) -> str:
         return self.rule.description
 
     def evaluate(self, context: "AssetConditionEvaluationContext") -> "AssetConditionResult":
         context.root_context.daemon_context.logger.debug(
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py` & `dagster-1.7.4/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import dataclasses
 import datetime
 import functools
+import os
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Callable,
@@ -238,21 +239,25 @@
     @root_property
     def _parent_has_updated_subset_and_new_latest_storage_id(
         self,
     ) -> Tuple[ValidAssetSubset, Optional[int]]:
         """Returns the set of asset partitions whose parents have updated since the last time this
         condition was evaluated.
         """
+        max_child_partitions_str = os.getenv("DAGSTER_MAX_AMP_CHILD_PARTITIONS", None)
         (
             asset_partitions,
             cursor,
         ) = self.root_context.instance_queryer.asset_partitions_with_newly_updated_parents_and_new_cursor(
             latest_storage_id=self.previous_max_storage_id,
             child_asset_key=self.root_context.asset_key,
             map_old_time_partitions=False,
+            max_child_partitions=int(max_child_partitions_str)
+            if max_child_partitions_str
+            else None,
         )
         return AssetSubset.from_asset_partitions_set(
             self.asset_key, self.partitions_def, asset_partitions
         ), cursor
 
     @property
     @root_property
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_daemon_context.py` & `dagster-1.7.4/dagster/_core/definitions/asset_daemon_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_daemon_cursor.py` & `dagster-1.7.4/dagster/_core/definitions/asset_daemon_cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     handled_root_subset: Optional[AssetSubset],
 ) -> "AssetConditionEvaluationState":
     """Generates an AssetDaemonCursor from information available on the old cursor format."""
     from dagster._core.definitions.asset_condition.asset_condition import (
         AssetConditionEvaluationState,
         RuleCondition,
     )
-    from dagster._core.definitions.auto_materialize_rule import MaterializeOnMissingRule
+    from dagster._core.definitions.auto_materialize_rule_impls import MaterializeOnMissingRule
 
     return AssetConditionEvaluationState(
         previous_evaluation=latest_evaluation,
         previous_tick_evaluation_timestamp=latest_timestamp,
         max_storage_id=latest_storage_id,
         # the only information we need to preserve from the previous cursor is the handled subset
         extra_state_by_unique_id={
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_dep.py` & `dagster-1.7.4/dagster/_core/definitions/asset_dep.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_graph.py` & `dagster-1.7.4/dagster/_core/definitions/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_graph_differ.py` & `dagster-1.7.4/dagster/_core/definitions/asset_graph_differ.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.7.4/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_in.py` & `dagster-1.7.4/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_job.py` & `dagster-1.7.4/dagster/_core/definitions/asset_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         create_unexecutable_external_assets_from_assets_def,
     )
 
     selected_keys = selection.resolve(parent_asset_graph)
     invalid_keys = selected_keys - parent_asset_graph.executable_asset_keys
     if invalid_keys:
         raise DagsterInvalidDefinitionError(
-            "Selected keys keys must be a subset of existing executable asset keys."
+            "Selected keys must be a subset of existing executable asset keys."
             f" Invalid selected keys: {invalid_keys}",
         )
 
     _infer_and_validate_common_partitions_def(parent_asset_graph, selected_keys)
 
     selected_check_keys = selection.resolve_checks(parent_asset_graph)
 
@@ -629,15 +629,20 @@
             subsetted_assets_defs.append(assets_def)
         else:
             for asset_keys in color_mapping.values():
                 subsetted_assets_defs.append(
                     assets_def.subset_for(asset_keys, selected_asset_check_keys=None)
                 )
 
-    return AssetGraph.from_assets(subsetted_assets_defs)
+    # We didn't color asset checks, so add any that are in their own node.
+    assets_defs_with_only_checks = [
+        ad for ad in asset_graph.assets_defs if has_only_asset_checks(ad)
+    ]
+
+    return AssetGraph.from_assets(subsetted_assets_defs + assets_defs_with_only_checks)
 
 
 def _ensure_resources_dont_conflict(
     asset_graph: AssetGraph,
     resource_defs: Mapping[str, ResourceDefinition],
 ) -> None:
     """Ensures that resources between assets, source assets, and provided resource dictionary do not conflict."""
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_key.py` & `dagster-1.7.4/dagster/_core/definitions/asset_key.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_layer.py` & `dagster-1.7.4/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_out.py` & `dagster-1.7.4/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_selection.py` & `dagster-1.7.4/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.7.4/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_spec.py` & `dagster-1.7.4/dagster/_core/definitions/asset_spec.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/asset_subset.py` & `dagster-1.7.4/dagster/_core/definitions/asset_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/assets.py` & `dagster-1.7.4/dagster/_core/definitions/assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -459,14 +459,15 @@
         freshness_policies_by_output_name: Optional[Mapping[str, Optional[FreshnessPolicy]]] = None,
         auto_materialize_policies_by_output_name: Optional[
             Mapping[str, Optional[AutoMaterializePolicy]]
         ] = None,
         backfill_policy: Optional[BackfillPolicy] = None,
         can_subset: bool = False,
         check_specs: Optional[Sequence[AssetCheckSpec]] = None,
+        owners_by_key: Optional[Mapping[AssetKey, Sequence[Union[str, AssetOwner]]]] = None,
     ) -> "AssetsDefinition":
         """Constructs an AssetsDefinition from a GraphDefinition.
 
         Args:
             graph_def (GraphDefinition): The GraphDefinition that is an asset.
             keys_by_input_name (Optional[Mapping[str, AssetKey]]): A mapping of the input
                 names of the decorated graph to their corresponding asset keys. If not provided,
@@ -503,26 +504,28 @@
             descriptions_by_output_name (Optional[Mapping[str, Optional[str]]]): Defines a description to be
                 associated with each of the output asstes for this graph.
             metadata_by_output_name (Optional[Mapping[str, Optional[RawMetadataMapping]]]): Defines metadata to
                 be associated with each of the output assets for this node. Keys are names of the
                 outputs, and values are dictionaries of metadata to be associated with the related
                 asset.
             tags_by_output_name (Optional[Mapping[str, Optional[Mapping[str, str]]]]): Defines
-                tags to be associated with each othe output assets for this node. Keys are the names
+                tags to be associated with each of the output assets for this node. Keys are the names
                 of outputs, and values are dictionaries of tags to be associated with the related
                 asset.
             freshness_policies_by_output_name (Optional[Mapping[str, Optional[FreshnessPolicy]]]): Defines a
                 FreshnessPolicy to be associated with some or all of the output assets for this node.
                 Keys are the names of the outputs, and values are the FreshnessPolicies to be attached
                 to the associated asset.
             auto_materialize_policies_by_output_name (Optional[Mapping[str, Optional[AutoMaterializePolicy]]]): Defines an
                 AutoMaterializePolicy to be associated with some or all of the output assets for this node.
                 Keys are the names of the outputs, and values are the AutoMaterializePolicies to be attached
                 to the associated asset.
             backfill_policy (Optional[BackfillPolicy]): Defines this asset's BackfillPolicy
+            owners_by_key (Optional[Mapping[AssetKey, Sequence[Union[str, AssetOwner]]]]): Defines
+                owners to be associated with each of the asset keys for this node.
 
         """
         return AssetsDefinition._from_node(
             node_def=graph_def,
             keys_by_input_name=keys_by_input_name,
             keys_by_output_name=keys_by_output_name,
             key_prefix=key_prefix,
@@ -536,14 +539,15 @@
             metadata_by_output_name=metadata_by_output_name,
             tags_by_output_name=tags_by_output_name,
             freshness_policies_by_output_name=freshness_policies_by_output_name,
             auto_materialize_policies_by_output_name=auto_materialize_policies_by_output_name,
             backfill_policy=backfill_policy,
             can_subset=can_subset,
             check_specs=check_specs,
+            owners_by_key=owners_by_key,
         )
 
     @public
     @staticmethod
     def from_op(
         op_def: OpDefinition,
         *,
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.7.4/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 from enum import Enum
-from typing import TYPE_CHECKING, AbstractSet, Dict, FrozenSet, NamedTuple, Optional, Sequence
+from typing import AbstractSet, Dict, FrozenSet, NamedTuple, Optional, Sequence
 
 import dagster._check as check
 from dagster._annotations import deprecated, experimental, public
+from dagster._core.definitions.asset_condition.asset_condition import AssetCondition
+from dagster._core.definitions.auto_materialize_rule import (
+    AutoMaterializeRule,
+    AutoMaterializeRuleSnapshot,
+)
 from dagster._serdes.serdes import (
     NamedTupleSerializer,
     UnpackContext,
     UnpackedValue,
     whitelist_for_serdes,
 )
 
-if TYPE_CHECKING:
-    from dagster._core.definitions.asset_condition.asset_condition import AssetCondition
-    from dagster._core.definitions.auto_materialize_rule import (
-        AutoMaterializeRule,
-        AutoMaterializeRuleSnapshot,
-    )
-
 
 class AutoMaterializePolicySerializer(NamedTupleSerializer):
     def before_unpack(
         self, context: UnpackContext, unpacked_dict: Dict[str, UnpackedValue]
     ) -> Dict[str, UnpackedValue]:
-        from dagster._core.definitions.auto_materialize_rule import AutoMaterializeRule
-
         backcompat_map = {
             "on_missing": AutoMaterializeRule.materialize_on_missing(),
             "on_new_parent_data": AutoMaterializeRule.materialize_on_parent_updated(),
             "for_freshness": AutoMaterializeRule.materialize_on_required_for_freshness(),
         }
 
         # determine if this namedtuple was serialized with the old format (booleans for rules)
@@ -57,17 +53,17 @@
     old_fields={"time_window_partition_scope_minutes": 1e-6},
     serializer=AutoMaterializePolicySerializer,
 )
 class AutoMaterializePolicy(
     NamedTuple(
         "_AutoMaterializePolicy",
         [
-            ("rules", FrozenSet["AutoMaterializeRule"]),
+            ("rules", FrozenSet[AutoMaterializeRule]),
             ("max_materializations_per_minute", Optional[int]),
-            ("asset_condition", Optional["AssetCondition"]),
+            ("asset_condition", Optional[AssetCondition]),
         ],
     )
 ):
     """An AutoMaterializePolicy specifies how Dagster should attempt to keep an asset up-to-date.
 
     Each policy consists of a set of AutoMaterializeRules, which are used to determine whether an
     asset or a partition of an asset should or should not be auto-materialized.
@@ -122,15 +118,15 @@
 
     """
 
     def __new__(
         cls,
         rules: AbstractSet["AutoMaterializeRule"],
         max_materializations_per_minute: Optional[int] = 1,
-        asset_condition: Optional["AssetCondition"] = None,
+        asset_condition: Optional[AssetCondition] = None,
     ):
         from dagster._core.definitions.auto_materialize_rule import AutoMaterializeRule
 
         check.invariant(
             max_materializations_per_minute is None or max_materializations_per_minute > 0,
             "max_materializations_per_minute must be positive. To disable rate-limiting, set it"
             " to None. To disable auto materializing, remove the policy.",
@@ -169,15 +165,15 @@
         from dagster._core.definitions.auto_materialize_rule import AutoMaterializeDecisionType
 
         return {
             rule for rule in self.rules if rule.decision_type == AutoMaterializeDecisionType.SKIP
         }
 
     @staticmethod
-    def from_asset_condition(asset_condition: "AssetCondition") -> "AutoMaterializePolicy":
+    def from_asset_condition(asset_condition: AssetCondition) -> "AutoMaterializePolicy":
         """Constructs an AutoMaterializePolicy which will materialize an asset partition whenever
         the provided asset_condition evaluates to True.
 
         Args:
             asset_condition (AssetCondition): The condition which determines whether an asset
                 partition should be materialized.
         """
@@ -281,22 +277,22 @@
             return AutoMaterializePolicyType.EAGER
         return AutoMaterializePolicyType.LAZY
 
     @property
     def rule_snapshots(self) -> Sequence["AutoMaterializeRuleSnapshot"]:
         return [rule.to_snapshot() for rule in self.rules]
 
-    def to_asset_condition(self) -> "AssetCondition":
+    def to_asset_condition(self) -> AssetCondition:
         """Converts a set of materialize / skip rules into a single binary expression."""
         from .asset_condition.asset_condition import (
             AndAssetCondition,
             NotAssetCondition,
             OrAssetCondition,
         )
-        from .auto_materialize_rule import DiscardOnMaxMaterializationsExceededRule
+        from .auto_materialize_rule_impls import DiscardOnMaxMaterializationsExceededRule
 
         if self.asset_condition is not None:
             return self.asset_condition
 
         materialize_condition = OrAssetCondition(
             operands=[
                 rule.to_asset_condition()
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/auto_materialize_rule.py` & `dagster-1.7.4/dagster/_core/definitions/auto_materialize_rule_impls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,266 +1,63 @@
 import datetime
-from abc import ABC, abstractmethod, abstractproperty
+import os
 from collections import defaultdict
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Dict,
     Iterable,
+    List,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Set,
 )
 
-import pytz
-
-import dagster._check as check
-from dagster._annotations import deprecated, experimental, public
+from dagster._annotations import deprecated, experimental
 from dagster._core.definitions.asset_subset import AssetSubset, ValidAssetSubset
+from dagster._core.definitions.auto_materialize_rule import AutoMaterializeRule
 from dagster._core.definitions.auto_materialize_rule_evaluation import (
     AutoMaterializeDecisionType,
-    AutoMaterializeRuleSnapshot,
     ParentUpdatedRuleEvaluationData,
     WaitingOnAssetsRuleEvaluationData,
 )
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.freshness_based_auto_materialize import (
     freshness_evaluation_results_for_asset_key,
 )
 from dagster._core.definitions.multi_dimensional_partitions import MultiPartitionsDefinition
 from dagster._core.definitions.time_window_partitions import (
     TimeWindow,
     TimeWindowPartitionsDefinition,
     get_time_partitions_def,
 )
 from dagster._core.errors import DagsterInvariantViolationError
+from dagster._core.event_api import AssetRecordsFilter
 from dagster._core.storage.dagster_run import IN_PROGRESS_RUN_STATUSES, RunsFilter
 from dagster._core.storage.tags import AUTO_MATERIALIZE_TAG
 from dagster._serdes.serdes import (
     whitelist_for_serdes,
 )
 from dagster._utils.schedules import (
     cron_string_iterator,
-    is_valid_cron_string,
     reverse_cron_string_iterator,
 )
 
 from .base_asset_graph import sort_key_for_asset_partition
 
 if TYPE_CHECKING:
     from dagster._core.definitions.asset_condition.asset_condition import (
-        AssetCondition,
         AssetConditionResult,
     )
 
     from .asset_condition.asset_condition_evaluation_context import AssetConditionEvaluationContext
 
 
-class AutoMaterializeRule(ABC):
-    """An AutoMaterializeRule defines a bit of logic which helps determine if a materialization
-    should be kicked off for a given asset partition.
-
-    Each rule can have one of two decision types, `MATERIALIZE` (indicating that an asset partition
-    should be materialized) or `SKIP` (indicating that the asset partition should not be
-    materialized).
-
-    Materialize rules are evaluated first, and skip rules operate over the set of candidates that
-    are produced by the materialize rules. Other than that, there is no ordering between rules.
-    """
-
-    @abstractproperty
-    def decision_type(self) -> AutoMaterializeDecisionType:
-        """The decision type of the rule (either `MATERIALIZE` or `SKIP`)."""
-        ...
-
-    @abstractproperty
-    def description(self) -> str:
-        """A human-readable description of this rule. As a basic guideline, this string should
-        complete the sentence: 'Indicates an asset should be (materialize/skipped) when ____'.
-        """
-        ...
-
-    def to_asset_condition(self) -> "AssetCondition":
-        """Converts this AutoMaterializeRule into an AssetCondition."""
-        from .asset_condition.asset_condition import RuleCondition
-
-        return RuleCondition(rule=self)
-
-    @abstractmethod
-    def evaluate_for_asset(
-        self, context: "AssetConditionEvaluationContext"
-    ) -> "AssetConditionResult":
-        """The core evaluation function for the rule. This function takes in a context object and
-        returns a mapping from evaluated rules to the set of asset partitions that the rule applies
-        to.
-        """
-        ...
-
-    @public
-    @staticmethod
-    def materialize_on_required_for_freshness() -> "MaterializeOnRequiredForFreshnessRule":
-        """(Deprecated) Materialize an asset partition if it is required to satisfy a freshness policy of this
-        asset or one of its downstream assets.
-
-        Note: This rule has no effect on partitioned assets.
-        """
-        return MaterializeOnRequiredForFreshnessRule()
-
-    @public
-    @staticmethod
-    def materialize_on_cron(
-        cron_schedule: str, timezone: str = "UTC", all_partitions: bool = False
-    ) -> "MaterializeOnCronRule":
-        """Materialize an asset partition if it has not been materialized since the latest cron
-        schedule tick. For assets with a time component to their partitions_def, this rule will
-        request all partitions that have been missed since the previous tick.
-
-        Args:
-            cron_schedule (str): A cron schedule string (e.g. "`0 * * * *`") indicating the ticks for
-                which this rule should fire.
-            timezone (str): The timezone in which this cron schedule should be evaluated. Defaults
-                to "UTC".
-            all_partitions (bool): If True, this rule fires for all partitions of this asset on each
-                cron tick. If False, this rule fires only for the last partition of this asset.
-                Defaults to False.
-        """
-        check.param_invariant(
-            is_valid_cron_string(cron_schedule), "cron_schedule", "must be a valid cron string"
-        )
-        check.param_invariant(
-            timezone in pytz.all_timezones_set, "timezone", "must be a valid timezone"
-        )
-        return MaterializeOnCronRule(
-            cron_schedule=cron_schedule, timezone=timezone, all_partitions=all_partitions
-        )
-
-    @public
-    @staticmethod
-    def materialize_on_parent_updated(
-        updated_parent_filter: Optional["AutoMaterializeAssetPartitionsFilter"] = None,
-    ) -> "MaterializeOnParentUpdatedRule":
-        """Materialize an asset partition if one of its parents has been updated more recently
-        than it has.
-
-        Note: For time-partitioned or dynamic-partitioned assets downstream of an unpartitioned
-        asset, this rule will only fire for the most recent partition of the downstream.
-
-        Args:
-            updated_parent_filter (Optional[AutoMaterializeAssetPartitionsFilter]): Filter to apply
-                to updated parents. If a parent was updated but does not pass the filter criteria,
-                then it won't count as updated for the sake of this rule.
-        """
-        return MaterializeOnParentUpdatedRule(updated_parent_filter=updated_parent_filter)
-
-    @public
-    @staticmethod
-    def materialize_on_missing() -> "MaterializeOnMissingRule":
-        """Materialize an asset partition if it has never been materialized before. This rule will
-        not fire for non-root assets unless that asset's parents have been updated.
-        """
-        return MaterializeOnMissingRule()
-
-    @public
-    @staticmethod
-    def skip_on_parent_missing() -> "SkipOnParentMissingRule":
-        """Skip materializing an asset partition if one of its parent asset partitions has never
-        been materialized (for regular assets) or observed (for observable source assets).
-        """
-        return SkipOnParentMissingRule()
-
-    @public
-    @staticmethod
-    def skip_on_parent_outdated() -> "SkipOnParentOutdatedRule":
-        """Skip materializing an asset partition if any of its parents has not incorporated the
-        latest data from its ancestors.
-        """
-        return SkipOnParentOutdatedRule()
-
-    @public
-    @staticmethod
-    def skip_on_not_all_parents_updated(
-        require_update_for_all_parent_partitions: bool = False,
-    ) -> "SkipOnNotAllParentsUpdatedRule":
-        """Skip materializing an asset partition if any of its parents have not been updated since
-        the asset's last materialization.
-
-        Args:
-            require_update_for_all_parent_partitions (Optional[bool]): Applies only to an unpartitioned
-                asset or an asset partition that depends on more than one partition in any upstream asset.
-                If true, requires all upstream partitions in each upstream asset to be materialized since
-                the downstream asset's last materialization in order to update it. If false, requires at
-                least one upstream partition in each upstream asset to be materialized since the downstream
-                asset's last materialization in order to update it. Defaults to false.
-        """
-        return SkipOnNotAllParentsUpdatedRule(require_update_for_all_parent_partitions)
-
-    @staticmethod
-    def skip_on_not_all_parents_updated_since_cron(
-        cron_schedule: str, timezone: str = "UTC"
-    ) -> "SkipOnNotAllParentsUpdatedSinceCronRule":
-        """Skip materializing an asset partition if any of its parents have not been updated since
-        the latest tick of the given cron schedule.
-
-        Args:
-            cron_schedule (str): A cron schedule string (e.g. "`0 * * * *`").
-            timezone (str): The timezone in which this cron schedule should be evaluated. Defaults
-                to "UTC".
-        """
-        return SkipOnNotAllParentsUpdatedSinceCronRule(
-            cron_schedule=cron_schedule, timezone=timezone
-        )
-
-    @public
-    @staticmethod
-    def skip_on_required_but_nonexistent_parents() -> "SkipOnRequiredButNonexistentParentsRule":
-        """Skip an asset partition if it depends on parent partitions that do not exist.
-
-        For example, imagine a downstream asset is time-partitioned, starting in 2022, but has a
-        time-partitioned parent which starts in 2023. This rule will skip attempting to materialize
-        downstream partitions from before 2023, since the parent partitions do not exist.
-        """
-        return SkipOnRequiredButNonexistentParentsRule()
-
-    @public
-    @staticmethod
-    def skip_on_backfill_in_progress(
-        all_partitions: bool = False,
-    ) -> "SkipOnBackfillInProgressRule":
-        """Skip an asset's partitions if targeted by an in-progress backfill.
-
-        Args:
-            all_partitions (bool): If True, skips all partitions of the asset being backfilled,
-                regardless of whether the specific partition is targeted by a backfill.
-                If False, skips only partitions targeted by a backfill. Defaults to False.
-        """
-        return SkipOnBackfillInProgressRule(all_partitions)
-
-    @staticmethod
-    def skip_on_run_in_progress() -> "SkipOnRunInProgressRule":
-        return SkipOnRunInProgressRule()
-
-    def to_snapshot(self) -> AutoMaterializeRuleSnapshot:
-        """Returns a serializable snapshot of this rule for historical evaluations."""
-        return AutoMaterializeRuleSnapshot(
-            class_name=self.__class__.__name__,
-            description=self.description,
-            decision_type=self.decision_type,
-        )
-
-    def __eq__(self, other) -> bool:
-        # override the default NamedTuple __eq__ method to factor in types
-        return type(self) == type(other) and super().__eq__(other)
-
-    def __hash__(self) -> int:
-        # override the default NamedTuple __hash__ method to factor in types
-        return hash(hash(type(self)) + super().__hash__())
-
-
 @deprecated(
     breaking_version="1.8",
     additional_warn_text="Lazy auto-materialize is deprecated, in favor of explicit cron-based "
     "scheduling rules. Additional alternatives to replicate more of the lazy auto-materialize "
     "behavior will be provided before this is fully removed.",
 )
 @whitelist_for_serdes
@@ -441,30 +238,50 @@
         context: "AssetConditionEvaluationContext",
         asset_partitions: Iterable[AssetKeyPartitionKey],
     ) -> Iterable[AssetKeyPartitionKey]:
         if self.latest_run_required_tags is None:
             return asset_partitions
 
         will_update_asset_partitions: Set[AssetKeyPartitionKey] = set()
+        storage_ids_to_fetch_by_key: Dict[AssetKey, List[int]] = defaultdict(list)
 
-        asset_partitions_by_latest_run_id: Dict[str, Set[AssetKeyPartitionKey]] = defaultdict(set)
         for asset_partition in asset_partitions:
             if context.will_update_asset_partition(asset_partition):
                 will_update_asset_partitions.add(asset_partition)
             else:
-                record = context.instance_queryer.get_latest_materialization_or_observation_record(
-                    asset_partition
+                latest_storage_id = (
+                    context.instance_queryer.get_latest_materialization_or_observation_storage_id(
+                        asset_partition=asset_partition
+                    )
                 )
+                if latest_storage_id is not None:
+                    storage_ids_to_fetch_by_key[asset_partition.asset_key].append(latest_storage_id)
 
-                if record is None:
-                    raise RuntimeError(
-                        f"No materialization record found for asset partition {asset_partition}"
-                    )
+        asset_partitions_by_latest_run_id: Dict[str, Set[AssetKeyPartitionKey]] = defaultdict(set)
+
+        step = int(os.getenv("DAGSTER_ASSET_DAEMON_RUN_TAGS_EVENT_FETCH_LIMIT", "1000"))
 
-                asset_partitions_by_latest_run_id[record.run_id].add(asset_partition)
+        for asset_key, storage_ids_to_fetch in storage_ids_to_fetch_by_key.items():
+            for i in range(0, len(storage_ids_to_fetch), step):
+                storage_ids = storage_ids_to_fetch[i : i + step]
+                fetch_records = (
+                    context.instance_queryer.instance.fetch_observations
+                    if context.asset_graph.get(asset_key).is_observable
+                    else context.instance_queryer.instance.fetch_materializations
+                )
+                for record in fetch_records(
+                    records_filter=AssetRecordsFilter(
+                        asset_key=asset_key,
+                        storage_ids=storage_ids,
+                    ),
+                    limit=step,
+                ).records:
+                    asset_partitions_by_latest_run_id[record.run_id].add(
+                        AssetKeyPartitionKey(asset_key, record.partition_key)
+                    )
 
         if len(asset_partitions_by_latest_run_id) > 0:
             run_ids_with_required_tags = context.instance_queryer.instance.get_run_ids(
                 filters=RunsFilter(
                     run_ids=list(asset_partitions_by_latest_run_id.keys()),
                     tags=self.latest_run_required_tags,
                 )
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/auto_materialize_rule_evaluation.py` & `dagster-1.7.4/dagster/_core/definitions/auto_materialize_rule_evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import hashlib
 from abc import ABC, abstractproperty
 from collections import defaultdict
 from enum import Enum
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Dict,
@@ -310,15 +309,15 @@
                 return None
             evaluation = child_evaluations[0]
         else:
             unique_id_parts = [
                 OrAssetCondition.__name__,
                 *[e.condition_snapshot.unique_id for e in child_evaluations],
             ]
-            unique_id = hashlib.md5("".join(unique_id_parts).encode()).hexdigest()
+            unique_id = non_secure_md5_hash_str("".join(unique_id_parts).encode())
             decision_type_snapshot = AssetConditionSnapshot(
                 class_name=OrAssetCondition.__name__, description="Any of", unique_id=unique_id
             )
             true_subset = AssetSubset.empty(asset_key, self.partitions_def)
             for e in child_evaluations:
                 true_subset |= e.true_subset
             evaluation = AssetConditionEvaluation(
@@ -337,15 +336,15 @@
             return evaluation
 
         # non-materialize conditions are inverted
         unique_id_parts = [
             NotAssetCondition.__name__,
             evaluation.condition_snapshot.unique_id,
         ]
-        unique_id = hashlib.md5("".join(unique_id_parts).encode()).hexdigest()
+        unique_id = non_secure_md5_hash_str("".join(unique_id_parts).encode())
 
         if is_partitioned:
             # In reality, we'd like to invert the inner true_subset here, but this is an
             # expensive operation, and error-prone as the set of all partitions may have changed
             # since the evaluation was stored. Instead, we just use an empty subset.
             true_subset = AssetSubset.empty(asset_key, self.partitions_def)
         else:
@@ -428,15 +427,15 @@
         )
 
         # the top level condition is the AND of all the sub-conditions
         unique_id_parts = [
             AndAssetCondition.__name__,
             *[e.condition_snapshot.unique_id for e in child_evaluations],
         ]
-        unique_id = hashlib.md5("".join(unique_id_parts).encode()).hexdigest()
+        unique_id = non_secure_md5_hash_str("".join(unique_id_parts).encode())
         condition_snapshot = AssetConditionSnapshot(
             class_name=AndAssetCondition.__name__, description="All of", unique_id=unique_id
         )
 
         # all AssetSubsets generated here are created using the current partitions_def, so they
         # will be valid
         true_subset = materialize_evaluation.true_subset.as_valid(self.partitions_def)
@@ -470,18 +469,16 @@
 
     def unpack(
         self,
         unpacked_dict: Dict[str, UnpackedValue],
         whitelist_map: WhitelistMap,
         context: UnpackContext,
     ) -> AutoMaterializeRuleEvaluation:
-        from .auto_materialize_rule import (
-            AutoMaterializeRule,
-            DiscardOnMaxMaterializationsExceededRule,
-        )
+        from .auto_materialize_rule import AutoMaterializeRule
+        from .auto_materialize_rule_impls import DiscardOnMaxMaterializationsExceededRule
 
         if self.klass in (
             FreshnessAutoMaterializeCondition,
             DownstreamFreshnessAutoMaterializeCondition,
         ):
             return AutoMaterializeRuleEvaluation(
                 rule_snapshot=AutoMaterializeRule.materialize_on_required_for_freshness().to_snapshot(),
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/auto_materialize_sensor_definition.py` & `dagster-1.7.4/dagster/_core/definitions/auto_materialize_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/backfill_policy.py` & `dagster-1.7.4/dagster/_core/definitions/backfill_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/base_asset_graph.py` & `dagster-1.7.4/dagster/_core/definitions/base_asset_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,14 @@
 
 
 T_AssetNode = TypeVar("T_AssetNode", bound=BaseAssetNode)
 
 
 class BaseAssetGraph(ABC, Generic[T_AssetNode]):
     _asset_nodes_by_key: Mapping[AssetKey, T_AssetNode]
-    _asset_nodes_by_check_key: Mapping[AssetCheckKey, T_AssetNode]
 
     @property
     def asset_nodes(self) -> Iterable[T_AssetNode]:
         return self._asset_nodes_by_key.values()
 
     def has(self, asset_key: AssetKey) -> bool:
         return asset_key in self._asset_nodes_by_key
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.7.4/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/composition.py` & `dagster-1.7.4/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/config.py` & `dagster-1.7.4/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/configurable.py` & `dagster-1.7.4/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/data_time.py` & `dagster-1.7.4/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/data_version.py` & `dagster-1.7.4/dagster/_core/definitions/data_version.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.7.4/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/decorators/asset_check_decorator.py` & `dagster-1.7.4/dagster/_core/definitions/decorators/asset_check_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.7.4/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1067,26 +1067,28 @@
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = ...,
     check_specs: Optional[Sequence[AssetCheckSpec]] = None,
     key: Optional[CoercibleToAssetKey] = None,
 ) -> Callable[[Callable[..., Any]], AssetsDefinition]: ...
 
 
 @experimental_param(param="tags")
+@experimental_param(param="owners")
 def graph_asset(
     compose_fn: Optional[Callable] = None,
     *,
     name: Optional[str] = None,
     description: Optional[str] = None,
     ins: Optional[Mapping[str, AssetIn]] = None,
     config: Optional[Union[ConfigMapping, Mapping[str, Any]]] = None,
     key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
     group_name: Optional[str] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
     metadata: Optional[RawMetadataMapping] = None,
     tags: Optional[Mapping[str, str]] = None,
+    owners: Optional[Sequence[str]] = None,
     freshness_policy: Optional[FreshnessPolicy] = None,
     auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
     backfill_policy: Optional[BackfillPolicy] = None,
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
     check_specs: Optional[Sequence[AssetCheckSpec]] = None,
     key: Optional[CoercibleToAssetKey] = None,
 ) -> Union[AssetsDefinition, Callable[[Callable[..., Any]], AssetsDefinition]]:
@@ -1125,14 +1127,17 @@
             not provided, the name "default" is used.
         partitions_def (Optional[PartitionsDefinition]): Defines the set of partition keys that
             compose the asset.
         metadata (Optional[RawMetadataMapping]): Dictionary of metadata to be associated with
             the asset.
         tags (Optional[Mapping[str, str]]): Tags for filtering and organizing. These tags are not
             attached to runs of the asset.
+        owners (Optional[Sequence[str]]): A list of strings representing owners of the asset. Each
+            string can be a user's email address, or a team name prefixed with `team:`,
+            e.g. `team:finops`.
         freshness_policy (Optional[FreshnessPolicy]): A constraint telling Dagster how often this asset is
             intended to be updated with respect to its root data.
         auto_materialize_policy (Optional[AutoMaterializePolicy]): The AutoMaterializePolicy to use
             for this asset.
         backfill_policy (Optional[BackfillPolicy]): The BackfillPolicy to use for this asset.
         key (Optional[CoeercibleToAssetKey]): The key for this asset. If provided, cannot specify key_prefix or name.
 
@@ -1159,14 +1164,15 @@
             ins=ins,
             config=config,
             key_prefix=key_prefix,
             group_name=group_name,
             partitions_def=partitions_def,
             metadata=metadata,
             tags=tags,
+            owners=owners,
             freshness_policy=freshness_policy,
             auto_materialize_policy=auto_materialize_policy,
             backfill_policy=backfill_policy,
             resource_defs=resource_defs,
             check_specs=check_specs,
             key=key,
         )
@@ -1178,14 +1184,15 @@
             ins=ins,
             config=config,
             key_prefix=key_prefix,
             group_name=group_name,
             partitions_def=partitions_def,
             metadata=metadata,
             tags=tags,
+            owners=owners,
             freshness_policy=freshness_policy,
             auto_materialize_policy=auto_materialize_policy,
             backfill_policy=backfill_policy,
             resource_defs=resource_defs,
             check_specs=check_specs,
             key=key,
         )
@@ -1199,14 +1206,15 @@
     ins: Optional[Mapping[str, AssetIn]],
     config: Optional[Union[ConfigMapping, Mapping[str, Any]]],
     key_prefix: Optional[CoercibleToAssetKeyPrefix],
     group_name: Optional[str],
     partitions_def: Optional[PartitionsDefinition],
     metadata: Optional[RawMetadataMapping],
     tags: Optional[Mapping[str, str]],
+    owners: Optional[Sequence[str]],
     freshness_policy: Optional[FreshnessPolicy],
     auto_materialize_policy: Optional[AutoMaterializePolicy],
     backfill_policy: Optional[BackfillPolicy],
     resource_defs: Optional[Mapping[str, ResourceDefinition]],
     check_specs: Optional[Sequence[AssetCheckSpec]],
     key: Optional[CoercibleToAssetKey],
 ) -> AssetsDefinition:
@@ -1261,14 +1269,15 @@
         auto_materialize_policies_by_output_name=(
             {"result": auto_materialize_policy} if auto_materialize_policy else None
         ),
         backfill_policy=backfill_policy,
         descriptions_by_output_name={"result": description} if description else None,
         resource_defs=resource_defs,
         check_specs=check_specs,
+        owners_by_key={out_asset_key: owners} if owners else None,
     )
 
 
 def graph_multi_asset(
     *,
     outs: Mapping[str, AssetOut],
     name: Optional[str] = None,
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.7.4/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.7.4/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.7.4/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.7.4/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.7.4/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.7.4/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.7.4/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.7.4/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.7.4/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.7.4/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/definitions_class.py` & `dagster-1.7.4/dagster/_core/definitions/definitions_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/dependency.py` & `dagster-1.7.4/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/events.py` & `dagster-1.7.4/dagster/_core/definitions/events.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/executor_definition.py` & `dagster-1.7.4/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/external_asset.py` & `dagster-1.7.4/dagster/_core/definitions/external_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/freshness_based_auto_materialize.py` & `dagster-1.7.4/dagster/_core/definitions/freshness_based_auto_materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/freshness_checks/last_update.py` & `dagster-1.7.4/dagster/_core/definitions/freshness_checks/last_update.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/freshness_checks/sensor.py` & `dagster-1.7.4/dagster/_core/definitions/freshness_checks/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/freshness_checks/shared_builder.py` & `dagster-1.7.4/dagster/_core/definitions/freshness_checks/shared_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/freshness_checks/time_partition.py` & `dagster-1.7.4/dagster/_core/definitions/freshness_checks/time_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/freshness_checks/utils.py` & `dagster-1.7.4/dagster/_core/definitions/freshness_checks/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import datetime
-import hashlib
 from typing import Iterator, Optional, Sequence, Union, cast
 
 from dagster import _check as check
 from dagster._core.definitions.asset_check_spec import AssetCheckSeverity
 from dagster._core.definitions.asset_checks import AssetChecksDefinition
 from dagster._core.event_api import AssetRecordsFilter, EventLogRecord
 from dagster._core.events import DagsterEventType
 from dagster._core.execution.context.compute import AssetCheckExecutionContext
 from dagster._core.instance import DagsterInstance
+from dagster._utils.security import non_secure_md5_hash_str
 
 from ..assets import AssetsDefinition, SourceAsset
 from ..events import AssetKey, CoercibleToAssetKey
 
 # Constants
 DEFAULT_FRESHNESS_SEVERITY = AssetCheckSeverity.WARN
 DEFAULT_FRESHNESS_TIMEZONE = "UTC"
@@ -233,10 +233,10 @@
 def unique_id_from_asset_keys(asset_keys: Sequence[AssetKey]) -> str:
     """Generate a unique ID from the provided asset keys.
 
     This is necessary to disambiguate between different ops underlying freshness checks without
     forcing the user to provide a name for the underlying op.
     """
     sorted_asset_keys = sorted(asset_keys, key=lambda asset_key: asset_key.to_string())
-    return hashlib.md5(
+    return non_secure_md5_hash_str(
         ",".join([str(asset_key) for asset_key in sorted_asset_keys]).encode()
-    ).hexdigest()[:8]
+    )[:8]
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/freshness_policy.py` & `dagster-1.7.4/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.7.4/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/graph_definition.py` & `dagster-1.7.4/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/hook_definition.py` & `dagster-1.7.4/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/hook_invocation.py` & `dagster-1.7.4/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/inference.py` & `dagster-1.7.4/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/input.py` & `dagster-1.7.4/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/instigation_logger.py` & `dagster-1.7.4/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/job_base.py` & `dagster-1.7.4/dagster/_core/definitions/job_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/job_definition.py` & `dagster-1.7.4/dagster/_core/definitions/job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/load_asset_checks_from_modules.py` & `dagster-1.7.4/dagster/_core/definitions/load_asset_checks_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.7.4/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/logger_definition.py` & `dagster-1.7.4/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/logger_invocation.py` & `dagster-1.7.4/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/materialize.py` & `dagster-1.7.4/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.7.4/dagster/_core/definitions/metadata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 import dagster._check as check
 import dagster._seven as seven
 from dagster._annotations import PublicAttr, deprecated, deprecated_param, experimental, public
 from dagster._core.definitions.asset_key import AssetKey
 from dagster._core.errors import DagsterInvalidMetadata
 from dagster._model import DagsterModel
+from dagster._model.pydantic_compat_layer import model_fields
 from dagster._serdes import whitelist_for_serdes
 from dagster._serdes.serdes import (
     FieldSerializer,
     PackableValue,
     UnpackContext,
     WhitelistMap,
     pack_value,
@@ -1248,15 +1249,15 @@
     @staticmethod
     def _strip_namespace_from_key(key: str) -> str:
         return key.split("/", 1)[1]
 
     def keys(self) -> AbstractSet[str]:
         return {
             self._namespaced_key(key)
-            for key in self.__fields__.keys()
+            for key in model_fields(self).keys()
             # getattr returns the pydantic property on the subclass
             if getattr(self, key) is not None
         }
 
     def __getitem__(self, key: str) -> Any:
         # getattr returns the pydantic property on the subclass
         return getattr(self, self._strip_namespace_from_key(key))
@@ -1284,15 +1285,15 @@
             metadata (Mapping[str, Any]): A dictionary of metadata entries.
         """
         kwargs = {}
         for namespaced_key, value in metadata.items():
             splits = namespaced_key.split("/")
             if len(splits) == 2:
                 namespace, key = splits
-                if namespace == cls.namespace() and key in cls.__fields__:
+                if namespace == cls.namespace() and key in model_fields(cls):
                     kwargs[key] = value.value if isinstance(value, MetadataValue) else value
 
         return cls(**kwargs)
 
 
 class TableMetadataSet(NamespacedMetadataSet):
     """Metadata entries that apply to definitions, observations, or materializations of assets that
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/metadata/table.py` & `dagster-1.7.4/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.7.4/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.7.4/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/node_container.py` & `dagster-1.7.4/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/node_definition.py` & `dagster-1.7.4/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/observe.py` & `dagster-1.7.4/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/op_definition.py` & `dagster-1.7.4/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/op_invocation.py` & `dagster-1.7.4/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/op_selection.py` & `dagster-1.7.4/dagster/_core/definitions/op_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/output.py` & `dagster-1.7.4/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/partition.py` & `dagster-1.7.4/dagster/_core/definitions/partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/partition_key_range.py` & `dagster-1.7.4/dagster/_core/definitions/partition_key_range.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/partition_mapping.py` & `dagster-1.7.4/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.7.4/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/policy.py` & `dagster-1.7.4/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/reconstruct.py` & `dagster-1.7.4/dagster/_core/definitions/reconstruct.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/remote_asset_graph.py` & `dagster-1.7.4/dagster/_core/definitions/remote_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.7.4/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.7.4/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.7.4/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.7.4/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.7.4/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.7.4/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.7.4/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/resource_annotation.py` & `dagster-1.7.4/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/resource_definition.py` & `dagster-1.7.4/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/resource_invocation.py` & `dagster-1.7.4/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/resource_requirement.py` & `dagster-1.7.4/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/result.py` & `dagster-1.7.4/dagster/_core/definitions/result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/run_config.py` & `dagster-1.7.4/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/run_config_schema.py` & `dagster-1.7.4/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/run_request.py` & `dagster-1.7.4/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.7.4/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/schedule_definition.py` & `dagster-1.7.4/dagster/_core/definitions/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/schema_change_checks.py` & `dagster-1.7.4/dagster/_core/definitions/schema_change_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.7.4/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/selector.py` & `dagster-1.7.4/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/sensor_definition.py` & `dagster-1.7.4/dagster/_core/definitions/sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/source_asset.py` & `dagster-1.7.4/dagster/_core/definitions/source_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/step_launcher.py` & `dagster-1.7.4/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/target.py` & `dagster-1.7.4/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.7.4/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files 11% similar despite different names*

```diff
@@ -48,21 +48,23 @@
     the upstream is hourly, then each daily partition in the downstream asset will map to the 24
     hourly partitions in the upstream that occur on that day.
 
     Attributes:
         start_offset (int): If not 0, then the starts of the upstream windows are shifted by this
             offset relative to the starts of the downstream windows. For example, if start_offset=-1
             and end_offset=0, then the downstream partition "2022-07-04" would map to the upstream
-            partitions "2022-07-03" and "2022-07-04". Only permitted to be non-zero when the
-            upstream and downstream PartitionsDefinitions are the same. Defaults to 0.
+            partitions "2022-07-03" and "2022-07-04". If the upstream and downstream
+            PartitionsDefinitions are different, then the offset is in the units of the downstream.
+            Defaults to 0.
         end_offset (int): If not 0, then the ends of the upstream windows are shifted by this
             offset relative to the ends of the downstream windows. For example, if start_offset=0
             and end_offset=1, then the downstream partition "2022-07-04" would map to the upstream
-            partitions "2022-07-04" and "2022-07-05". Only permitted to be non-zero when the
-            upstream and downstream PartitionsDefinitions are the same. Defaults to 0.
+            partitions "2022-07-04" and "2022-07-05". If the upstream and downstream
+            PartitionsDefinitions are different, then the offset is in the units of the downstream.
+            Defaults to 0.
         allow_nonexistent_upstream_partitions (bool): Defaults to false. If true, does not
             raise an error when mapped upstream partitions fall outside the start-end time window of the
             partitions def. For example, if the upstream partitions def starts on "2023-01-01" but
             the downstream starts on "2022-01-01", setting this bool to true would return no
             partition keys when get_upstream_partitions_for_partitions is called with "2022-06-01".
             When set to false, would raise an error.
 
@@ -133,14 +135,15 @@
         return self._map_partitions(
             downstream_partitions_subset.partitions_def,
             upstream_partitions_def,
             downstream_partitions_subset,
             start_offset=self.start_offset,
             end_offset=self.end_offset,
             current_time=current_time,
+            mapping_downstream_to_upstream=True,
         )
 
     def get_downstream_partitions_for_partitions(
         self,
         upstream_partitions_subset: PartitionsSubset,
         upstream_partitions_def: PartitionsDefinition,
         downstream_partitions_def: Optional[PartitionsDefinition],
@@ -155,14 +158,15 @@
         return self._map_partitions(
             upstream_partitions_def,
             downstream_partitions_def,
             upstream_partitions_subset,
             end_offset=-self.start_offset,
             start_offset=-self.end_offset,
             current_time=current_time,
+            mapping_downstream_to_upstream=False,
         ).partitions_subset
 
     def _merge_time_windows(self, time_windows: Sequence[TimeWindow]) -> Sequence[TimeWindow]:
         """Takes a list of potentially-overlapping TimeWindows and merges any overlapping windows."""
         if not time_windows:
             return []
 
@@ -185,43 +189,37 @@
         self,
         from_partitions_def: PartitionsDefinition,
         to_partitions_def: Optional[PartitionsDefinition],
         from_partitions_subset: PartitionsSubset,
         start_offset: int,
         end_offset: int,
         current_time: Optional[datetime],
+        mapping_downstream_to_upstream: bool,
     ) -> UpstreamPartitionsResult:
         """Maps the partitions in from_partitions_subset to partitions in to_partitions_def.
 
         If partitions in from_partitions_subset represent time windows that do not exist in
         to_partitions_def, raises an error if raise_error_on_invalid_mapped_partition is True.
         Otherwise, filters out the partitions that do not exist in to_partitions_def and returns
         the filtered subset, also returning a bool indicating whether there were mapped time windows
         that did not exist in to_partitions_def.
+
+        Args:
+            mapping_downstream_to_upstream (bool): True if from_partitions_def is the downstream
+                partitions def and to_partitions_def is the upstream partitions def.
         """
         if not isinstance(from_partitions_subset, BaseTimeWindowPartitionsSubset):
             check.failed("from_partitions_subset must be a BaseTimeWindowPartitionsSubset")
 
         if not isinstance(from_partitions_def, TimeWindowPartitionsDefinition):
             check.failed("from_partitions_def must be a TimeWindowPartitionsDefinition")
 
         if not isinstance(to_partitions_def, TimeWindowPartitionsDefinition):
             check.failed("to_partitions_def must be a TimeWindowPartitionsDefinition")
 
-        if (start_offset != 0 or end_offset != 0) and (
-            from_partitions_def.cron_schedule != to_partitions_def.cron_schedule
-        ):
-            raise DagsterInvalidDefinitionError(
-                "Can't use the start_offset or end_offset parameters of"
-                " TimeWindowPartitionMapping when the cron schedule of the upstream"
-                " PartitionsDefinition is different than the cron schedule of the downstream"
-                f" one. Attempted to map from cron schedule '{from_partitions_def.cron_schedule}' "
-                f"to cron schedule '{to_partitions_def.cron_schedule}'."
-            )
-
         if to_partitions_def.timezone != from_partitions_def.timezone:
             raise DagsterInvalidDefinitionError(
                 f"Timezones {to_partitions_def.timezone} and {from_partitions_def.timezone} don't match"
             )
 
         result = self._do_cheap_partition_mapping_if_possible(
             from_partitions_def=from_partitions_def,
@@ -232,74 +230,72 @@
             current_time=current_time,
         )
         if result is not None:
             return result
 
         first_window = to_partitions_def.get_first_partition_window(current_time=current_time)
         last_window = to_partitions_def.get_last_partition_window(current_time=current_time)
+        full_window = (
+            TimeWindow(first_window.start, last_window.end)
+            if first_window is not None and last_window is not None
+            else None
+        )
 
         time_windows = []
         for from_partition_time_window in from_partitions_subset.included_time_windows:
             from_start_dt, from_end_dt = from_partition_time_window
 
-            offsetted_start_dt = _offsetted_datetime(
-                from_partitions_def, from_start_dt, start_offset
-            )
-            offsetted_end_dt = _offsetted_datetime(from_partitions_def, from_end_dt, end_offset)
-
-            # Don't allow offsetting to push the windows out of the bounds of the target
-            # PartitionsDefinition
-            if first_window is not None and last_window is not None:
-                if start_offset < 0:
-                    offsetted_start_dt = max(
-                        first_window.start, offsetted_start_dt, key=lambda d: d.timestamp()
-                    )
-
-                if end_offset < 0:
-                    offsetted_end_dt = max(
-                        first_window.start, offsetted_end_dt, key=lambda d: d.timestamp()
-                    )
-
-                if start_offset > 0:
-                    offsetted_start_dt = min(
-                        last_window.end, offsetted_start_dt, key=lambda d: d.timestamp()
-                    )
-
-                if end_offset > 0:
-                    offsetted_end_dt = min(
-                        last_window.end, offsetted_end_dt, key=lambda d: d.timestamp()
-                    )
+            if mapping_downstream_to_upstream:
+                offsetted_from_start_dt = _offsetted_datetime_with_bounds(
+                    from_partitions_def, from_start_dt, start_offset, full_window
+                )
+                offsetted_from_end_dt = _offsetted_datetime_with_bounds(
+                    from_partitions_def, from_end_dt, end_offset, full_window
+                )
+            else:
+                # we'll apply the offsets later, after we've found the corresponding windows
+                offsetted_from_start_dt = from_start_dt
+                offsetted_from_end_dt = from_end_dt
 
             # Align the windows to partition boundaries in the target PartitionsDefinition
             if (from_partitions_def.cron_schedule == to_partitions_def.cron_schedule) or (
                 from_partitions_def.is_basic_daily and to_partitions_def.is_basic_hourly
             ):
                 # If the above conditions hold true, then we're confident that the partition
                 # boundaries in the PartitionsDefinition that we're mapping from match up with
                 # boundaries in the PartitionsDefinition that we're mapping to. That means
                 # we can just use these boundaries directly instead of finding nearby boundaries.
-                window_start = offsetted_start_dt
-                window_end = offsetted_end_dt
+                to_start_dt = offsetted_from_start_dt
+                to_end_dt = offsetted_from_end_dt
             else:
                 # The partition boundaries that we're mapping from might land in the middle of
                 # partitions that we're mapping to, so find those partitions.
                 to_start_partition_key = to_partitions_def.get_partition_key_for_timestamp(
-                    offsetted_start_dt.timestamp(), end_closed=False
+                    offsetted_from_start_dt.timestamp(), end_closed=False
                 )
                 to_end_partition_key = to_partitions_def.get_partition_key_for_timestamp(
-                    offsetted_end_dt.timestamp(), end_closed=True
+                    offsetted_from_end_dt.timestamp(), end_closed=True
                 )
 
-                window_start = to_partitions_def.start_time_for_partition_key(
-                    to_start_partition_key
+                to_start_dt = to_partitions_def.start_time_for_partition_key(to_start_partition_key)
+                to_end_dt = to_partitions_def.end_time_for_partition_key(to_end_partition_key)
+
+            if mapping_downstream_to_upstream:
+                offsetted_to_start_dt = to_start_dt
+                offsetted_to_end_dt = to_end_dt
+            else:
+                offsetted_to_start_dt = _offsetted_datetime_with_bounds(
+                    to_partitions_def, to_start_dt, start_offset, full_window
+                )
+                offsetted_to_end_dt = _offsetted_datetime_with_bounds(
+                    to_partitions_def, to_end_dt, end_offset, full_window
                 )
-                window_end = to_partitions_def.end_time_for_partition_key(to_end_partition_key)
 
-            if window_start.timestamp() < window_end.timestamp():
-                time_windows.append(TimeWindow(window_start, window_end))
+            if offsetted_to_start_dt.timestamp() < offsetted_to_end_dt.timestamp():
+                time_windows.append(TimeWindow(offsetted_to_start_dt, offsetted_to_end_dt))
 
         filtered_time_windows = []
         required_but_nonexistent_partition_keys = set()
 
         for time_window in time_windows:
             if (
                 first_window
@@ -442,14 +438,34 @@
             return UpstreamPartitionsResult(
                 to_partitions_def.empty_subset(), required_but_nonexistent_partition_keys
             )
 
         return None
 
 
+def _offsetted_datetime_with_bounds(
+    partitions_def: TimeWindowPartitionsDefinition,
+    dt: datetime,
+    offset: int,
+    bounds_window: Optional[TimeWindow],
+) -> datetime:
+    offsetted_dt = _offsetted_datetime(partitions_def, dt, offset)
+
+    # Don't allow offsetting to push the windows out of the bounds of the target
+    # PartitionsDefinition
+    if bounds_window is not None:
+        if offset < 0:
+            offsetted_dt = max(bounds_window.start, offsetted_dt, key=lambda d: d.timestamp())
+
+        if offset > 0:
+            offsetted_dt = min(bounds_window.end, offsetted_dt, key=lambda d: d.timestamp())
+
+    return offsetted_dt
+
+
 def _offsetted_datetime(
     partitions_def: TimeWindowPartitionsDefinition, dt: datetime, offset: int
 ) -> datetime:
     if partitions_def.is_basic_daily and offset != 0:
         result = dt + timedelta(days=offset)
         # Handle DST transitions
         if result.hour == 23:
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.7.4/dagster/_core/definitions/time_window_partitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,16 +482,18 @@
                 f" {self.end_offset} partition{'' if self.end_offset == 1 else 's'}."
             )
         return partition_def_str
 
     def __repr__(self):
         # Between python 3.8 and 3.9 the repr of a datetime object changed.
         # Replaces start time with timestamp as a workaround to make sure the repr is consistent across versions.
+        # Make sure to update this __repr__ if any new fields are added to TimeWindowPartitionsDefinition.
         return (
             f"TimeWindowPartitionsDefinition(start={self.start.timestamp()},"
+            f" end={self.end.timestamp() if self.end else None},"
             f" timezone='{self.timezone}', fmt='{self.fmt}', end_offset={self.end_offset},"
             f" cron_schedule='{self.cron_schedule}')"
         )
 
     def __hash__(self):
         return hash(tuple(self.__repr__()))
 
@@ -724,16 +726,17 @@
 
     def end_time_for_partition_key(self, partition_key: str) -> datetime:
         return self.time_window_for_partition_key(partition_key).end
 
     @functools.lru_cache(maxsize=5)
     def get_partition_keys_in_time_window(self, time_window: TimeWindow) -> Sequence[str]:
         result: List[str] = []
+        time_window_end_timestamp = time_window.end.timestamp()
         for partition_time_window in self._iterate_time_windows(time_window.start):
-            if partition_time_window.start.timestamp() < time_window.end.timestamp():
+            if partition_time_window.start.timestamp() < time_window_end_timestamp:
                 result.append(
                     dst_safe_strftime(
                         partition_time_window.start, self.timezone, self.fmt, self.cron_schedule
                     )
                 )
             else:
                 break
```

### Comparing `dagster-1.7.3/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.7.4/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/utils.py` & `dagster-1.7.4/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/definitions/version_strategy.py` & `dagster-1.7.4/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/errors.py` & `dagster-1.7.4/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/event_api.py` & `dagster-1.7.4/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/events/__init__.py` & `dagster-1.7.4/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/events/log.py` & `dagster-1.7.4/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/events/utils.py` & `dagster-1.7.4/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/api.py` & `dagster-1.7.4/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/asset_backfill.py` & `dagster-1.7.4/dagster/_core/execution/asset_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/backfill.py` & `dagster-1.7.4/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/build_resources.py` & `dagster-1.7.4/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/compute_logs.py` & `dagster-1.7.4/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/context/compute.py` & `dagster-1.7.4/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/context/hook.py` & `dagster-1.7.4/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/context/init.py` & `dagster-1.7.4/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/context/input.py` & `dagster-1.7.4/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/context/invocation.py` & `dagster-1.7.4/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/context/logger.py` & `dagster-1.7.4/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/context/output.py` & `dagster-1.7.4/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/context/system.py` & `dagster-1.7.4/dagster/_core/execution/context/system.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,42 @@
 """This module contains the execution context objects that are internal to the system.
 Not every property on these should be exposed to random Jane or Joe dagster user
 so we have a different layer of objects that encode the explicit public API
 in the user_context module.
 """
 
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
-from hashlib import sha256
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Dict,
     Iterable,
     List,
     Mapping,
     NamedTuple,
     Optional,
-    Sequence,
     Set,
     Union,
     cast,
 )
 
 import dagster._check as check
 from dagster._annotations import public
-from dagster._core.definitions.data_version import (
-    DATA_VERSION_TAG,
-    SKIP_PARTITION_DATA_VERSION_DEPENDENCY_THRESHOLD,
-    extract_data_version_from_entry,
-)
 from dagster._core.definitions.dependency import OpNode
 from dagster._core.definitions.events import AssetKey, AssetLineageInfo
 from dagster._core.definitions.hook_definition import HookDefinition
 from dagster._core.definitions.job_base import IJob
 from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.metadata import RawMetadataValue
 from dagster._core.definitions.multi_dimensional_partitions import MultiPartitionsDefinition
 from dagster._core.definitions.op_definition import OpDefinition
 from dagster._core.definitions.partition import PartitionsDefinition, PartitionsSubset
 from dagster._core.definitions.partition_key_range import PartitionKeyRange
 from dagster._core.definitions.partition_mapping import (
-    PartitionMapping,
     infer_partition_mapping,
 )
 from dagster._core.definitions.policy import RetryPolicy
 from dagster._core.definitions.reconstruct import ReconstructableJob
 from dagster._core.definitions.repository_definition.repository_definition import (
     RepositoryDefinition,
 )
@@ -70,25 +61,24 @@
     ASSET_PARTITION_RANGE_START_TAG,
     MULTIDIMENSIONAL_PARTITION_PREFIX,
     PARTITION_NAME_TAG,
 )
 from dagster._core.system_config.objects import ResolvedRunConfig
 from dagster._core.types.dagster_type import DagsterType
 
+from .data_version_cache import DataVersionCache, InputAssetVersionInfo
 from .input import InputContext
 from .output import OutputContext, get_output_context
 
 if TYPE_CHECKING:
     from dagster._core.definitions.data_version import (
         DataVersion,
     )
     from dagster._core.definitions.dependency import NodeHandle
     from dagster._core.definitions.resource_definition import Resources
-    from dagster._core.event_api import EventLogRecord
-    from dagster._core.events import DagsterEventType
     from dagster._core.execution.plan.plan import ExecutionPlan
     from dagster._core.execution.plan.state import KnownExecutionState
     from dagster._core.instance import DagsterInstance
 
     from .hook import HookContext
 
 
@@ -334,14 +324,18 @@
         return self._output_capture
 
     def for_step(
         self,
         step: ExecutionStep,
         known_state: Optional["KnownExecutionState"] = None,
     ) -> IStepContext:
+        # TODO: refactoring to build up reasonable layer of prefetching -- 2024-04-27 schrockn
+        # if is_step_in_asset_graph_layer(step, self.job_def):
+        # ... prefetch input asset version info
+
         return StepExecutionContext(
             plan_data=self.plan_data,
             execution_data=self._execution_data,
             log_manager=self._log_manager.with_tags(**step.logging_tags),
             step=step,
             output_capture=self.output_capture,
             known_state=known_state,
@@ -500,33 +494,21 @@
 
     def for_type(self, dagster_type: DagsterType) -> "TypeCheckContext":
         return TypeCheckContext(
             self.run_id, self.log, self._execution_data.scoped_resources_builder, dagster_type
         )
 
 
-@dataclass
-class InputAssetVersionInfo:
-    # This is the storage id of the last materialization/observation of any partition of an asset.
-    # Thus it is computed the same way for both partitioned and non-partitioned assets.
-    storage_id: int
-
-    # This is the event type of the event referenced by storage_id
-    event_type: "DagsterEventType"
-
-    # If the input asset is partitioned, this is a hash of the sorted data versions of each dependency
-    # partition. If the input asset is not partitioned, this is the data version of the asset. It
-    # can be none if we are sourcing a materialization from before data versions.
-    data_version: Optional["DataVersion"]
-
-    # This is the run_id on the event that the storage_id references
-    run_id: str
-
-    # This is the timestamp on the event that the storage_id references
-    timestamp: float
+def is_step_in_asset_graph_layer(step: ExecutionStep, job_def: JobDefinition) -> bool:
+    """Whether this step is aware of the asset graph definition layer inferred by presence of asset info on outputs."""
+    for output in step.step_outputs:
+        asset_info = job_def.asset_layer.asset_info_for_output(step.node_handle, output.name)
+        if asset_info is not None:
+            return True
+    return False
 
 
 class StepExecutionContext(PlanExecutionContext, IStepContext):
     """Context for the execution of a step. Users should not instantiate this class directly.
 
     This context assumes that user code can be run directly, and thus includes resource and information.
     """
@@ -585,17 +567,15 @@
         if self.job_def.get_all_hooks_for_handle(self.node_handle):
             self._step_output_capture = {}
             self._step_output_metadata_capture = {}
 
         self._output_metadata: Dict[str, Any] = {}
         self._seen_outputs: Dict[str, Union[str, Set[str]]] = {}
 
-        self._input_asset_version_info: Dict[AssetKey, Optional["InputAssetVersionInfo"]] = {}
-        self._is_external_input_asset_version_info_loaded = False
-        self._data_version_cache: Dict[AssetKey, "DataVersion"] = {}
+        self._data_version_cache = DataVersionCache(self)
 
         self._requires_typed_event_stream = False
         self._typed_event_stream_error_message = None
 
     # In this mode no conversion is done on returned values and missing but expected outputs are not
     # allowed.
     @property
@@ -940,21 +920,15 @@
 
     @property
     def is_sda_step(self) -> bool:
         """Whether this step corresponds to a software define asset, inferred by presence of asset info on outputs.
 
         note: ops can materialize assets as well.
         """
-        for output in self.step.step_outputs:
-            asset_info = self.job_def.asset_layer.asset_info_for_output(
-                self.node_handle, output.name
-            )
-            if asset_info is not None:
-                return True
-        return False
+        return is_step_in_asset_graph_layer(self.step, self.job_def)
 
     @property
     def is_in_graph_asset(self) -> bool:
         """If the step is an op in a graph-backed asset returns True. Checks by first confirming the
         step is in a graph, then checking that the node corresponds to an AssetsDefinitions in the asset layer.
         """
         return (
@@ -968,159 +942,45 @@
         """Whether this step corresponds to at least one asset check."""
         return any(
             self.job_def.asset_layer.asset_check_key_for_output(self.node_handle, output.name)
             for output in self.step.step_outputs
         )
 
     def set_data_version(self, asset_key: AssetKey, data_version: "DataVersion") -> None:
-        self._data_version_cache[asset_key] = data_version
+        return self._data_version_cache.set_data_version(asset_key, data_version)
 
     def has_data_version(self, asset_key: AssetKey) -> bool:
-        return asset_key in self._data_version_cache
+        return self._data_version_cache.has_data_version(asset_key)
 
     def get_data_version(self, asset_key: AssetKey) -> "DataVersion":
-        return self._data_version_cache[asset_key]
+        return self._data_version_cache.get_data_version(asset_key)
 
     @property
     def input_asset_records(self) -> Optional[Mapping[AssetKey, Optional["InputAssetVersionInfo"]]]:
-        return self._input_asset_version_info
+        return self._data_version_cache.input_asset_version_info
 
     @property
     def is_external_input_asset_version_info_loaded(self) -> bool:
-        return self._is_external_input_asset_version_info_loaded
+        return self._data_version_cache.is_external_input_asset_version_info_loaded
 
-    def get_input_asset_version_info(self, key: AssetKey) -> Optional["InputAssetVersionInfo"]:
-        if key not in self._input_asset_version_info:
-            self._fetch_input_asset_version_info(key)
-        return self._input_asset_version_info[key]
+    def maybe_fetch_and_get_input_asset_version_info(
+        self, key: AssetKey
+    ) -> Optional["InputAssetVersionInfo"]:
+        return self._data_version_cache.maybe_fetch_and_get_input_asset_version_info(key)
 
     # "external" refers to records for inputs generated outside of this step
     def fetch_external_input_asset_version_info(self) -> None:
-        output_keys = self.get_output_asset_keys()
-
-        all_dep_keys: List[AssetKey] = []
-        for output_key in output_keys:
-            if output_key not in self.job_def.asset_layer.asset_deps:
-                continue
-            dep_keys = self.job_def.asset_layer.get(output_key).parent_keys
-            for key in dep_keys:
-                if key not in all_dep_keys and key not in output_keys:
-                    all_dep_keys.append(key)
-
-        self._input_asset_version_info = {}
-        for key in all_dep_keys:
-            self._fetch_input_asset_version_info(key)
-        self._is_external_input_asset_version_info_loaded = True
-
-    def _fetch_input_asset_version_info(self, key: AssetKey) -> None:
-        from dagster._core.definitions.data_version import (
-            extract_data_version_from_entry,
-        )
-
-        event = self._get_input_asset_event(key)
-        if event is None:
-            self._input_asset_version_info[key] = None
-        else:
-            storage_id = event.storage_id
-            # Input name will be none if this is an internal dep
-            input_name = self.job_def.asset_layer.input_for_asset_key(self.node_handle, key)
-            # Exclude AllPartitionMapping for now to avoid huge queries
-            if input_name and self.has_asset_partitions_for_input(input_name):
-                subset = self.asset_partitions_subset_for_input(
-                    input_name, require_valid_partitions=False
-                )
-                input_keys = list(subset.get_partition_keys())
-
-                # This check represents a temporary constraint that prevents huge query results for upstream
-                # partition data versions from timing out runs. If a partitioned dependency (a) uses an
-                # AllPartitionMapping; and (b) has greater than or equal to
-                # SKIP_PARTITION_DATA_VERSION_DEPENDENCY_THRESHOLD dependency partitions, then we
-                # process it as a non-partitioned dependency (note that this was the behavior for
-                # all partition dependencies prior to 2023-08).  This means that stale status
-                # results cannot be accurately computed for the dependency, and there is thus
-                # corresponding logic in the CachingStaleStatusResolver to account for this. This
-                # constraint should be removed when we have thoroughly examined the performance of
-                # the data version retrieval query and can guarantee decent performance.
-                if len(input_keys) < SKIP_PARTITION_DATA_VERSION_DEPENDENCY_THRESHOLD:
-                    data_version = self._get_partitions_data_version_from_keys(key, input_keys)
-                else:
-                    data_version = extract_data_version_from_entry(event.event_log_entry)
-            else:
-                data_version = extract_data_version_from_entry(event.event_log_entry)
-            self._input_asset_version_info[key] = InputAssetVersionInfo(
-                storage_id,
-                check.not_none(event.event_log_entry.dagster_event).event_type,
-                data_version,
-                event.run_id,
-                event.timestamp,
-            )
-
-    def partition_mapping_for_input(self, input_name: str) -> Optional[PartitionMapping]:
-        asset_layer = self.job_def.asset_layer
-        upstream_asset_key = asset_layer.asset_key_for_input(self.node_handle, input_name)
-        if upstream_asset_key:
-            upstream_asset_partitions_def = asset_layer.get(upstream_asset_key).partitions_def
-            assets_def = asset_layer.assets_def_for_node(self.node_handle)
-            partitions_def = assets_def.partitions_def if assets_def else None
-            explicit_partition_mapping = self.job_def.asset_layer.partition_mapping_for_node_input(
-                self.node_handle, upstream_asset_key
-            )
-            return infer_partition_mapping(
-                explicit_partition_mapping,
-                partitions_def,
-                upstream_asset_partitions_def,
-            )
-        else:
-            return None
-
-    def _get_input_asset_event(self, key: AssetKey) -> Optional["EventLogRecord"]:
-        event = self.instance.get_latest_data_version_record(key)
-        if event:
-            self._check_input_asset_event(key, event)
-        return event
-
-    def _check_input_asset_event(self, key: AssetKey, event: "EventLogRecord") -> None:
-        assert event.event_log_entry
-        event_data_version = extract_data_version_from_entry(event.event_log_entry)
-        if key in self._data_version_cache and self._data_version_cache[key] != event_data_version:
-            self.log.warning(
-                f"Data version mismatch for asset {key}. Data version from materialization within"
-                f" current step is `{self._data_version_cache[key]}`. Data version from most recent"
-                f" materialization is `{event_data_version}`. Most recent materialization will be"
-                " used for provenance tracking."
-            )
-
-    def _get_partitions_data_version_from_keys(
-        self, key: AssetKey, partition_keys: Sequence[str]
-    ) -> "DataVersion":
-        from dagster._core.definitions.data_version import (
-            DataVersion,
-        )
-        from dagster._core.events import DagsterEventType
-
-        # TODO: this needs to account for observations also
-        event_type = DagsterEventType.ASSET_MATERIALIZATION
-        tags_by_partition = self.instance._event_storage.get_latest_tags_by_partition(  # noqa: SLF001
-            key, event_type, [DATA_VERSION_TAG], asset_partitions=list(partition_keys)
-        )
-        partition_data_versions = [
-            pair[1][DATA_VERSION_TAG]
-            for pair in sorted(tags_by_partition.items(), key=lambda x: x[0])
-        ]
-        hash_sig = sha256()
-        hash_sig.update(bytearray("".join(partition_data_versions), "utf8"))
-        return DataVersion(hash_sig.hexdigest())
+        return self._data_version_cache.fetch_external_input_asset_version_info()
 
     # Call this to clear the cache for an input asset record. This is necessary when an old
     # materialization for an asset was loaded during `fetch_external_input_asset_records` because an
     # intrastep asset is not required, but then that asset is materialized during the step. If we
     # don't clear the cache for this asset, then we won't use the most up-to-date asset record.
     def wipe_input_asset_version_info(self, key: AssetKey) -> None:
-        if key in self._input_asset_version_info:
-            del self._input_asset_version_info[key]
+        return self._data_version_cache.wipe_input_asset_version_info(key)
 
     def get_output_asset_keys(self) -> AbstractSet[AssetKey]:
         output_keys: Set[AssetKey] = set()
         for step_output in self.step.step_outputs:
             asset_info = self.job_def.asset_layer.asset_info_for_output(
                 self.node_handle, step_output.name
             )
```

### Comparing `dagster-1.7.3/dagster/_core/execution/context_creation_job.py` & `dagster-1.7.4/dagster/_core/execution/context_creation_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/execute_in_process.py` & `dagster-1.7.4/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.7.4/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/execution_result.py` & `dagster-1.7.4/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/host_mode.py` & `dagster-1.7.4/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/job_backfill.py` & `dagster-1.7.4/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/job_execution_result.py` & `dagster-1.7.4/dagster/_core/execution/job_execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/memoization.py` & `dagster-1.7.4/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/active.py` & `dagster-1.7.4/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/compute.py` & `dagster-1.7.4/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.7.4/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.7.4/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/execute_step.py` & `dagster-1.7.4/dagster/_core/execution/plan/execute_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -709,15 +709,15 @@
     deps = step_context.job_def.asset_layer.get(asset_key).parent_keys
     for key in deps:
         # For deps external to this step, this will retrieve the cached record that was stored prior
         # to step execution. For inputs internal to this step, it may trigger a query to retrieve
         # the most recent materialization record (it will retrieve a cached record if it's already
         # been asked for). For this to be correct, the output materializations for the step must be
         # generated in topological order -- we assume this.
-        version_info = step_context.get_input_asset_version_info(key)
+        version_info = step_context.maybe_fetch_and_get_input_asset_version_info(key)
 
         # This can only happen for source assets that have never been observed.
         if version_info is None:
             storage_id = None
             data_version = DEFAULT_DATA_VERSION
         else:
             storage_id = version_info.storage_id
```

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/external_step.py` & `dagster-1.7.4/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/handle.py` & `dagster-1.7.4/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/inputs.py` & `dagster-1.7.4/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/instance_concurrency_context.py` & `dagster-1.7.4/dagster/_core/execution/plan/instance_concurrency_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.7.4/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/objects.py` & `dagster-1.7.4/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/outputs.py` & `dagster-1.7.4/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/plan.py` & `dagster-1.7.4/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/state.py` & `dagster-1.7.4/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/step.py` & `dagster-1.7.4/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/plan/utils.py` & `dagster-1.7.4/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.7.4/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/resolve_versions.py` & `dagster-1.7.4/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/resources_init.py` & `dagster-1.7.4/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/retries.py` & `dagster-1.7.4/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.7.4/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/stats.py` & `dagster-1.7.4/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/submit_asset_runs.py` & `dagster-1.7.4/dagster/_core/execution/submit_asset_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/tags.py` & `dagster-1.7.4/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/validate_run_config.py` & `dagster-1.7.4/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/watch_orphans.py` & `dagster-1.7.4/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/execution/with_resources.py` & `dagster-1.7.4/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/executor/base.py` & `dagster-1.7.4/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/executor/child_process_executor.py` & `dagster-1.7.4/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/executor/in_process.py` & `dagster-1.7.4/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/executor/init.py` & `dagster-1.7.4/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/executor/multiprocess.py` & `dagster-1.7.4/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.7.4/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.7.4/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/instance/__init__.py` & `dagster-1.7.4/dagster/_core/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/instance/config.py` & `dagster-1.7.4/dagster/_core/instance/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/instance/ref.py` & `dagster-1.7.4/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/instance_for_test.py` & `dagster-1.7.4/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/launcher/base.py` & `dagster-1.7.4/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.7.4/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.7.4/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/log_manager.py` & `dagster-1.7.4/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/nux.py` & `dagster-1.7.4/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/op_concurrency_limits_counter.py` & `dagster-1.7.4/dagster/_core/op_concurrency_limits_counter.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/origin.py` & `dagster-1.7.4/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/pipes/client.py` & `dagster-1.7.4/dagster/_core/pipes/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/pipes/context.py` & `dagster-1.7.4/dagster/_core/pipes/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/pipes/subprocess.py` & `dagster-1.7.4/dagster/_core/pipes/subprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/pipes/utils.py` & `dagster-1.7.4/dagster/_core/pipes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/remote_representation/__init__.py` & `dagster-1.7.4/dagster/_core/remote_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/remote_representation/code_location.py` & `dagster-1.7.4/dagster/_core/remote_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/remote_representation/external.py` & `dagster-1.7.4/dagster/_core/remote_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/remote_representation/external_data.py` & `dagster-1.7.4/dagster/_core/remote_representation/external_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/remote_representation/feature_flags.py` & `dagster-1.7.4/dagster/_core/remote_representation/feature_flags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/remote_representation/grpc_server_registry.py` & `dagster-1.7.4/dagster/_core/remote_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/remote_representation/grpc_server_state_subscriber.py` & `dagster-1.7.4/dagster/_core/remote_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/remote_representation/handle.py` & `dagster-1.7.4/dagster/_core/remote_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/remote_representation/historical.py` & `dagster-1.7.4/dagster/_core/remote_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/remote_representation/job_index.py` & `dagster-1.7.4/dagster/_core/remote_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/remote_representation/origin.py` & `dagster-1.7.4/dagster/_core/remote_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/remote_representation/represented.py` & `dagster-1.7.4/dagster/_core/remote_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/run_coordinator/base.py` & `dagster-1.7.4/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.7.4/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.7.4/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/scheduler/__init__.py` & `dagster-1.7.4/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/scheduler/execution.py` & `dagster-1.7.4/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/scheduler/instigation.py` & `dagster-1.7.4/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/scheduler/scheduler.py` & `dagster-1.7.4/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/secrets/env_file.py` & `dagster-1.7.4/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/selector/subset_selector.py` & `dagster-1.7.4/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/snap/__init__.py` & `dagster-1.7.4/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/snap/dagster_types.py` & `dagster-1.7.4/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/snap/dep_snapshot.py` & `dagster-1.7.4/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.7.4/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/snap/job_snapshot.py` & `dagster-1.7.4/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/snap/mode.py` & `dagster-1.7.4/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/snap/node.py` & `dagster-1.7.4/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.7.4/dagster/_core/snap/snap_to_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/DEVELOPING.md` & `dagster-1.7.4/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/README.md` & `dagster-1.7.4/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/env.py` & `dagster-1.7.4/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py` & `dagster-1.7.4/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/asset_check_execution_record.py` & `dagster-1.7.4/dagster/_core/storage/asset_check_execution_record.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/asset_value_loader.py` & `dagster-1.7.4/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/base_storage.py` & `dagster-1.7.4/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.7.4/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/captured_log_manager.py` & `dagster-1.7.4/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.7.4/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/compute_log_manager.py` & `dagster-1.7.4/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/config.py` & `dagster-1.7.4/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/dagster_run.py` & `dagster-1.7.4/dagster/_core/storage/dagster_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/db_io_manager.py` & `dagster-1.7.4/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/event_log/__init__.py` & `dagster-1.7.4/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/event_log/base.py` & `dagster-1.7.4/dagster/_core/storage/event_log/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.7.4/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/event_log/migration.py` & `dagster-1.7.4/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.7.4/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/event_log/schema.py` & `dagster-1.7.4/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.7.4/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.7.4/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.7.4/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.7.4/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/file_manager.py` & `dagster-1.7.4/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/fs_io_manager.py` & `dagster-1.7.4/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/input_manager.py` & `dagster-1.7.4/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/io_manager.py` & `dagster-1.7.4/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/legacy_storage.py` & `dagster-1.7.4/dagster/_core/storage/legacy_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.7.4/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/mem_io_manager.py` & `dagster-1.7.4/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.7.4/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/migration/bigint_migration.py` & `dagster-1.7.4/dagster/_core/storage/migration/bigint_migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/migration/utils.py` & `dagster-1.7.4/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.7.4/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/output_manager.py` & `dagster-1.7.4/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/partition_status_cache.py` & `dagster-1.7.4/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/root.py` & `dagster-1.7.4/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/runs/base.py` & `dagster-1.7.4/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/runs/in_memory.py` & `dagster-1.7.4/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/runs/migration.py` & `dagster-1.7.4/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/runs/schema.py` & `dagster-1.7.4/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.7.4/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.7.4/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.7.4/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/schedules/base.py` & `dagster-1.7.4/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/schedules/migration.py` & `dagster-1.7.4/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/schedules/schema.py` & `dagster-1.7.4/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.7.4/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.7.4/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.7.4/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/sql.py` & `dagster-1.7.4/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/sqlalchemy_compat.py` & `dagster-1.7.4/dagster/_core/storage/sqlalchemy_compat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/sqlite.py` & `dagster-1.7.4/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/sqlite_storage.py` & `dagster-1.7.4/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/tags.py` & `dagster-1.7.4/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/temp_file_manager.py` & `dagster-1.7.4/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/storage/upath_io_manager.py` & `dagster-1.7.4/dagster/_core/storage/upath_io_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,16 +269,14 @@
 
     def _load_single_input(self, path: "UPath", context: InputContext) -> Any:
         context.log.debug(self.get_loading_input_log_message(path))
         obj = self.load_from_path(context=context, path=path)
         if asyncio.iscoroutine(obj):
             obj = asyncio.run(obj)
 
-        context.add_input_metadata({"path": MetadataValue.path(str(path))})
-
         return obj
 
     def _load_partition_from_path(
         self,
         context: InputContext,
         partition_key: str,
         path: "UPath",
```

### Comparing `dagster-1.7.3/dagster/_core/system_config/composite_descent.py` & `dagster-1.7.4/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/system_config/objects.py` & `dagster-1.7.4/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/telemetry.py` & `dagster-1.7.4/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/telemetry_upload.py` & `dagster-1.7.4/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/test_utils.py` & `dagster-1.7.4/dagster/_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.7.4/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/types/config_schema.py` & `dagster-1.7.4/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/types/dagster_type.py` & `dagster-1.7.4/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/types/decorator.py` & `dagster-1.7.4/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/types/loadable_target_origin.py` & `dagster-1.7.4/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/types/primitive_mapping.py` & `dagster-1.7.4/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/types/python_dict.py` & `dagster-1.7.4/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/types/python_set.py` & `dagster-1.7.4/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/types/python_tuple.py` & `dagster-1.7.4/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/types/transform_typing.py` & `dagster-1.7.4/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/utility_ops.py` & `dagster-1.7.4/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/utils.py` & `dagster-1.7.4/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/workspace/autodiscovery.py` & `dagster-1.7.4/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/workspace/batch_asset_record_loader.py` & `dagster-1.7.4/dagster/_core/workspace/batch_asset_record_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/workspace/config_schema.py` & `dagster-1.7.4/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/workspace/context.py` & `dagster-1.7.4/dagster/_core/workspace/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/workspace/load.py` & `dagster-1.7.4/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/workspace/load_target.py` & `dagster-1.7.4/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/workspace/permissions.py` & `dagster-1.7.4/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_core/workspace/workspace.py` & `dagster-1.7.4/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_daemon/__init__.py` & `dagster-1.7.4/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_daemon/asset_daemon.py` & `dagster-1.7.4/dagster/_daemon/asset_daemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,20 +411,28 @@
                         thread_name_prefix="asset_daemon_worker",
                     )
                 )
 
             while True:
                 start_time = pendulum.now("UTC").timestamp()
                 yield SpanMarker.START_SPAN
-                yield from self._run_iteration_impl(
-                    workspace_process_context,
-                    threadpool_executor=threadpool_executor,
-                    amp_tick_futures=amp_tick_futures,
-                    debug_crash_flags={},
-                )
+                try:
+                    yield from self._run_iteration_impl(
+                        workspace_process_context,
+                        threadpool_executor=threadpool_executor,
+                        amp_tick_futures=amp_tick_futures,
+                        debug_crash_flags={},
+                    )
+                except Exception:
+                    error_info = DaemonErrorCapture.on_exception(
+                        exc_info=sys.exc_info(),
+                        logger=self._logger,
+                        log_message="AssetDaemon caught an error",
+                    )
+                    yield error_info
                 yield SpanMarker.END_SPAN
                 end_time = pendulum.now("UTC").timestamp()
                 loop_duration = end_time - start_time
                 sleep_time = max(0, MIN_INTERVAL_LOOP_SECONDS - loop_duration)
                 shutdown_event.wait(sleep_time)
                 yield None
```

### Comparing `dagster-1.7.3/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.7.4/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.7.4/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_daemon/backfill.py` & `dagster-1.7.4/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_daemon/cli/__init__.py` & `dagster-1.7.4/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_daemon/controller.py` & `dagster-1.7.4/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_daemon/daemon.py` & `dagster-1.7.4/dagster/_daemon/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 import sys
 import time
 import uuid
 from abc import ABC, abstractmethod
 from collections import deque
 from contextlib import AbstractContextManager, ExitStack
 from enum import Enum
@@ -23,14 +24,15 @@
 from dagster._daemon.backfill import execute_backfill_iteration
 from dagster._daemon.monitoring import (
     execute_concurrency_slots_iteration,
     execute_run_monitoring_iteration,
 )
 from dagster._daemon.sensor import execute_sensor_iteration_loop
 from dagster._daemon.types import DaemonHeartbeat
+from dagster._daemon.utils import DaemonErrorCapture
 from dagster._scheduler.scheduler import execute_scheduler_iteration_loop
 from dagster._utils.error import (
     SerializableErrorInfo,
     serializable_error_info_from_exc_info,
 )
 
 if TYPE_CHECKING:
@@ -42,14 +44,18 @@
 
 
 DAEMON_HEARTBEAT_ERROR_LIMIT = 5  # Show at most 5 errors
 TELEMETRY_LOGGING_INTERVAL = 3600 * 24  # Interval (in seconds) at which to log that daemon is alive
 _telemetry_daemon_session_id = str(uuid.uuid4())
 
 
+def _get_error_sleep_interval():
+    return int(os.getenv("DAGSTER_DAEMON_CORE_LOOP_EXCEPTION_SLEEP_INTERVAL", "5"))
+
+
 def get_telemetry_daemon_session_id() -> str:
     return _telemetry_daemon_session_id
 
 
 class SpanMarker(Enum):
     START_SPAN = "START_SPAN"
     END_SPAN = "END_SPAN"
@@ -120,20 +126,25 @@
                     except StopIteration:
                         self._logger.error(
                             "Daemon loop finished without raising an error - daemon loops should"
                             " run forever until they are interrupted."
                         )
                         break
                     except Exception:
-                        error_info = serializable_error_info_from_exc_info(sys.exc_info())
-                        self._logger.error(
-                            "Caught error, daemon loop will restart:\n%s", error_info
+                        error_info = DaemonErrorCapture.on_exception(
+                            exc_info=sys.exc_info(),
+                            logger=self._logger,
+                            log_message="Caught error, daemon loop will restart",
                         )
                         self._errors.appendleft((error_info, pendulum.now("UTC")))
                         daemon_generator.close()
+
+                        # Wait a bit to ensure that errors don't happen in a tight loop
+                        daemon_shutdown_event.wait(_get_error_sleep_interval())
+
                         daemon_generator = self.core_loop(
                             workspace_process_context, daemon_shutdown_event
                         )
             finally:
                 # cleanup the generator if it was stopped part-way through
                 daemon_generator.close()
```

### Comparing `dagster-1.7.3/dagster/_daemon/monitoring/concurrency.py` & `dagster-1.7.4/dagster/_daemon/monitoring/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_daemon/monitoring/run_monitoring.py` & `dagster-1.7.4/dagster/_daemon/monitoring/run_monitoring.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.7.4/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_daemon/sensor.py` & `dagster-1.7.4/dagster/_daemon/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,21 +261,30 @@
     while True:
         start_time = pendulum.now("UTC").timestamp()
         if until and start_time >= until:
             # provide a way of organically ending the loop to support test environment
             break
 
         yield SpanMarker.START_SPAN
-        yield from execute_sensor_iteration(
-            workspace_process_context,
-            logger,
-            threadpool_executor=threadpool_executor,
-            submit_threadpool_executor=submit_threadpool_executor,
-            sensor_tick_futures=sensor_tick_futures,
-        )
+
+        try:
+            yield from execute_sensor_iteration(
+                workspace_process_context,
+                logger,
+                threadpool_executor=threadpool_executor,
+                submit_threadpool_executor=submit_threadpool_executor,
+                sensor_tick_futures=sensor_tick_futures,
+            )
+        except Exception:
+            error_info = DaemonErrorCapture.on_exception(
+                exc_info=sys.exc_info(),
+                logger=logger,
+                log_message="SensorDaemon caught an error",
+            )
+            yield error_info
         # Yield to check for heartbeats in case there were no yields within
         # execute_sensor_iteration
         yield SpanMarker.END_SPAN
 
         end_time = pendulum.now("UTC").timestamp()
 
         loop_duration = end_time - start_time
```

### Comparing `dagster-1.7.3/dagster/_daemon/types.py` & `dagster-1.7.4/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_daemon/utils.py` & `dagster-1.7.4/dagster/_daemon/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_daemon/workspace.py` & `dagster-1.7.4/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_generate/download.py` & `dagster-1.7.4/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_generate/generate.py` & `dagster-1.7.4/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.7.4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.7.4/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_grpc/__generated__/api_pb2.pyi` & `dagster-1.7.4/dagster/_grpc/__generated__/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.7.4/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_grpc/__init__.py` & `dagster-1.7.4/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_grpc/client.py` & `dagster-1.7.4/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_grpc/compile.py` & `dagster-1.7.4/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_grpc/impl.py` & `dagster-1.7.4/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_grpc/protos/api.proto` & `dagster-1.7.4/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_grpc/proxy_server.py` & `dagster-1.7.4/dagster/_grpc/proxy_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_grpc/server.py` & `dagster-1.7.4/dagster/_grpc/server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_grpc/server_watcher.py` & `dagster-1.7.4/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_grpc/types.py` & `dagster-1.7.4/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_grpc/utils.py` & `dagster-1.7.4/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_loggers/__init__.py` & `dagster-1.7.4/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_model/__init__.py` & `dagster-1.7.4/dagster/_model/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from functools import cached_property
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Hashable, Optional
 
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, PrivateAttr
 from typing_extensions import Self
 
 from .pydantic_compat_layer import USING_PYDANTIC_2
 
 
 class DagsterModel(BaseModel):
     """Standardizes on Pydantic settings that are stricter than the default.
     - Frozen, to avoid complexity caused by mutation.
     - extra=forbid, to avoid bugs caused by accidentally constructing with the wrong arguments.
     - arbitrary_types_allowed, to allow non-model class params to be validated with isinstance.
     - Avoid pydantic reading a cached property class as part of the schema.
     """
 
+    _cached_method_cache__internal__: Dict[Hashable, Any] = PrivateAttr(default_factory=dict)
+
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     if USING_PYDANTIC_2:
         model_config = ConfigDict(  # type: ignore
             extra="forbid",
             frozen=True,
```

### Comparing `dagster-1.7.3/dagster/_model/pydantic_compat_layer.py` & `dagster-1.7.4/dagster/_model/pydantic_compat_layer.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,16 +37,27 @@
         return self.field.annotation
 
     @property
     def metadata(self) -> List[str]:
         return getattr(self.field, "metadata", [])
 
     @property
-    def alias(self) -> str:
-        return self.field.alias
+    def alias(self) -> Optional[str]:
+        if USING_PYDANTIC_2:
+            return self.field.alias
+        else:
+            return self.field.alias if self.field.alias != self.field.name else None
+
+    @property
+    def serialization_alias(self) -> Optional[str]:
+        return getattr(self.field, "serialization_alias", None)
+
+    @property
+    def validation_alias(self) -> Optional[str]:
+        return getattr(self.field, "validation_alias", None)
 
     @property
     def default(self) -> Any:
         return self.field.default
 
     @property
     def description(self) -> Optional[str]:
```

### Comparing `dagster-1.7.3/dagster/_module_alias_map.py` & `dagster-1.7.4/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_scheduler/scheduler.py` & `dagster-1.7.4/dagster/_scheduler/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 )
 from dagster._core.scheduler.scheduler import DEFAULT_MAX_CATCHUP_RUNS, DagsterSchedulerError
 from dagster._core.storage.dagster_run import DagsterRun, DagsterRunStatus, RunsFilter
 from dagster._core.storage.tags import RUN_KEY_TAG, SCHEDULED_EXECUTION_TIME_TAG
 from dagster._core.telemetry import SCHEDULED_RUN_CREATED, hash_name, log_action
 from dagster._core.utils import InheritContextThreadPoolExecutor
 from dagster._core.workspace.context import IWorkspaceProcessContext
+from dagster._daemon.utils import DaemonErrorCapture
 from dagster._scheduler.stale import resolve_stale_or_missing_assets
 from dagster._seven.compat.pendulum import to_timezone
 from dagster._utils import DebugCrashFlags, SingleInstigatorDebugCrashFlags, check_for_debug_crash
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 from dagster._utils.log import default_date_format_string
 from dagster._utils.merger import merge_dicts
 
@@ -71,14 +72,17 @@
     os.getenv("DAGSTER_SCHEDULE_CHECKPOINT_INTERVAL_SECONDS", "3600")
 )
 
 LAST_ITERATION_CHECKPOINT_JITTER_SECONDS = int(
     os.getenv("DAGSTER_SCHEDULE_CHECKPOINT_JITTER_SECONDS", "600")
 )
 
+# How long to wait if an error is raised in the SchedulerDaemon iteration
+ERROR_INTERVAL_TIME = 5
+
 
 class _ScheduleLaunchContext(AbstractContextManager):
     def __init__(
         self,
         external_schedule: ExternalSchedule,
         tick: InstigatorTick,
         instance: DagsterInstance,
@@ -216,35 +220,46 @@
                     )
                 )
 
         while True:
             start_time = pendulum.now("UTC").timestamp()
             end_datetime_utc = pendulum.now("UTC")
 
+            next_interval_time = _get_next_scheduler_iteration_time(start_time)
+
             yield SpanMarker.START_SPAN
-            yield from launch_scheduled_runs(
-                workspace_process_context,
-                logger,
-                end_datetime_utc=end_datetime_utc,
-                iteration_times=iteration_times,
-                threadpool_executor=threadpool_executor,
-                submit_threadpool_executor=submit_threadpool_executor,
-                scheduler_run_futures=scheduler_run_futures,
-                max_catchup_runs=max_catchup_runs,
-                max_tick_retries=max_tick_retries,
-            )
+            try:
+                yield from launch_scheduled_runs(
+                    workspace_process_context,
+                    logger,
+                    end_datetime_utc=end_datetime_utc,
+                    iteration_times=iteration_times,
+                    threadpool_executor=threadpool_executor,
+                    submit_threadpool_executor=submit_threadpool_executor,
+                    scheduler_run_futures=scheduler_run_futures,
+                    max_catchup_runs=max_catchup_runs,
+                    max_tick_retries=max_tick_retries,
+                )
+            except Exception:
+                error_info = DaemonErrorCapture.on_exception(
+                    exc_info=sys.exc_info(),
+                    logger=logger,
+                    log_message="SchedulerDaemon caught an error",
+                )
+                yield error_info
+                # Wait a few seconds after an error
+                next_interval_time = min(start_time + ERROR_INTERVAL_TIME, next_interval_time)
+
             yield SpanMarker.END_SPAN
             end_time = pendulum.now("UTC").timestamp()
 
-            next_minute_time = _get_next_scheduler_iteration_time(start_time)
-
-            if next_minute_time > end_time:
+            if next_interval_time > end_time:
                 # Sleep until the beginning of the next minute, plus a small epsilon to
                 # be sure that we're past the start of the minute
-                shutdown_event.wait(next_minute_time - end_time + 0.001)
+                shutdown_event.wait(next_interval_time - end_time + 0.001)
                 yield
 
 
 def launch_scheduled_runs(
     workspace_process_context: IWorkspaceProcessContext,
     logger: logging.Logger,
     end_datetime_utc: "DateTime",
```

### Comparing `dagster-1.7.3/dagster/_scheduler/stale.py` & `dagster-1.7.4/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_serdes/__init__.py` & `dagster-1.7.4/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_serdes/config_class.py` & `dagster-1.7.4/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_serdes/ipc.py` & `dagster-1.7.4/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_serdes/serdes.py` & `dagster-1.7.4/dagster/_serdes/serdes.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 )
 
 import pydantic
 from typing_extensions import Final, Self, TypeAlias, TypeVar
 
 import dagster._check as check
 import dagster._seven as seven
+from dagster._model.pydantic_compat_layer import model_fields
 from dagster._utils import is_named_tuple_instance, is_named_tuple_subclass
 from dagster._utils.cached_method import cached_method
 from dagster._utils.warnings import disable_dagster_warnings
 
 from .errors import DeserializationError, SerdesUsageError, SerializationError
 
 if TYPE_CHECKING:
@@ -671,31 +672,30 @@
 
 
 class PydanticModelSerializer(ObjectSerializer[T_PydanticModel]):
     def object_as_mapping(self, value: T_PydanticModel) -> Mapping[str, Any]:
         value_dict = value.__dict__
 
         result = {}
-        for key, field in self.klass.__fields__.items():
+        for key, field in model_fields(self.klass).items():
             if field.alias is None and (
-                getattr(field, "serialization_alias", None) is not None
-                or getattr(field, "validation_alias", None) is not None
+                field.serialization_alias is not None or field.validation_alias is not None
             ):
                 raise SerializationError(
                     "Can't serialize pydantic models with serialization or validation aliases. Use "
                     "the storage_field_names argument to whitelist_for_serdes instead."
                 )
             result_key = field.alias if field.alias else key
             result[result_key] = value_dict[key]
 
         return result
 
     @property
     def constructor_param_names(self) -> Sequence[str]:
-        return [field.alias or key for key, field in self.klass.__fields__.items()]
+        return [field.alias or key for key, field in model_fields(self.klass).items()]
 
 
 class FieldSerializer(Serializer):
     _instance = None
 
     # Because `FieldSerializer` is not currently parameterizable (all variation is contained in the
     # logic of pack/unpack), we store references to a singleton instance in the whitelist map to
```

### Comparing `dagster-1.7.3/dagster/_serdes/utils.py` & `dagster-1.7.4/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_seven/__init__.py` & `dagster-1.7.4/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_seven/abc.py` & `dagster-1.7.4/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_seven/compat/pendulum.py` & `dagster-1.7.4/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/__init__.py` & `dagster-1.7.4/dagster/_utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 import packaging.version
+from filelock import FileLock
 from typing_extensions import Literal, TypeAlias, TypeGuard
 
 import dagster._check as check
 import dagster._seven as seven
 
 from .internal_init import IHasInternalInit as IHasInternalInit
 
@@ -612,20 +613,38 @@
 
 
 def process_is_alive(pid: int) -> bool:
     if seven.IS_WINDOWS:
         import psutil
 
         return psutil.pid_exists(pid=pid)
-    else:
-        try:
-            subprocess.check_output(["ps", str(pid)])
-        except subprocess.CalledProcessError as exc:
-            assert exc.returncode == 1
+
+    # https://stackoverflow.com/questions/568271/how-to-check-if-there-exists-a-process-with-a-given-pid-in-python
+    if pid < 0:
+        return False
+    if pid == 0:
+        # According to "man 2 kill" PID 0 refers to every process
+        # in the process group of the calling process.
+        # On certain systems 0 is a valid PID but we have no way
+        # to know that in a portable fashion.
+        raise ValueError("invalid PID 0")
+    try:
+        os.kill(pid, 0)
+    except OSError as err:
+        if err.errno == errno.ESRCH:
+            # ESRCH == No such process
             return False
+        elif err.errno == errno.EPERM:
+            # EPERM clearly means there's a process to deny access to
+            return True
+        else:
+            # According to "man 2 kill" possible error values are
+            # (EINVAL, EPERM, ESRCH)
+            raise
+    else:
         return True
 
 
 def compose(*args):
     """Compose python functions args such that compose(f, g)(x) is equivalent to f(g(x))."""  # noqa: D402
     # reduce using functional composition over all the arguments, with the identity function as
     # initializer
@@ -776,7 +795,42 @@
 
 def is_uuid(value: str) -> bool:
     try:
         uuid.UUID(value)
         return True
     except ValueError:
         return False
+
+
+def run_with_concurrent_update_guard(
+    target_file_path: Path,
+    update_fn: Callable[..., None],
+    *,
+    guard_timeout_seconds: float = 60,
+    **kwargs,
+) -> None:
+    """This function prevents multiple processes attempting to update the same target artifacts
+    from running concurrently. It uses a lock file to ensure that only one process can update the
+    target file at a time.
+
+    If the target file has been updated by another process while waiting for the lock, we skip
+    running the update_fn, assuming we are about to do redundant work.
+
+    Args:
+        target_file_path (Path): The path to the target file that needs to be updated.
+        update_fn (Callable[[Any], None]): The function that will update the target file.
+        guard_timeout_seconds (float): The maximum time to wait for the lock to be released.
+            Default: 60 seconds.
+        **kwargs: The keyword arguments to pass to the function.
+    """
+    start_mtime = 0
+    if target_file_path.exists():
+        start_mtime = target_file_path.lstat().st_mtime
+
+    with FileLock(target_file_path.with_suffix(".concurrent-update-lock")).acquire(
+        timeout=guard_timeout_seconds
+    ):
+        # double check if the target file has been updated by another process while waiting for lock
+        if target_file_path.exists() and target_file_path.lstat().st_mtime > start_mtime:
+            return
+        update_fn(**kwargs)
+        return
```

### Comparing `dagster-1.7.3/dagster/_utils/alert.py` & `dagster-1.7.4/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/backoff.py` & `dagster-1.7.4/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/cached_method.py` & `dagster-1.7.4/dagster/_utils/cached_method.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from functools import wraps
-from typing import Callable, Dict, Hashable, Mapping, Tuple, TypeVar
+from typing import Callable, Hashable, Mapping, Tuple, TypeVar
 
 from typing_extensions import Concatenate, ParamSpec
 
 from dagster._seven import get_arg_names
 
 S = TypeVar("S")
 T = TypeVar("T")
 T_Callable = TypeVar("T_Callable", bound=Callable)
 P = ParamSpec("P")
 
 
 NO_ARGS_HASH_VALUE = 0
 
-CACHED_METHOD_FIELD_SUFFIX = "_cached__internal__"
+CACHED_METHOD_CACHE_FIELD = "_cached_method_cache__internal__"
 
 
 def cached_method(method: Callable[Concatenate[S, P], T]) -> Callable[Concatenate[S, P], T]:
     """Caches the results of a method call.
 
     Usage:
 
@@ -56,25 +56,27 @@
 
     However, the use of _any_ @cached_method decorated method a introduces ~20x (as in 2100%)
     overhead per call over undecorated methods, so use this carefully. The operation
     that this caches should be expensive enough so that 15% overhead on the function
     call is immaterial.  See for https://github.com/dagster-io/dagster/pull/20212
     script, data, and discussion of these matters.
     """
-    cache_attr_name = method.__name__ + CACHED_METHOD_FIELD_SUFFIX
-
+    # Cache these once self is first observed to avoid expensive work on each access
     arg_names = None
 
     @wraps(method)
     def _cached_method_wrapper(self: S, *args: P.args, **kwargs: P.kwargs) -> T:
-        if not hasattr(self, cache_attr_name):
-            cache: Dict[Hashable, T] = {}
-            setattr(self, cache_attr_name, cache)
-        else:
-            cache = getattr(self, cache_attr_name)
+        if not hasattr(self, CACHED_METHOD_CACHE_FIELD):
+            setattr(self, CACHED_METHOD_CACHE_FIELD, {})
+
+        cache_dict = getattr(self, CACHED_METHOD_CACHE_FIELD)
+        if method.__name__ not in cache_dict:
+            cache_dict[method.__name__] = {}
+
+        cache = cache_dict[method.__name__]
 
         canonical_kwargs = None
         if args:
             # Entering this block introduces about 15% overhead per call
             # See top-level docblock for more details.
 
             # nonlocal required to bind to variable in enclosing scope
```

### Comparing `dagster-1.7.3/dagster/_utils/caching_instance_queryer.py` & `dagster-1.7.4/dagster/_utils/caching_instance_queryer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import os
 from collections import defaultdict
 from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Dict,
     Iterable,
@@ -534,14 +533,15 @@
     @cached_method
     def asset_partitions_with_newly_updated_parents_and_new_cursor(
         self,
         *,
         latest_storage_id: Optional[int],
         child_asset_key: AssetKey,
         map_old_time_partitions: bool = True,
+        max_child_partitions: Optional[int] = None,
     ) -> Tuple[AbstractSet[AssetKeyPartitionKey], Optional[int]]:
         """Finds asset partitions of the given child whose parents have been materialized since
         latest_storage_id.
         """
         child_asset = self.asset_graph.get(child_asset_key)
         if not child_asset.parent_keys:
             return set(), latest_storage_id
@@ -644,17 +644,16 @@
                     # add a more helpful error message to the stack
                     raise DagsterInvalidDefinitionError(
                         f"Could not map partitions between parent {parent_asset_key.to_string()} "
                         f"and child {child_asset_key.to_string()}."
                     ) from e
 
                 child_partitions = reversed(list(child_partitions_subset.get_partition_keys()))
-                max_child_partitions = os.getenv("DAGSTER_MAX_AMP_CHILD_PARTITIONS", None)
-                if max_child_partitions:
-                    child_partitions = list(child_partitions)[: int(max_child_partitions)]
+                if max_child_partitions is not None:
+                    child_partitions = list(child_partitions)[:max_child_partitions]
 
                 for child_partition in child_partitions:
                     # we need to see if the child is planned for the same run, but this is
                     # expensive, so we try to avoid doing so in as many situations as possible
                     child_asset_partition = AssetKeyPartitionKey(child_asset_key, child_partition)
                     if (
                         # if child has a different partitions def than the parent, then it must
```

### Comparing `dagster-1.7.3/dagster/_utils/concurrency.py` & `dagster-1.7.4/dagster/_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/container.py` & `dagster-1.7.4/dagster/_utils/container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/dagster_type.py` & `dagster-1.7.4/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/env.py` & `dagster-1.7.4/dagster/_utils/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/error.py` & `dagster-1.7.4/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/external.py` & `dagster-1.7.4/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/forked_pdb.py` & `dagster-1.7.4/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/hosted_user_process.py` & `dagster-1.7.4/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/indenting_printer.py` & `dagster-1.7.4/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/internal_init.py` & `dagster-1.7.4/dagster/_utils/internal_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/interrupts.py` & `dagster-1.7.4/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/log.py` & `dagster-1.7.4/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/merger.py` & `dagster-1.7.4/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/net.py` & `dagster-1.7.4/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/schedules.py` & `dagster-1.7.4/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/tags.py` & `dagster-1.7.4/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/temp_file.py` & `dagster-1.7.4/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/test/__init__.py` & `dagster-1.7.4/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/test/data_versions.py` & `dagster-1.7.4/dagster/_utils/test/data_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/test/mysql_instance.py` & `dagster-1.7.4/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/test/postgres_instance.py` & `dagster-1.7.4/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/test/schedule_storage.py` & `dagster-1.7.4/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/timing.py` & `dagster-1.7.4/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/typed_dict.py` & `dagster-1.7.4/dagster/_utils/typed_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/typing_api.py` & `dagster-1.7.4/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/warnings.py` & `dagster-1.7.4/dagster/_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster/_utils/yaml_utils.py` & `dagster-1.7.4/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.3/dagster.egg-info/PKG-INFO` & `dagster-1.7.4/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.3
+Version: 1.7.4
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
```

### Comparing `dagster-1.7.3/dagster.egg-info/SOURCES.txt` & `dagster-1.7.4/dagster.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 dagster/_core/definitions/asset_sensor_definition.py
 dagster/_core/definitions/asset_spec.py
 dagster/_core/definitions/asset_subset.py
 dagster/_core/definitions/assets.py
 dagster/_core/definitions/auto_materialize_policy.py
 dagster/_core/definitions/auto_materialize_rule.py
 dagster/_core/definitions/auto_materialize_rule_evaluation.py
+dagster/_core/definitions/auto_materialize_rule_impls.py
 dagster/_core/definitions/auto_materialize_sensor_definition.py
 dagster/_core/definitions/backfill_policy.py
 dagster/_core/definitions/base_asset_graph.py
 dagster/_core/definitions/cacheable_assets.py
 dagster/_core/definitions/composition.py
 dagster/_core/definitions/config.py
 dagster/_core/definitions/configurable.py
@@ -242,14 +243,15 @@
 dagster/_core/execution/submit_asset_runs.py
 dagster/_core/execution/tags.py
 dagster/_core/execution/validate_run_config.py
 dagster/_core/execution/watch_orphans.py
 dagster/_core/execution/with_resources.py
 dagster/_core/execution/context/__init__.py
 dagster/_core/execution/context/compute.py
+dagster/_core/execution/context/data_version_cache.py
 dagster/_core/execution/context/hook.py
 dagster/_core/execution/context/init.py
 dagster/_core/execution/context/input.py
 dagster/_core/execution/context/invocation.py
 dagster/_core/execution/context/logger.py
 dagster/_core/execution/context/output.py
 dagster/_core/execution/context/system.py
```

### Comparing `dagster-1.7.3/dagster.egg-info/requires.txt` & `dagster-1.7.4/dagster.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 structlog
 sqlalchemy<3,>=1.0
 toposort>=1.0
 watchdog>=0.8.3
 docstring-parser
 pydantic!=1.10.7,<3,>1.10.0
 rich
-dagster-pipes==1.7.3
+filelock
+dagster-pipes==1.7.4
 
 [:platform_system == "Windows"]
 psutil>=1.0
 pywin32!=226
 
 [:python_version < "3.11"]
 protobuf<5,>=3.20.0
```

### Comparing `dagster-1.7.3/setup.py` & `dagster-1.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,16 @@
         'pywin32!=226; platform_system=="Windows"',
         "docstring-parser",
         "universal_pathlib; python_version<'3.12'",
         "universal_pathlib>=0.2.0; python_version>='3.12'",
         # https://github.com/pydantic/pydantic/issues/5821
         "pydantic>1.10.0,!= 1.10.7,<3",
         "rich",
-        "dagster-pipes==1.7.3",
+        "filelock",
+        "dagster-pipes==1.7.4",
     ],
     extras_require={
         "docker": ["docker"],
         "test": [
             "buildkite-test-collector",
             "docker",
             f"grpcio-tools>={GRPC_VERSION_FLOOR}",
```

