# Comparing `tmp/waylay_sdk_storage_types-0.4.2.20240430.tar.gz` & `tmp/waylay_sdk_storage_types-0.4.2b20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_storage_types-0.4.2.20240430.tar", last modified: Thu May  2 07:57:47 2024, max compression
+gzip compressed data, was "waylay_sdk_storage_types-0.4.2b20240423.tar", last modified: Wed Apr 24 07:48:30 2024, max compression
```

## Comparing `waylay_sdk_storage_types-0.4.2.20240430.tar` & `waylay_sdk_storage_types-0.4.2b20240423.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.449646 waylay_sdk_storage_types-0.4.2.20240430/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-02 07:57:47.449646 waylay_sdk_storage_types-0.4.2.20240430/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 07:57:47.449646 waylay_sdk_storage_types-0.4.2.20240430/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.441646 waylay_sdk_storage_types-0.4.2.20240430/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.441646 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.441646 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.441646 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.449646 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/authentication_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/bucket_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/bucket_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/bucket_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/bucket_object_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/bucketcreationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/bucketpolicystatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/channeltype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/event_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/expiry.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/hal_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/httpmethod.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/links.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/location_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/notification_queue_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/notification_queue_status_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/payload_config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/queuesetupstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/sign.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/store.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/storetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/subscription_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/subscriptions_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/system_channel_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/system_channel_config_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/tenant_status_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/venttype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/web_script_channel_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/web_script_channel_config_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.449646 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/queries/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/queries/bucket_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/queries/object_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/queries/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-02 07:57:41.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/queries/subscription_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:57:47.449646 waylay_sdk_storage_types-0.4.2.20240430/src/waylay_sdk_storage_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-02 07:57:47.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay_sdk_storage_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-02 07:57:47.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay_sdk_storage_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 07:57:47.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay_sdk_storage_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-02 07:57:47.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay_sdk_storage_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 07:57:47.000000 waylay_sdk_storage_types-0.4.2.20240430/src/waylay_sdk_storage_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:30.613674 waylay_sdk_storage_types-0.4.2b20240423/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-24 07:48:30.613674 waylay_sdk_storage_types-0.4.2b20240423/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:48:30.613674 waylay_sdk_storage_types-0.4.2b20240423/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:30.605674 waylay_sdk_storage_types-0.4.2b20240423/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:30.601674 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:30.601674 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:30.605674 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:30.609674 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/authentication_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/bucket_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/bucket_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/bucket_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/bucket_object_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/bucketcreationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/bucketpolicystatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/channeltype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/expiry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/hal_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/httpmethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/location_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/notification_queue_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/notification_queue_status_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/payload_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/queuesetupstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/storetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/subscription_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/subscriptions_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/system_channel_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/system_channel_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/tenant_status_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/venttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/web_script_channel_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/web_script_channel_config_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:30.613674 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/queries/about_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/queries/bucket_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/queries/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/queries/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-24 07:48:26.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/queries/subscription_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:48:30.613674 waylay_sdk_storage_types-0.4.2b20240423/src/waylay_sdk_storage_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-24 07:48:30.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay_sdk_storage_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-24 07:48:30.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay_sdk_storage_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:48:30.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay_sdk_storage_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-24 07:48:30.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay_sdk_storage_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 07:48:30.000000 waylay_sdk_storage_types-0.4.2b20240423/src/waylay_sdk_storage_types.egg-info/top_level.txt
```

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/LICENSE.txt` & `waylay_sdk_storage_types-0.4.2b20240423/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/PKG-INFO` & `waylay_sdk_storage_types-0.4.2b20240423/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-storage-types
-Version: 0.4.2.20240430
+Version: 0.4.2b20240423
 Summary: Waylay Storage Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -21,15 +21,15 @@
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-storage-py.git
 Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/storage.html
 Keywords: Waylay Storage,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: waylay-sdk-core~=0.2.1
-Requires-Dist: waylay-sdk-storage==0.4.2.20240430
+Requires-Dist: waylay-sdk-storage==0.4.2b20240423
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
```

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/README.md` & `waylay_sdk_storage_types-0.4.2b20240423/README.md`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/pyproject.toml` & `waylay_sdk_storage_types-0.4.2b20240423/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-storage-types"
-version = "0.4.2.20240430"
+version = "0.4.2b20240423"
 description = "Waylay Storage Types "
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Storage" , "Types"]
 requires-python = ">= 3.9"
 dependencies = [
     "waylay-sdk-core ~= 0.2.1",
-    "waylay-sdk-storage == 0.4.2.20240430",
+    "waylay-sdk-storage == 0.4.2b20240423",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
```

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/__init__.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
  Manage storage buckets and subscriptions.
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
 """
 
-__version__ = "0.4.2.20240430"
+__version__ = "0.4.2b20240423"
 
 # import models into model package
 from .auth import AUTH
 from .authentication_config import AuthenticationConfig
 from .bucket import Bucket
 from .bucket_configuration import BucketConfiguration
 from .bucket_listing import BucketListing
```

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/auth.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/auth.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/authentication_config.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/authentication_config.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/bucket.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/bucket.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/bucket_configuration.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/bucket_configuration.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/bucket_listing.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/bucket_listing.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/bucket_object.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/bucket_object.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/bucket_object_listing.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/bucket_object_listing.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/bucketcreationstatus.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/bucketcreationstatus.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/bucketpolicystatus.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/bucketpolicystatus.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/channel.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/channel.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/event_filter.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/event_filter.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/expiry.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/expiry.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/hal_entity.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/hal_entity.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/hal_link.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/hal_link.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/http_validation_error.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/notification_queue_status.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/notification_queue_status.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/notification_queue_status_report.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/notification_queue_status_report.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/payload_config.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/payload_config.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/queuesetupstatus.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/queuesetupstatus.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/response_list.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/response_list.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/store.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/store.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/subscription_config.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/subscription_config.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/subscriptions.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/subscriptions.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/subscriptions_listing.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/subscriptions_listing.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/system_channel_config.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/system_channel_config.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/tenant_status_report.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/tenant_status_report.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/validation_error.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/models/web_script_channel_config.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/models/web_script_channel_config.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/queries/about_api.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/queries/about_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/queries/bucket_api.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/queries/bucket_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/queries/object_api.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/queries/object_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay/services/storage/queries/subscription_api.py` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay/services/storage/queries/subscription_api.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay_sdk_storage_types.egg-info/PKG-INFO` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay_sdk_storage_types.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-storage-types
-Version: 0.4.2.20240430
+Version: 0.4.2b20240423
 Summary: Waylay Storage Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -21,15 +21,15 @@
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-storage-py.git
 Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/storage.html
 Keywords: Waylay Storage,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: waylay-sdk-core~=0.2.1
-Requires-Dist: waylay-sdk-storage==0.4.2.20240430
+Requires-Dist: waylay-sdk-storage==0.4.2b20240423
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
```

### Comparing `waylay_sdk_storage_types-0.4.2.20240430/src/waylay_sdk_storage_types.egg-info/SOURCES.txt` & `waylay_sdk_storage_types-0.4.2b20240423/src/waylay_sdk_storage_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

