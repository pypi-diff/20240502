# Comparing `tmp/waylay_sdk_registry_types-2.13.0b20240423.tar.gz` & `tmp/waylay-sdk-registry-types-2.13.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_registry_types-2.13.0b20240423.tar", last modified: Wed Apr 24 07:43:55 2024, max compression
+gzip compressed data, was "waylay-sdk-registry-types-2.13.0rc0.tar", last modified: Fri Mar 29 13:21:52 2024, max compression
```

## Comparing `waylay_sdk_registry_types-2.13.0b20240423.tar` & `waylay-sdk-registry-types-2.13.0rc0.tar`

### file list

```diff
@@ -1,256 +1,414 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:55.782701 waylay_sdk_registry_types-2.13.0b20240423/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-24 07:43:55.782701 waylay_sdk_registry_types-2.13.0b20240423/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:43:55.782701 waylay_sdk_registry_types-2.13.0b20240423/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:55.742700 waylay_sdk_registry_types-2.13.0b20240423/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:55.742700 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:55.742700 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:55.742700 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:55.778701 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/
--rw-r--r--   0 runner    (1001) docker     (127)    17809 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/active_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/active_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/active_event_sse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/alt_embedded_version_i_kfserving_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/alt_embedded_version_i_plug_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/alt_embedded_version_i_webscript_response_with_invoke_link_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/alt_version_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/any_job_for_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/any_job_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/any_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/any_job_status_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/archive_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/asset_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/asset_condition_content_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/asset_condition_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/asset_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/asset_summary_with_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/asset_summary_with_hal_link_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/assets_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/batch_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/batch_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/batch_job_status_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/batch_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/build1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/build_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/build_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/build_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/build_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/build_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/cleanup_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/compiled_runtime_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/completed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/completed_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/completed_event_sse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/content_validation_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/create_webscripts_copy_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/delayed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/delayed_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/delayed_event_sse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy_args_deploy_spec_overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy_spec_openfaas_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deprecate_previous_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/documentation_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/entity_with_links_i_kfserving_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/entity_with_links_i_plug_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/entity_with_links_i_webscript_response_with_invoke_link_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/event_ack.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/event_close.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/event_keep_alive.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/event_with_close_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/example_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/exposed_openfaas_deploy_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/failed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/failed_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/failed_event_sse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/failure_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/function_deploy_overrides_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/function_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/function_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/function_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/get_model_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/get_plug_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/get_plug_response_v2_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/get_plug_response_v2_links_draft.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/get_plug_response_v2_links_published.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/get_webscript_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/get_webscript_response_v2_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/invoke_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_and_function_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_cause.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_causes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_event_response_active_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_event_response_completed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_event_response_delayed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_event_response_failed_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_event_response_waiting_children_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_event_response_waiting_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_events_and_function_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_events_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_hal_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state_active.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state_completed.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state_delayed.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state_failed.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state_finished.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state_unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state_waiting.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state_waiting_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_status_and_entity_hal_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_status_hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_status_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_type_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_type_build.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_type_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_type_notify.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_type_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_type_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_type_undeploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_type_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/jobs_for_model_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/jobs_for_model_response_v2_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/jobs_for_plug_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/jobs_for_plug_response_v2_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/jobs_for_webscript_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/jobs_for_webscript_response_v2_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/jobs_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/keep_alive_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/kf_serving_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/kfserving_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/language_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/latest_models_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/latest_plugs_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/latest_version_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/latest_webscripts_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/model1.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/model2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/model_versions_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/notify_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/parent_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug1.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_property_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_property_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_property_format_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_versions_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/post_model_job_async_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/post_model_job_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/post_plug_job_async_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/post_plug_job_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/post_webscript_job_async_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/post_webscript_job_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/provided_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/queue_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/rebuild_model_async_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/rebuild_model_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/rebuild_plug_async_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/rebuild_plug_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/rebuild_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/rebuild_webscript_async_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/rebuild_webscript_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/registry_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/request_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/resource_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/root_page_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/runtime_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/runtime_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/runtime_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/runtime_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/runtime_version_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/scale1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/scale_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/scale_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/scale_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/semantic_version_range.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/show_related_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/status_any.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/status_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/status_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/status_include.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/stream_closing.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/stream_ready.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/tags_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/timestamp_absolute.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/timestamp_age.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/timestamp_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeploy1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeploy_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeploy_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeploy_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeploy_submitted_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeploy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeployed_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/update_metadata_request_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/update_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify_job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify_model_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify_plug_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify_webscript_sync_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/waiting_children_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/waiting_children_event_sse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/waiting_event_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/waiting_event_sse.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/waiting_event_sse_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/webscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/webscript1.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/webscript2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/webscript_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/webscript_response_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/webscript_response_with_invoke_link_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/webscript_versions_response_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:55.778701 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    42896 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/models_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    44431 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/plugs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/runtimes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/schemas_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    42896 2024-04-24 07:43:51.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/webscripts_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:43:55.782701 waylay_sdk_registry_types-2.13.0b20240423/src/waylay_sdk_registry_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-24 07:43:55.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay_sdk_registry_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14308 2024-04-24 07:43:55.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay_sdk_registry_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:43:55.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay_sdk_registry_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-24 07:43:55.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay_sdk_registry_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 07:43:55.000000 waylay_sdk_registry_types-2.13.0b20240423/src/waylay_sdk_registry_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.657172 waylay-sdk-registry-types-2.13.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-03-29 13:21:52.653172 waylay-sdk-registry-types-2.13.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 13:21:52.657172 waylay-sdk-registry-types-2.13.0rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.581172 waylay-sdk-registry-types-2.13.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.581172 waylay-sdk-registry-types-2.13.0rc0/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.581172 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.581172 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.649172 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    32620 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/active_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/active_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/active_event_sse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/alt_embedded_version_i_kfserving_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/alt_embedded_version_i_plug_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/alt_embedded_version_i_webscript_response_with_invoke_link_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/alt_version_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_function_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_for_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_status_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/archive_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_condition_content_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_condition_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_path_params_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_summary_with_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_summary_with_hal_link_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/assets_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/async_deploy_query_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/async_query_default_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/async_verify_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch_job_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/cleanup_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/compiled_runtime_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/completed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/completed_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/completed_event_sse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/content_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/content_validation_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_function_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_function_query_v2_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_kf_serving_async_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_plug_async_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_webscript_async_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_webscripts_copy_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/delayed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/delayed_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/delayed_event_sse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_args_deploy_spec_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_spec_openfaas_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deprecate_previous_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/documentation_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_with_links_i_kfserving_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_with_links_i_plug_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_with_links_i_webscript_response_with_invoke_link_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/error_and_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_ack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_keep_alive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_type_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_with_close_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/example_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/exposed_openfaas_deploy_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/failed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/failed_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/failed_event_sse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/failure_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/force_delete_query_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_deploy_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_deploy_overrides_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_job_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_name_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_content_params_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_invokable_webscript_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_model_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2_links_draft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2_links_published.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_runtime_by_name_and_version_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_runtime_by_name_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_runtime_example_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_runtime_versions_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_webscript_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_webscript_response_v2_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invokable_webscript_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invokable_webscript_response_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invokable_webscript_response_entity_webscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invoke_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invoke_internal_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_and_function_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_cause.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_causes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_active_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_completed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_delayed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_failed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_waiting_children_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_waiting_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_active_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_completed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_delayed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_failed_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_waiting_children_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_waiting_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_events_and_function_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_events_filter_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_events_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_hal_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_reference_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_completed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_delayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_failed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_finished.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_waiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_waiting_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_status_and_entity_hal_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_status_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_status_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_submitted_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_undeploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_model_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_model_response_v2_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_plug_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_plug_response_v2_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_webscript_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_webscript_response_v2_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/keep_alive_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_multiple_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_multiple_with_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_query_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_with_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_latest_version_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_latest_versions_query_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_latest_versions_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_versions_query_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kfserving_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/language_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_function_versions_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_function_versions_query_show_related.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_functions_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_models_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plug_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plug_version_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plug_versions_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plug_versions_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plugs_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plugs_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_version_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_webscripts_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_configuration_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_configuration_object_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_configuration_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_create_debug_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_debug_plug_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_debug_plug_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_documentation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_function_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_create_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_meta_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request_metadata_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request_metadata_documentation_any_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_request_metadata_raw_data_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_response_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_script_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_script_meta_raw_data_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_plug_script_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_required_properties_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_required_property_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/media_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/message_and_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model_versions_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/name_and_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_kf_serving_versions_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_as_job_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_as_job_reference_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_from_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_from_legacy_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_is_not_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_plug_versions_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_webscript_versions_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/notify_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/openfaas_deploy_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/openfaas_function_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/operation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/operation_status_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/paging_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/parent_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/patch_interface_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/patch_metadata_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/patch_plug_request_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_delete_force_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_listing_and_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_listing_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property_format_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_versions_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_model_job_async_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_model_job_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_plug_job_async_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_plug_job_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_webscript_job_async_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_webscript_job_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/provided_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/publish_function_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/queue_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_computed_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_model_async_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_model_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_plug_async_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_plug_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_submitted_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_webscript_async_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_webscript_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/registry_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/remove_function_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/remove_plug_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/request_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/resource_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/root_page_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_name_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_summary_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_and_path_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_specification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/schema_by_id_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/schema_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/semantic_version_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/show_related_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status_any.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status_include.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/stream_closing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/stream_ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/supported_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/tag_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/tags_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/timestamp_absolute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/timestamp_age.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/timestamp_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_submitted_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeployed_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/unhealthy_invokable_webscript_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/update_draft_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/update_metadata_request_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/update_metadata_request_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/update_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/user_plug_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_model_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_plug_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_query_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_webscript_sync_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/version_includes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/versions_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/versions_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_children_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_children_event_sse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_event_sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_event_sse_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_latest_version_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_latest_versions_query_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_latest_versions_query_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_response_with_invoke_link_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_versions_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_asset_hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_embedded_alt_versions_i_kfserving_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_embedded_alt_versions_i_plug_response_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_embedded_alt_versions_i_webscript_response_with_invoke_link_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_entity_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/with_paging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.653172 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39273 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/models_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40842 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/plugs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9424 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/runtimes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/schemas_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39273 2024-03-29 13:21:48.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/webscripts_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 13:21:52.653172 waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-03-29 13:21:52.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24621 2024-03-29 13:21:52.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 13:21:52.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-29 13:21:52.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 13:21:52.000000 waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/top_level.txt
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/LICENSE.txt` & `waylay-sdk-registry-types-2.13.0rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/PKG-INFO` & `waylay-sdk-registry-types-2.13.0rc0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-registry-types
-Version: 2.13.0b20240423
+Version: 2.13.0rc0
 Summary: Waylay Function Registry Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,23 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-registry-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/registry.html
 Keywords: Waylay Function Registry,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
-Requires-Dist: waylay-sdk-registry==2.13.0b20240423
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-registry==2.13.0rc0
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -45,51 +44,56 @@
 Requires-Dist: pyyaml; extra == "dev"
 Requires-Dist: jsf>=0.11.1; extra == "dev"
 
 # Waylay Registry Service
 V2 API to build and deploy Waylay functions (plugs, webscripts, BYOML models).
 
 This Python package is automatically generated based on the 
-Waylay Registry OpenAPI specification (API version: 2.13.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/registry.html).
+Waylay Registry OpenAPI specification (API version: 2.13.0-beta.0)
 
 It is considered an extension of the waylay-sdk-registry package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-registry`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-registry is included in:
-- ```pip install waylay-sdk-core[registry]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[registry]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-registry and waylay-sdk-registry-types are included in:
-- ```pip install waylay-sdk-core[registry,registry-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[registry,registry-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-registry-types` is installed
-from waylay.services.registry.models.root_page_response import RootPageResponse
+from ..models.function_type import FunctionType
+from ..models.job_state_result import JobStateResult
+from ..models.job_type_schema import JobTypeSchema
+from ..models.jobs_response import JobsResponse
 try:
-    # Get Service Status
-    # calls `GET /registry/v2/`
-    api_response = await waylay_client.registry.about.get(
+    # List Jobs
+    # calls `GET /registry/v2/jobs/`
+    api_response = await waylay_client.registry.jobs.list(
+        # query parameters:
+        query = {
+        },
     )
-    print("The response of registry.about.get:\n")
+    print("The response of registry.jobs.list:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling registry.about.get: %s\n" % e)
+    print("Exception when calling registry.jobs.list: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/README.md` & `waylay-sdk-registry-types-2.13.0rc0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 # Waylay Registry Service
 V2 API to build and deploy Waylay functions (plugs, webscripts, BYOML models).
 
 This Python package is automatically generated based on the 
-Waylay Registry OpenAPI specification (API version: 2.13.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/registry.html).
+Waylay Registry OpenAPI specification (API version: 2.13.0-beta.0)
 
 It is considered an extension of the waylay-sdk-registry package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-registry`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-registry is included in:
-- ```pip install waylay-sdk-core[registry]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[registry]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-registry and waylay-sdk-registry-types are included in:
-- ```pip install waylay-sdk-core[registry,registry-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[registry,registry-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-registry-types` is installed
-from waylay.services.registry.models.root_page_response import RootPageResponse
+from ..models.function_type import FunctionType
+from ..models.job_state_result import JobStateResult
+from ..models.job_type_schema import JobTypeSchema
+from ..models.jobs_response import JobsResponse
 try:
-    # Get Service Status
-    # calls `GET /registry/v2/`
-    api_response = await waylay_client.registry.about.get(
+    # List Jobs
+    # calls `GET /registry/v2/jobs/`
+    api_response = await waylay_client.registry.jobs.list(
+        # query parameters:
+        query = {
+        },
     )
-    print("The response of registry.about.get:\n")
+    print("The response of registry.jobs.list:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling registry.about.get: %s\n" % e)
+    print("Exception when calling registry.jobs.list: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/pyproject.toml` & `waylay-sdk-registry-types-2.13.0rc0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-registry-types"
-version = "2.13.0b20240423"
+version = "2.13.0rc0"
 description = "Waylay Function Registry Types "
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Function Registry" , "Types"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.1",
-    "waylay-sdk-registry == 2.13.0b20240423",
+    "waylay-sdk ~= 0.0.4rc5",
+    "waylay-sdk-registry == 2.13.0rc0",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
 
 [project.urls]
 Homepage = "https://www.waylay.io/"
-Documentation = "https://docs.waylay.io/#/api/?id=software-development-kits"
+Documentation = "https://docs.waylay.io/#/"
 Repository = "https://github.com/waylayio/waylay-sdk-registry-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/registry.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/active_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/active_event_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,9 +21,12 @@
 
 class ActiveEventData(WaylayBaseModel):
     """ActiveEventData."""
 
     prev: QueueEvents | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/active_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/active_event_sse.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,9 +25,12 @@
 class ActiveEventSSE(WaylayBaseModel):
     """A message that notifies a state change in a background job.."""
 
     event: ActiveEventSSEEvent
     data: JobEventResponseActiveEventData
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/alt_embedded_version_i_kfserving_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/delayed_event_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
+    StrictFloat,
+    StrictInt,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.kfserving_response_v2 import KfservingResponseV2
 
+class DelayedEventData(WaylayBaseModel):
+    """DelayedEventData."""
 
-class AltEmbeddedVersionIKfservingResponseV2(WaylayBaseModel):
-    """Embedded representations of the _latest_ draft/published versions.."""
-
-    draft: KfservingResponseV2 | None = None
-    published: KfservingResponseV2 | None = None
+    delay: StrictFloat | StrictInt
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/alt_embedded_version_i_plug_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/alt_embedded_version_i_plug_response_v2.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,9 +22,12 @@
 class AltEmbeddedVersionIPlugResponseV2(WaylayBaseModel):
     """Embedded representations of the _latest_ draft/published versions.."""
 
     draft: PlugResponseV2 | None = None
     published: PlugResponseV2 | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/alt_embedded_version_i_webscript_response_with_invoke_link_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_webscript_response_v2_links.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.webscript_response_with_invoke_link_v2 import (
-    WebscriptResponseWithInvokeLinkV2,
-)
+from ..models.hal_link import HALLink
 
 
-class AltEmbeddedVersionIWebscriptResponseWithInvokeLinkV2(WaylayBaseModel):
-    """Embedded representations of the _latest_ draft/published versions.."""
+class JobsForWebscriptResponseV2Links(WaylayBaseModel):
+    """Link to the function entity.."""
 
-    draft: WebscriptResponseWithInvokeLinkV2 | None = None
-    published: WebscriptResponseWithInvokeLinkV2 | None = None
+    webscript: HALLink | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/alt_version_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/alt_version_hal_link.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,9 +25,12 @@
 class AltVersionHALLink(WaylayBaseModel):
     """AltVersionHALLink."""
 
     draft: GetPlugResponseV2LinksDraft | None = None
     published: GetPlugResponseV2LinksPublished | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/any_job_for_function.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_for_function.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/any_job_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/any_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/any_job_status_summary.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/any_job_status_summary.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/archive_format.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/archive_format.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/asset_condition.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_condition.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,9 +53,12 @@
     var_schema: Any | None = Field(
         default=None,
         description="The json schema validator that applies (in case of `application/json` entries).",
         alias="schema",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/asset_condition_content_type.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_condition_content_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/asset_condition_pattern.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_condition_pattern.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/asset_role.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_role.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/asset_summary_with_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/asset_summary_with_hal_link.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,9 +28,12 @@
     links: AssetSummaryWithHALLinkLinks = Field(alias="_links")
     name: StrictStr = Field(description="File name")
     title: StrictStr | None = None
     description: StrictStr | None = None
     role: AssetRole | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/asset_summary_with_hal_link_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_model_response_v2_links.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,18 @@
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.hal_link import HALLink
 
 
-class AssetSummaryWithHALLinkLinks(WaylayBaseModel):
-    """HAL links to the asset."""
+class JobsForModelResponseV2Links(WaylayBaseModel):
+    """Link to the function entity.."""
 
-    asset: HALLink
+    model: HALLink | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/assets_conditions.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/assets_conditions.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,9 +33,12 @@
     max_size: StrictStr | None = Field(
         default=None,
         description="The maximum size of the archive (in bytes, unless unit is provided)",
         alias="maxSize",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/batch.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,9 +43,12 @@
     created_by: StrictStr = Field(
         description="The user that initiated this job", alias="createdBy"
     )
     function: FunctionRef | None = None
     links: JobHALLinks = Field(alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/batch_args.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch_args.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,9 +25,12 @@
     """BatchArgs."""
 
     plug_name: StrictStr = Field(alias="plugName")
     function_type: FunctionType = Field(alias="functionType")
     child_type: StrictStr | None = Field(default=None, alias="childType")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/batch_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch_job_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,9 +42,12 @@
         description="The user that created this job", alias="createdBy"
     )
     operation: StrictStr = Field(description="Request operation")
     function: FunctionRef | None = None
     job: JobStatus
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/batch_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/hal_link.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
-    Field,
-    StrictFloat,
-    StrictInt,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class BatchResult(WaylayBaseModel):
-    """BatchResult."""
+class HALLink(WaylayBaseModel):
+    """HALLink."""
 
-    job_count: StrictFloat | StrictInt | None = Field(default=None, alias="jobCount")
+    href: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/build.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,9 +46,12 @@
     )
     operation: StrictStr = Field(description="Request operation")
     function: FunctionRef | None = None
     job: JobStatus | None = None
     failure_reason: FailureReason | None = Field(default=None, alias="failureReason")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/build1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build1.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,9 +43,12 @@
     created_by: StrictStr = Field(
         description="The user that initiated this job", alias="createdBy"
     )
     function: FunctionRef | None = None
     links: JobAndFunctionHALLink = Field(alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/build_args.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,17 @@
     """Input arguments to a job that builds a function.."""
 
     runtime_name: StrictStr = Field(alias="runtimeName")
     runtime_version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org",
         alias="runtimeVersion",
     )
-    revision: StrictStr = Field(
-        description="The revision hash of the current (draft) function revision"
+    revision: StrictStr | None = Field(
+        default=None,
+        description="The revision hash of the current (draft) function revision",
     )
     storage_location: StrictStr = Field(
         description="Location of the function assets.", alias="storageLocation"
     )
     image_name: StrictStr = Field(
         description="Provided (or defaulted) image name to publish the function image.",
         alias="imageName",
@@ -55,9 +56,12 @@
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
                 r"must validate the regular expression /^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/build_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_job_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,9 +42,12 @@
         description="The user that created this job", alias="createdBy"
     )
     operation: StrictStr = Field(description="Request operation")
     function: FunctionRef | None = None
     job: JobStatus
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/build_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,9 +27,12 @@
     digest: StrictStr = Field(description="SHA digest of the built image.")
     log: List[StrictStr] | None = Field(
         default=None, description="Detailed logs of the build steps."
     )
     status: StrictStr | None = Field(default=None, description="Outcome of the build.")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/build_spec.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/build_spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,9 +23,12 @@
 class BuildSpec(WaylayBaseModel):
     """BuildSpec."""
 
     context: StrictStr
     args: Dict[str, StrictStr]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/cleanup_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/cleanup_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,9 +22,12 @@
 
 class CleanupResult(WaylayBaseModel):
     """The result data for a completed cleanup job.."""
 
     scheduled_job: JobReference | None = Field(default=None, alias="scheduledJob")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/compiled_runtime_version.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/compiled_runtime_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,9 +69,12 @@
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
                 r"must validate the regular expression /^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/completed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_event_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.any_job_result import AnyJobResult
 from ..models.queue_events import QueueEvents
 
 
-class CompletedEventData(WaylayBaseModel):
-    """CompletedEventData."""
+class WaitingEventData(WaylayBaseModel):
+    """WaitingEventData."""
 
     prev: QueueEvents | None = None
-    returnvalue: AnyJobResult
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/completed_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/completed_event_sse.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,9 +25,12 @@
 class CompletedEventSSE(WaylayBaseModel):
     """A message that notifies a state change in a background job.."""
 
     event: CompletedEventSSEEvent
     data: JobEventResponseCompletedEventData
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/content_validation_listing.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/content_validation_listing.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,9 +23,12 @@
 
 class ContentValidationListing(WaylayBaseModel):
     """Content listing."""
 
     assets: List[AssetSummaryWithHALLink]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/create_webscripts_copy_parameter.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/create_webscripts_copy_parameter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/delayed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/resource_limits.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,21 +9,24 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
-    StrictFloat,
-    StrictInt,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class DelayedEventData(WaylayBaseModel):
-    """DelayedEventData."""
+class ResourceLimits(WaylayBaseModel):
+    """ResourceLimits."""
 
-    delay: StrictFloat | StrictInt
+    memory: StrictStr
+    cpu: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/delayed_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/delayed_event_sse.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,9 +25,12 @@
 class DelayedEventSSE(WaylayBaseModel):
     """A message that notifies a state change in a background job.."""
 
     event: DelayedEventSSEEvent
     data: JobEventResponseDelayedEventData
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,9 +46,12 @@
     )
     operation: StrictStr = Field(description="Request operation")
     function: FunctionRef | None = None
     job: JobStatus | None = None
     failure_reason: FailureReason | None = Field(default=None, alias="failureReason")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy1.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,9 +43,12 @@
     created_by: StrictStr = Field(
         description="The user that initiated this job", alias="createdBy"
     )
     function: FunctionRef | None = None
     links: JobAndFunctionHALLink = Field(alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy_args.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,16 +39,17 @@
         alias="imageName",
     )
     runtime_name: StrictStr = Field(alias="runtimeName")
     runtime_version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org",
         alias="runtimeVersion",
     )
-    revision: StrictStr = Field(
-        description="The revision hash of the current (draft) function revision"
+    revision: StrictStr | None = Field(
+        default=None,
+        description="The revision hash of the current (draft) function revision",
     )
     deploy_spec_overrides: DeployArgsDeploySpecOverrides = Field(
         alias="deploySpecOverrides"
     )
 
     @field_validator("runtime_version")
     @classmethod
@@ -57,9 +58,12 @@
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
                 r"must validate the regular expression /^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy_args_deploy_spec_overrides.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_args_deploy_spec_overrides.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,9 +41,12 @@
     limits: ResourceLimits | None = None
     requests: ResourceLimits | None = None
     read_only_root_filesystem: StrictBool | None = Field(
         default=None, alias="readOnlyRootFilesystem"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_job_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,35 +16,38 @@
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.deploy_args import DeployArgs
-from ..models.deploy_result import DeployResult
-from ..models.deploy_type import DeployType
 from ..models.function_ref import FunctionRef
 from ..models.job_state_result import JobStateResult
 from ..models.job_status import JobStatus
+from ..models.verify_args import VerifyArgs
+from ..models.verify_result import VerifyResult
+from ..models.verify_type import VerifyType
 
 
-class DeployJobStatus(WaylayBaseModel):
-    """DeployJobStatus."""
+class VerifyJobStatus(WaylayBaseModel):
+    """VerifyJobStatus."""
 
-    type: DeployType
+    type: VerifyType
     state: JobStateResult
-    request: DeployArgs
-    result: DeployResult | None = None
+    request: VerifyArgs
+    result: VerifyResult | None = None
     created_at: datetime = Field(
         description="The timestamp of creation of this job", alias="createdAt"
     )
     created_by: StrictStr = Field(
         description="The user that created this job", alias="createdBy"
     )
     operation: StrictStr = Field(description="Request operation")
     function: FunctionRef | None = None
     job: JobStatus
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,21 +10,24 @@
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
     Field,
+    StrictFloat,
+    StrictInt,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.exposed_openfaas_deploy_spec import ExposedOpenfaasDeploySpec
 
+class StatusResponse(WaylayBaseModel):
+    """StatusResponse."""
 
-class DeployResult(WaylayBaseModel):
-    """The result data for a completed deployment job.."""
-
-    deploy_spec: ExposedOpenfaasDeploySpec = Field(alias="deploySpec")
+    status_code: StrictFloat | StrictInt = Field(alias="statusCode")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy_spec.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,9 +24,12 @@
     """DeploySpec."""
 
     openfaas_spec: DeploySpecOpenfaasSpec | None = Field(
         default=None, alias="openfaasSpec"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deploy_spec_openfaas_spec.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_spec_openfaas_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,9 +41,12 @@
     limits: ResourceLimits | None = None
     requests: ResourceLimits | None = None
     read_only_root_filesystem: StrictBool | None = Field(
         default=None, alias="readOnlyRootFilesystem"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/deprecate_previous_policy.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deprecate_previous_policy.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/documentation.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/documentation.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,9 +34,12 @@
         default=None, description="Documentation of the plug input parameters."
     )
     output: List[DocumentationProperty] | None = Field(
         default=None, description="Documentation of the plug response parameters."
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/documentation_property.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/documentation_property.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,9 +22,12 @@
 class DocumentationProperty(WaylayBaseModel):
     """DocumentationProperty."""
 
     name: StrictStr = Field(description="Name of the documented property.")
     description: StrictStr = Field(description="Documentation of the property.")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/entity_with_links_i_kfserving_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_with_links_i_kfserving_response_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,9 +64,12 @@
     )
     draft: StrictBool = Field(
         description="If <code>true</code> this function is a draft function and it's assets are still mutable."
     )
     model: KFServingManifest
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/entity_with_links_i_plug_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_with_links_i_plug_response_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,9 +64,12 @@
     )
     draft: StrictBool = Field(
         description="If <code>true</code> this function is a draft function and it's assets are still mutable."
     )
     plug: PlugManifest
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/entity_with_links_i_webscript_response_with_invoke_link_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/entity_with_links_i_webscript_response_with_invoke_link_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,9 +68,12 @@
     webscript: WebscriptManifest
     secret: StrictStr | None = Field(
         default=None,
         description="The secret for this webscript deployment. This is <code>null</code> when <code>allowHmac=false</code> in the webscript specificaton.",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/event_with_close_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/event_with_close_sse.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/example_reference.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/example_reference.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/exposed_openfaas_deploy_spec.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/exposed_openfaas_deploy_spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,9 +30,12 @@
     namespace: StrictStr
     labels: Dict[str, StrictStr] | None = None
     annotations: Dict[str, StrictStr] | None = None
     limits: ResourceLimits | None = None
     requests: ResourceLimits | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/failed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/name.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,21 +14,19 @@
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.queue_events import QueueEvents
 
+class Name(WaylayBaseModel):
+    """Name."""
 
-class FailedEventData(WaylayBaseModel):
-    """FailedEventData."""
-
-    prev: QueueEvents | None = None
-    failed_reason: StrictStr = Field(
-        description="The failure reason of the job", alias="failedReason"
-    )
+    name: StrictStr = Field(description="The name of the function.")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/failed_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/failed_event_sse.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,9 +25,12 @@
 class FailedEventSSE(WaylayBaseModel):
     """A message that notifies a state change in a background job.."""
 
     event: FailedEventSSEEvent
     data: JobEventResponseFailedEventData
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/failure_reason.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/patch_interface_query.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import List
-
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class FailureReason(WaylayBaseModel):
-    """FailureReason."""
+class PatchInterfaceQuery(WaylayBaseModel):
+    """PatchInterfaceQuery."""
 
-    log: List[StrictStr] = Field(description="Log lines associated with this failure.")
-    events: List[StrictStr] = Field(description="Events associated with this failure.")
-    cause: StrictStr | None = Field(
-        default=None, description="Main cause for the failure."
+    comment: StrictStr | None = Field(
+        default=None,
+        description="An optional user-specified comment corresponding to the operation.",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/file_upload.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/file_upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,9 +21,12 @@
 
 class FileUpload(WaylayBaseModel):
     """A single asset file.."""
 
     file: StrictBytes | StrictStr | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/function_deploy_overrides_type.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_deploy_overrides_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,9 +29,12 @@
     env_vars: Dict[str, StrictStr] | None = Field(default=None, alias="envVars")
     labels: Dict[str, StrictStr] | None = None
     annotations: Dict[str, StrictStr] | None = None
     limits: ResourceLimits | None = None
     requests: ResourceLimits | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/function_meta.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,9 +35,12 @@
     )
     category: StrictStr | None = Field(
         default=None,
         description="A category for this function (Deprecated: use tags to categorise your functions)",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/function_ref.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_job_args.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,41 +20,37 @@
     field_validator,
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.function_type import FunctionType
 
+class FunctionJobArgs(WaylayBaseModel):
+    """Job arguments shared by all function jobs."""
 
-class FunctionRef(WaylayBaseModel):
-    """FunctionRef."""
-
-    function_type: FunctionType = Field(alias="functionType")
-    name: StrictStr = Field(description="The logical name for the function.")
-    version: StrictStr | None = Field(
-        default=None,
-        description="The semantic version of the function (all versions if undefined)",
-    )
-    runtime: StrictStr | None = None
-    runtime_version: Annotated[str, Field(strict=True)] | None = Field(
-        default=None,
+    runtime_name: StrictStr = Field(alias="runtimeName")
+    runtime_version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org",
         alias="runtimeVersion",
     )
+    revision: StrictStr | None = Field(
+        default=None,
+        description="The revision hash of the current (draft) function revision",
+    )
 
     @field_validator("runtime_version")
     @classmethod
     def runtime_version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
-        if value is None:
-            return value
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
                 r"must validate the regular expression /^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/function_type.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/get_model_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_model_response_v2.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,9 +24,12 @@
 class GetModelResponseV2(WaylayBaseModel):
     """Model Found."""
 
     entity: KfservingResponseV2
     links: GetPlugResponseV2Links = Field(alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/get_plug_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,9 +24,12 @@
 class GetPlugResponseV2(WaylayBaseModel):
     """Plug Found."""
 
     entity: PlugResponseV2
     links: GetPlugResponseV2Links = Field(alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/get_plug_response_v2_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2_links.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,9 +27,12 @@
     """HAL links to related jobs and plugs."""
 
     draft: GetPlugResponseV2LinksDraft | None = None
     published: GetPlugResponseV2LinksPublished | None = None
     jobs: HALLink | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/get_plug_response_v2_links_draft.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2_links_published.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,21 @@
     ConfigDict,
     StrictBool,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class GetPlugResponseV2LinksDraft(WaylayBaseModel):
-    """Link to the lastest draft version.."""
+class GetPlugResponseV2LinksPublished(WaylayBaseModel):
+    """Link to the lastest published version.."""
 
     draft: StrictBool
     href: StrictStr
     version: StrictStr
     deprecated: StrictBool
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/get_plug_response_v2_links_published.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_plug_response_v2_links_draft.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,18 +15,21 @@
     ConfigDict,
     StrictBool,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class GetPlugResponseV2LinksPublished(WaylayBaseModel):
-    """Link to the lastest published version.."""
+class GetPlugResponseV2LinksDraft(WaylayBaseModel):
+    """Link to the lastest draft version.."""
 
     draft: StrictBool
     href: StrictStr
     version: StrictStr
     deprecated: StrictBool
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/get_webscript_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_webscript_job_sync_response_v2.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
-    Field,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.get_webscript_response_v2_links import GetWebscriptResponseV2Links
 from ..models.webscript_response_v2 import WebscriptResponseV2
 
 
-class GetWebscriptResponseV2(WaylayBaseModel):
-    """Webscript Found."""
+class PostWebscriptJobSyncResponseV2(WaylayBaseModel):
+    """Webscript Deployed."""
 
+    message: StrictStr
     entity: WebscriptResponseV2
-    links: GetWebscriptResponseV2Links = Field(alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/get_webscript_response_v2_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_status_hal_link.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,16 +15,18 @@
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.hal_link import HALLink
 
 
-class GetWebscriptResponseV2Links(WaylayBaseModel):
+class JobStatusHALLink(WaylayBaseModel):
     """HAL links to related actions.."""
 
-    invoke: HALLink | None = None
-    jobs: HALLink | None = None
+    job: HALLink | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,20 +9,25 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
-    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.hal_link import HALLink
 
-class HALLink(WaylayBaseModel):
-    """HALLink."""
 
-    href: StrictStr
+class Plug(WaylayBaseModel):
+    """Plug."""
+
+    event: HALLink | None = None
+    plug: HALLink
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/invoke_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/invoke_hal_link.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,9 +21,12 @@
 
 class InvokeHALLink(WaylayBaseModel):
     """InvokeHALLink."""
 
     invoke: HALLink | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_and_function_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_and_function_hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_cause.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_cause.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,9 +41,12 @@
     old_value: StrictStr | None = Field(
         default=None,
         description="The old configuration value used by the last succeeded job.",
         alias="oldValue",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_causes.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_computed_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.job_cause import JobCause
+from ..models.job_causes import JobCauses
 
 
-class JobCauses(WaylayBaseModel):
-    """The motivations for including or excluding a job in response to a <em>rebuild</em> request.."""
+class RebuildComputedResponse(WaylayBaseModel):
+    """Rebuild Ignored."""
 
-    build: JobCause | None = None
-    deploy: JobCause | None = None
-    verify: JobCause | None = None
-    undeploy: JobCause | None = None
-    scale: JobCause | None = None
+    message: StrictStr
+    causes: JobCauses
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_event_response_active_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_active_event_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,9 +31,12 @@
     links: JobStatusAndEntityHALLinks = Field(alias="_links")
     job: JobReference
     data: ActiveEventData
     timestamp: datetime = Field(description="Timestamp of the event")
     function: FunctionRef
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_event_response_completed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_completed_event_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,9 +31,12 @@
     links: JobStatusAndEntityHALLinks = Field(alias="_links")
     job: JobReference
     data: CompletedEventData
     timestamp: datetime = Field(description="Timestamp of the event")
     function: FunctionRef
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_event_response_delayed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_waiting_children_event_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,32 +8,35 @@
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
 from datetime import datetime
+from typing import Any, Dict
 
 from pydantic import (
     ConfigDict,
     Field,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.delayed_event_data import DelayedEventData
 from ..models.function_ref import FunctionRef
 from ..models.job_reference import JobReference
 from ..models.job_status_and_entity_hal_links import JobStatusAndEntityHALLinks
 
 
-class JobEventResponseDelayedEventData(WaylayBaseModel):
+class JobEventResponseWaitingChildrenEventData(WaylayBaseModel):
     """Event object describing a state change of a background job.."""
 
     links: JobStatusAndEntityHALLinks = Field(alias="_links")
     job: JobReference
-    data: DelayedEventData
+    data: Dict[str, Any]
     timestamp: datetime = Field(description="Timestamp of the event")
     function: FunctionRef
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_event_response_failed_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_failed_event_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,9 +31,12 @@
     links: JobStatusAndEntityHALLinks = Field(alias="_links")
     job: JobReference
     data: FailedEventData
     timestamp: datetime = Field(description="Timestamp of the event")
     function: FunctionRef
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_event_response_waiting_children_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_response_waiting_event_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,32 +8,35 @@
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
 from datetime import datetime
-from typing import Any, Dict
 
 from pydantic import (
     ConfigDict,
     Field,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.function_ref import FunctionRef
 from ..models.job_reference import JobReference
 from ..models.job_status_and_entity_hal_links import JobStatusAndEntityHALLinks
+from ..models.waiting_event_data import WaitingEventData
 
 
-class JobEventResponseWaitingChildrenEventData(WaylayBaseModel):
+class JobEventResponseWaitingEventData(WaylayBaseModel):
     """Event object describing a state change of a background job.."""
 
     links: JobStatusAndEntityHALLinks = Field(alias="_links")
     job: JobReference
-    data: Dict[str, Any]
+    data: WaitingEventData
     timestamp: datetime = Field(description="Timestamp of the event")
     function: FunctionRef
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_event_response_waiting_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_payload_waiting_children_event_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,32 +8,31 @@
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
 from datetime import datetime
+from typing import Any, Dict
 
 from pydantic import (
     ConfigDict,
     Field,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.function_ref import FunctionRef
 from ..models.job_reference import JobReference
-from ..models.job_status_and_entity_hal_links import JobStatusAndEntityHALLinks
-from ..models.waiting_event_data import WaitingEventData
 
 
-class JobEventResponseWaitingEventData(WaylayBaseModel):
-    """Event object describing a state change of a background job.."""
+class JobEventPayloadWaitingChildrenEventData(WaylayBaseModel):
+    """JobEventPayloadWaitingChildrenEventData."""
 
-    links: JobStatusAndEntityHALLinks = Field(alias="_links")
     job: JobReference
-    data: WaitingEventData
+    data: Dict[str, Any]
     timestamp: datetime = Field(description="Timestamp of the event")
-    function: FunctionRef
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_event_sse.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_events_and_function_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_events_and_function_hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_events_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_hal_link.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,18 @@
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.hal_link import HALLink
 
 
-class JobEventsHALLink(WaylayBaseModel):
-    """HAL links to related actions.."""
+class JobsHALLink(WaylayBaseModel):
+    """JobsHALLink."""
 
-    event: HALLink | None = None
+    jobs: HALLink | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_hal_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript2.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,16 +15,19 @@
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.hal_link import HALLink
 
 
-class JobHALLinks(WaylayBaseModel):
-    """HAL links to related actions.."""
+class Webscript2(WaylayBaseModel):
+    """Webscript2."""
 
-    event: HALLink | None = None
     job: HALLink | None = None
+    webscript: HALLink
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_reference.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model2.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
-    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.job_type import JobType
+from ..models.hal_link import HALLink
 
 
-class JobReference(WaylayBaseModel):
-    """JobReference."""
+class Model2(WaylayBaseModel):
+    """Model2."""
 
-    type: JobType
-    id: StrictStr | None = None
+    job: HALLink | None = None
+    model: HALLink
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,9 +24,12 @@
 class JobResponse(WaylayBaseModel):
     """Job Found."""
 
     job: AnyJobStatus
     links: JobEventsAndFunctionHALLink = Field(alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state_finished.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_finished.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_result.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state_waiting.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_waiting.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_state_waiting_children.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_state_waiting_children.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,9 +36,12 @@
     finished_on: datetime | None = Field(default=None, alias="finishedOn")
     processed_on: datetime | None = Field(default=None, alias="processedOn")
     failed_reason: StrictStr | None = Field(default=None, alias="failedReason")
     parent: ParentKeys | None = None
     delay: StrictFloat | StrictInt | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_status_and_entity_hal_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_status_and_entity_hal_links.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_status_hal_link.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_hal_links.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,19 @@
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.hal_link import HALLink
 
 
-class JobStatusHALLink(WaylayBaseModel):
+class JobHALLinks(WaylayBaseModel):
     """HAL links to related actions.."""
 
+    event: HALLink | None = None
     job: HALLink | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_type.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_version_level.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,21 +10,18 @@
 """
 
 from __future__ import annotations
 
 from enum import Enum
 
 
-class JobType(str, Enum):
-    """JobType."""
+class LatestVersionLevel(str, Enum):
+    """Level of latest versions that should be included.."""
 
-    BUILD = "build"
-    DEPLOY = "deploy"
-    VERIFY = "verify"
-    UNDEPLOY = "undeploy"
-    BATCH = "batch"
-    SCALE = "scale"
-    CLEANUP = "cleanup"
-    NOTIFY = "notify"
+    MAJOR = "major"
+    MINOR = "minor"
+    PATCH = "patch"
+    TRUE = "true"
+    FALSE = "false"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/job_type_schema.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_type_schema.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/jobs_for_model_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_model_response_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,9 +30,12 @@
     jobs: List[AnyJobForFunction] = Field(
         description="Listing of jobs related to the function deployment. This includes active jobs, and the most recently failed job (per type) that was archived on the entity."
     )
     function: FunctionRef
     links: JobsForModelResponseV2Links | None = Field(default=None, alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/jobs_for_model_response_v2_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model1.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,20 @@
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.hal_link import HALLink
 
 
-class JobsForModelResponseV2Links(WaylayBaseModel):
-    """Link to the function entity.."""
+class Model1(WaylayBaseModel):
+    """Model1."""
 
-    model: HALLink | None = None
+    event: HALLink | None = None
+    job: HALLink | None = None
+    model: HALLink
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/jobs_for_plug_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_plug_response_v2.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,9 +30,12 @@
     jobs: List[AnyJobForFunction] = Field(
         description="Listing of jobs related to the function deployment. This includes active jobs, and the most recently failed job (per type) that was archived on the entity."
     )
     function: FunctionRef
     links: JobsForPlugResponseV2Links | None = Field(default=None, alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/jobs_for_plug_response_v2_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_required_property_object.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,21 +9,29 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
+    StrictBool,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.hal_link import HALLink
+from ..models.plug_property_data_type import PlugPropertyDataType
 
 
-class JobsForPlugResponseV2Links(WaylayBaseModel):
-    """Link to the function entity.."""
+class LegacyRequiredPropertyObject(WaylayBaseModel):
+    """LegacyRequiredPropertyObject."""
 
-    plug: HALLink | None = None
+    name: StrictStr
+    type: PlugPropertyDataType
+    mandatory: StrictBool
+    sensitive: StrictBool
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/jobs_for_webscript_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_webscript_response_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,9 +32,12 @@
     jobs: List[AnyJobForFunction] = Field(
         description="Listing of jobs related to the function deployment. This includes active jobs, and the most recently failed job (per type) that was archived on the entity."
     )
     function: FunctionRef
     links: JobsForWebscriptResponseV2Links | None = Field(default=None, alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/jobs_for_webscript_response_v2_links.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/tag.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
+    Field,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.hal_link import HALLink
 
+class Tag(WaylayBaseModel):
+    """One or more tags can be assigned to a function entity to facilitate grouping and searching.."""
 
-class JobsForWebscriptResponseV2Links(WaylayBaseModel):
-    """Link to the function entity.."""
-
-    webscript: HALLink | None = None
+    name: StrictStr = Field(description="Name of the tag")
+    color: StrictStr = Field(description="Color associated with the tag in an UI.")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/jobs_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/keep_alive_event_sse.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,33 +7,32 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import List
-
 from pydantic import (
     ConfigDict,
     Field,
-    StrictFloat,
-    StrictInt,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.any_job_status_summary import AnyJobStatusSummary
+from ..models.event_keep_alive import EventKeepAlive
 
 
-class JobsResponse(WaylayBaseModel):
-    """Jobs Found."""
+class KeepAliveEventSSE(WaylayBaseModel):
+    """A message that acknowledges that the stream is still alive.."""
 
-    limit: StrictFloat | StrictInt | None = Field(
-        default=None, description="The page size used for this query result."
-    )
-    jobs: List[AnyJobStatusSummary] = Field(
-        description="Listing of jobs that satisfy the query."
+    event: EventKeepAlive
+    data: StrictStr | None = Field(
+        default=None,
+        description="A text message acknowledging that events will be forwarded.",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/keep_alive_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/operation.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
-    Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.event_keep_alive import EventKeepAlive
+from ..models.job_type import JobType
 
 
-class KeepAliveEventSSE(WaylayBaseModel):
-    """A message that acknowledges that the stream is still alive.."""
+class Operation(WaylayBaseModel):
+    """Operation."""
 
-    event: EventKeepAlive
-    data: StrictStr | None = Field(
-        default=None,
-        description="A text message acknowledging that events will be forwarded.",
-    )
+    id: StrictStr
+    description: StrictStr
+    name: StrictStr
+    type: JobType
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/kf_serving_manifest.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/legacy_debug_plug_manifest.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
 import re
+from typing import Dict
 
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
     field_validator,
 )
@@ -25,34 +26,40 @@
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.function_deploy_overrides_type import FunctionDeployOverridesType
 from ..models.function_meta import FunctionMeta
 from ..models.semantic_version_range import SemanticVersionRange
 
 
-class KFServingManifest(WaylayBaseModel):
-    """KFServingManifest."""
+class LegacyDebugPlugManifest(WaylayBaseModel):
+    """LegacyDebugPlugManifest."""
 
     deploy: FunctionDeployOverridesType | None = None
     name: StrictStr = Field(description="The logical name for the function.")
     version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org"
     )
     runtime: StrictStr
     runtime_version: SemanticVersionRange | None = Field(
         default=None, alias="runtimeVersion"
     )
     metadata: FunctionMeta
+    tenant: StrictStr
+    dependencies: Dict[str, StrictStr] | None = None
+    script: StrictStr
 
     @field_validator("version")
     @classmethod
     def version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
                 r"must validate the regular expression /^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/kfserving_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kfserving_response_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,9 +56,12 @@
     )
     draft: StrictBool = Field(
         description="If <code>true</code> this function is a draft function and it's assets are still mutable."
     )
     model: KFServingManifest
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/language_release.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/language_release.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,9 +28,12 @@
     version: StrictStr = Field(
         description="Release version of the language or framework."
     )
     title: StrictStr = Field(description="Display title.")
     description: StrictStr | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/latest_models_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_models_response_v2.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,9 +39,12 @@
         default=None, description="The page number of a paged query result."
     )
     entities: List[EntityWithLinksIKfservingResponseV2] = Field(
         description="The specification and deployment status of the queried functions"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/latest_plugs_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_plugs_response_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,9 +37,12 @@
         default=None, description="The page number of a paged query result."
     )
     entities: List[EntityWithLinksIPlugResponseV2] = Field(
         description="The specification and deployment status of the queried functions"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/latest_version_level.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_children_event_sse_event.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 """
 
 from __future__ import annotations
 
 from enum import Enum
 
 
-class LatestVersionLevel(str, Enum):
-    """Level of latest versions that should be included.."""
+class WaitingChildrenEventSSEEvent(str, Enum):
+    """The job queue event that trigged this message."""
 
-    MAJOR = "major"
-    MINOR = "minor"
-    PATCH = "patch"
-    TRUE = "true"
-    FALSE = "false"
+    WAITING_MINUS_CHILDREN = "waiting-children"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/latest_webscripts_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_versions_response_v2.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,31 +17,34 @@
     ConfigDict,
     Field,
     StrictFloat,
     StrictInt,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.entity_with_links_i_webscript_response_with_invoke_link_v2 import (
-    EntityWithLinksIWebscriptResponseWithInvokeLinkV2,
+from ..models.webscript_response_with_invoke_link_v2 import (
+    WebscriptResponseWithInvokeLinkV2,
 )
 
 
-class LatestWebscriptsResponseV2(WaylayBaseModel):
-    """Webscripts Found."""
+class WebscriptVersionsResponseV2(WaylayBaseModel):
+    """Webscript Versions Found."""
 
     limit: StrictFloat | StrictInt | None = Field(
         default=None, description="The page size used for this query result."
     )
     count: StrictFloat | StrictInt = Field(
         description="The total count of matching items, from which this result is one page."
     )
     page: StrictFloat | StrictInt | None = Field(
         default=None, description="The page number of a paged query result."
     )
-    entities: List[EntityWithLinksIWebscriptResponseWithInvokeLinkV2] = Field(
+    entities: List[WebscriptResponseWithInvokeLinkV2] = Field(
         description="The specification and deployment status of the queried functions"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/model.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/completed_event_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,19 +12,23 @@
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.hal_link import HALLink
+from ..models.any_job_result import AnyJobResult
+from ..models.queue_events import QueueEvents
 
 
-class Model(WaylayBaseModel):
-    """Model."""
+class CompletedEventData(WaylayBaseModel):
+    """CompletedEventData."""
 
-    event: HALLink | None = None
-    model: HALLink
+    prev: QueueEvents | None = None
+    returnvalue: AnyJobResult
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/model1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug1.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,17 +15,20 @@
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.hal_link import HALLink
 
 
-class Model1(WaylayBaseModel):
-    """Model1."""
+class Plug1(WaylayBaseModel):
+    """Plug1."""
 
     event: HALLink | None = None
     job: HALLink | None = None
-    model: HALLink
+    plug: HALLink
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/model2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/parent_keys.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.hal_link import HALLink
 
+class ParentKeys(WaylayBaseModel):
+    """ParentKeys."""
 
-class Model2(WaylayBaseModel):
-    """Model2."""
-
-    job: HALLink | None = None
-    model: HALLink
+    id: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/model_versions_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model_versions_response_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,9 +37,12 @@
         default=None, description="The page number of a paged query result."
     )
     entities: List[KfservingResponseV2] = Field(
         description="The specification and deployment status of the queried functions"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/notify_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/notify_result.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,9 +21,12 @@
 
 class NotifyResult(WaylayBaseModel):
     """The result data for a change notification.."""
 
     operation: RequestOperation
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/parent_keys.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_model_job_sync_response_v2.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,16 +13,22 @@
 
 from pydantic import (
     ConfigDict,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.kfserving_response_v2 import KfservingResponseV2
 
-class ParentKeys(WaylayBaseModel):
-    """ParentKeys."""
 
-    id: StrictStr
+class PostModelJobSyncResponseV2(WaylayBaseModel):
+    """Model Deployed."""
+
+    message: StrictStr
+    entity: KfservingResponseV2
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/message_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.hal_link import HALLink
 
+class MessageResponse(WaylayBaseModel):
+    """MessageResponse."""
 
-class Plug(WaylayBaseModel):
-    """Plug."""
-
-    event: HALLink | None = None
-    plug: HALLink
+    message: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_delete_force_query.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,23 +9,27 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
+    Field,
+    StrictBool,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.hal_link import HALLink
 
+class PlugDeleteForceQuery(WaylayBaseModel):
+    """PlugDeleteForceQuery."""
 
-class Plug1(WaylayBaseModel):
-    """Plug1."""
-
-    event: HALLink | None = None
-    job: HALLink | None = None
-    plug: HALLink
+    force: StrictBool | None = Field(
+        default=None,
+        description="If <code>true</code>, the plug version(s) will be undeployed and removed. Otherwise, the plug version(s) will only be <code>deprecated</code>, i.e removed from regular listings.",
+    )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/jobs_for_plug_response_v2_links.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,16 +15,18 @@
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.hal_link import HALLink
 
 
-class Plug2(WaylayBaseModel):
-    """Plug2."""
+class JobsForPlugResponseV2Links(WaylayBaseModel):
+    """Link to the function entity.."""
 
-    job: HALLink | None = None
-    plug: HALLink
+    plug: HALLink | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_interface.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,9 +34,12 @@
         default=None, description="The named input parameters of a plug"
     )
     output: List[PlugProperty] | None = Field(
         default=None, description="The named output parameters of a plug"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_manifest.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_manifest.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,9 +54,12 @@
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
                 r"must validate the regular expression /^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_meta.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,9 +54,12 @@
         default=None,
         description="Display title for this function.",
         alias="friendlyName",
     )
     documentation: Documentation | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_property.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,9 +33,12 @@
     mandatory: StrictBool | None = Field(
         default=None, description="If <code>true</code> this property is required."
     )
     format: PlugPropertyFormat | None = None
     default_value: Any | None = Field(default=None, alias="defaultValue")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_property_data_type.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property_data_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_property_format.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property_format.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,9 +28,12 @@
     type: PlugPropertyFormatType | None = None
     values: List[Any] | None = Field(
         default=None,
         description='The enumerated value domain when <code>type="enum"</code>',
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_property_format_type.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_property_format_type.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_response_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,9 +56,12 @@
     )
     draft: StrictBool = Field(
         description="If <code>true</code> this function is a draft function and it's assets are still mutable."
     )
     plug: PlugManifest
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/plug_versions_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug_versions_response_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,9 +37,12 @@
         default=None, description="The page number of a paged query result."
     )
     entities: List[PlugResponseV2] = Field(
         description="The specification and deployment status of the queried functions"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/post_model_job_async_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_model_job_async_response_v2.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,9 +26,12 @@
     """Model Deployment Initiated."""
 
     message: StrictStr
     links: JobHALLinks = Field(alias="_links")
     entity: KfservingResponseV2
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/post_model_job_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/plug2.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
-    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.kfserving_response_v2 import KfservingResponseV2
+from ..models.hal_link import HALLink
 
 
-class PostModelJobSyncResponseV2(WaylayBaseModel):
-    """Model Deployed."""
+class Plug2(WaylayBaseModel):
+    """Plug2."""
 
-    message: StrictStr
-    entity: KfservingResponseV2
+    job: HALLink | None = None
+    plug: HALLink
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/post_plug_job_async_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/post_plug_job_async_response_v2.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,9 +26,12 @@
     """Plug Deployment Initiated."""
 
     message: StrictStr
     links: JobHALLinks = Field(alias="_links")
     entity: PlugResponseV2
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/post_plug_job_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_multiple_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,25 +7,28 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
+from typing import List
+
 from pydantic import (
     ConfigDict,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.plug_response_v2 import PlugResponseV2
-
 
-class PostPlugJobSyncResponseV2(WaylayBaseModel):
-    """Plug Deployed."""
+class KFServingDeleteMultipleResponse(WaylayBaseModel):
+    """Models Deleted."""
 
-    message: StrictStr
-    entity: PlugResponseV2
+    name: StrictStr
+    versions: List[StrictStr]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/post_webscript_job_async_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/job_submitted_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,20 +15,21 @@
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.job_hal_links import JobHALLinks
-from ..models.webscript_response_v2 import WebscriptResponseV2
 
 
-class PostWebscriptJobAsyncResponseV2(WaylayBaseModel):
-    """Webscript Deployment Initiated."""
+class JobSubmittedResponse(WaylayBaseModel):
+    """JobSubmittedResponse."""
 
     message: StrictStr
     links: JobHALLinks = Field(alias="_links")
-    entity: WebscriptResponseV2
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/post_webscript_job_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_webscript_async_response_v2.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,23 +9,31 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
+    Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.job_causes import JobCauses
+from ..models.job_hal_links import JobHALLinks
 from ..models.webscript_response_v2 import WebscriptResponseV2
 
 
-class PostWebscriptJobSyncResponseV2(WaylayBaseModel):
-    """Webscript Deployed."""
+class RebuildWebscriptAsyncResponseV2(WaylayBaseModel):
+    """Webscript Rebuild Initiated."""
 
     message: StrictStr
+    links: JobHALLinks = Field(alias="_links")
+    causes: JobCauses
     entity: WebscriptResponseV2
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/provided_dependency.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/provided_dependency.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,9 +47,12 @@
     )
     native: StrictBool | None = Field(
         default=None,
         description="If true, the library is provided natively by the runtime: e.g. node for javascript.",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/queue_events.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/queue_events.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/rebuild_model_async_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/kf_serving_delete_multiple_with_job_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,30 +7,33 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
+from typing import List
+
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.job_causes import JobCauses
 from ..models.job_hal_links import JobHALLinks
-from ..models.kfserving_response_v2 import KfservingResponseV2
 
 
-class RebuildModelAsyncResponseV2(WaylayBaseModel):
-    """Model Rebuild Initiated."""
+class KFServingDeleteMultipleWithJobResponse(WaylayBaseModel):
+    """Model Deletions Initiated."""
 
+    name: StrictStr
+    versions: List[StrictStr]
     message: StrictStr
     links: JobHALLinks = Field(alias="_links")
-    causes: JobCauses
-    entity: KfservingResponseV2
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/rebuild_model_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_model_sync_response_v2.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,9 +25,12 @@
     """Model Rebuild Ignored."""
 
     message: StrictStr
     causes: JobCauses
     entity: KfservingResponseV2
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/rebuild_plug_async_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_model_async_response_v2.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,21 +16,24 @@
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.job_causes import JobCauses
 from ..models.job_hal_links import JobHALLinks
-from ..models.plug_response_v2 import PlugResponseV2
+from ..models.kfserving_response_v2 import KfservingResponseV2
 
 
-class RebuildPlugAsyncResponseV2(WaylayBaseModel):
-    """Plug Rebuild Initiated."""
+class RebuildModelAsyncResponseV2(WaylayBaseModel):
+    """Model Rebuild Initiated."""
 
     message: StrictStr
     links: JobHALLinks = Field(alias="_links")
     causes: JobCauses
-    entity: PlugResponseV2
+    entity: KfservingResponseV2
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/rebuild_plug_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_plug_sync_response_v2.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,9 +25,12 @@
     """Plug Rebuild Ignored."""
 
     message: StrictStr
     causes: JobCauses
     entity: PlugResponseV2
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/rebuild_policy.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_policy.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/rebuild_webscript_async_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/rebuild_webscript_sync_response_v2.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
-    Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.job_causes import JobCauses
-from ..models.job_hal_links import JobHALLinks
 from ..models.webscript_response_v2 import WebscriptResponseV2
 
 
-class RebuildWebscriptAsyncResponseV2(WaylayBaseModel):
-    """Webscript Rebuild Initiated."""
+class RebuildWebscriptSyncResponseV2(WaylayBaseModel):
+    """Webscript Rebuild Ignored."""
 
     message: StrictStr
-    links: JobHALLinks = Field(alias="_links")
     causes: JobCauses
     entity: WebscriptResponseV2
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/rebuild_webscript_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/get_webscript_response_v2.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
-    StrictStr,
+    Field,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.job_causes import JobCauses
+from ..models.get_webscript_response_v2_links import GetWebscriptResponseV2Links
 from ..models.webscript_response_v2 import WebscriptResponseV2
 
 
-class RebuildWebscriptSyncResponseV2(WaylayBaseModel):
-    """Webscript Rebuild Ignored."""
+class GetWebscriptResponseV2(WaylayBaseModel):
+    """Webscript Found."""
 
-    message: StrictStr
-    causes: JobCauses
     entity: WebscriptResponseV2
+    links: GetWebscriptResponseV2Links = Field(alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/registry_error_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/registry_error_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,9 +28,12 @@
 
     error: StrictStr
     code: StrictStr
     status_code: StrictFloat | StrictInt = Field(alias="statusCode")
     data: Dict[str, StrictStr] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/request_operation.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/request_operation.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/resource_limits.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/operation_status_error.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,16 +14,21 @@
 from pydantic import (
     ConfigDict,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class ResourceLimits(WaylayBaseModel):
-    """ResourceLimits."""
+class OperationStatusError(WaylayBaseModel):
+    """OperationStatusError."""
 
-    memory: StrictStr
-    cpu: StrictStr
+    name: StrictStr
+    message: StrictStr
+    stack: StrictStr | None = None
+    code: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/root_page_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/root_page_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,9 +45,12 @@
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
                 r"must validate the regular expression /^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/runtime_attributes.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,34 +22,38 @@
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class RuntimeAttributes(WaylayBaseModel):
-    """RuntimeAttributes."""
+class RuntimeVersionInfo(WaylayBaseModel):
+    """A summary of a selected version for a runtime."""
 
     deprecated: StrictBool = Field(
         description="If true, the function uses a deprecated runtime."
     )
     upgradable: StrictBool = Field(
         description="If true, a newer runtime for this function is available using the `rebuild` API."
     )
-    name: StrictStr
     version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org"
     )
+    title: StrictStr
+    description: StrictStr | None = None
 
     @field_validator("version")
     @classmethod
     def version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
                 r"must validate the regular expression /^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/runtime_summary.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,9 +32,12 @@
     title: StrictStr
     description: StrictStr | None = None
     function_type: FunctionType = Field(alias="functionType")
     archive_format: ArchiveFormat = Field(alias="archiveFormat")
     versions: List[RuntimeVersionInfo]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/runtime_summary_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/named_parameters_typeof_is_not_legacy.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,25 +7,28 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import List
-
 from pydantic import (
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.runtime_summary import RuntimeSummary
+from ..models.legacy_plug_request_metadata_documentation import (
+    LegacyPlugRequestMetadataDocumentation,
+)
 
 
-class RuntimeSummaryResponse(WaylayBaseModel):
-    """Runtimes Found."""
+class NamedParametersTypeofIsNotLegacy(WaylayBaseModel):
+    """NamedParametersTypeofIsNotLegacy."""
 
-    runtimes: List[RuntimeSummary]
+    documentation: LegacyPlugRequestMetadataDocumentation | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/runtime_version_info.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/function_manifest.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,45 +12,50 @@
 from __future__ import annotations
 
 import re
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictBool,
     StrictStr,
     field_validator,
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.function_deploy_overrides_type import FunctionDeployOverridesType
+from ..models.function_meta import FunctionMeta
+from ..models.semantic_version_range import SemanticVersionRange
 
-class RuntimeVersionInfo(WaylayBaseModel):
-    """A summary of a selected version for a runtime."""
 
-    deprecated: StrictBool = Field(
-        description="If true, the function uses a deprecated runtime."
-    )
-    upgradable: StrictBool = Field(
-        description="If true, a newer runtime for this function is available using the `rebuild` API."
-    )
+class FunctionManifest(WaylayBaseModel):
+    """FunctionManifest."""
+
+    deploy: FunctionDeployOverridesType | None = None
+    name: StrictStr = Field(description="The logical name for the function.")
     version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org"
     )
-    title: StrictStr
-    description: StrictStr | None = None
+    runtime: StrictStr
+    runtime_version: SemanticVersionRange | None = Field(
+        default=None, alias="runtimeVersion"
+    )
+    metadata: FunctionMeta
 
     @field_validator("version")
     @classmethod
     def version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
                 r"must validate the regular expression /^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/runtime_version_response.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_version_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,9 +21,12 @@
 
 class RuntimeVersionResponse(WaylayBaseModel):
     """: Runtime Version Found."""
 
     runtime: CompiledRuntimeVersion
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/scale.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,9 +48,12 @@
     )
     operation: StrictStr = Field(description="Request operation")
     function: FunctionRef | None = None
     job: JobStatus | None = None
     failure_reason: FailureReason | None = Field(default=None, alias="failureReason")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/scale1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify1.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,21 +19,21 @@
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.function_ref import FunctionRef
 from ..models.job_and_function_hal_link import JobAndFunctionHALLink
 from ..models.job_state_result import JobStateResult
-from ..models.scale_type import ScaleType
+from ..models.verify_type import VerifyType
 
 
-class Scale1(WaylayBaseModel):
-    """Scale1."""
+class Verify1(WaylayBaseModel):
+    """Verify1."""
 
-    type: ScaleType
+    type: VerifyType
     operation: StrictStr = Field(
         description="The operation name for the background task."
     )
     id: StrictStr = Field(
         description="The id of the background job, or the constant `_unknown_`"
     )
     state: JobStateResult
@@ -43,9 +43,12 @@
     created_by: StrictStr = Field(
         description="The user that initiated this job", alias="createdBy"
     )
     function: FunctionRef | None = None
     links: JobAndFunctionHALLink = Field(alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/scale_args.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale_args.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,25 +35,29 @@
     )
     endpoint: StrictStr = Field(description="The (openfaas) endpoint service name")
     runtime_name: StrictStr = Field(alias="runtimeName")
     runtime_version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org",
         alias="runtimeVersion",
     )
-    revision: StrictStr = Field(
-        description="The revision hash of the current (draft) function revision"
+    revision: StrictStr | None = Field(
+        default=None,
+        description="The revision hash of the current (draft) function revision",
     )
     replicas: StrictFloat | StrictInt = Field(description="Number of target replicas")
 
     @field_validator("runtime_version")
     @classmethod
     def runtime_version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
                 r"must validate the regular expression /^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/scale_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale_job_status.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,9 +44,12 @@
         description="The user that created this job", alias="createdBy"
     )
     operation: StrictStr = Field(description="Request operation")
     function: FunctionRef | None = None
     job: JobStatus
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/semantic_version_range.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/semantic_version_range.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/status_filter.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status_filter.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 )
 
 from typing_extensions import (
     Annotated,  # >=3.9
 )
 
 from ..models.status_any import StatusAny
-from ..models.status_exclude import StatusExclude
 from ..models.status_include import StatusInclude
 
 StatusFilter = Union[
-    Annotated[StatusInclude, ""], Annotated[StatusExclude, ""], Annotated[StatusAny, ""]
+    Annotated[StatusInclude, ""],
+    Annotated[
+        str,
+        "Any status value with a `-` postfix appended, excludes that status as a filter.",
+    ],
+    Annotated[StatusAny, ""],
 ]
 """Inclusion or exclusion filter on the `status` property.."""
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/status_include.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/status_include.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/stream_closing.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/stream_ready.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,21 +14,24 @@
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.event_close import EventClose
+from ..models.event_ack import EventAck
 
 
-class StreamClosing(WaylayBaseModel):
-    """A message that notifies that the server will not send more events, and that the client should close.."""
+class StreamReady(WaylayBaseModel):
+    """A message that acknowledges that the server will sent job state changes.."""
 
-    event: EventClose
+    event: EventAck
     data: StrictStr = Field(
-        description="A text message describing the cause for closing the stream."
+        description="A text message acknowledging what events will be forwarded."
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/stream_ready.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/failed_event_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,21 +14,24 @@
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.event_ack import EventAck
+from ..models.queue_events import QueueEvents
 
 
-class StreamReady(WaylayBaseModel):
-    """A message that acknowledges that the server will sent job state changes.."""
+class FailedEventData(WaylayBaseModel):
+    """FailedEventData."""
 
-    event: EventAck
-    data: StrictStr = Field(
-        description="A text message acknowledging what events will be forwarded."
+    prev: QueueEvents | None = None
+    failed_reason: StrictStr = Field(
+        description="The failure reason of the job", alias="failedReason"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/tag.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_summary_attrs.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,17 +14,26 @@
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.archive_format import ArchiveFormat
+from ..models.function_type import FunctionType
 
-class Tag(WaylayBaseModel):
-    """One or more tags can be assigned to a function entity to facilitate grouping and searching.."""
 
-    name: StrictStr = Field(description="Name of the tag")
-    color: StrictStr = Field(description="Color associated with the tag in an UI.")
+class RuntimeSummaryAttrs(WaylayBaseModel):
+    """RuntimeSummaryAttrs."""
+
+    name: StrictStr
+    title: StrictStr
+    description: StrictStr | None = None
+    function_type: FunctionType = Field(alias="functionType")
+    archive_format: ArchiveFormat = Field(alias="archiveFormat")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/timestamp_absolute.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/timestamp_absolute.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/timestamp_age.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/timestamp_age.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/timestamp_spec.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/timestamp_spec.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeploy.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,9 +46,12 @@
     )
     operation: StrictStr = Field(description="Request operation")
     function: FunctionRef | None = None
     job: JobStatus | None = None
     failure_reason: FailureReason | None = Field(default=None, alias="failureReason")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeploy1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/scale1.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,21 +19,21 @@
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.function_ref import FunctionRef
 from ..models.job_and_function_hal_link import JobAndFunctionHALLink
 from ..models.job_state_result import JobStateResult
-from ..models.undeploy_type import UndeployType
+from ..models.scale_type import ScaleType
 
 
-class Undeploy1(WaylayBaseModel):
-    """Undeploy1."""
+class Scale1(WaylayBaseModel):
+    """Scale1."""
 
-    type: UndeployType
+    type: ScaleType
     operation: StrictStr = Field(
         description="The operation name for the background task."
     )
     id: StrictStr = Field(
         description="The id of the background job, or the constant `_unknown_`"
     )
     state: JobStateResult
@@ -43,9 +43,12 @@
     created_by: StrictStr = Field(
         description="The user that initiated this job", alias="createdBy"
     )
     function: FunctionRef | None = None
     links: JobAndFunctionHALLink = Field(alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeploy_args.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_args.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,51 +12,49 @@
 from __future__ import annotations
 
 import re
 
 from pydantic import (
     ConfigDict,
     Field,
-    StrictBool,
     StrictStr,
     field_validator,
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class UndeployArgs(WaylayBaseModel):
-    """Input argument to an (openfaas) undeployment job for a function.."""
+class VerifyArgs(WaylayBaseModel):
+    """Input arguments for an (openfaas) deployment verification job.."""
 
     namespace: StrictStr = Field(
         description="The (openfaas) namespace for the target function."
     )
     endpoint: StrictStr = Field(description="The (openfaas) endpoint service name")
     runtime_name: StrictStr = Field(alias="runtimeName")
     runtime_version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org",
         alias="runtimeVersion",
     )
-    revision: StrictStr = Field(
-        description="The revision hash of the current (draft) function revision"
+    revision: StrictStr | None = Field(
+        default=None,
+        description="The revision hash of the current (draft) function revision",
     )
-    is_native_plug: StrictBool = Field(
-        description="If true, the function is not expected to be deployed on openfaas.",
-        alias="isNativePlug",
-    )
-    delete_entity: StrictBool = Field(alias="deleteEntity")
 
     @field_validator("runtime_version")
     @classmethod
     def runtime_version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
                 r"must validate the regular expression /^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeploy_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/deploy_job_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,35 +16,38 @@
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.deploy_args import DeployArgs
+from ..models.deploy_result import DeployResult
+from ..models.deploy_type import DeployType
 from ..models.function_ref import FunctionRef
 from ..models.job_state_result import JobStateResult
 from ..models.job_status import JobStatus
-from ..models.undeploy_args import UndeployArgs
-from ..models.undeploy_result import UndeployResult
-from ..models.undeploy_type import UndeployType
 
 
-class UndeployJobStatus(WaylayBaseModel):
-    """UndeployJobStatus."""
+class DeployJobStatus(WaylayBaseModel):
+    """DeployJobStatus."""
 
-    type: UndeployType
+    type: DeployType
     state: JobStateResult
-    request: UndeployArgs
-    result: UndeployResult | None = None
+    request: DeployArgs
+    result: DeployResult | None = None
     created_at: datetime = Field(
         description="The timestamp of creation of this job", alias="createdAt"
     )
     created_by: StrictStr = Field(
         description="The user that created this job", alias="createdBy"
     )
     operation: StrictStr = Field(description="Request operation")
     function: FunctionRef | None = None
     job: JobStatus
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeploy_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,9 +22,12 @@
     """The result data for a completed undeployment job.."""
 
     deployment: StrictBool
     assets: StrictBool
     registration: StrictBool
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeploy_submitted_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_submitted_response_v2.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,9 +32,12 @@
     message: StrictStr
     links: JobHALLinks = Field(alias="_links")
     versions: List[Annotated[str, Field(strict=True)]] = Field(
         description="The versions for which undeployment and/or removal is initiated."
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/undeployed_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeployed_response_v2.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,9 +29,12 @@
 
     message: StrictStr
     versions: List[Annotated[str, Field(strict=True)]] = Field(
         description="The versions that where deprecated, undeployed and/or removed."
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/update_metadata_request_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/update_metadata_request_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.tag import Tag
 
 
-class UpdateMetadataRequestV2(WaylayBaseModel):
-    """UpdateMetadataRequestV2."""
+class UpdateMetadataRequestV1(WaylayBaseModel):
+    """UpdateMetadataRequestV1."""
 
     author: StrictStr | None = Field(
         default=None, description="The author of the function."
     )
     description: StrictStr | None = Field(
         default=None, description="A description of the function"
     )
@@ -52,9 +52,12 @@
     friendly_name: StrictStr | None = Field(
         default=None,
         description="Display title for this function.",
         alias="friendlyName",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/update_record.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/update_record.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,9 +36,12 @@
         default=None,
         description="The job id's of the corresponding jobs, if applicable.",
     )
     at: datetime
     by: StrictStr = Field(description="The user that initiated this operation.")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,9 +46,12 @@
     )
     operation: StrictStr = Field(description="Request operation")
     function: FunctionRef | None = None
     job: JobStatus | None = None
     failure_reason: FailureReason | None = Field(default=None, alias="failureReason")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,45 +7,31 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from datetime import datetime
-
 from pydantic import (
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.function_ref import FunctionRef
-from ..models.job_and_function_hal_link import JobAndFunctionHALLink
-from ..models.job_state_result import JobStateResult
-from ..models.verify_type import VerifyType
+from ..models.archive_format import ArchiveFormat
+from ..models.function_type import FunctionType
 
 
-class Verify1(WaylayBaseModel):
-    """Verify1."""
-
-    type: VerifyType
-    operation: StrictStr = Field(
-        description="The operation name for the background task."
-    )
-    id: StrictStr = Field(
-        description="The id of the background job, or the constant `_unknown_`"
-    )
-    state: JobStateResult
-    created_at: datetime = Field(
-        description="The creation time of this job", alias="createdAt"
-    )
-    created_by: StrictStr = Field(
-        description="The user that initiated this job", alias="createdBy"
-    )
-    function: FunctionRef | None = None
-    links: JobAndFunctionHALLink = Field(alias="_links")
+class RuntimeInfo(WaylayBaseModel):
+    """Runtime attributes that are the same for all versions of a runtime.."""
+
+    name: StrictStr
+    function_type: FunctionType = Field(alias="functionType")
+    archive_format: ArchiveFormat = Field(alias="archiveFormat")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify_args.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy_args.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,45 +12,55 @@
 from __future__ import annotations
 
 import re
 
 from pydantic import (
     ConfigDict,
     Field,
+    StrictBool,
     StrictStr,
     field_validator,
 )
 from typing_extensions import (
     Annotated,  # >=3.11
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 
-class VerifyArgs(WaylayBaseModel):
-    """Input arguments for an (openfaas) deployment verification job.."""
+class UndeployArgs(WaylayBaseModel):
+    """Input argument to an (openfaas) undeployment job for a function.."""
 
     namespace: StrictStr = Field(
         description="The (openfaas) namespace for the target function."
     )
     endpoint: StrictStr = Field(description="The (openfaas) endpoint service name")
     runtime_name: StrictStr = Field(alias="runtimeName")
     runtime_version: Annotated[str, Field(strict=True)] = Field(
         description="A semantic version with _exactly_ a `major`, `minor` and `patch` specifier. No `pre-release` or `build` identifiers are allowed. See https://semver.org",
         alias="runtimeVersion",
     )
-    revision: StrictStr = Field(
-        description="The revision hash of the current (draft) function revision"
+    revision: StrictStr | None = Field(
+        default=None,
+        description="The revision hash of the current (draft) function revision",
     )
+    is_native_plug: StrictBool = Field(
+        description="If true, the function is not expected to be deployed on openfaas.",
+        alias="isNativePlug",
+    )
+    delete_entity: StrictBool = Field(alias="deleteEntity")
 
     @field_validator("runtime_version")
     @classmethod
     def runtime_version_validate_regular_expression(cls, value):
         """Validate the regular expression."""
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
                 r"must validate the regular expression /^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify_job_status.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/undeploy1.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,34 +17,38 @@
     ConfigDict,
     Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.function_ref import FunctionRef
+from ..models.job_and_function_hal_link import JobAndFunctionHALLink
 from ..models.job_state_result import JobStateResult
-from ..models.job_status import JobStatus
-from ..models.verify_args import VerifyArgs
-from ..models.verify_result import VerifyResult
-from ..models.verify_type import VerifyType
+from ..models.undeploy_type import UndeployType
 
 
-class VerifyJobStatus(WaylayBaseModel):
-    """VerifyJobStatus."""
+class Undeploy1(WaylayBaseModel):
+    """Undeploy1."""
 
-    type: VerifyType
+    type: UndeployType
+    operation: StrictStr = Field(
+        description="The operation name for the background task."
+    )
+    id: StrictStr = Field(
+        description="The id of the background job, or the constant `_unknown_`"
+    )
     state: JobStateResult
-    request: VerifyArgs
-    result: VerifyResult | None = None
     created_at: datetime = Field(
-        description="The timestamp of creation of this job", alias="createdAt"
+        description="The creation time of this job", alias="createdAt"
     )
     created_by: StrictStr = Field(
-        description="The user that created this job", alias="createdBy"
+        description="The user that initiated this job", alias="createdBy"
     )
-    operation: StrictStr = Field(description="Request operation")
     function: FunctionRef | None = None
-    job: JobStatus
+    links: JobAndFunctionHALLink = Field(alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify_model_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_model_sync_response_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,9 +25,12 @@
     """Model Health Verified."""
 
     message: StrictStr
     entity: KfservingResponseV2
     result: VerifyResult
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify_plug_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_plug_sync_response_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,9 +25,12 @@
     """Plug Health Verified."""
 
     message: StrictStr
     entity: PlugResponseV2
     result: VerifyResult
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify_result.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,9 +27,12 @@
     healthy: StrictBool = Field(description="If true, the deployment check succeeded.")
     replicas: StrictFloat | StrictInt | None = Field(
         default=None,
         description="The number of replicas this function was running at the time of the check.",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/verify_webscript_sync_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/verify_webscript_sync_response_v2.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,9 +25,12 @@
     """Webscript Health Verified."""
 
     message: StrictStr
     entity: WebscriptResponseV2
     result: VerifyResult
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/waiting_children_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_children_event_sse.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,9 +25,12 @@
 class WaitingChildrenEventSSE(WaylayBaseModel):
     """A message that notifies a state change in a background job.."""
 
     event: WaitingChildrenEventSSEEvent
     data: JobEventResponseWaitingChildrenEventData
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/waiting_children_event_sse_event.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/batch_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,17 +7,27 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from enum import Enum
-
-
-class WaitingChildrenEventSSEEvent(str, Enum):
-    """The job queue event that trigged this message."""
-
-    WAITING_MINUS_CHILDREN = "waiting-children"
-
-    def __str__(self) -> str:
-        return str(self.value)
+from pydantic import (
+    ConfigDict,
+    Field,
+    StrictFloat,
+    StrictInt,
+)
+from waylay.sdk.api._models import BaseModel as WaylayBaseModel
+
+
+class BatchResult(WaylayBaseModel):
+    """BatchResult."""
+
+    job_count: StrictFloat | StrictInt | None = Field(default=None, alias="jobCount")
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
+    )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/waiting_event_data.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/error_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.queue_events import QueueEvents
 
+class ErrorResponse(WaylayBaseModel):
+    """ErrorResponse."""
 
-class WaitingEventData(WaylayBaseModel):
-    """WaitingEventData."""
-
-    prev: QueueEvents | None = None
+    error: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/waiting_event_sse.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/waiting_event_sse.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,9 +25,12 @@
 class WaitingEventSSE(WaylayBaseModel):
     """A message that notifies a state change in a background job.."""
 
     event: WaitingEventSSEEvent
     data: JobEventResponseWaitingEventData
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/webscript.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,9 +22,12 @@
 class Webscript(WaylayBaseModel):
     """Webscript."""
 
     event: HALLink | None = None
     webscript: HALLink
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/webscript1.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,19 @@
     ConfigDict,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.hal_link import HALLink
 
 
-class Webscript1(WaylayBaseModel):
-    """Webscript1."""
+class Model(WaylayBaseModel):
+    """Model."""
 
     event: HALLink | None = None
-    job: HALLink | None = None
-    webscript: HALLink
+    model: HALLink
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/webscript2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/runtime_params.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 
 """
 
 from __future__ import annotations
 
 from pydantic import (
     ConfigDict,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.hal_link import HALLink
 
+class RuntimeParams(WaylayBaseModel):
+    """RuntimeParams."""
 
-class Webscript2(WaylayBaseModel):
-    """Webscript2."""
-
-    job: HALLink | None = None
-    webscript: HALLink
+    name: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/webscript_manifest.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,9 +58,12 @@
         if not re.match(r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$", value):
             raise ValueError(
                 r"must validate the regular expression /^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)$/"
             )
         return value
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/webscript_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_response_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,9 +60,12 @@
     webscript: WebscriptManifest
     secret: StrictStr | None = Field(
         default=None,
         description="The secret for this webscript deployment. This is <code>null</code> when <code>allowHmac=false</code> in the webscript specificaton.",
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/webscript_response_with_invoke_link_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/webscript_response_with_invoke_link_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,9 +62,12 @@
     secret: StrictStr | None = Field(
         default=None,
         description="The secret for this webscript deployment. This is <code>null</code> when <code>allowHmac=false</code> in the webscript specificaton.",
     )
     links: InvokeHALLink | None = Field(default=None, alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/models/webscript_versions_response_v2.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/models/latest_webscripts_response_v2.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,31 +17,34 @@
     ConfigDict,
     Field,
     StrictFloat,
     StrictInt,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.webscript_response_with_invoke_link_v2 import (
-    WebscriptResponseWithInvokeLinkV2,
+from ..models.entity_with_links_i_webscript_response_with_invoke_link_v2 import (
+    EntityWithLinksIWebscriptResponseWithInvokeLinkV2,
 )
 
 
-class WebscriptVersionsResponseV2(WaylayBaseModel):
-    """Webscript Versions Found."""
+class LatestWebscriptsResponseV2(WaylayBaseModel):
+    """Webscripts Found."""
 
     limit: StrictFloat | StrictInt | None = Field(
         default=None, description="The page size used for this query result."
     )
     count: StrictFloat | StrictInt = Field(
         description="The total count of matching items, from which this result is one page."
     )
     page: StrictFloat | StrictInt | None = Field(
         default=None, description="The page number of a paged query result."
     )
-    entities: List[WebscriptResponseWithInvokeLinkV2] = Field(
+    entities: List[EntityWithLinksIWebscriptResponseWithInvokeLinkV2] = Field(
         description="The specification and deployment status of the queried functions"
     )
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/about_api.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/default_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,12 +20,13 @@
     return field_name
 
 
 class GetQuery(WaylayBaseModel):
     """Model for `get` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/jobs_api.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/jobs_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         StrictBool | None,
         Field(
             description="If set to <code>true</code>, the event stream will include events of the job's dependants. E.g., when subscribing to a verify job with `children=true`, you will also receive the events of the underlying build and deploy jobs. Defaults to <code>false</code>."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_events_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -63,14 +64,15 @@
     return field_name
 
 
 class GetQuery(WaylayBaseModel):
     """Model for `get` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -120,12 +122,13 @@
         Any | None,
         Field(
             description="Filter on jobs that created after the given timestamp or age"
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/models_api.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/models_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,28 +30,26 @@
 from ..models.job_type_schema import JobTypeSchema
 from ..models.rebuild_policy import RebuildPolicy
 from ..models.show_related_type import ShowRelatedType
 from ..models.status_filter import StatusFilter
 
 
 def _create_query_alias_for(field_name: str) -> str:
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "author":
         return "author"
     if field_name == "comment":
         return "comment"
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "deprecate_previous":
         return "deprecatePrevious"
     if field_name == "dry_run":
         return "dryRun"
     if field_name == "var_async":
         return "async"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     if field_name == "version":
         return "version"
     if field_name == "name":
         return "name"
     if field_name == "draft":
         return "draft"
     if field_name == "runtime":
@@ -60,38 +58,26 @@
         return "copy"
     return field_name
 
 
 class CreateQuery(WaylayBaseModel):
     """Model for `create` query parameters."""
 
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     author: Annotated[
         StrictStr | None,
         Field(
             description="Optionally changes the author metadata when updating a function."
         ),
     ] = None
     comment: Annotated[
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
     deprecate_previous: Annotated[
         DeprecatePreviousPolicy | None,
         Field(
             description="Set the cleanup policy used to automatically deprecate/delete previous versions."
         ),
     ] = None
     dry_run: Annotated[
@@ -102,14 +88,20 @@
     ] = None
     var_async: Annotated[
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
+    scale_to_zero: Annotated[
+        StrictBool | None,
+        Field(
+            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. Saves computing resources when the function is not to be used immediately."
+        ),
+    ] = None
     version: Annotated[
         Any | None,
         Field(
             description="If set, the function version will be an increment of the latest existing version that satisfies the `version` range. Note that this increment always takes precedence over an explicit `version` in the function manifest."
         ),
     ] = None
     name: Annotated[
@@ -134,52 +126,37 @@
         Any | None,
         Field(
             description="Indicates the _source_ of initial assets for a _new function_.  When using this query parameter, the request body does not need to contain assets, but any assets in the request body will overwrite the copied assets.  #### Selection of _assets_ source  * If set as `<sourceName>[@<sourceVersionRange>]`, the _new function_ will be created with copied assets of the selected _source function_. * If set as `!example`, a `runtime` query parameter is required, and the _new function_ will be initialized with assets of the _runtime example_.  #### Selection of the _source function_  When `<sourceVersionRange>` is a range (or is not given), the latest _published_ version (in that range) is used.  If no _published_ version exists, the latest _draft_ is selected.  If no versions in the range exist, a `404` _Not Found_ error is returned.  #### The `name` of the _new function_  If a `name` is NOT specified (either as query parameter, or in an optional manifest asset in the request body), the `name` of the _new function_ will be that of the _source function_.  #### The `version` of the _new function_  When the _target_ and _source_ name are equal, the `version` query parameters is defaulted to `<sourceVersionRange>` (`~<sourceVersionRange>` when it's an exact version)  The version of the _new function_ will be: * If a `version` is NOT specified (either as query parameter, in an optional manifest asset, or as `<sourceVersionRange>` _default_)    * a **patch increment** (`<major>.<minor>.<patch>+1`) of the latest **existing version** with the target `name`    * **`1.0.0`** otherwise  * If a `version` is specified:    * the **lowest version** in that range **if no existing version** is in that range.    * an **increment** of the latest existing version, **at the highest level** (_major_,_minor_,_patch_) allowed by that range.    * otherwise, if all allowed versions already exist, a **`409` _Duplicate_ error** is raised.  #### Deployment overrides  The new function will use the deployment overrides of the copied function, unless a _manifest_ was specified in the request body."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_create_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _delete_asset_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class DeleteAssetQuery(WaylayBaseModel):
     """Model for `delete_asset` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -198,14 +175,15 @@
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_delete_asset_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -222,14 +200,15 @@
         StrictBool | None,
         Field(
             description="If set to `true`, the result will be a listing of the files in the asset, annotated with metadata and validation report from the asset conditions of the functions runtime."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_archive_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -246,14 +225,15 @@
         StrictBool | None,
         Field(
             description="If set to `true`, the result will be a listing of the files in the asset, annotated with metadata and validation report from the asset conditions of the functions runtime."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_asset_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -278,14 +258,15 @@
         StrictBool | None,
         Field(
             description="Configures the inclusion of _deprecated_ versions when selecting latest versions per name. By default, deprecated versions are only considered when no other versions are available. If set to `true`, deprecated versions are **included**. If set to `false`, deprecated versions are **excluded**."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_latest_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -293,14 +274,15 @@
     return field_name
 
 
 class GetQuery(WaylayBaseModel):
     """Model for `get` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -350,14 +332,15 @@
         Any | None,
         Field(
             description="Filter on jobs that created after the given timestamp or age"
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_jobs_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -527,14 +510,15 @@
         ShowRelatedType | None,
         Field(
             description="Sets the representation of related function versions (like the _latest_ draft and/or published) in the response. - `embed`: as full summary representation (in `_embedded`). - `link`: as HAL link in (in `_links`). - `none`: omitted."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -656,14 +640,15 @@
     ] = None
     runtime: Annotated[
         List[StrictStr] | None,
         Field(description="Filter on the runtime of the function."),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_versions_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -680,14 +665,15 @@
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_patch_metadata_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -736,50 +722,45 @@
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_publish_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _rebuild_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "comment":
         return "comment"
     if field_name == "dry_run":
         return "dryRun"
     if field_name == "var_async":
         return "async"
     if field_name == "upgrade":
         return "upgrade"
     if field_name == "force_version":
         return "forceVersion"
     if field_name == "ignore_checks":
         return "ignoreChecks"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     if field_name == "skip_rebuild":
         return "skipRebuild"
     return field_name
 
 
 class RebuildQuery(WaylayBaseModel):
     """Model for `rebuild` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
-        ),
-    ] = None
     comment: Annotated[
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
     dry_run: Annotated[
@@ -808,22 +789,29 @@
     ] = None
     ignore_checks: Annotated[
         StrictBool | None,
         Field(
             description="If set to true, checks that normally prevent a rebuild are overriden. These checks include: * function state in `pending`, `running`, `failed` or `undeployed` * backoff period due to recent failures * usage of deprecated dependencies * running jobs on entity * the `dryRun` option"
         ),
     ] = None
+    scale_to_zero: Annotated[
+        StrictBool | None,
+        Field(
+            description="Indicates whether the function needs to be scaled down after successful (re-)deployment. If not set, the function is scaled to zero only if it was not active before this command."
+        ),
+    ] = None
     skip_rebuild: Annotated[
         StrictBool | None,
         Field(
             description="If set, the function will not be rebuild. Always uses the current runtime version when re-deploying/re-verifying the function."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_rebuild_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -864,14 +852,15 @@
         StrictBool | None,
         Field(
             description="If `true`, the `DELETE` operation * undeploys the (openfaas) function: it becomes no longer available for invocation. * does NOT remove the function from registry: it stays in an `undeployed` status.  All assets and definitions are retained, so the version can be restored later with a  _rebuild_ action.  If `false`, the `DELETE` operation * _only_ marks the plug function as _deprecated_, the function remains active but is removed from the default listings.   This also applies to _draft_ versions.  This parameter is incompatible with `force=true`.  If not set the default behaviour applies: * _draft_ versions are _undeployed_ and _removed_ from registry. * non-_draft_ versions are marked _deprecated_ only."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_remove_version_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -912,52 +901,37 @@
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_remove_versions_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _update_asset_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class UpdateAssetQuery(WaylayBaseModel):
     """Model for `update_asset` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -976,52 +950,37 @@
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_update_asset_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _update_assets_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class UpdateAssetsQuery(WaylayBaseModel):
     """Model for `update_assets` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -1040,44 +999,46 @@
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_update_assets_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _verify_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "var_async":
         return "async"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     return field_name
 
 
 class VerifyQuery(WaylayBaseModel):
     """Model for `verify` query parameters."""
 
-    scale_to_zero: Annotated[
+    var_async: Annotated[
         StrictBool | None,
         Field(
-            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
+            description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
-    var_async: Annotated[
+    scale_to_zero: Annotated[
         StrictBool | None,
         Field(
-            description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
+            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_verify_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/plugs_api.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/webscripts_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,35 +24,32 @@
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.archive_format import ArchiveFormat
 from ..models.deprecate_previous_policy import DeprecatePreviousPolicy
 from ..models.function_type import FunctionType
 from ..models.job_state_result import JobStateResult
 from ..models.job_type_schema import JobTypeSchema
-from ..models.plug_type import PlugType
 from ..models.rebuild_policy import RebuildPolicy
 from ..models.show_related_type import ShowRelatedType
 from ..models.status_filter import StatusFilter
 
 
 def _create_query_alias_for(field_name: str) -> str:
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "author":
         return "author"
     if field_name == "comment":
         return "comment"
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "deprecate_previous":
         return "deprecatePrevious"
     if field_name == "dry_run":
         return "dryRun"
     if field_name == "var_async":
         return "async"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     if field_name == "version":
         return "version"
     if field_name == "name":
         return "name"
     if field_name == "draft":
         return "draft"
     if field_name == "runtime":
@@ -61,38 +58,26 @@
         return "copy"
     return field_name
 
 
 class CreateQuery(WaylayBaseModel):
     """Model for `create` query parameters."""
 
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     author: Annotated[
         StrictStr | None,
         Field(
             description="Optionally changes the author metadata when updating a function."
         ),
     ] = None
     comment: Annotated[
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
     deprecate_previous: Annotated[
         DeprecatePreviousPolicy | None,
         Field(
             description="Set the cleanup policy used to automatically deprecate/delete previous versions."
         ),
     ] = None
     dry_run: Annotated[
@@ -103,14 +88,20 @@
     ] = None
     var_async: Annotated[
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
+    scale_to_zero: Annotated[
+        StrictBool | None,
+        Field(
+            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. Saves computing resources when the function is not to be used immediately."
+        ),
+    ] = None
     version: Annotated[
         Any | None,
         Field(
             description="If set, the function version will be an increment of the latest existing version that satisfies the `version` range. Note that this increment always takes precedence over an explicit `version` in the function manifest."
         ),
     ] = None
     name: Annotated[
@@ -135,52 +126,37 @@
         Any | None,
         Field(
             description="Indicates the _source_ of initial assets for a _new function_.  When using this query parameter, the request body does not need to contain assets, but any assets in the request body will overwrite the copied assets.  #### Selection of _assets_ source  * If set as `<sourceName>[@<sourceVersionRange>]`, the _new function_ will be created with copied assets of the selected _source function_. * If set as `!example`, a `runtime` query parameter is required, and the _new function_ will be initialized with assets of the _runtime example_.  #### Selection of the _source function_  When `<sourceVersionRange>` is a range (or is not given), the latest _published_ version (in that range) is used.  If no _published_ version exists, the latest _draft_ is selected.  If no versions in the range exist, a `404` _Not Found_ error is returned.  #### The `name` of the _new function_  If a `name` is NOT specified (either as query parameter, or in an optional manifest asset in the request body), the `name` of the _new function_ will be that of the _source function_.  #### The `version` of the _new function_  When the _target_ and _source_ name are equal, the `version` query parameters is defaulted to `<sourceVersionRange>` (`~<sourceVersionRange>` when it's an exact version)  The version of the _new function_ will be: * If a `version` is NOT specified (either as query parameter, in an optional manifest asset, or as `<sourceVersionRange>` _default_)    * a **patch increment** (`<major>.<minor>.<patch>+1`) of the latest **existing version** with the target `name`    * **`1.0.0`** otherwise  * If a `version` is specified:    * the **lowest version** in that range **if no existing version** is in that range.    * an **increment** of the latest existing version, **at the highest level** (_major_,_minor_,_patch_) allowed by that range.    * otherwise, if all allowed versions already exist, a **`409` _Duplicate_ error** is raised.  #### Deployment overrides  The new function will use the deployment overrides of the copied function, unless a _manifest_ was specified in the request body."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_create_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _delete_asset_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class DeleteAssetQuery(WaylayBaseModel):
     """Model for `delete_asset` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -199,14 +175,15 @@
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_delete_asset_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -223,14 +200,15 @@
         StrictBool | None,
         Field(
             description="If set to `true`, the result will be a listing of the files in the asset, annotated with metadata and validation report from the asset conditions of the functions runtime."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_archive_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -247,51 +225,48 @@
         StrictBool | None,
         Field(
             description="If set to `true`, the result will be a listing of the files in the asset, annotated with metadata and validation report from the asset conditions of the functions runtime."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_asset_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _get_latest_query_alias_for(field_name: str) -> str:
-    if field_name == "type":
-        return "type"
     if field_name == "include_draft":
         return "includeDraft"
     if field_name == "include_deprecated":
         return "includeDeprecated"
     return field_name
 
 
 class GetLatestQuery(WaylayBaseModel):
     """Model for `get_latest` query parameters."""
 
-    type: Annotated[
-        PlugType | None, Field(description="If set, filters on the type of plug.")
-    ] = None
     include_draft: Annotated[
         StrictBool | None,
         Field(
             description="Configures the inclusion of _draft_ versions when selecting latest versions per name. By default, draft versions are only considered when no other versions are available. If set to `true`, draft versions are **included**. If set to `false`, draft versions are **excluded**."
         ),
     ] = None
     include_deprecated: Annotated[
         StrictBool | None,
         Field(
             description="Configures the inclusion of _deprecated_ versions when selecting latest versions per name. By default, deprecated versions are only considered when no other versions are available. If set to `true`, deprecated versions are **included**. If set to `false`, deprecated versions are **excluded**."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_latest_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -299,14 +274,15 @@
     return field_name
 
 
 class GetQuery(WaylayBaseModel):
     """Model for `get` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -356,40 +332,31 @@
         Any | None,
         Field(
             description="Filter on jobs that created after the given timestamp or age"
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_jobs_query_alias_for,
         populate_by_name=True,
     )
 
 
-def _list_query_alias_for(field_name: str) -> str:
-    if field_name == "tags":
-        return "tags"
-    if field_name == "type":
-        return "type"
+def _list_versions_query_alias_for(field_name: str) -> str:
     if field_name == "limit":
         return "limit"
     if field_name == "page":
         return "page"
-    if field_name == "include_draft":
-        return "includeDraft"
-    if field_name == "include_deprecated":
-        return "includeDeprecated"
     if field_name == "deprecated":
         return "deprecated"
     if field_name == "draft":
         return "draft"
-    if field_name == "name_version":
-        return "nameVersion"
     if field_name == "version":
         return "version"
     if field_name == "status":
         return "status"
     if field_name == "runtime_version":
         return "runtimeVersion"
     if field_name == "created_by":
@@ -400,39 +367,24 @@
         return "createdBefore"
     if field_name == "created_after":
         return "createdAfter"
     if field_name == "updated_before":
         return "updatedBefore"
     if field_name == "updated_after":
         return "updatedAfter"
-    if field_name == "name":
-        return "name"
     if field_name == "archive_format":
         return "archiveFormat"
     if field_name == "runtime":
         return "runtime"
-    if field_name == "latest":
-        return "latest"
-    if field_name == "show_related":
-        return "showRelated"
     return field_name
 
 
-class ListQuery(WaylayBaseModel):
-    """Model for `list` query parameters."""
+class ListVersionsQuery(WaylayBaseModel):
+    """Model for `list_versions` query parameters."""
 
-    tags: Annotated[
-        Any | None,
-        Field(
-            description="Filter on the tags of the item. Can be a single tag, or a list of tags. When multiple tags are specified, an item must have all of the tags to be selected."
-        ),
-    ] = None
-    type: Annotated[
-        PlugType | None, Field(description="If set, filters on the type of plug.")
-    ] = None
     limit: Annotated[
         Annotated[float, Field(strict=True, ge=0)]
         | Annotated[int, Field(strict=True, ge=0)]
         | None,
         Field(
             description="The maximum number of items to be return from this query. Has a deployment-defined default and maximum value."
         ),
@@ -441,40 +393,22 @@
         Annotated[float, Field(strict=True, ge=0)]
         | Annotated[int, Field(strict=True, ge=0)]
         | None,
         Field(
             description="The number of pages to skip when returning result to this query."
         ),
     ] = None
-    include_draft: Annotated[
-        StrictBool | None,
-        Field(
-            description="Configures the inclusion of _draft_ versions when selecting latest versions per name. By default, draft versions are only considered when no other versions are available. If set to `true`, draft versions are **included**. If set to `false`, draft versions are **excluded**."
-        ),
-    ] = None
-    include_deprecated: Annotated[
-        StrictBool | None,
-        Field(
-            description="Configures the inclusion of _deprecated_ versions when selecting latest versions per name. By default, deprecated versions are only considered when no other versions are available. If set to `true`, deprecated versions are **included**. If set to `false`, deprecated versions are **excluded**."
-        ),
-    ] = None
     deprecated: Annotated[
         StrictBool | None,
         Field(description="Filter on the deprecation status of the function."),
     ] = None
     draft: Annotated[
         StrictBool | None,
         Field(description="Filter on the draft status of the function."),
     ] = None
-    name_version: Annotated[
-        List[Annotated[str, Field(strict=True)]] | None,
-        Field(
-            description="Filter on exact `{name}@{version}` functions. Using this filter implies a `latest=false` default, returning multiple versions of the same named versions if they are filtered."
-        ),
-    ] = None
     version: Annotated[
         StrictStr | None,
         Field(
             description="Filter on the version of the function (case-sensitive, supports wildcards)."
         ),
     ] = None
     status: Annotated[
@@ -518,60 +452,47 @@
     ] = None
     updated_after: Annotated[
         Any | None,
         Field(
             description="Filter on funtions that were updated after the given timestamp or age."
         ),
     ] = None
-    name: Annotated[
-        StrictStr | None,
-        Field(
-            description="Filter on the name of the function. This is case-insensitive and supports wild-cards `?` (any one character) and `*` (any sequence of characters)."
-        ),
-    ] = None
     archive_format: Annotated[
         List[ArchiveFormat] | None,
         Field(description="Filter on the archive format of the function."),
     ] = None
     runtime: Annotated[
         List[StrictStr] | None,
         Field(description="Filter on the runtime of the function."),
     ] = None
-    latest: Annotated[
-        StrictBool | None,
-        Field(
-            description="When `true`, only the latest version per function name is returned. If set to `false`, multiple versions per named function can be returned. Defaults to `true`, except when specific versions are selected with the `nameVersion` filter."
-        ),
-    ] = None
-    show_related: Annotated[
-        ShowRelatedType | None,
-        Field(
-            description="Sets the representation of related function versions (like the _latest_ draft and/or published) in the response. - `embed`: as full summary representation (in `_embedded`). - `link`: as HAL link in (in `_links`). - `none`: omitted."
-        ),
-    ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
-        alias_generator=_list_query_alias_for,
+        alias_generator=_list_versions_query_alias_for,
         populate_by_name=True,
     )
 
 
-def _list_versions_query_alias_for(field_name: str) -> str:
-    if field_name == "tags":
-        return "tags"
+def _list_query_alias_for(field_name: str) -> str:
     if field_name == "limit":
         return "limit"
     if field_name == "page":
         return "page"
+    if field_name == "include_draft":
+        return "includeDraft"
+    if field_name == "include_deprecated":
+        return "includeDeprecated"
     if field_name == "deprecated":
         return "deprecated"
     if field_name == "draft":
         return "draft"
+    if field_name == "name_version":
+        return "nameVersion"
     if field_name == "version":
         return "version"
     if field_name == "status":
         return "status"
     if field_name == "runtime_version":
         return "runtimeVersion"
     if field_name == "created_by":
@@ -582,30 +503,30 @@
         return "createdBefore"
     if field_name == "created_after":
         return "createdAfter"
     if field_name == "updated_before":
         return "updatedBefore"
     if field_name == "updated_after":
         return "updatedAfter"
+    if field_name == "name":
+        return "name"
     if field_name == "archive_format":
         return "archiveFormat"
     if field_name == "runtime":
         return "runtime"
+    if field_name == "latest":
+        return "latest"
+    if field_name == "show_related":
+        return "showRelated"
     return field_name
 
 
-class ListVersionsQuery(WaylayBaseModel):
-    """Model for `list_versions` query parameters."""
+class ListQuery(WaylayBaseModel):
+    """Model for `list` query parameters."""
 
-    tags: Annotated[
-        Any | None,
-        Field(
-            description="Filter on the tags of the item. Can be a single tag, or a list of tags. When multiple tags are specified, an item must have all of the tags to be selected."
-        ),
-    ] = None
     limit: Annotated[
         Annotated[float, Field(strict=True, ge=0)]
         | Annotated[int, Field(strict=True, ge=0)]
         | None,
         Field(
             description="The maximum number of items to be return from this query. Has a deployment-defined default and maximum value."
         ),
@@ -614,22 +535,40 @@
         Annotated[float, Field(strict=True, ge=0)]
         | Annotated[int, Field(strict=True, ge=0)]
         | None,
         Field(
             description="The number of pages to skip when returning result to this query."
         ),
     ] = None
+    include_draft: Annotated[
+        StrictBool | None,
+        Field(
+            description="Configures the inclusion of _draft_ versions when selecting latest versions per name. By default, draft versions are only considered when no other versions are available. If set to `true`, draft versions are **included**. If set to `false`, draft versions are **excluded**."
+        ),
+    ] = None
+    include_deprecated: Annotated[
+        StrictBool | None,
+        Field(
+            description="Configures the inclusion of _deprecated_ versions when selecting latest versions per name. By default, deprecated versions are only considered when no other versions are available. If set to `true`, deprecated versions are **included**. If set to `false`, deprecated versions are **excluded**."
+        ),
+    ] = None
     deprecated: Annotated[
         StrictBool | None,
         Field(description="Filter on the deprecation status of the function."),
     ] = None
     draft: Annotated[
         StrictBool | None,
         Field(description="Filter on the draft status of the function."),
     ] = None
+    name_version: Annotated[
+        List[Annotated[str, Field(strict=True)]] | None,
+        Field(
+            description="Filter on exact `{name}@{version}` functions. Using this filter implies a `latest=false` default, returning multiple versions of the same named versions if they are filtered."
+        ),
+    ] = None
     version: Annotated[
         StrictStr | None,
         Field(
             description="Filter on the version of the function (case-sensitive, supports wildcards)."
         ),
     ] = None
     status: Annotated[
@@ -673,51 +612,46 @@
     ] = None
     updated_after: Annotated[
         Any | None,
         Field(
             description="Filter on funtions that were updated after the given timestamp or age."
         ),
     ] = None
+    name: Annotated[
+        StrictStr | None,
+        Field(
+            description="Filter on the name of the function. This is case-insensitive and supports wild-cards `?` (any one character) and `*` (any sequence of characters)."
+        ),
+    ] = None
     archive_format: Annotated[
         List[ArchiveFormat] | None,
         Field(description="Filter on the archive format of the function."),
     ] = None
     runtime: Annotated[
         List[StrictStr] | None,
         Field(description="Filter on the runtime of the function."),
     ] = None
-
-    model_config = ConfigDict(
-        protected_namespaces=(),
-        extra="allow",
-        alias_generator=_list_versions_query_alias_for,
-        populate_by_name=True,
-    )
-
-
-def _patch_interface_query_alias_for(field_name: str) -> str:
-    if field_name == "comment":
-        return "comment"
-    return field_name
-
-
-class PatchInterfaceQuery(WaylayBaseModel):
-    """Model for `patch_interface` query parameters."""
-
-    comment: Annotated[
-        StrictStr | None,
+    latest: Annotated[
+        StrictBool | None,
         Field(
-            description="An optional user-specified comment corresponding to the operation."
+            description="When `true`, only the latest version per function name is returned. If set to `false`, multiple versions per named function can be returned. Defaults to `true`, except when specific versions are selected with the `nameVersion` filter."
+        ),
+    ] = None
+    show_related: Annotated[
+        ShowRelatedType | None,
+        Field(
+            description="Sets the representation of related function versions (like the _latest_ draft and/or published) in the response. - `embed`: as full summary representation (in `_embedded`). - `link`: as HAL link in (in `_links`). - `none`: omitted."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
-        alias_generator=_patch_interface_query_alias_for,
+        alias_generator=_list_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _patch_metadata_query_alias_for(field_name: str) -> str:
     if field_name == "comment":
         return "comment"
@@ -731,14 +665,15 @@
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_patch_metadata_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -787,50 +722,45 @@
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_publish_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _rebuild_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "comment":
         return "comment"
     if field_name == "dry_run":
         return "dryRun"
     if field_name == "var_async":
         return "async"
     if field_name == "upgrade":
         return "upgrade"
     if field_name == "force_version":
         return "forceVersion"
     if field_name == "ignore_checks":
         return "ignoreChecks"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     if field_name == "skip_rebuild":
         return "skipRebuild"
     return field_name
 
 
 class RebuildQuery(WaylayBaseModel):
     """Model for `rebuild` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
-        ),
-    ] = None
     comment: Annotated[
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
     dry_run: Annotated[
@@ -859,22 +789,29 @@
     ] = None
     ignore_checks: Annotated[
         StrictBool | None,
         Field(
             description="If set to true, checks that normally prevent a rebuild are overriden. These checks include: * function state in `pending`, `running`, `failed` or `undeployed` * backoff period due to recent failures * usage of deprecated dependencies * running jobs on entity * the `dryRun` option"
         ),
     ] = None
+    scale_to_zero: Annotated[
+        StrictBool | None,
+        Field(
+            description="Indicates whether the function needs to be scaled down after successful (re-)deployment. If not set, the function is scaled to zero only if it was not active before this command."
+        ),
+    ] = None
     skip_rebuild: Annotated[
         StrictBool | None,
         Field(
             description="If set, the function will not be rebuild. Always uses the current runtime version when re-deploying/re-verifying the function."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_rebuild_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -904,25 +841,26 @@
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
     force: Annotated[
         StrictBool | None,
         Field(
-            description="If <code>true</code>, the plug version(s) will be undeployed and removed. Otherwise, the plug version(s) will only be <code>deprecated</code>, i.e removed from regular listings."
+            description="If <code>true</code>, the function version will be immediately undeployed and removed.  Otherwise, the removal will be delayed to allow current invocations to end. During that period, the function is marked _deprecated_."
         ),
     ] = None
     undeploy: Annotated[
         StrictBool | None,
         Field(
-            description="If `true`, the `DELETE` operation * undeploys the (openfaas) function for the plug: it becomes no longer available for invocation. * does NOT remove the plug from registry: it stays in an `undeployed` status.  All assets and definitions are retained, so the plug can be restored later with a  _rebuild_ action.  If `false`, the `DELETE` operation * _only_ marks the plug version(s) as _deprecated_: the plug remains active but is removed from the default listings.   This also applies to _draft_ versions.  This parameter is incompatible with `force=true`.  If not set the default behaviour applies: * _draft_ versions are _undeployed_ and _removed_ from registry. * non-_draft_ versions are marked _deprecated_ only."
+            description="If `true`, the `DELETE` operation * undeploys the (openfaas) function: it becomes no longer available for invocation. * does NOT remove the function from registry: it stays in an `undeployed` status.  All assets and definitions are retained, so the version can be restored later with a  _rebuild_ action.  If `false`, the `DELETE` operation * _only_ marks the plug function as _deprecated_, the function remains active but is removed from the default listings.   This also applies to _draft_ versions.  This parameter is incompatible with `force=true`.  If not set the default behaviour applies: * _draft_ versions are _undeployed_ and _removed_ from registry. * non-_draft_ versions are marked _deprecated_ only."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_remove_version_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -952,63 +890,48 @@
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
     force: Annotated[
         StrictBool | None,
         Field(
-            description="If <code>true</code>, the plug version(s) will be undeployed and removed. Otherwise, the plug version(s) will only be <code>deprecated</code>, i.e removed from regular listings."
+            description="If <code>true</code>, the function version will be immediately undeployed and removed.  Otherwise, the removal will be delayed to allow current invocations to end. During that period, the function is marked _deprecated_."
         ),
     ] = None
     undeploy: Annotated[
         StrictBool | None,
         Field(
-            description="If `true`, the `DELETE` operation * undeploys the (openfaas) function for the plug: it becomes no longer available for invocation. * does NOT remove the plug from registry: it stays in an `undeployed` status.  All assets and definitions are retained, so the plug can be restored later with a  _rebuild_ action.  If `false`, the `DELETE` operation * _only_ marks the plug version(s) as _deprecated_: the plug remains active but is removed from the default listings.   This also applies to _draft_ versions.  This parameter is incompatible with `force=true`.  If not set the default behaviour applies: * _draft_ versions are _undeployed_ and _removed_ from registry. * non-_draft_ versions are marked _deprecated_ only."
+            description="If `true`, the `DELETE` operation * undeploys the (openfaas) function: it becomes no longer available for invocation. * does NOT remove the function from registry: it stays in an `undeployed` status.  All assets and definitions are retained, so the version can be restored later with a  _rebuild_ action.  If `false`, the `DELETE` operation * _only_ marks the plug function as _deprecated_, the function remains active but is removed from the default listings.   This also applies to _draft_ versions.  This parameter is incompatible with `force=true`.  If not set the default behaviour applies: * _draft_ versions are _undeployed_ and _removed_ from registry. * non-_draft_ versions are marked _deprecated_ only."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_remove_versions_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _update_asset_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class UpdateAssetQuery(WaylayBaseModel):
     """Model for `update_asset` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -1027,52 +950,37 @@
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_update_asset_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _update_assets_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class UpdateAssetsQuery(WaylayBaseModel):
     """Model for `update_assets` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -1091,44 +999,46 @@
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_update_assets_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _verify_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "var_async":
         return "async"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     return field_name
 
 
 class VerifyQuery(WaylayBaseModel):
     """Model for `verify` query parameters."""
 
-    scale_to_zero: Annotated[
+    var_async: Annotated[
         StrictBool | None,
         Field(
-            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
+            description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
-    var_async: Annotated[
+    scale_to_zero: Annotated[
         StrictBool | None,
         Field(
-            description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
+            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_verify_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/runtimes_api.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/runtimes_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         StrictBool | None,
         Field(
             description="If set to `true`, deprecated runtimes will be included in the query."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_example_archive_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -81,14 +82,15 @@
         StrictBool | None,
         Field(
             description="If set to `true`, deprecated runtimes will be included in the query."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_example_asset_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -129,14 +131,15 @@
         List[ArchiveFormat] | None,
         Field(
             description="If set, filters on the <code>archiveFormat</code> of a runtime. Uses an exact match."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_latest_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -153,14 +156,15 @@
         StrictBool | None,
         Field(
             description="If set to `true`, deprecated runtimes will be included in the query."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -217,14 +221,15 @@
         List[ArchiveFormat] | None,
         Field(
             description="If set, filters on the <code>archiveFormat</code> of a runtime. Uses an exact match."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -273,12 +278,13 @@
         List[ArchiveFormat] | None,
         Field(
             description="If set, filters on the <code>archiveFormat</code> of a runtime. Uses an exact match."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_versions_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/schemas_api.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/schemas_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     return field_name
 
 
 class GetByRoleQuery(WaylayBaseModel):
     """Model for `get_by_role` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_by_role_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -35,12 +36,13 @@
     return field_name
 
 
 class GetQuery(WaylayBaseModel):
     """Model for `get` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay/services/registry/queries/webscripts_api.py` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay/services/registry/queries/plugs_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,34 +24,33 @@
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.archive_format import ArchiveFormat
 from ..models.deprecate_previous_policy import DeprecatePreviousPolicy
 from ..models.function_type import FunctionType
 from ..models.job_state_result import JobStateResult
 from ..models.job_type_schema import JobTypeSchema
+from ..models.plug_type import PlugType
 from ..models.rebuild_policy import RebuildPolicy
 from ..models.show_related_type import ShowRelatedType
 from ..models.status_filter import StatusFilter
 
 
 def _create_query_alias_for(field_name: str) -> str:
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "author":
         return "author"
     if field_name == "comment":
         return "comment"
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "deprecate_previous":
         return "deprecatePrevious"
     if field_name == "dry_run":
         return "dryRun"
     if field_name == "var_async":
         return "async"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     if field_name == "version":
         return "version"
     if field_name == "name":
         return "name"
     if field_name == "draft":
         return "draft"
     if field_name == "runtime":
@@ -60,38 +59,26 @@
         return "copy"
     return field_name
 
 
 class CreateQuery(WaylayBaseModel):
     """Model for `create` query parameters."""
 
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     author: Annotated[
         StrictStr | None,
         Field(
             description="Optionally changes the author metadata when updating a function."
         ),
     ] = None
     comment: Annotated[
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
     deprecate_previous: Annotated[
         DeprecatePreviousPolicy | None,
         Field(
             description="Set the cleanup policy used to automatically deprecate/delete previous versions."
         ),
     ] = None
     dry_run: Annotated[
@@ -102,14 +89,20 @@
     ] = None
     var_async: Annotated[
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
+    scale_to_zero: Annotated[
+        StrictBool | None,
+        Field(
+            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. Saves computing resources when the function is not to be used immediately."
+        ),
+    ] = None
     version: Annotated[
         Any | None,
         Field(
             description="If set, the function version will be an increment of the latest existing version that satisfies the `version` range. Note that this increment always takes precedence over an explicit `version` in the function manifest."
         ),
     ] = None
     name: Annotated[
@@ -134,52 +127,37 @@
         Any | None,
         Field(
             description="Indicates the _source_ of initial assets for a _new function_.  When using this query parameter, the request body does not need to contain assets, but any assets in the request body will overwrite the copied assets.  #### Selection of _assets_ source  * If set as `<sourceName>[@<sourceVersionRange>]`, the _new function_ will be created with copied assets of the selected _source function_. * If set as `!example`, a `runtime` query parameter is required, and the _new function_ will be initialized with assets of the _runtime example_.  #### Selection of the _source function_  When `<sourceVersionRange>` is a range (or is not given), the latest _published_ version (in that range) is used.  If no _published_ version exists, the latest _draft_ is selected.  If no versions in the range exist, a `404` _Not Found_ error is returned.  #### The `name` of the _new function_  If a `name` is NOT specified (either as query parameter, or in an optional manifest asset in the request body), the `name` of the _new function_ will be that of the _source function_.  #### The `version` of the _new function_  When the _target_ and _source_ name are equal, the `version` query parameters is defaulted to `<sourceVersionRange>` (`~<sourceVersionRange>` when it's an exact version)  The version of the _new function_ will be: * If a `version` is NOT specified (either as query parameter, in an optional manifest asset, or as `<sourceVersionRange>` _default_)    * a **patch increment** (`<major>.<minor>.<patch>+1`) of the latest **existing version** with the target `name`    * **`1.0.0`** otherwise  * If a `version` is specified:    * the **lowest version** in that range **if no existing version** is in that range.    * an **increment** of the latest existing version, **at the highest level** (_major_,_minor_,_patch_) allowed by that range.    * otherwise, if all allowed versions already exist, a **`409` _Duplicate_ error** is raised.  #### Deployment overrides  The new function will use the deployment overrides of the copied function, unless a _manifest_ was specified in the request body."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_create_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _delete_asset_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class DeleteAssetQuery(WaylayBaseModel):
     """Model for `delete_asset` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -198,14 +176,15 @@
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_delete_asset_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -222,14 +201,15 @@
         StrictBool | None,
         Field(
             description="If set to `true`, the result will be a listing of the files in the asset, annotated with metadata and validation report from the asset conditions of the functions runtime."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_archive_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -246,46 +226,53 @@
         StrictBool | None,
         Field(
             description="If set to `true`, the result will be a listing of the files in the asset, annotated with metadata and validation report from the asset conditions of the functions runtime."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_asset_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _get_latest_query_alias_for(field_name: str) -> str:
+    if field_name == "type":
+        return "type"
     if field_name == "include_draft":
         return "includeDraft"
     if field_name == "include_deprecated":
         return "includeDeprecated"
     return field_name
 
 
 class GetLatestQuery(WaylayBaseModel):
     """Model for `get_latest` query parameters."""
 
+    type: Annotated[
+        PlugType | None, Field(description="If set, filters on the type of plug.")
+    ] = None
     include_draft: Annotated[
         StrictBool | None,
         Field(
             description="Configures the inclusion of _draft_ versions when selecting latest versions per name. By default, draft versions are only considered when no other versions are available. If set to `true`, draft versions are **included**. If set to `false`, draft versions are **excluded**."
         ),
     ] = None
     include_deprecated: Annotated[
         StrictBool | None,
         Field(
             description="Configures the inclusion of _deprecated_ versions when selecting latest versions per name. By default, deprecated versions are only considered when no other versions are available. If set to `true`, deprecated versions are **included**. If set to `false`, deprecated versions are **excluded**."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_latest_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -293,14 +280,15 @@
     return field_name
 
 
 class GetQuery(WaylayBaseModel):
     """Model for `get` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -350,30 +338,41 @@
         Any | None,
         Field(
             description="Filter on jobs that created after the given timestamp or age"
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_jobs_query_alias_for,
         populate_by_name=True,
     )
 
 
-def _list_versions_query_alias_for(field_name: str) -> str:
+def _list_query_alias_for(field_name: str) -> str:
+    if field_name == "tags":
+        return "tags"
+    if field_name == "type":
+        return "type"
     if field_name == "limit":
         return "limit"
     if field_name == "page":
         return "page"
+    if field_name == "include_draft":
+        return "includeDraft"
+    if field_name == "include_deprecated":
+        return "includeDeprecated"
     if field_name == "deprecated":
         return "deprecated"
     if field_name == "draft":
         return "draft"
+    if field_name == "name_version":
+        return "nameVersion"
     if field_name == "version":
         return "version"
     if field_name == "status":
         return "status"
     if field_name == "runtime_version":
         return "runtimeVersion"
     if field_name == "created_by":
@@ -384,24 +383,39 @@
         return "createdBefore"
     if field_name == "created_after":
         return "createdAfter"
     if field_name == "updated_before":
         return "updatedBefore"
     if field_name == "updated_after":
         return "updatedAfter"
+    if field_name == "name":
+        return "name"
     if field_name == "archive_format":
         return "archiveFormat"
     if field_name == "runtime":
         return "runtime"
+    if field_name == "latest":
+        return "latest"
+    if field_name == "show_related":
+        return "showRelated"
     return field_name
 
 
-class ListVersionsQuery(WaylayBaseModel):
-    """Model for `list_versions` query parameters."""
+class ListQuery(WaylayBaseModel):
+    """Model for `list` query parameters."""
 
+    tags: Annotated[
+        Any | None,
+        Field(
+            description="Filter on the tags of the item. Can be a single tag, or a list of tags. When multiple tags are specified, an item must have all of the tags to be selected."
+        ),
+    ] = None
+    type: Annotated[
+        PlugType | None, Field(description="If set, filters on the type of plug.")
+    ] = None
     limit: Annotated[
         Annotated[float, Field(strict=True, ge=0)]
         | Annotated[int, Field(strict=True, ge=0)]
         | None,
         Field(
             description="The maximum number of items to be return from this query. Has a deployment-defined default and maximum value."
         ),
@@ -410,22 +424,40 @@
         Annotated[float, Field(strict=True, ge=0)]
         | Annotated[int, Field(strict=True, ge=0)]
         | None,
         Field(
             description="The number of pages to skip when returning result to this query."
         ),
     ] = None
+    include_draft: Annotated[
+        StrictBool | None,
+        Field(
+            description="Configures the inclusion of _draft_ versions when selecting latest versions per name. By default, draft versions are only considered when no other versions are available. If set to `true`, draft versions are **included**. If set to `false`, draft versions are **excluded**."
+        ),
+    ] = None
+    include_deprecated: Annotated[
+        StrictBool | None,
+        Field(
+            description="Configures the inclusion of _deprecated_ versions when selecting latest versions per name. By default, deprecated versions are only considered when no other versions are available. If set to `true`, deprecated versions are **included**. If set to `false`, deprecated versions are **excluded**."
+        ),
+    ] = None
     deprecated: Annotated[
         StrictBool | None,
         Field(description="Filter on the deprecation status of the function."),
     ] = None
     draft: Annotated[
         StrictBool | None,
         Field(description="Filter on the draft status of the function."),
     ] = None
+    name_version: Annotated[
+        List[Annotated[str, Field(strict=True)]] | None,
+        Field(
+            description="Filter on exact `{name}@{version}` functions. Using this filter implies a `latest=false` default, returning multiple versions of the same named versions if they are filtered."
+        ),
+    ] = None
     version: Annotated[
         StrictStr | None,
         Field(
             description="Filter on the version of the function (case-sensitive, supports wildcards)."
         ),
     ] = None
     status: Annotated[
@@ -469,46 +501,61 @@
     ] = None
     updated_after: Annotated[
         Any | None,
         Field(
             description="Filter on funtions that were updated after the given timestamp or age."
         ),
     ] = None
+    name: Annotated[
+        StrictStr | None,
+        Field(
+            description="Filter on the name of the function. This is case-insensitive and supports wild-cards `?` (any one character) and `*` (any sequence of characters)."
+        ),
+    ] = None
     archive_format: Annotated[
         List[ArchiveFormat] | None,
         Field(description="Filter on the archive format of the function."),
     ] = None
     runtime: Annotated[
         List[StrictStr] | None,
         Field(description="Filter on the runtime of the function."),
     ] = None
+    latest: Annotated[
+        StrictBool | None,
+        Field(
+            description="When `true`, only the latest version per function name is returned. If set to `false`, multiple versions per named function can be returned. Defaults to `true`, except when specific versions are selected with the `nameVersion` filter."
+        ),
+    ] = None
+    show_related: Annotated[
+        ShowRelatedType | None,
+        Field(
+            description="Sets the representation of related function versions (like the _latest_ draft and/or published) in the response. - `embed`: as full summary representation (in `_embedded`). - `link`: as HAL link in (in `_links`). - `none`: omitted."
+        ),
+    ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
-        alias_generator=_list_versions_query_alias_for,
+        alias_generator=_list_query_alias_for,
         populate_by_name=True,
     )
 
 
-def _list_query_alias_for(field_name: str) -> str:
+def _list_versions_query_alias_for(field_name: str) -> str:
+    if field_name == "tags":
+        return "tags"
     if field_name == "limit":
         return "limit"
     if field_name == "page":
         return "page"
-    if field_name == "include_draft":
-        return "includeDraft"
-    if field_name == "include_deprecated":
-        return "includeDeprecated"
     if field_name == "deprecated":
         return "deprecated"
     if field_name == "draft":
         return "draft"
-    if field_name == "name_version":
-        return "nameVersion"
     if field_name == "version":
         return "version"
     if field_name == "status":
         return "status"
     if field_name == "runtime_version":
         return "runtimeVersion"
     if field_name == "created_by":
@@ -519,30 +566,30 @@
         return "createdBefore"
     if field_name == "created_after":
         return "createdAfter"
     if field_name == "updated_before":
         return "updatedBefore"
     if field_name == "updated_after":
         return "updatedAfter"
-    if field_name == "name":
-        return "name"
     if field_name == "archive_format":
         return "archiveFormat"
     if field_name == "runtime":
         return "runtime"
-    if field_name == "latest":
-        return "latest"
-    if field_name == "show_related":
-        return "showRelated"
     return field_name
 
 
-class ListQuery(WaylayBaseModel):
-    """Model for `list` query parameters."""
+class ListVersionsQuery(WaylayBaseModel):
+    """Model for `list_versions` query parameters."""
 
+    tags: Annotated[
+        Any | None,
+        Field(
+            description="Filter on the tags of the item. Can be a single tag, or a list of tags. When multiple tags are specified, an item must have all of the tags to be selected."
+        ),
+    ] = None
     limit: Annotated[
         Annotated[float, Field(strict=True, ge=0)]
         | Annotated[int, Field(strict=True, ge=0)]
         | None,
         Field(
             description="The maximum number of items to be return from this query. Has a deployment-defined default and maximum value."
         ),
@@ -551,40 +598,22 @@
         Annotated[float, Field(strict=True, ge=0)]
         | Annotated[int, Field(strict=True, ge=0)]
         | None,
         Field(
             description="The number of pages to skip when returning result to this query."
         ),
     ] = None
-    include_draft: Annotated[
-        StrictBool | None,
-        Field(
-            description="Configures the inclusion of _draft_ versions when selecting latest versions per name. By default, draft versions are only considered when no other versions are available. If set to `true`, draft versions are **included**. If set to `false`, draft versions are **excluded**."
-        ),
-    ] = None
-    include_deprecated: Annotated[
-        StrictBool | None,
-        Field(
-            description="Configures the inclusion of _deprecated_ versions when selecting latest versions per name. By default, deprecated versions are only considered when no other versions are available. If set to `true`, deprecated versions are **included**. If set to `false`, deprecated versions are **excluded**."
-        ),
-    ] = None
     deprecated: Annotated[
         StrictBool | None,
         Field(description="Filter on the deprecation status of the function."),
     ] = None
     draft: Annotated[
         StrictBool | None,
         Field(description="Filter on the draft status of the function."),
     ] = None
-    name_version: Annotated[
-        List[Annotated[str, Field(strict=True)]] | None,
-        Field(
-            description="Filter on exact `{name}@{version}` functions. Using this filter implies a `latest=false` default, returning multiple versions of the same named versions if they are filtered."
-        ),
-    ] = None
     version: Annotated[
         StrictStr | None,
         Field(
             description="Filter on the version of the function (case-sensitive, supports wildcards)."
         ),
     ] = None
     status: Annotated[
@@ -628,45 +657,53 @@
     ] = None
     updated_after: Annotated[
         Any | None,
         Field(
             description="Filter on funtions that were updated after the given timestamp or age."
         ),
     ] = None
-    name: Annotated[
-        StrictStr | None,
-        Field(
-            description="Filter on the name of the function. This is case-insensitive and supports wild-cards `?` (any one character) and `*` (any sequence of characters)."
-        ),
-    ] = None
     archive_format: Annotated[
         List[ArchiveFormat] | None,
         Field(description="Filter on the archive format of the function."),
     ] = None
     runtime: Annotated[
         List[StrictStr] | None,
         Field(description="Filter on the runtime of the function."),
     ] = None
-    latest: Annotated[
-        StrictBool | None,
-        Field(
-            description="When `true`, only the latest version per function name is returned. If set to `false`, multiple versions per named function can be returned. Defaults to `true`, except when specific versions are selected with the `nameVersion` filter."
-        ),
-    ] = None
-    show_related: Annotated[
-        ShowRelatedType | None,
+
+    model_config = ConfigDict(
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
+        alias_generator=_list_versions_query_alias_for,
+        populate_by_name=True,
+    )
+
+
+def _patch_interface_query_alias_for(field_name: str) -> str:
+    if field_name == "comment":
+        return "comment"
+    return field_name
+
+
+class PatchInterfaceQuery(WaylayBaseModel):
+    """Model for `patch_interface` query parameters."""
+
+    comment: Annotated[
+        StrictStr | None,
         Field(
-            description="Sets the representation of related function versions (like the _latest_ draft and/or published) in the response. - `embed`: as full summary representation (in `_embedded`). - `link`: as HAL link in (in `_links`). - `none`: omitted."
+            description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
-        alias_generator=_list_query_alias_for,
+        alias_generator=_patch_interface_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _patch_metadata_query_alias_for(field_name: str) -> str:
     if field_name == "comment":
         return "comment"
@@ -680,14 +717,15 @@
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_patch_metadata_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -736,50 +774,45 @@
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_publish_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _rebuild_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "comment":
         return "comment"
     if field_name == "dry_run":
         return "dryRun"
     if field_name == "var_async":
         return "async"
     if field_name == "upgrade":
         return "upgrade"
     if field_name == "force_version":
         return "forceVersion"
     if field_name == "ignore_checks":
         return "ignoreChecks"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     if field_name == "skip_rebuild":
         return "skipRebuild"
     return field_name
 
 
 class RebuildQuery(WaylayBaseModel):
     """Model for `rebuild` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
-        ),
-    ] = None
     comment: Annotated[
         StrictStr | None,
         Field(
             description="An optional user-specified comment corresponding to the operation."
         ),
     ] = None
     dry_run: Annotated[
@@ -808,22 +841,29 @@
     ] = None
     ignore_checks: Annotated[
         StrictBool | None,
         Field(
             description="If set to true, checks that normally prevent a rebuild are overriden. These checks include: * function state in `pending`, `running`, `failed` or `undeployed` * backoff period due to recent failures * usage of deprecated dependencies * running jobs on entity * the `dryRun` option"
         ),
     ] = None
+    scale_to_zero: Annotated[
+        StrictBool | None,
+        Field(
+            description="Indicates whether the function needs to be scaled down after successful (re-)deployment. If not set, the function is scaled to zero only if it was not active before this command."
+        ),
+    ] = None
     skip_rebuild: Annotated[
         StrictBool | None,
         Field(
             description="If set, the function will not be rebuild. Always uses the current runtime version when re-deploying/re-verifying the function."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_rebuild_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -853,25 +893,26 @@
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
     force: Annotated[
         StrictBool | None,
         Field(
-            description="If <code>true</code>, the function version will be immediately undeployed and removed.  Otherwise, the removal will be delayed to allow current invocations to end. During that period, the function is marked _deprecated_."
+            description="If <code>true</code>, the plug version(s) will be undeployed and removed. Otherwise, the plug version(s) will only be <code>deprecated</code>, i.e removed from regular listings."
         ),
     ] = None
     undeploy: Annotated[
         StrictBool | None,
         Field(
-            description="If `true`, the `DELETE` operation * undeploys the (openfaas) function: it becomes no longer available for invocation. * does NOT remove the function from registry: it stays in an `undeployed` status.  All assets and definitions are retained, so the version can be restored later with a  _rebuild_ action.  If `false`, the `DELETE` operation * _only_ marks the plug function as _deprecated_, the function remains active but is removed from the default listings.   This also applies to _draft_ versions.  This parameter is incompatible with `force=true`.  If not set the default behaviour applies: * _draft_ versions are _undeployed_ and _removed_ from registry. * non-_draft_ versions are marked _deprecated_ only."
+            description="If `true`, the `DELETE` operation * undeploys the (openfaas) function for the plug: it becomes no longer available for invocation. * does NOT remove the plug from registry: it stays in an `undeployed` status.  All assets and definitions are retained, so the plug can be restored later with a  _rebuild_ action.  If `false`, the `DELETE` operation * _only_ marks the plug version(s) as _deprecated_: the plug remains active but is removed from the default listings.   This also applies to _draft_ versions.  This parameter is incompatible with `force=true`.  If not set the default behaviour applies: * _draft_ versions are _undeployed_ and _removed_ from registry. * non-_draft_ versions are marked _deprecated_ only."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_remove_version_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -901,63 +942,48 @@
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
     force: Annotated[
         StrictBool | None,
         Field(
-            description="If <code>true</code>, the function version will be immediately undeployed and removed.  Otherwise, the removal will be delayed to allow current invocations to end. During that period, the function is marked _deprecated_."
+            description="If <code>true</code>, the plug version(s) will be undeployed and removed. Otherwise, the plug version(s) will only be <code>deprecated</code>, i.e removed from regular listings."
         ),
     ] = None
     undeploy: Annotated[
         StrictBool | None,
         Field(
-            description="If `true`, the `DELETE` operation * undeploys the (openfaas) function: it becomes no longer available for invocation. * does NOT remove the function from registry: it stays in an `undeployed` status.  All assets and definitions are retained, so the version can be restored later with a  _rebuild_ action.  If `false`, the `DELETE` operation * _only_ marks the plug function as _deprecated_, the function remains active but is removed from the default listings.   This also applies to _draft_ versions.  This parameter is incompatible with `force=true`.  If not set the default behaviour applies: * _draft_ versions are _undeployed_ and _removed_ from registry. * non-_draft_ versions are marked _deprecated_ only."
+            description="If `true`, the `DELETE` operation * undeploys the (openfaas) function for the plug: it becomes no longer available for invocation. * does NOT remove the plug from registry: it stays in an `undeployed` status.  All assets and definitions are retained, so the plug can be restored later with a  _rebuild_ action.  If `false`, the `DELETE` operation * _only_ marks the plug version(s) as _deprecated_: the plug remains active but is removed from the default listings.   This also applies to _draft_ versions.  This parameter is incompatible with `force=true`.  If not set the default behaviour applies: * _draft_ versions are _undeployed_ and _removed_ from registry. * non-_draft_ versions are marked _deprecated_ only."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_remove_versions_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _update_asset_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class UpdateAssetQuery(WaylayBaseModel):
     """Model for `update_asset` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -976,52 +1002,37 @@
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_update_asset_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _update_assets_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
-    if field_name == "deploy":
-        return "deploy"
     if field_name == "chown":
         return "chown"
     if field_name == "comment":
         return "comment"
     if field_name == "author":
         return "author"
     if field_name == "var_async":
         return "async"
     return field_name
 
 
 class UpdateAssetsQuery(WaylayBaseModel):
     """Model for `update_assets` query parameters."""
 
-    scale_to_zero: Annotated[
-        StrictBool | None,
-        Field(
-            description="If set to <code>true</code>, after successful deployment, the deployed function will be scaled to zero. This saves computing resources when the function is not to be used immediately."
-        ),
-    ] = None
-    deploy: Annotated[
-        StrictBool | None,
-        Field(
-            description="Indicates that a function should be _deployed_ when its assets are valid.  * If `true` (default), jobs to build and deploy the function will be initiated after it is checked that the assets are valid. Invalid assets lead to a validation error, and the function and its assets are not created or updated. * If `false`, the uploaded assets are stored and the function is created/updated in `registered` state. Asset validation errors are only returned as warning, and stored as `failureReason` on the function entity. Use an _asset update_ or _rebuild_ to initiate a build and deploy at a later stage."
-        ),
-    ] = None
     chown: Annotated[
         StrictBool | None,
         Field(
             description="If set, ownership of the draft function is transferred to the current user."
         ),
     ] = None
     comment: Annotated[
@@ -1040,44 +1051,46 @@
         StrictBool | None,
         Field(
             description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_update_assets_query_alias_for,
         populate_by_name=True,
     )
 
 
 def _verify_query_alias_for(field_name: str) -> str:
-    if field_name == "scale_to_zero":
-        return "scaleToZero"
     if field_name == "var_async":
         return "async"
+    if field_name == "scale_to_zero":
+        return "scaleToZero"
     return field_name
 
 
 class VerifyQuery(WaylayBaseModel):
     """Model for `verify` query parameters."""
 
-    scale_to_zero: Annotated[
+    var_async: Annotated[
         StrictBool | None,
         Field(
-            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
+            description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
         ),
     ] = None
-    var_async: Annotated[
+    scale_to_zero: Annotated[
         StrictBool | None,
         Field(
-            description="Unless this is set to <code>false</code>, the server will start the required job actions asynchronously and return a <code>202</code> <em>Accepted</em> response. If <code>false</code> the request will block until the job actions are completed, or a timeout occurs."
+            description="Indicates whether the function needs to be scaled down after successful verification. If not set, the function is scaled to zero only if it was not active before this command."
         ),
     ] = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_verify_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_registry_types-2.13.0b20240423/src/waylay_sdk_registry_types.egg-info/PKG-INFO` & `waylay-sdk-registry-types-2.13.0rc0/src/waylay_sdk_registry_types.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-registry-types
-Version: 2.13.0b20240423
+Version: 2.13.0rc0
 Summary: Waylay Function Registry Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,23 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-registry-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/registry.html
 Keywords: Waylay Function Registry,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
-Requires-Dist: waylay-sdk-registry==2.13.0b20240423
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-registry==2.13.0rc0
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -45,51 +44,56 @@
 Requires-Dist: pyyaml; extra == "dev"
 Requires-Dist: jsf>=0.11.1; extra == "dev"
 
 # Waylay Registry Service
 V2 API to build and deploy Waylay functions (plugs, webscripts, BYOML models).
 
 This Python package is automatically generated based on the 
-Waylay Registry OpenAPI specification (API version: 2.13.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/registry.html).
+Waylay Registry OpenAPI specification (API version: 2.13.0-beta.0)
 
 It is considered an extension of the waylay-sdk-registry package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-registry`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-registry is included in:
-- ```pip install waylay-sdk-core[registry]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[registry]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-registry and waylay-sdk-registry-types are included in:
-- ```pip install waylay-sdk-core[registry,registry-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[registry,registry-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-registry-types` is installed
-from waylay.services.registry.models.root_page_response import RootPageResponse
+from ..models.function_type import FunctionType
+from ..models.job_state_result import JobStateResult
+from ..models.job_type_schema import JobTypeSchema
+from ..models.jobs_response import JobsResponse
 try:
-    # Get Service Status
-    # calls `GET /registry/v2/`
-    api_response = await waylay_client.registry.about.get(
+    # List Jobs
+    # calls `GET /registry/v2/jobs/`
+    api_response = await waylay_client.registry.jobs.list(
+        # query parameters:
+        query = {
+        },
     )
-    print("The response of registry.about.get:\n")
+    print("The response of registry.jobs.list:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling registry.about.get: %s\n" % e)
+    print("Exception when calling registry.jobs.list: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

