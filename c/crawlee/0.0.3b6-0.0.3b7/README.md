# Comparing `tmp/crawlee-0.0.3b6.tar.gz` & `tmp/crawlee-0.0.3b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlee-0.0.3b6.tar", max compression
+gzip compressed data, was "crawlee-0.0.3b7.tar", max compression
```

## Comparing `crawlee-0.0.3b6.tar` & `crawlee-0.0.3b7.tar`

### file list

```diff
@@ -1,79 +1,81 @@
--rw-r--r--   0        0        0    11355 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/LICENSE
--rw-r--r--   0        0        0       17 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/README.md
--rw-r--r--   0        0        0     6386 2024-04-30 09:08:43.136986 crawlee-0.0.3b6/pyproject.toml
--rw-r--r--   0        0        0       31 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/__init__.py
--rw-r--r--   0        0        0     3341 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/byte_size.py
--rw-r--r--   0        0        0      759 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/crypto.py
--rw-r--r--   0        0        0     3365 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/data_processing.py
--rw-r--r--   0        0        0     1950 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/env_vars.py
--rw-r--r--   0        0        0     4668 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/file.py
--rw-r--r--   0        0        0     5262 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/globs.py
--rw-r--r--   0        0        0     2056 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/lru_cache.py
--rw-r--r--   0        0        0      918 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/math.py
--rw-r--r--   0        0        0      715 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/measure_time.py
--rw-r--r--   0        0        0     1585 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/recurring_task.py
--rw-r--r--   0        0        0     4765 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/requests.py
--rw-r--r--   0        0        0     2414 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/system.py
--rw-r--r--   0        0        0     1429 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/_utils/wait.py
--rw-r--r--   0        0        0      142 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/autoscaling/__init__.py
--rw-r--r--   0        0        0    14883 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/autoscaling/autoscaled_pool.py
--rw-r--r--   0        0        0        0 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/autoscaling/py.typed
--rw-r--r--   0        0        0    15793 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/autoscaling/snapshotter.py
--rw-r--r--   0        0        0     9293 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/autoscaling/system_status.py
--rw-r--r--   0        0        0     5140 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/autoscaling/types.py
--rw-r--r--   0        0        0      186 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/basic_crawler/__init__.py
--rw-r--r--   0        0        0    20483 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/basic_crawler/basic_crawler.py
--rw-r--r--   0        0        0     5749 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/basic_crawler/context_pipeline.py
--rw-r--r--   0        0        0     2279 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/basic_crawler/router.py
--rw-r--r--   0        0        0     2688 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/basic_crawler/types.py
--rw-r--r--   0        0        0       86 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/beautifulsoup_crawler/__init__.py
--rw-r--r--   0        0        0     5359 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
--rw-r--r--   0        0        0      524 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/beautifulsoup_crawler/types.py
--rw-r--r--   0        0        0     1246 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/configuration.py
--rw-r--r--   0        0        0      272 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/enqueue_strategy.py
--rw-r--r--   0        0        0       91 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/events/__init__.py
--rw-r--r--   0        0        0     7211 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/events/event_manager.py
--rw-r--r--   0        0        0     2683 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/events/local_event_manager.py
--rw-r--r--   0        0        0        0 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/events/py.typed
--rw-r--r--   0        0        0     1303 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/events/types.py
--rw-r--r--   0        0        0        0 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/http_clients/__init__.py
--rw-r--r--   0        0        0     1615 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/http_clients/base_http_client.py
--rw-r--r--   0        0        0     2031 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/http_clients/httpx_client.py
--rw-r--r--   0        0        0       38 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/http_crawler/__init__.py
--rw-r--r--   0        0        0     3216 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/http_crawler/http_crawler.py
--rw-r--r--   0        0        0      329 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/http_crawler/types.py
--rw-r--r--   0        0        0     4719 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/log_config.py
--rw-r--r--   0        0        0        0 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/py.typed
--rw-r--r--   0        0        0     6207 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/request.py
--rw-r--r--   0        0        0      365 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/resource_clients/__init__.py
--rw-r--r--   0        0        0     5687 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/resource_clients/base_resource_client.py
--rw-r--r--   0        0        0     2980 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/resource_clients/base_resource_collection_client.py
--rw-r--r--   0        0        0    19714 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/resource_clients/dataset_client.py
--rw-r--r--   0        0        0     1819 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/resource_clients/dataset_collection_client.py
--rw-r--r--   0        0        0    20474 2024-04-30 09:08:21.145113 crawlee-0.0.3b6/src/crawlee/resource_clients/key_value_store_client.py
--rw-r--r--   0        0        0     1936 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/resource_clients/key_value_store_collection_client.py
--rw-r--r--   0        0        0        0 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/resource_clients/py.typed
--rw-r--r--   0        0        0    22452 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/resource_clients/request_queue_client.py
--rw-r--r--   0        0        0     1912 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/resource_clients/request_queue_collection_client.py
--rw-r--r--   0        0        0       67 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/sessions/__init__.py
--rw-r--r--   0        0        0     2430 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/sessions/models.py
--rw-r--r--   0        0        0        0 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/sessions/py.typed
--rw-r--r--   0        0        0     8155 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/sessions/session.py
--rw-r--r--   0        0        0    11695 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/sessions/session_pool.py
--rw-r--r--   0        0        0     1645 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storage_client_manager.py
--rw-r--r--   0        0        0      106 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storage_clients/__init__.py
--rw-r--r--   0        0        0     1574 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storage_clients/base_storage_client.py
--rw-r--r--   0        0        0    11477 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storage_clients/memory_storage_client.py
--rw-r--r--   0        0        0        0 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storage_clients/py.typed
--rw-r--r--   0        0        0      150 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/__init__.py
--rw-r--r--   0        0        0     7600 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/base_storage.py
--rw-r--r--   0        0        0    15526 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/dataset.py
--rw-r--r--   0        0        0     4999 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/key_value_store.py
--rw-r--r--   0        0        0     6489 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/models.py
--rw-r--r--   0        0        0        0 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/py.typed
--rw-r--r--   0        0        0     2593 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/request_list.py
--rw-r--r--   0        0        0     2775 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/request_provider.py
--rw-r--r--   0        0        0    25883 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/storages/request_queue.py
--rw-r--r--   0        0        0      630 2024-04-30 09:08:21.149113 crawlee-0.0.3b6/src/crawlee/types.py
--rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 crawlee-0.0.3b6/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/LICENSE
+-rw-r--r--   0        0        0       17 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/README.md
+-rw-r--r--   0        0        0     6386 2024-05-02 12:00:48.558217 crawlee-0.0.3b7/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/blocked.py
+-rw-r--r--   0        0        0     3341 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/byte_size.py
+-rw-r--r--   0        0        0      759 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/crypto.py
+-rw-r--r--   0        0        0     3365 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/data_processing.py
+-rw-r--r--   0        0        0     1950 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/env_vars.py
+-rw-r--r--   0        0        0     4668 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/file.py
+-rw-r--r--   0        0        0     5262 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/globs.py
+-rw-r--r--   0        0        0     2056 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/lru_cache.py
+-rw-r--r--   0        0        0      918 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/math.py
+-rw-r--r--   0        0        0      715 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/measure_time.py
+-rw-r--r--   0        0        0     1585 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/recurring_task.py
+-rw-r--r--   0        0        0     4765 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/requests.py
+-rw-r--r--   0        0        0     2414 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/system.py
+-rw-r--r--   0        0        0     1429 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/_utils/wait.py
+-rw-r--r--   0        0        0      142 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/autoscaling/__init__.py
+-rw-r--r--   0        0        0    14883 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/autoscaling/autoscaled_pool.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/autoscaling/py.typed
+-rw-r--r--   0        0        0    15793 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/autoscaling/snapshotter.py
+-rw-r--r--   0        0        0     9293 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/autoscaling/system_status.py
+-rw-r--r--   0        0        0     5140 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/autoscaling/types.py
+-rw-r--r--   0        0        0      186 2024-05-02 12:00:31.734202 crawlee-0.0.3b7/src/crawlee/basic_crawler/__init__.py
+-rw-r--r--   0        0        0    24151 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/basic_crawler/basic_crawler.py
+-rw-r--r--   0        0        0     4696 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/basic_crawler/context_pipeline.py
+-rw-r--r--   0        0        0     2145 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/basic_crawler/errors.py
+-rw-r--r--   0        0        0     2279 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/basic_crawler/router.py
+-rw-r--r--   0        0        0     2798 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/basic_crawler/types.py
+-rw-r--r--   0        0        0       86 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/beautifulsoup_crawler/__init__.py
+-rw-r--r--   0        0        0     7219 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py
+-rw-r--r--   0        0        0      524 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/beautifulsoup_crawler/types.py
+-rw-r--r--   0        0        0     1246 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/configuration.py
+-rw-r--r--   0        0        0      272 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/enqueue_strategy.py
+-rw-r--r--   0        0        0       91 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/events/__init__.py
+-rw-r--r--   0        0        0     7211 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/events/event_manager.py
+-rw-r--r--   0        0        0     2683 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/events/local_event_manager.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/events/py.typed
+-rw-r--r--   0        0        0     1303 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/events/types.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/http_clients/__init__.py
+-rw-r--r--   0        0        0     1857 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/http_clients/base_http_client.py
+-rw-r--r--   0        0        0     4263 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/http_clients/httpx_client.py
+-rw-r--r--   0        0        0       38 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/http_crawler/__init__.py
+-rw-r--r--   0        0        0     4512 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/http_crawler/http_crawler.py
+-rw-r--r--   0        0        0      329 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/http_crawler/types.py
+-rw-r--r--   0        0        0     4719 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/log_config.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/py.typed
+-rw-r--r--   0        0        0     6670 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/request.py
+-rw-r--r--   0        0        0      365 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/resource_clients/__init__.py
+-rw-r--r--   0        0        0     5687 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/resource_clients/base_resource_client.py
+-rw-r--r--   0        0        0     2980 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0        0        0    19714 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/resource_clients/dataset_client.py
+-rw-r--r--   0        0        0     1819 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/resource_clients/dataset_collection_client.py
+-rw-r--r--   0        0        0    20474 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/resource_clients/key_value_store_client.py
+-rw-r--r--   0        0        0     1936 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/resource_clients/key_value_store_collection_client.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/resource_clients/py.typed
+-rw-r--r--   0        0        0    22452 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/resource_clients/request_queue_client.py
+-rw-r--r--   0        0        0     1912 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/resource_clients/request_queue_collection_client.py
+-rw-r--r--   0        0        0       67 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/sessions/__init__.py
+-rw-r--r--   0        0        0     2430 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/sessions/models.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/sessions/py.typed
+-rw-r--r--   0        0        0     8084 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/sessions/session.py
+-rw-r--r--   0        0        0    11695 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/sessions/session_pool.py
+-rw-r--r--   0        0        0     1645 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/storage_client_manager.py
+-rw-r--r--   0        0        0      106 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/storage_clients/__init__.py
+-rw-r--r--   0        0        0     1574 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/storage_clients/base_storage_client.py
+-rw-r--r--   0        0        0    11477 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/storage_clients/memory_storage_client.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/storage_clients/py.typed
+-rw-r--r--   0        0        0      150 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/storages/__init__.py
+-rw-r--r--   0        0        0     7600 2024-05-02 12:00:31.738202 crawlee-0.0.3b7/src/crawlee/storages/base_storage.py
+-rw-r--r--   0        0        0    15526 2024-05-02 12:00:31.742202 crawlee-0.0.3b7/src/crawlee/storages/dataset.py
+-rw-r--r--   0        0        0     4999 2024-05-02 12:00:31.742202 crawlee-0.0.3b7/src/crawlee/storages/key_value_store.py
+-rw-r--r--   0        0        0     6489 2024-05-02 12:00:31.742202 crawlee-0.0.3b7/src/crawlee/storages/models.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:00:31.742202 crawlee-0.0.3b7/src/crawlee/storages/py.typed
+-rw-r--r--   0        0        0     2593 2024-05-02 12:00:31.742202 crawlee-0.0.3b7/src/crawlee/storages/request_list.py
+-rw-r--r--   0        0        0     2775 2024-05-02 12:00:31.742202 crawlee-0.0.3b7/src/crawlee/storages/request_provider.py
+-rw-r--r--   0        0        0    25883 2024-05-02 12:00:31.742202 crawlee-0.0.3b7/src/crawlee/storages/request_queue.py
+-rw-r--r--   0        0        0      630 2024-05-02 12:00:31.742202 crawlee-0.0.3b7/src/crawlee/types.py
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 crawlee-0.0.3b7/PKG-INFO
```

### Comparing `crawlee-0.0.3b6/LICENSE` & `crawlee-0.0.3b7/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/pyproject.toml` & `crawlee-0.0.3b7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "crawlee"
-version = "0.0.3b6"
+version = "0.0.3b7"
 description = "Crawlee for Python"
 authors = ["Apify Technologies s.r.o. <support@apify.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "crawlee", from = "src" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -62,15 +62,15 @@
 python-dateutil = "^2.9.0"
 sortedcollections = "^2.1.0"
 typing-extensions = "^4.1.0"
 tldextract = "^5.1.2"
 
 [tool.poetry.group.dev.dependencies]
 build = "~1.2.0"
-filelock = "~3.13.1"
+filelock = "~3.14.0"
 mypy = "~1.10.0"
 pre-commit = "~3.7.0"
 pydoc-markdown = "~4.8.2"
 pytest = "~8.2.0"
 pytest-asyncio = "~0.23.5"
 pytest-cov = "~5.0.0"
 pytest-only = "~2.1.0"
```

### Comparing `crawlee-0.0.3b6/src/crawlee/_utils/byte_size.py` & `crawlee-0.0.3b7/src/crawlee/_utils/byte_size.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/_utils/crypto.py` & `crawlee-0.0.3b7/src/crawlee/_utils/crypto.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/_utils/data_processing.py` & `crawlee-0.0.3b7/src/crawlee/_utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/_utils/env_vars.py` & `crawlee-0.0.3b7/src/crawlee/_utils/env_vars.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/_utils/file.py` & `crawlee-0.0.3b7/src/crawlee/_utils/file.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/_utils/globs.py` & `crawlee-0.0.3b7/src/crawlee/_utils/globs.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/_utils/lru_cache.py` & `crawlee-0.0.3b7/src/crawlee/_utils/lru_cache.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/_utils/math.py` & `crawlee-0.0.3b7/src/crawlee/_utils/math.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/_utils/measure_time.py` & `crawlee-0.0.3b7/src/crawlee/_utils/measure_time.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/_utils/recurring_task.py` & `crawlee-0.0.3b7/src/crawlee/_utils/recurring_task.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/_utils/requests.py` & `crawlee-0.0.3b7/src/crawlee/_utils/requests.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/_utils/system.py` & `crawlee-0.0.3b7/src/crawlee/_utils/system.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/_utils/wait.py` & `crawlee-0.0.3b7/src/crawlee/_utils/wait.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/autoscaling/autoscaled_pool.py` & `crawlee-0.0.3b7/src/crawlee/autoscaling/autoscaled_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/autoscaling/snapshotter.py` & `crawlee-0.0.3b7/src/crawlee/autoscaling/snapshotter.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/autoscaling/system_status.py` & `crawlee-0.0.3b7/src/crawlee/autoscaling/system_status.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/autoscaling/types.py` & `crawlee-0.0.3b7/src/crawlee/autoscaling/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/basic_crawler/basic_crawler.py` & `crawlee-0.0.3b7/src/crawlee/basic_crawler/basic_crawler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Inspiration: https://github.com/apify/crawlee/blob/v3.7.3/packages/basic-crawler/src/internals/basic-crawler.ts
 from __future__ import annotations
 
 import tempfile
+from contextlib import AsyncExitStack
 from datetime import timedelta
 from functools import partial
 from logging import getLogger
 from typing import TYPE_CHECKING, AsyncGenerator, Awaitable, Callable, Generic, Sequence, Union, cast
 
 import httpx
 from tldextract import TLDExtract
@@ -14,49 +15,51 @@
 from crawlee import Glob
 from crawlee._utils.wait import wait_for
 from crawlee.autoscaling import AutoscaledPool, ConcurrencySettings
 from crawlee.autoscaling.snapshotter import Snapshotter
 from crawlee.autoscaling.system_status import SystemStatus
 from crawlee.basic_crawler.context_pipeline import (
     ContextPipeline,
+)
+from crawlee.basic_crawler.errors import (
     ContextPipelineInitializationError,
     ContextPipelineInterruptedError,
     RequestHandlerError,
+    SessionError,
+    UserDefinedErrorHandlerError,
 )
 from crawlee.basic_crawler.router import Router
 from crawlee.basic_crawler.types import (
     BasicCrawlingContext,
     FinalStatistics,
     RequestHandlerRunResult,
     SendRequestFunction,
 )
 from crawlee.configuration import Configuration
 from crawlee.enqueue_strategy import EnqueueStrategy
 from crawlee.events.local_event_manager import LocalEventManager
 from crawlee.http_clients.httpx_client import HttpxClient
 from crawlee.request import BaseRequestData, Request, RequestState
+from crawlee.sessions import SessionPool
 from crawlee.storages.request_queue import RequestQueue
 
 if TYPE_CHECKING:
     import re
 
     from crawlee.http_clients.base_http_client import BaseHttpClient, HttpResponse
+    from crawlee.sessions.session import Session
     from crawlee.storages.request_provider import RequestProvider
 
 TCrawlingContext = TypeVar('TCrawlingContext', bound=BasicCrawlingContext, default=BasicCrawlingContext)
 ErrorHandler = Callable[[TCrawlingContext, Exception], Awaitable[Union[Request, None]]]
 FailedRequestHandler = Callable[[TCrawlingContext, Exception], Awaitable[None]]
 
 logger = getLogger(__name__)
 
 
-class UserDefinedErrorHandlerError(Exception):
-    """Wraps an exception thrown from an user-defined error handler."""
-
-
 class BasicCrawler(Generic[TCrawlingContext]):
     """Provides a simple framework for parallel crawling of web pages.
 
     The URLs to crawl are fed either from a static list of URLs or from a dynamic queue of URLs enabling recursive
     crawling of websites.
 
     `BasicCrawler` is a low-level tool that requires the user to implement the page download and data extraction
@@ -68,28 +71,38 @@
         self,
         *,
         request_provider: RequestProvider | None = None,
         router: Callable[[TCrawlingContext], Awaitable[None]] | None = None,
         http_client: BaseHttpClient | None = None,
         concurrency_settings: ConcurrencySettings | None = None,
         max_request_retries: int = 3,
+        max_session_rotations: int = 10,
         configuration: Configuration | None = None,
         request_handler_timeout: timedelta = timedelta(minutes=1),
+        session_pool: SessionPool | None = None,
+        use_session_pool: bool = True,
+        retry_on_blocked: bool = True,
         _context_pipeline: ContextPipeline[TCrawlingContext] | None = None,
     ) -> None:
         """Initialize the BasicCrawler.
 
         Args:
             request_provider: Provides requests to be processed
             router: A callable to which request handling is delegated
             http_client: HTTP client to be used for `BasicCrawlingContext.send_request` and HTTP-only crawling.
             concurrency_settings: Allows fine-tuning concurrency levels
             max_request_retries: Maximum amount of attempts at processing a request
+            max_session_rotations: Maximum number of session rotations per request.
+                The crawler will automatically rotate the session in case of a proxy error or if it gets blocked by
+                the website.
             configuration: Crawler configuration
             request_handler_timeout: How long is a single request handler allowed to run
+            use_session_pool: Enables using the session pool for crawling
+            session_pool: A preconfigured SessionPool instance if you wish to use non-default configuration
+            retry_on_blocked: If set to True, the crawler will try to automatically bypass any detected bot protection
             _context_pipeline: Allows extending the request lifecycle and modifying the crawling context.
                 This parameter is meant to be used by child classes, not when BasicCrawler is instantiated directly.
         """
         self._router: Router[TCrawlingContext] | None = None
 
         if isinstance(cast(Router, router), Router):
             self._router = cast(Router[TCrawlingContext], router)
@@ -101,14 +114,15 @@
 
         self._context_pipeline = (_context_pipeline or ContextPipeline()).compose(self._check_url_after_redirects)
 
         self._error_handler: ErrorHandler[TCrawlingContext] | None = None
         self._failed_request_handler: FailedRequestHandler[TCrawlingContext] | None = None
 
         self._max_request_retries = max_request_retries
+        self._max_session_rotations = max_session_rotations
 
         self._request_provider = request_provider
         self._configuration = configuration or Configuration()
 
         self._request_handler_timeout = request_handler_timeout
         self._internal_timeout = (
             self._configuration.internal_timeout
@@ -125,14 +139,19 @@
             system_status=SystemStatus(self._snapshotter),
             is_finished_function=self.__is_finished_function,
             is_task_ready_function=self.__is_task_ready_function,
             run_task_function=self.__run_task_function,
             concurrency_settings=concurrency_settings,
         )
 
+        self._use_session_pool = use_session_pool
+        self._session_pool: SessionPool = session_pool or SessionPool()
+
+        self._retry_on_blocked = retry_on_blocked
+
     @property
     def router(self) -> Router[TCrawlingContext]:
         """The router used to handle each individual crawling request."""
         if self._router is None:
             self._router = Router[TCrawlingContext]()
 
         return self._router
@@ -140,14 +159,28 @@
     @router.setter
     def router(self, router: Router[TCrawlingContext]) -> None:
         if self._router is not None:
             raise RuntimeError('A router is already set')
 
         self._router = router
 
+    async def _get_session(self) -> Session | None:
+        """If session pool is being used, try to take a session from it."""
+        if not self._use_session_pool:
+            return None
+
+        return await wait_for(
+            self._session_pool.get_session,
+            timeout=self._internal_timeout,
+            timeout_message='Fetching a session from the pool timed out after '
+            f'{self._internal_timeout.total_seconds()} seconds',
+            max_retries=3,
+            logger=logger,
+        )
+
     async def get_request_provider(self) -> RequestProvider:
         """Return the configured request provider. If none is configured, open and return the default request queue."""
         if not self._request_provider:
             self._request_provider = await RequestQueue.open()
 
         return self._request_provider
 
@@ -184,27 +217,37 @@
         )
 
     async def run(self, requests: list[str | BaseRequestData] | None = None) -> FinalStatistics:
         """Run the crawler until all requests are processed."""
         if requests is not None:
             await self.add_requests(requests)
 
-        async with self._event_manager, self._snapshotter:
+        async with AsyncExitStack() as exit_stack:
+            await exit_stack.enter_async_context(self._event_manager)
+            await exit_stack.enter_async_context(self._snapshotter)
+
+            if self._use_session_pool:
+                await exit_stack.enter_async_context(self._session_pool)
+
             await self._pool.run()
 
         return FinalStatistics()
 
-    def _should_retry_request(self, crawling_context: BasicCrawlingContext) -> bool:
+    def _should_retry_request(self, crawling_context: BasicCrawlingContext, error: Exception) -> bool:
+        if crawling_context.request.no_retry:
+            return False
+
+        if isinstance(error, SessionError):
+            return ((crawling_context.request.session_rotation_count or 0) + 1) < self._max_session_rotations
+
         max_request_retries = crawling_context.request.max_retries
         if max_request_retries is None:
             max_request_retries = self._max_request_retries
 
-        return (
-            not crawling_context.request.no_retry and (crawling_context.request.retry_count + 1) < max_request_retries
-        )
+        return (crawling_context.request.retry_count + 1) < max_request_retries
 
     async def _check_url_after_redirects(
         self, crawling_context: TCrawlingContext
     ) -> AsyncGenerator[TCrawlingContext, None]:
         """Invoked at the end of the context pipeline to make sure that the `loaded_url` still matches enqueue_strategy.
 
         This is done to filter out links that redirect outside of the crawled domain.
@@ -269,15 +312,15 @@
 
         # The URL does not match any `include` pattern - reject it
         return False
 
     async def _handle_request_error(self, crawling_context: TCrawlingContext, error: Exception) -> None:
         request_provider = await self.get_request_provider()
 
-        if self._should_retry_request(crawling_context):
+        if self._should_retry_request(crawling_context, error):
             request = crawling_context.request
             request.retry_count += 1
 
             if self._error_handler:
                 try:
                     new_request = await self._error_handler(crawling_context, error)
                 except Exception as e:
@@ -303,17 +346,24 @@
 
         if self._failed_request_handler:
             try:
                 await self._failed_request_handler(crawling_context, error)
             except Exception as e:
                 raise UserDefinedErrorHandlerError('Exception thrown in user-defined failed request handler') from e
 
-    def _prepare_send_request_function(self) -> SendRequestFunction:
-        async def send_request(url: str, *, method: str = 'get', headers: dict[str, str] | None = None) -> HttpResponse:
-            return await self._http_client.send_request(url, method=method, headers=httpx.Headers(headers))
+    def _prepare_send_request_function(self, session: Session | None) -> SendRequestFunction:
+        async def send_request(
+            url: str,
+            *,
+            method: str = 'get',
+            headers: dict[str, str] | None = None,
+        ) -> HttpResponse:
+            return await self._http_client.send_request(
+                url, method=method, headers=httpx.Headers(headers), session=session
+            )
 
         return send_request
 
     async def _commit_request_handler_result(
         self, context: BasicCrawlingContext, result: RequestHandlerRunResult
     ) -> None:
         request_provider = await self.get_request_provider()
@@ -346,36 +396,35 @@
         request_provider = await self.get_request_provider()
         return await request_provider.is_finished()
 
     async def __is_task_ready_function(self) -> bool:
         request_provider = await self.get_request_provider()
         return not await request_provider.is_empty()
 
-    async def __run_task_function(self) -> None:
+    async def __run_task_function(self) -> None:  # noqa: PLR0912
         request_provider = await self.get_request_provider()
 
         request = await wait_for(
             lambda: request_provider.fetch_next_request(),
             timeout=self._internal_timeout,
             timeout_message=f'Fetching next request failed after {self._internal_timeout.total_seconds()} seconds',
             logger=logger,
             max_retries=3,
         )
 
         if request is None:
             return
 
-        # TODO: fetch session from the session pool
-        # https://github.com/apify/crawlee-py/issues/110
-
+        session = await self._get_session()
         result = RequestHandlerRunResult()
 
         crawling_context = BasicCrawlingContext(
             request=request,
-            send_request=self._prepare_send_request_function(),
+            session=session,
+            send_request=self._prepare_send_request_function(session),
             add_requests=result.add_requests,
         )
 
         try:
             request.state = RequestState.REQUEST_HANDLER
 
             await wait_for(
@@ -394,14 +443,17 @@
                 timeout_message='Marking request as handled timed out after '
                 f'{self._internal_timeout.total_seconds()} seconds',
                 logger=logger,
                 max_retries=3,
             )
 
             request.state = RequestState.DONE
+
+            if crawling_context.session:
+                crawling_context.session.mark_good()
         except RequestHandlerError as primary_error:
             primary_error = cast(
                 RequestHandlerError[TCrawlingContext], primary_error
             )  # valid thanks to ContextPipeline
 
             try:
                 request.state = RequestState.ERROR_HANDLER
@@ -424,29 +476,57 @@
                 logger.exception(
                     'An exception occurred during handling of failed request. This places the crawler '
                     'and its underlying storages into an unknown state and crawling will be terminated.',
                     exc_info=secondary_error,
                 )
                 request.state = RequestState.ERROR
                 raise
+
+            if crawling_context.session:
+                crawling_context.session.mark_bad()
+        except SessionError as session_error:
+            if not crawling_context.session:
+                raise RuntimeError('SessionError raised in a crawling context without a session') from session_error
+
+            if self._should_retry_request(crawling_context, session_error):
+                logger.warning('Encountered a session error, rotating session and retrying')
+
+                crawling_context.session.retire()
+
+                if crawling_context.request.session_rotation_count is None:
+                    crawling_context.request.session_rotation_count = 0
+                crawling_context.request.session_rotation_count += 1
+
+                await request_provider.reclaim_request(request)
+            else:
+                logger.exception('Request failed and reached maximum retries', exc_info=session_error)
+
+                await wait_for(
+                    lambda: request_provider.mark_request_as_handled(crawling_context.request),
+                    timeout=self._internal_timeout,
+                    timeout_message='Marking request as handled timed out after '
+                    f'{self._internal_timeout.total_seconds()} seconds',
+                    logger=logger,
+                    max_retries=3,
+                )
         except ContextPipelineInterruptedError as interruped_error:
             logger.debug('The context pipeline was interrupted', exc_info=interruped_error)
 
             await wait_for(
                 lambda: request_provider.mark_request_as_handled(crawling_context.request),
                 timeout=self._internal_timeout,
                 timeout_message='Marking request as handled timed out after '
                 f'{self._internal_timeout.total_seconds()} seconds',
                 logger=logger,
                 max_retries=3,
             )
         except ContextPipelineInitializationError as initialization_error:
-            if self._should_retry_request(crawling_context):
+            if self._should_retry_request(crawling_context, initialization_error):
                 logger.debug(
-                    'An exception occured during the initialization of crawling context, a retry is in order',
+                    'An exception occurred during the initialization of crawling context, a retry is in order',
                     exc_info=initialization_error,
                 )
 
                 request = crawling_context.request
                 request.retry_count += 1
                 request.state = RequestState.DONE
                 await request_provider.reclaim_request(request)
@@ -457,14 +537,17 @@
                     lambda: request_provider.mark_request_as_handled(crawling_context.request),
                     timeout=self._internal_timeout,
                     timeout_message='Marking request as handled timed out after '
                     f'{self._internal_timeout.total_seconds()} seconds',
                     logger=logger,
                     max_retries=3,
                 )
+
+            if crawling_context.session:
+                crawling_context.session.mark_bad()
         except Exception as internal_error:
             logger.exception(
                 'An exception occurred during handling of a request. This places the crawler '
                 'and its underlying storages into an unknown state and crawling will be terminated.',
                 exc_info=internal_error,
             )
             raise
```

### Comparing `crawlee-0.0.3b6/src/crawlee/basic_crawler/context_pipeline.py` & `crawlee-0.0.3b7/src/crawlee/basic_crawler/context_pipeline.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,26 @@
 from __future__ import annotations
 
 from typing import Any, AsyncGenerator, Awaitable, Callable, Generator, Generic, cast
 
 from typing_extensions import TypeVar
 
+from crawlee.basic_crawler.errors import (
+    ContextPipelineFinalizationError,
+    ContextPipelineInitializationError,
+    ContextPipelineInterruptedError,
+    RequestHandlerError,
+    SessionError,
+)
 from crawlee.basic_crawler.types import BasicCrawlingContext
 
 TCrawlingContext = TypeVar('TCrawlingContext', bound=BasicCrawlingContext, default=BasicCrawlingContext)
 TMiddlewareCrawlingContext = TypeVar('TMiddlewareCrawlingContext', bound=BasicCrawlingContext)
 
 
-class RequestHandlerError(Exception, Generic[TCrawlingContext]):
-    """Wraps an exception thrown from a request handler (router) and extends it with crawling context."""
-
-    def __init__(self, wrapped_exception: Exception, crawling_context: TCrawlingContext) -> None:
-        self.wrapped_exception = wrapped_exception
-        self.crawling_context = crawling_context
-
-
-class ContextPipelineInitializationError(Exception):
-    """Wraps an exception thrown in the initialization step of a context pipeline middleware.
-
-    We may not have the complete context at this point, so only `BasicCrawlingContext` is provided.
-    """
-
-    def __init__(self, wrapped_exception: Exception, crawling_context: BasicCrawlingContext) -> None:
-        self.wrapped_exception = wrapped_exception
-        self.crawling_context = crawling_context
-
-
-class ContextPipelineInterruptedError(Exception):
-    """May be thrown in the initialization phase of a middleware to signal that the request should not be processed."""
-
-
-class ContextPipelineFinalizationError(Exception):
-    """Wraps an exception thrown in the finalization step of a context pipeline middleware.
-
-    We may not have the complete context at this point, so only `BasicCrawlingContext` is provided.
-    """
-
-    def __init__(self, wrapped_exception: Exception, crawling_context: BasicCrawlingContext) -> None:
-        self.wrapped_exception = wrapped_exception
-        self.crawling_context = crawling_context
-
-
 class ContextPipeline(Generic[TCrawlingContext]):
     """Encapsulates the logic of gradually enhancing the crawling context with additional information and utilities.
 
     The enhancement is done by a chain of middlewares that are added to the pipeline after it's creation.
     """
 
     def __init__(
@@ -83,26 +56,30 @@
 
         try:
             for member in reversed(chain):
                 if member._middleware:  # noqa: SLF001
                     middleware_instance = member._middleware(crawling_context)  # noqa: SLF001
                     try:
                         result = await middleware_instance.__anext__()
+                    except SessionError:  # Session errors get special treatment
+                        raise
                     except StopAsyncIteration as e:
                         raise RuntimeError('The middleware did not yield') from e
                     except ContextPipelineInterruptedError:
                         raise
                     except Exception as e:
                         raise ContextPipelineInitializationError(e, crawling_context) from e
 
                     crawling_context = result
                     cleanup_stack.append(middleware_instance)
 
             try:
                 await final_context_consumer(cast(TCrawlingContext, crawling_context))
+            except SessionError:  # Session errors get special treatment
+                raise
             except Exception as e:
                 raise RequestHandlerError(e, crawling_context) from e
         finally:
             for middleware_instance in reversed(cleanup_stack):
                 try:
                     result = await middleware_instance.__anext__()
                 except StopAsyncIteration:  # noqa: PERF203
```

### Comparing `crawlee-0.0.3b6/src/crawlee/basic_crawler/router.py` & `crawlee-0.0.3b7/src/crawlee/basic_crawler/router.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/basic_crawler/types.py` & `crawlee-0.0.3b7/src/crawlee/basic_crawler/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing_extensions import NotRequired, TypedDict, Unpack
 
 if TYPE_CHECKING:
     from crawlee import Glob
     from crawlee.enqueue_strategy import EnqueueStrategy
     from crawlee.http_clients.base_http_client import HttpResponse
     from crawlee.request import BaseRequestData, Request
+    from crawlee.sessions.session import Session
 
 
 class AddRequestsFunctionKwargs(TypedDict):
     """Keyword arguments type for AddRequestsFunction."""
 
     limit: NotRequired[int]
     base_url: NotRequired[str]
@@ -45,23 +46,28 @@
     ) -> Coroutine[None, None, None]: ...
 
 
 class SendRequestFunction(Protocol):
     """Type of a function for performing an HTTP request."""
 
     def __call__(  # noqa: D102
-        self, url: str, *, method: str = 'get', headers: dict[str, str] | None = None
+        self,
+        url: str,
+        *,
+        method: str = 'get',
+        headers: dict[str, str] | None = None,
     ) -> Coroutine[None, None, HttpResponse]: ...
 
 
 @dataclass(frozen=True)
 class BasicCrawlingContext:
     """Basic crawling context intended to be extended by crawlers."""
 
     request: Request
+    session: Session | None
     send_request: SendRequestFunction
     add_requests: AddRequestsFunction
 
 
 @dataclass(frozen=True)
 class FinalStatistics:
     """Statistics about a crawler run."""
```

### Comparing `crawlee-0.0.3b6/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py` & `crawlee-0.0.3b7/src/crawlee/beautifulsoup_crawler/beautifulsoup_crawler.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,28 +3,31 @@
 import asyncio
 from datetime import timedelta
 from typing import TYPE_CHECKING, Any, AsyncGenerator, Awaitable, Callable, Iterable, Literal
 
 import httpx
 from typing_extensions import Unpack
 
+from crawlee._utils.blocked import RETRY_CSS_SELECTORS
 from crawlee.basic_crawler.basic_crawler import BasicCrawler
 from crawlee.basic_crawler.context_pipeline import ContextPipeline
+from crawlee.basic_crawler.errors import SessionError
 from crawlee.beautifulsoup_crawler.types import BeautifulSoupCrawlingContext
 from crawlee.enqueue_strategy import EnqueueStrategy
 from crawlee.http_clients.httpx_client import HttpxClient
 from crawlee.http_crawler.types import HttpCrawlingContext
 from crawlee.request import BaseRequestData
 
 if TYPE_CHECKING:
     from datetime import timedelta
 
     from crawlee.autoscaling.autoscaled_pool import ConcurrencySettings
     from crawlee.basic_crawler.types import AddRequestsFunctionKwargs, BasicCrawlingContext
     from crawlee.configuration import Configuration
+    from crawlee.sessions.session_pool import SessionPool
     from crawlee.storages.request_provider import RequestProvider
 
 
 class BeautifulSoupCrawler(BasicCrawler[BeautifulSoupCrawlingContext]):
     """A crawler that fetches the request URL using `httpx` and parses the result with `BeautifulSoup`."""
 
     def __init__(
@@ -34,14 +37,17 @@
         request_provider: RequestProvider | None = None,
         router: Callable[[BeautifulSoupCrawlingContext], Awaitable[None]] | None = None,
         concurrency_settings: ConcurrencySettings | None = None,
         configuration: Configuration | None = None,
         request_handler_timeout: timedelta | None = None,
         additional_http_error_status_codes: Iterable[int] = (),
         ignore_http_error_status_codes: Iterable[int] = (),
+        session_pool: SessionPool | None = None,
+        use_session_pool: bool = True,
+        retry_on_blocked: bool = True,
     ) -> None:
         """Initialize the BeautifulSoupCrawler.
 
         Args:
             parser: The type of parser that should be used by BeautifulSoup
 
             request_provider: Provides requests to be processed
@@ -54,16 +60,27 @@
 
             request_handler_timeout: How long is a single request handler allowed to run
 
             additional_http_error_status_codes: HTTP status codes that should be considered errors (and trigger a retry)
 
             ignore_http_error_status_codes: HTTP status codes that are normally considered errors but we want to treat
                 them as successful
+
+            use_session_pool: Enables using the session pool for crawling
+
+            session_pool: A preconfigured SessionPool instance if you wish to use non-default configuration
+
+            retry_on_blocked: If set to True, the crawler will try to automatically bypass any detected bot protection
         """
-        context_pipeline = ContextPipeline().compose(self._make_http_request).compose(self._parse_http_response)
+        context_pipeline = (
+            ContextPipeline()
+            .compose(self._make_http_request)
+            .compose(self._parse_http_response)
+            .compose(self._handle_blocked_request)
+        )
 
         self._client = httpx.AsyncClient()
         self._parser = parser
 
         basic_crawler_kwargs = {}
 
         if request_handler_timeout is not None:
@@ -74,28 +91,53 @@
             router=router,
             concurrency_settings=concurrency_settings,
             configuration=configuration,
             http_client=HttpxClient(
                 additional_http_error_status_codes=additional_http_error_status_codes,
                 ignore_http_error_status_codes=ignore_http_error_status_codes,
             ),
+            use_session_pool=use_session_pool,
+            session_pool=session_pool,
+            retry_on_blocked=retry_on_blocked,
             _context_pipeline=context_pipeline,
             **basic_crawler_kwargs,  # type: ignore
         )
 
     async def _make_http_request(self, context: BasicCrawlingContext) -> AsyncGenerator[HttpCrawlingContext, None]:
-        result = await self._http_client.crawl(context.request)
+        result = await self._http_client.crawl(context.request, context.session)
 
         yield HttpCrawlingContext(
             request=context.request,
+            session=context.session,
             send_request=context.send_request,
             add_requests=context.add_requests,
             http_response=result.http_response,
         )
 
+    async def _handle_blocked_request(
+        self, crawling_context: BeautifulSoupCrawlingContext
+    ) -> AsyncGenerator[BeautifulSoupCrawlingContext, None]:
+        if self._retry_on_blocked:
+            status_code = crawling_context.http_response.status_code
+
+            if crawling_context.session and crawling_context.session.is_blocked_status_code(status_code=status_code):
+                raise SessionError(f'Assuming the session is blocked based on HTTP status code {status_code}')
+
+            matched_selectors = [
+                selector for selector in RETRY_CSS_SELECTORS if crawling_context.soup.find(selector) is not None
+            ]
+
+            if matched_selectors:
+                raise SessionError(
+                    'Assuming the session is blocked - '
+                    f"HTTP response matched the following selectors: {'; '.join(matched_selectors)}"
+                )
+
+        yield crawling_context
+
     async def _parse_http_response(
         self, context: HttpCrawlingContext
     ) -> AsyncGenerator[BeautifulSoupCrawlingContext, None]:
         from bs4 import BeautifulSoup, Tag
 
         soup = await asyncio.to_thread(lambda: BeautifulSoup(context.http_response.read(), self._parser))
 
@@ -122,13 +164,14 @@
             uses_patterns = 'include' in kwargs or 'exclude' in kwargs
             kwargs.setdefault('strategy', EnqueueStrategy.SAME_HOSTNAME if uses_patterns else EnqueueStrategy.ALL)
 
             await context.add_requests(requests, **kwargs)
 
         yield BeautifulSoupCrawlingContext(
             request=context.request,
+            session=context.session,
             send_request=context.send_request,
             add_requests=context.add_requests,
             enqueue_links=enqueue_links,
             http_response=context.http_response,
             soup=soup,
         )
```

### Comparing `crawlee-0.0.3b6/src/crawlee/beautifulsoup_crawler/types.py` & `crawlee-0.0.3b7/src/crawlee/beautifulsoup_crawler/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/configuration.py` & `crawlee-0.0.3b7/src/crawlee/configuration.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/events/event_manager.py` & `crawlee-0.0.3b7/src/crawlee/events/event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/events/local_event_manager.py` & `crawlee-0.0.3b7/src/crawlee/events/local_event_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/events/types.py` & `crawlee-0.0.3b7/src/crawlee/events/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/http_clients/base_http_client.py` & `crawlee-0.0.3b7/src/crawlee/http_clients/base_http_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Iterable, Protocol
 
 if TYPE_CHECKING:
     from httpx import Headers  # Type from `httpx` is used here because it is lightweight and convenient
 
     from crawlee.request import Request
+    from crawlee.sessions.session import Session
 
 
 class HttpResponse(Protocol):
     """Response to an HTTP call."""
 
     def read(self) -> bytes:
         """Read the content of the response body."""
@@ -34,20 +35,24 @@
 
 class BaseHttpClient(ABC):
     """An HTTP client used for making HTTP calls in crawlers (`BasicCrawler` subclasses)."""
 
     def __init__(
         self,
         *,
+        persist_cookies_per_session: bool = True,
         additional_http_error_status_codes: Iterable[int] = (),
         ignore_http_error_status_codes: Iterable[int] = (),
     ) -> None:
+        self._persist_cookies_per_session = persist_cookies_per_session
         self._additional_http_error_status_codes = set(additional_http_error_status_codes)
         self._ignore_http_error_status_codes = set(ignore_http_error_status_codes)
 
     @abstractmethod
-    async def crawl(self, request: Request) -> HttpCrawlingResult:
+    async def crawl(self, request: Request, session: Session | None) -> HttpCrawlingResult:
         """Perform a crawl of an URL."""
 
     @abstractmethod
-    async def send_request(self, url: str, *, method: str, headers: Headers | dict[str, str]) -> HttpResponse:
+    async def send_request(
+        self, url: str, *, method: str, headers: Headers | dict[str, str], session: Session | None = None
+    ) -> HttpResponse:
         """Perform an HTTP request."""
```

### Comparing `crawlee-0.0.3b6/src/crawlee/http_crawler/http_crawler.py` & `crawlee-0.0.3b7/src/crawlee/http_crawler/http_crawler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, AsyncGenerator, Awaitable, Callable, Iterable
 
 from crawlee.basic_crawler.basic_crawler import BasicCrawler
 from crawlee.basic_crawler.context_pipeline import ContextPipeline
+from crawlee.basic_crawler.errors import SessionError
 from crawlee.http_clients.httpx_client import HttpxClient
 from crawlee.http_crawler.types import HttpCrawlingContext
 
 if TYPE_CHECKING:
     from datetime import timedelta
 
     from crawlee.autoscaling.autoscaled_pool import ConcurrencySettings
     from crawlee.basic_crawler.types import BasicCrawlingContext
     from crawlee.configuration import Configuration
+    from crawlee.sessions.session_pool import SessionPool
     from crawlee.storages.request_provider import RequestProvider
 
 
 class HttpCrawler(BasicCrawler[HttpCrawlingContext]):
     """A crawler that fetches the request URL using `httpx`."""
 
     def __init__(
@@ -25,14 +27,17 @@
         request_provider: RequestProvider | None = None,
         router: Callable[[HttpCrawlingContext], Awaitable[None]] | None = None,
         concurrency_settings: ConcurrencySettings | None = None,
         configuration: Configuration | None = None,
         request_handler_timeout: timedelta | None = None,
         additional_http_error_status_codes: Iterable[int] = (),
         ignore_http_error_status_codes: Iterable[int] = (),
+        session_pool: SessionPool | None = None,
+        use_session_pool: bool = True,
+        retry_on_blocked: bool = True,
     ) -> None:
         """Initialize the HttpCrawler.
 
         Args:
             request_provider: Provides requests to be processed
 
             router: A callable to which request handling is delegated
@@ -43,16 +48,22 @@
 
             request_handler_timeout: How long is a single request handler allowed to run
 
             additional_http_error_status_codes: HTTP status codes that should be considered errors (and trigger a retry)
 
             ignore_http_error_status_codes: HTTP status codes that are normally considered errors but we want to treat
                 them as successful
+
+            use_session_pool: Enables using the session pool for crawling
+
+            session_pool: A preconfigured SessionPool instance if you wish to use non-default configuration
+
+            retry_on_blocked: If set to True, the crawler will try to automatically bypass any detected bot protection
         """
-        context_pipeline = ContextPipeline().compose(self._make_http_request)
+        context_pipeline = ContextPipeline().compose(self._make_http_request).compose(self._handle_blocked_request)
 
         basic_crawler_kwargs = {}
 
         if request_handler_timeout is not None:
             basic_crawler_kwargs['request_handler_timeout'] = request_handler_timeout
 
         super().__init__(
@@ -61,21 +72,36 @@
             request_provider=request_provider,
             concurrency_settings=concurrency_settings,
             configuration=configuration,
             http_client=HttpxClient(
                 additional_http_error_status_codes=additional_http_error_status_codes,
                 ignore_http_error_status_codes=ignore_http_error_status_codes,
             ),
+            session_pool=session_pool,
+            use_session_pool=use_session_pool,
+            retry_on_blocked=retry_on_blocked,
             **basic_crawler_kwargs,  # type: ignore
         )
 
     async def _make_http_request(
         self, crawling_context: BasicCrawlingContext
     ) -> AsyncGenerator[HttpCrawlingContext, None]:
-        result = await self._http_client.crawl(crawling_context.request)
+        result = await self._http_client.crawl(crawling_context.request, crawling_context.session)
 
         yield HttpCrawlingContext(
             request=crawling_context.request,
+            session=crawling_context.session,
             send_request=crawling_context.send_request,
             add_requests=crawling_context.add_requests,
             http_response=result.http_response,
         )
+
+    async def _handle_blocked_request(
+        self, crawling_context: HttpCrawlingContext
+    ) -> AsyncGenerator[HttpCrawlingContext, None]:
+        if self._retry_on_blocked:
+            status_code = crawling_context.http_response.status_code
+
+            if crawling_context.session and crawling_context.session.is_blocked_status_code(status_code=status_code):
+                raise SessionError(f'Assuming the session is blocked based on HTTP status code {status_code}')
+
+        yield crawling_context
```

### Comparing `crawlee-0.0.3b6/src/crawlee/log_config.py` & `crawlee-0.0.3b7/src/crawlee/log_config.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/request.py` & `crawlee-0.0.3b7/src/crawlee/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -137,14 +137,24 @@
 
     @max_retries.setter
     def max_retries(self, new_max_retries: int) -> None:
         self.user_data.setdefault('__crawlee', {})
         self.user_data['__crawlee']['maxRetries'] = new_max_retries
 
     @property
+    def session_rotation_count(self) -> int | None:
+        """Crawlee-specific number of finished session rotations for the request."""
+        return self.crawlee_data.session_rotation_count
+
+    @session_rotation_count.setter
+    def session_rotation_count(self, new_session_rotation_count: int) -> None:
+        self.user_data.setdefault('__crawlee', {})
+        self.user_data['__crawlee']['sessionRotationCount'] = new_session_rotation_count
+
+    @property
     def enqueue_strategy(self) -> EnqueueStrategy:
         """The strategy used when enqueueing the request."""
         return (
             EnqueueStrategy(self.crawlee_data.enqueue_strategy)
             if self.crawlee_data.enqueue_strategy
             else EnqueueStrategy.ALL
         )
```

### Comparing `crawlee-0.0.3b6/src/crawlee/resource_clients/base_resource_client.py` & `crawlee-0.0.3b7/src/crawlee/resource_clients/base_resource_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/resource_clients/base_resource_collection_client.py` & `crawlee-0.0.3b7/src/crawlee/resource_clients/base_resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/resource_clients/dataset_client.py` & `crawlee-0.0.3b7/src/crawlee/resource_clients/dataset_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/resource_clients/dataset_collection_client.py` & `crawlee-0.0.3b7/src/crawlee/resource_clients/dataset_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/resource_clients/key_value_store_client.py` & `crawlee-0.0.3b7/src/crawlee/resource_clients/key_value_store_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/resource_clients/key_value_store_collection_client.py` & `crawlee-0.0.3b7/src/crawlee/resource_clients/key_value_store_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/resource_clients/request_queue_client.py` & `crawlee-0.0.3b7/src/crawlee/resource_clients/request_queue_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/resource_clients/request_queue_collection_client.py` & `crawlee-0.0.3b7/src/crawlee/resource_clients/request_queue_collection_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/sessions/models.py` & `crawlee-0.0.3b7/src/crawlee/sessions/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/sessions/session.py` & `crawlee-0.0.3b7/src/crawlee/sessions/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,29 +183,25 @@
         If the session does not work due to some external factors as server error such as 5XX you probably want
         to use `mark_bad` method.
         """
         self._error_score += self._max_error_score
         self._usage_count += 1
         # Note: We emit an event here because of the Puppeteer in TS implementation.
 
-    def retire_on_blocked_status_codes(
+    def is_blocked_status_code(
         self,
         *,
         status_code: int,
         additional_blocked_status_codes: list[int] | None = None,
     ) -> bool:
         """Evaluate whether a session should be retired based on the received HTTP status code.
 
         Args:
             status_code: The HTTP status code received from a server response.
             additional_blocked_status_codes: Optional additional status codes that should trigger session retirement.
 
         Returns:
-            True if the session was retired, False otherwise.
+            True if the session should be retired, False otherwise.
         """
         blocked_status_codes = self._blocked_status_codes + (additional_blocked_status_codes or [])
 
-        if status_code in blocked_status_codes:
-            self.retire()
-            return True
-
-        return False
+        return status_code in blocked_status_codes
```

### Comparing `crawlee-0.0.3b6/src/crawlee/sessions/session_pool.py` & `crawlee-0.0.3b7/src/crawlee/sessions/session_pool.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/storage_client_manager.py` & `crawlee-0.0.3b7/src/crawlee/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/storage_clients/base_storage_client.py` & `crawlee-0.0.3b7/src/crawlee/storage_clients/base_storage_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/storage_clients/memory_storage_client.py` & `crawlee-0.0.3b7/src/crawlee/storage_clients/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/storages/base_storage.py` & `crawlee-0.0.3b7/src/crawlee/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/storages/dataset.py` & `crawlee-0.0.3b7/src/crawlee/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/storages/key_value_store.py` & `crawlee-0.0.3b7/src/crawlee/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/storages/models.py` & `crawlee-0.0.3b7/src/crawlee/storages/models.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/storages/request_list.py` & `crawlee-0.0.3b7/src/crawlee/storages/request_list.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/storages/request_provider.py` & `crawlee-0.0.3b7/src/crawlee/storages/request_provider.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/storages/request_queue.py` & `crawlee-0.0.3b7/src/crawlee/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/src/crawlee/types.py` & `crawlee-0.0.3b7/src/crawlee/types.py`

 * *Files identical despite different names*

### Comparing `crawlee-0.0.3b6/PKG-INFO` & `crawlee-0.0.3b7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlee
-Version: 0.0.3b6
+Version: 0.0.3b7
 Summary: Crawlee for Python
 License: Apache-2.0
 Keywords: apify,automation,chrome,crawlee,crawler,headless,scraper,scraping
 Author: Apify Technologies s.r.o.
 Author-email: support@apify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

