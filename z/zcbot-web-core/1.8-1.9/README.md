# Comparing `tmp/zcbot-web-core-1.8.tar.gz` & `tmp/zcbot-web-core-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zcbot-web-core-1.8.tar", last modified: Mon Feb 26 10:27:36 2024, max compression
+gzip compressed data, was "dist\zcbot-web-core-1.9.tar", last modified: Mon Feb 26 13:43:39 2024, max compression
```

## Comparing `zcbot-web-core-1.8.tar` & `zcbot-web-core-1.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 10:27:36.150584 zcbot-web-core-1.8/
--rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-web-core-1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      367 2024-02-26 10:27:36.149584 zcbot-web-core-1.8/PKG-INFO
--rw-rw-rw-   0        0        0      129 2024-02-07 02:27:40.000000 zcbot-web-core-1.8/README.rst
--rw-rw-rw-   0        0        0       42 2024-02-26 10:27:36.150584 zcbot-web-core-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1336 2024-02-26 10:27:31.000000 zcbot-web-core-1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-26 10:27:36.087570 zcbot-web-core-1.8/zcbot_web_core/
--rw-rw-rw-   0        0        0      199 2024-02-07 03:53:22.000000 zcbot-web-core-1.8/zcbot_web_core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-26 10:27:36.095571 zcbot-web-core-1.8/zcbot_web_core/auth/
--rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/auth/__init__.py
--rw-rw-rw-   0        0        0     2095 2024-02-26 09:35:32.000000 zcbot-web-core-1.8/zcbot_web_core/auth/auth_cache_pool.py
--rw-rw-rw-   0        0        0     7868 2024-02-26 10:26:47.000000 zcbot-web-core-1.8/zcbot_web_core/auth/share_auth.py
-drwxrwxrwx   0        0        0        0 2024-02-26 10:27:36.109575 zcbot-web-core-1.8/zcbot_web_core/client/
--rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/client/__init__.py
--rw-rw-rw-   0        0        0     3966 2024-02-07 02:51:50.000000 zcbot-web-core-1.8/zcbot_web_core/client/minio_client.py
--rw-rw-rw-   0        0        0     5676 2024-02-07 02:51:50.000000 zcbot-web-core-1.8/zcbot_web_core/client/mongo_client.py
--rw-rw-rw-   0        0        0     2016 2024-02-07 02:48:39.000000 zcbot-web-core-1.8/zcbot_web_core/client/multi_database_mongo_client.py
--rw-rw-rw-   0        0        0     2314 2024-02-07 02:48:57.000000 zcbot-web-core-1.8/zcbot_web_core/client/multi_tenant_mongo_client.py
--rw-rw-rw-   0        0        0     1779 2024-02-07 02:51:50.000000 zcbot-web-core-1.8/zcbot_web_core/client/mysql_client.py
--rw-rw-rw-   0        0        0     2884 2024-02-07 02:49:48.000000 zcbot-web-core-1.8/zcbot_web_core/client/oss2_client.py
--rw-rw-rw-   0        0        0     1214 2024-02-07 02:55:28.000000 zcbot-web-core-1.8/zcbot_web_core/client/rabbit_client.py
--rw-rw-rw-   0        0        0      979 2024-02-07 02:55:09.000000 zcbot-web-core-1.8/zcbot_web_core/client/redis_client.py
--rw-rw-rw-   0        0        0     2473 2024-02-07 02:54:07.000000 zcbot-web-core-1.8/zcbot_web_core/client/zcbot_celery_client.py
--rw-rw-rw-   0        0        0     2484 2024-02-07 02:54:40.000000 zcbot-web-core-1.8/zcbot_web_core/client/zcbot_predict_client.py
-drwxrwxrwx   0        0        0        0 2024-02-26 10:27:36.111575 zcbot-web-core-1.8/zcbot_web_core/context/
--rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/context/__init__.py
--rw-rw-rw-   0        0        0      317 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/context/context_vars.py
-drwxrwxrwx   0        0        0        0 2024-02-26 10:27:36.114576 zcbot-web-core-1.8/zcbot_web_core/exception/
--rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/exception/__init__.py
--rw-rw-rw-   0        0        0      705 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-02-26 10:27:36.123578 zcbot-web-core-1.8/zcbot_web_core/lib/
--rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/lib/__init__.py
--rw-rw-rw-   0        0        0     1309 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/lib/cfg.py
--rw-rw-rw-   0        0        0     3041 2023-10-24 04:00:18.000000 zcbot-web-core-1.8/zcbot_web_core/lib/func.py
--rw-rw-rw-   0        0        0     1845 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/lib/logger.py
--rw-rw-rw-   0        0        0     1754 2023-10-24 04:00:18.000000 zcbot-web-core-1.8/zcbot_web_core/lib/secret.py
--rw-rw-rw-   0        0        0     9214 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/lib/time.py
--rw-rw-rw-   0        0        0     1052 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/lib/util.py
-drwxrwxrwx   0        0        0        0 2024-02-26 10:27:36.127579 zcbot-web-core-1.8/zcbot_web_core/middleware/
--rw-rw-rw-   0        0        0      799 2024-02-21 02:36:05.000000 zcbot-web-core-1.8/zcbot_web_core/middleware/__init__.py
--rw-rw-rw-   0        0        0     1772 2024-02-21 02:41:26.000000 zcbot-web-core-1.8/zcbot_web_core/middleware/auth.py
--rw-rw-rw-   0        0        0     1138 2024-02-21 02:13:55.000000 zcbot-web-core-1.8/zcbot_web_core/middleware/tenant.py
-drwxrwxrwx   0        0        0        0 2024-02-26 10:27:36.134580 zcbot-web-core-1.8/zcbot_web_core/model/
--rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/model/__init__.py
--rw-rw-rw-   0        0        0      543 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/model/base.py
--rw-rw-rw-   0        0        0      352 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/model/enums.py
--rw-rw-rw-   0        0        0     2437 2024-02-07 02:37:12.000000 zcbot-web-core-1.8/zcbot_web_core/model/handler.py
--rw-rw-rw-   0        0        0     1562 2024-02-26 09:47:10.000000 zcbot-web-core-1.8/zcbot_web_core/model/items.py
--rw-rw-rw-   0        0        0      369 2024-02-07 02:44:30.000000 zcbot-web-core-1.8/zcbot_web_core/model/query.py
-drwxrwxrwx   0        0        0        0 2024-02-26 10:27:36.136581 zcbot-web-core-1.8/zcbot_web_core/scheduler/
--rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/scheduler/__init__.py
--rw-rw-rw-   0        0        0     6025 2024-02-07 02:36:02.000000 zcbot-web-core-1.8/zcbot_web_core/scheduler/simple_server.py
-drwxrwxrwx   0        0        0        0 2024-02-26 10:27:36.141583 zcbot-web-core-1.8/zcbot_web_core/service/
--rw-rw-rw-   0        0        0       43 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/service/__init__.py
--rw-rw-rw-   0        0        0     2113 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/service/multi_process.py
--rw-rw-rw-   0        0        0     2368 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/service/multi_thread.py
--rw-rw-rw-   0        0        0     2132 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/service/thread_pool.py
-drwxrwxrwx   0        0        0        0 2024-02-26 10:27:36.148584 zcbot-web-core-1.8/zcbot_web_core/utils/
--rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/utils/__init__.py
--rw-rw-rw-   0        0        0     4844 2024-02-07 02:57:19.000000 zcbot-web-core-1.8/zcbot_web_core/utils/common.py
--rw-rw-rw-   0        0        0      193 2024-02-07 02:41:13.000000 zcbot-web-core-1.8/zcbot_web_core/utils/context_var.py
--rw-rw-rw-   0        0        0      272 2023-07-10 00:51:51.000000 zcbot-web-core-1.8/zcbot_web_core/utils/decator.py
--rw-rw-rw-   0        0        0     3335 2024-02-22 08:01:11.000000 zcbot-web-core-1.8/zcbot_web_core/utils/encryption.py
--rw-rw-rw-   0        0        0     4293 2024-02-07 02:36:02.000000 zcbot-web-core-1.8/zcbot_web_core/utils/excel_exporter.py
-drwxrwxrwx   0        0        0        0 2024-02-26 10:27:36.092571 zcbot-web-core-1.8/zcbot_web_core.egg-info/
--rw-rw-rw-   0        0        0      367 2024-02-26 10:27:35.000000 zcbot-web-core-1.8/zcbot_web_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1847 2024-02-26 10:27:35.000000 zcbot-web-core-1.8/zcbot_web_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 10:27:35.000000 zcbot-web-core-1.8/zcbot_web_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-02-26 10:27:35.000000 zcbot-web-core-1.8/zcbot_web_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-02-26 13:43:39.090436 zcbot-web-core-1.9/
+-rw-rw-rw-   0        0        0        0 2023-03-14 04:29:15.000000 zcbot-web-core-1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      367 2024-02-26 13:43:39.090436 zcbot-web-core-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      129 2024-02-07 02:27:40.000000 zcbot-web-core-1.9/README.rst
+-rw-rw-rw-   0        0        0       42 2024-02-26 13:43:39.091436 zcbot-web-core-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1336 2024-02-26 13:43:31.000000 zcbot-web-core-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-26 13:43:39.017419 zcbot-web-core-1.9/zcbot_web_core/
+-rw-rw-rw-   0        0        0      199 2024-02-07 03:53:22.000000 zcbot-web-core-1.9/zcbot_web_core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-26 13:43:39.026421 zcbot-web-core-1.9/zcbot_web_core/auth/
+-rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/auth/__init__.py
+-rw-rw-rw-   0        0        0     2095 2024-02-26 09:35:32.000000 zcbot-web-core-1.9/zcbot_web_core/auth/auth_cache_pool.py
+-rw-rw-rw-   0        0        0     7522 2024-02-26 10:29:48.000000 zcbot-web-core-1.9/zcbot_web_core/auth/share_auth.py
+drwxrwxrwx   0        0        0        0 2024-02-26 13:43:39.041425 zcbot-web-core-1.9/zcbot_web_core/client/
+-rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/client/__init__.py
+-rw-rw-rw-   0        0        0     3966 2024-02-07 02:51:50.000000 zcbot-web-core-1.9/zcbot_web_core/client/minio_client.py
+-rw-rw-rw-   0        0        0     5676 2024-02-07 02:51:50.000000 zcbot-web-core-1.9/zcbot_web_core/client/mongo_client.py
+-rw-rw-rw-   0        0        0     2016 2024-02-07 02:48:39.000000 zcbot-web-core-1.9/zcbot_web_core/client/multi_database_mongo_client.py
+-rw-rw-rw-   0        0        0     2314 2024-02-07 02:48:57.000000 zcbot-web-core-1.9/zcbot_web_core/client/multi_tenant_mongo_client.py
+-rw-rw-rw-   0        0        0     1779 2024-02-07 02:51:50.000000 zcbot-web-core-1.9/zcbot_web_core/client/mysql_client.py
+-rw-rw-rw-   0        0        0     2884 2024-02-07 02:49:48.000000 zcbot-web-core-1.9/zcbot_web_core/client/oss2_client.py
+-rw-rw-rw-   0        0        0     1214 2024-02-07 02:55:28.000000 zcbot-web-core-1.9/zcbot_web_core/client/rabbit_client.py
+-rw-rw-rw-   0        0        0      979 2024-02-07 02:55:09.000000 zcbot-web-core-1.9/zcbot_web_core/client/redis_client.py
+-rw-rw-rw-   0        0        0     2473 2024-02-07 02:54:07.000000 zcbot-web-core-1.9/zcbot_web_core/client/zcbot_celery_client.py
+-rw-rw-rw-   0        0        0     2484 2024-02-07 02:54:40.000000 zcbot-web-core-1.9/zcbot_web_core/client/zcbot_predict_client.py
+drwxrwxrwx   0        0        0        0 2024-02-26 13:43:39.044426 zcbot-web-core-1.9/zcbot_web_core/context/
+-rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/context/__init__.py
+-rw-rw-rw-   0        0        0      317 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/context/context_vars.py
+drwxrwxrwx   0        0        0        0 2024-02-26 13:43:39.046426 zcbot-web-core-1.9/zcbot_web_core/exception/
+-rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/exception/__init__.py
+-rw-rw-rw-   0        0        0      705 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-02-26 13:43:39.055428 zcbot-web-core-1.9/zcbot_web_core/lib/
+-rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/lib/__init__.py
+-rw-rw-rw-   0        0        0     1309 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/lib/cfg.py
+-rw-rw-rw-   0        0        0     3041 2023-10-24 04:00:18.000000 zcbot-web-core-1.9/zcbot_web_core/lib/func.py
+-rw-rw-rw-   0        0        0     1845 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/lib/logger.py
+-rw-rw-rw-   0        0        0     1754 2023-10-24 04:00:18.000000 zcbot-web-core-1.9/zcbot_web_core/lib/secret.py
+-rw-rw-rw-   0        0        0     9698 2024-02-26 13:42:25.000000 zcbot-web-core-1.9/zcbot_web_core/lib/time.py
+-rw-rw-rw-   0        0        0     1052 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/lib/util.py
+drwxrwxrwx   0        0        0        0 2024-02-26 13:43:39.059428 zcbot-web-core-1.9/zcbot_web_core/middleware/
+-rw-rw-rw-   0        0        0      799 2024-02-21 02:36:05.000000 zcbot-web-core-1.9/zcbot_web_core/middleware/__init__.py
+-rw-rw-rw-   0        0        0     1772 2024-02-21 02:41:26.000000 zcbot-web-core-1.9/zcbot_web_core/middleware/auth.py
+-rw-rw-rw-   0        0        0     1138 2024-02-21 02:13:55.000000 zcbot-web-core-1.9/zcbot_web_core/middleware/tenant.py
+drwxrwxrwx   0        0        0        0 2024-02-26 13:43:39.066431 zcbot-web-core-1.9/zcbot_web_core/model/
+-rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/model/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/model/base.py
+-rw-rw-rw-   0        0        0      352 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/model/enums.py
+-rw-rw-rw-   0        0        0     2437 2024-02-07 02:37:12.000000 zcbot-web-core-1.9/zcbot_web_core/model/handler.py
+-rw-rw-rw-   0        0        0     1562 2024-02-26 09:47:10.000000 zcbot-web-core-1.9/zcbot_web_core/model/items.py
+-rw-rw-rw-   0        0        0      369 2024-02-07 02:44:30.000000 zcbot-web-core-1.9/zcbot_web_core/model/query.py
+drwxrwxrwx   0        0        0        0 2024-02-26 13:43:39.070431 zcbot-web-core-1.9/zcbot_web_core/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     6025 2024-02-07 02:36:02.000000 zcbot-web-core-1.9/zcbot_web_core/scheduler/simple_server.py
+drwxrwxrwx   0        0        0        0 2024-02-26 13:43:39.078433 zcbot-web-core-1.9/zcbot_web_core/service/
+-rw-rw-rw-   0        0        0       43 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/service/__init__.py
+-rw-rw-rw-   0        0        0     2113 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/service/multi_process.py
+-rw-rw-rw-   0        0        0     2368 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/service/multi_thread.py
+-rw-rw-rw-   0        0        0     2132 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/service/thread_pool.py
+drwxrwxrwx   0        0        0        0 2024-02-26 13:43:39.087435 zcbot-web-core-1.9/zcbot_web_core/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/utils/__init__.py
+-rw-rw-rw-   0        0        0     4844 2024-02-07 02:57:19.000000 zcbot-web-core-1.9/zcbot_web_core/utils/common.py
+-rw-rw-rw-   0        0        0      193 2024-02-07 02:41:13.000000 zcbot-web-core-1.9/zcbot_web_core/utils/context_var.py
+-rw-rw-rw-   0        0        0      272 2023-07-10 00:51:51.000000 zcbot-web-core-1.9/zcbot_web_core/utils/decator.py
+-rw-rw-rw-   0        0        0     3335 2024-02-22 08:01:11.000000 zcbot-web-core-1.9/zcbot_web_core/utils/encryption.py
+-rw-rw-rw-   0        0        0     4293 2024-02-07 02:36:02.000000 zcbot-web-core-1.9/zcbot_web_core/utils/excel_exporter.py
+drwxrwxrwx   0        0        0        0 2024-02-26 13:43:39.022421 zcbot-web-core-1.9/zcbot_web_core.egg-info/
+-rw-rw-rw-   0        0        0      367 2024-02-26 13:43:38.000000 zcbot-web-core-1.9/zcbot_web_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1847 2024-02-26 13:43:38.000000 zcbot-web-core-1.9/zcbot_web_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-26 13:43:38.000000 zcbot-web-core-1.9/zcbot_web_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-02-26 13:43:38.000000 zcbot-web-core-1.9/zcbot_web_core.egg-info/top_level.txt
```

### Comparing `zcbot-web-core-1.8/setup.py` & `zcbot-web-core-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(name='zcbot-web-core',
-      version='1.8',
+      version='1.9',
       description='zcbot web core for zsodata',
       long_description=long_description,
       author='zsodata',
       author_email='team@zso.io',
       url='http://www.zsodata.com',
       install_requires=[
             # "fastapi==0.109.2",
```

### Comparing `zcbot-web-core-1.8/zcbot_web_core/auth/auth_cache_pool.py` & `zcbot-web-core-1.9/zcbot_web_core/auth/auth_cache_pool.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/auth/share_auth.py` & `zcbot-web-core-1.9/zcbot_web_core/auth/share_auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from fastapi.routing import APIRoute
 from starlette.requests import Request
 from ..lib import cfg
 from ..auth import auth_cache_pool
 from ..client.redis_client import Redis
 from ..exception.exceptions import NoAuthException
 from ..model.items import AuthUser, AuthApp
-from ..context.context_vars import tenant_context
 
 logger = logging.getLogger(__name__)
 
 # TODO 暂时如此
 FIX_WHITELIST = [
 ]
 
@@ -202,24 +201,14 @@
 
 
 # 用于handler来Depends，获取授权APP信息
 async def authed_app(request: Request) -> Optional[AuthApp]:
     return ShareAuth().get_auth_app(request)
 
 
-# async def authed_api(request: Request) -> Optional[AuthUser]:
-#     auth_user = ShareAuth().get_auth_api(request)
-#     if auth_user and auth_user.tenantCode:
-#
-#         tenant_context.set(auth_user.tenantCode)
-#     else:
-#         raise NoAuthException()
-#     return auth_user
-
-
 # 用于handler来Depends，获取授权用户所属租户
 async def authed_tenant(request: Request) -> Optional[str]:
     auth_user = ShareAuth().get_auth_user(request)
     if auth_user:
         return auth_user.tenantCode
     return None
```

### Comparing `zcbot-web-core-1.8/zcbot_web_core/client/minio_client.py` & `zcbot-web-core-1.9/zcbot_web_core/client/minio_client.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/client/mongo_client.py` & `zcbot-web-core-1.9/zcbot_web_core/client/mongo_client.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/client/multi_database_mongo_client.py` & `zcbot-web-core-1.9/zcbot_web_core/client/multi_database_mongo_client.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/client/multi_tenant_mongo_client.py` & `zcbot-web-core-1.9/zcbot_web_core/client/multi_tenant_mongo_client.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/client/mysql_client.py` & `zcbot-web-core-1.9/zcbot_web_core/client/mysql_client.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/client/oss2_client.py` & `zcbot-web-core-1.9/zcbot_web_core/client/oss2_client.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/client/rabbit_client.py` & `zcbot-web-core-1.9/zcbot_web_core/client/rabbit_client.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/client/redis_client.py` & `zcbot-web-core-1.9/zcbot_web_core/client/redis_client.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/client/zcbot_celery_client.py` & `zcbot-web-core-1.9/zcbot_web_core/client/zcbot_celery_client.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/client/zcbot_predict_client.py` & `zcbot-web-core-1.9/zcbot_web_core/client/zcbot_predict_client.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/exception/exceptions.py` & `zcbot-web-core-1.9/zcbot_web_core/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/lib/cfg.py` & `zcbot-web-core-1.9/zcbot_web_core/lib/cfg.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/lib/func.py` & `zcbot-web-core-1.9/zcbot_web_core/lib/func.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/lib/logger.py` & `zcbot-web-core-1.9/zcbot_web_core/lib/logger.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/lib/secret.py` & `zcbot-web-core-1.9/zcbot_web_core/lib/secret.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/lib/time.py` & `zcbot-web-core-1.9/zcbot_web_core/lib/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Time Utilities
 
 fast approaches to commonly used time/date related functions
 """
 import datetime
+import math
 import time
 from typing import Optional
+
+import pytz
 from dateutil import tz
 
 
 def now() -> datetime.datetime:
     """
     get datetime instance of time of now
     :return: time of now
@@ -315,14 +318,25 @@
     time_array1 = time.mktime(time.strptime(local_date_srt, "%Y-%m-%d %H:%M:%S.%f"))
     time_array2 = int(time.mktime(utct_date2))  # 1606764117
     # print(time_array1)
     # print(time_array2)
     return time_array2
 
 
+# 获取当前时间到目标时间之间的秒数（用于做过期时间）
+def get_second_from_now(end_time):
+    if end_time and isinstance(end_time, datetime.datetime):
+        if not end_time.tzinfo:
+            end_time = end_time.astimezone(pytz.timezone('Asia/Shanghai'))
+        total_seconds = (end_time - datetime.datetime.now(pytz.timezone('Asia/Shanghai'))).total_seconds()
+        return math.floor(total_seconds)
+
+    return 0
+
+
 if __name__ == '__main__':
     print(time_to_timestamp('2023-06-27 00:00:00'))
     # print(get_time_stamp("2023-06-29T16:00:00.000Z"))
     # time_str = '2021-05-17'
     # print(time_to_timestamp(time_str))
     # print(parse_timestamp(str(int(now().timestamp()))))
     # print(str(1650591873000)[0:10])
```

### Comparing `zcbot-web-core-1.8/zcbot_web_core/lib/util.py` & `zcbot-web-core-1.9/zcbot_web_core/lib/util.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/middleware/__init__.py` & `zcbot-web-core-1.9/zcbot_web_core/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/middleware/auth.py` & `zcbot-web-core-1.9/zcbot_web_core/middleware/auth.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/middleware/tenant.py` & `zcbot-web-core-1.9/zcbot_web_core/middleware/tenant.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/model/base.py` & `zcbot-web-core-1.9/zcbot_web_core/model/base.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/model/handler.py` & `zcbot-web-core-1.9/zcbot_web_core/model/handler.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/model/items.py` & `zcbot-web-core-1.9/zcbot_web_core/model/items.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/scheduler/simple_server.py` & `zcbot-web-core-1.9/zcbot_web_core/scheduler/simple_server.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/service/multi_process.py` & `zcbot-web-core-1.9/zcbot_web_core/service/multi_process.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/service/multi_thread.py` & `zcbot-web-core-1.9/zcbot_web_core/service/multi_thread.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/service/thread_pool.py` & `zcbot-web-core-1.9/zcbot_web_core/service/thread_pool.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/utils/common.py` & `zcbot-web-core-1.9/zcbot_web_core/utils/common.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/utils/encryption.py` & `zcbot-web-core-1.9/zcbot_web_core/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core/utils/excel_exporter.py` & `zcbot-web-core-1.9/zcbot_web_core/utils/excel_exporter.py`

 * *Files identical despite different names*

### Comparing `zcbot-web-core-1.8/zcbot_web_core.egg-info/SOURCES.txt` & `zcbot-web-core-1.9/zcbot_web_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

