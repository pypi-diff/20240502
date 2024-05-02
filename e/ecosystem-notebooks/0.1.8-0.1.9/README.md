# Comparing `tmp/ecosystem-notebooks-0.1.8.tar.gz` & `tmp/ecosystem-notebooks-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecosystem-notebooks-0.1.8.tar", last modified: Fri Apr 19 09:48:58 2024, max compression
+gzip compressed data, was "ecosystem-notebooks-0.1.9.tar", last modified: Tue Apr 23 15:05:25 2024, max compression
```

## Comparing `ecosystem-notebooks-0.1.8.tar` & `ecosystem-notebooks-0.1.9.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.799048 ecosystem-notebooks-0.1.8/
--rw-r--r--   0 ericnewby   (501) staff       (20)     1069 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/LICENSE
--rw-r--r--   0 ericnewby   (501) staff       (20)      400 2023-10-13 03:48:11.000000 ecosystem-notebooks-0.1.8/MANIFEST.in
--rw-r--r--   0 ericnewby   (501) staff       (20)     3646 2024-04-19 09:48:58.798906 ecosystem-notebooks-0.1.8/PKG-INFO
--rw-r--r--   0 ericnewby   (501) staff       (20)     2966 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.8/README.rst
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.777580 ecosystem-notebooks-0.1.8/docs/
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.779780 ecosystem-notebooks-0.1.8/docs/images/
--rw-r--r--   0 ericnewby   (501) staff       (20)    62723 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/docs/images/jupyter_landing_page.png
--rw-r--r--   0 ericnewby   (501) staff       (20)    25467 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/docs/images/login.png
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.780472 ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/
--rw-r--r--   0 ericnewby   (501) staff       (20)     3646 2024-04-19 09:48:58.000000 ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/PKG-INFO
--rw-r--r--   0 ericnewby   (501) staff       (20)     3020 2024-04-19 09:48:58.000000 ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/SOURCES.txt
--rw-r--r--   0 ericnewby   (501) staff       (20)        1 2024-04-19 09:48:58.000000 ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/dependency_links.txt
--rw-r--r--   0 ericnewby   (501) staff       (20)       17 2024-04-19 09:48:58.000000 ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/requires.txt
--rw-r--r--   0 ericnewby   (501) staff       (20)       19 2024-04-19 09:48:58.000000 ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/top_level.txt
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.782269 ecosystem-notebooks-0.1.8/prediction/
--rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/__init__.py
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.790820 ecosystem-notebooks-0.1.8/prediction/apis/
--rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/__init__.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     6645 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/apis/algorithm_client_pulse.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1281 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/auth_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2852 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/apis/data_ingestion_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)    11030 2024-04-17 14:45:49.000000 ecosystem-notebooks-0.1.8/prediction/apis/data_management_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)    13059 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/data_munging_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)   132245 2024-04-19 08:38:39.000000 ecosystem-notebooks-0.1.8/prediction/apis/deployment_management.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1281 2024-04-10 18:52:10.000000 ecosystem-notebooks-0.1.8/prediction/apis/ecosystem_generation_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      889 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/ecosystem_home.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      408 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/ecosystem_main.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1146 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/ecosystem_user_profiles.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2085 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.8/prediction/apis/functions.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      263 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/apis/interactions.py
--rw-r--r--   0 ericnewby   (501) staff       (20)    21095 2024-04-10 03:03:23.000000 ecosystem-notebooks-0.1.8/prediction/apis/online_learning_management.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     9428 2024-04-10 18:23:18.000000 ecosystem-notebooks-0.1.8/prediction/apis/prediction_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2067 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.8/prediction/apis/quickflat.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      246 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/settings_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      811 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/transaction_categorization.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1145 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/user_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2601 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/apis/utilities.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2439 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/apis/worker_aws.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     4520 2024-04-10 18:26:15.000000 ecosystem-notebooks-0.1.8/prediction/apis/worker_file_service.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      520 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/worker_google.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     5168 2024-04-10 18:29:50.000000 ecosystem-notebooks-0.1.8/prediction/apis/worker_h2o.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      311 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/worker_microsoft.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      291 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/apis/worker_open_ai.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2860 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/apis/worker_uber.py
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.794825 ecosystem-notebooks-0.1.8/prediction/endpoints/
--rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/__init__.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     3020 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/algorithm_client_pulse.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1159 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/auth_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1765 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/data_ingestion_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     6030 2024-04-17 14:50:54.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/data_management_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     5350 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/data_munging_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      840 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/ecosystem_generation_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      598 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/ecosystem_home.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      335 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/ecosystem_main.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      754 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/ecosystem_user_profiles.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      155 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/interaction.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     5299 2024-04-07 09:47:48.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/prediction_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      178 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/settings_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      540 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/transaction_categorization.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      471 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/user_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1806 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/utilities.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1766 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/worker_aws.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2238 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/worker_file_service.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      331 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/worker_google.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     3591 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/worker_h2o.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      173 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/worker_microsoft.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      167 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/worker_open_ai.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      831 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/endpoints/worker_uber.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      324 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/prediction/export_to_notebook.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     3190 2024-04-10 02:58:53.000000 ecosystem-notebooks-0.1.8/prediction/jwt_access.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1952 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/nlp_utils.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     4412 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/notebook_functions.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     1689 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/prediction_utils.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     3815 2024-04-18 19:20:21.000000 ecosystem-notebooks-0.1.8/prediction/request_utils.py
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.794973 ecosystem-notebooks-0.1.8/prediction/utils/
--rw-r--r--   0 ericnewby   (501) staff       (20)     5888 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/prediction/utils/endpoint_diff.py
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.795919 ecosystem-notebooks-0.1.8/runtime/
--rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/__init__.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      666 2024-04-10 03:03:23.000000 ecosystem-notebooks-0.1.8/runtime/access.py
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.797448 ecosystem-notebooks-0.1.8/runtime/apis/
--rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/apis/__init__.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     5011 2024-04-15 14:37:55.000000 ecosystem-notebooks-0.1.8/runtime/apis/data_management_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     9917 2024-04-16 16:08:31.000000 ecosystem-notebooks-0.1.8/runtime/apis/predictor_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      452 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/apis/restart_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      840 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/apis/runtime_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)    14076 2023-04-24 06:53:33.000000 ecosystem-notebooks-0.1.8/runtime/apis/worker_utilities.py
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.798457 ecosystem-notebooks-0.1.8/runtime/endpoints/
--rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/endpoints/__init__.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2431 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/runtime/endpoints/data_management_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     2538 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/runtime/endpoints/predictor_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      302 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/endpoints/restart_controller.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      283 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/endpoints/runtime_engine.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     6123 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/runtime/endpoints/worker_utilities.py
--rw-r--r--   0 ericnewby   (501) staff       (20)      324 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.8/runtime/export_to_notebook.py
--rw-r--r--   0 ericnewby   (501) staff       (20)     3632 2024-04-08 10:10:58.000000 ecosystem-notebooks-0.1.8/runtime/request_utils.py
-drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-19 09:48:58.798631 ecosystem-notebooks-0.1.8/runtime/utils/
--rw-r--r--   0 ericnewby   (501) staff       (20)     5079 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.8/runtime/utils/endpoint_diff.py
--rw-r--r--   0 ericnewby   (501) staff       (20)       38 2024-04-19 09:48:58.799102 ecosystem-notebooks-0.1.8/setup.cfg
--rw-r--r--   0 ericnewby   (501) staff       (20)     2151 2024-04-19 09:48:53.000000 ecosystem-notebooks-0.1.8/setup.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-23 15:05:25.362275 ecosystem-notebooks-0.1.9/
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1069 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/LICENSE
+-rw-r--r--   0 ericnewby   (501) staff       (20)      400 2023-10-13 03:48:11.000000 ecosystem-notebooks-0.1.9/MANIFEST.in
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3693 2024-04-23 15:05:25.361840 ecosystem-notebooks-0.1.9/PKG-INFO
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2966 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.9/README.rst
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-23 15:05:25.318476 ecosystem-notebooks-0.1.9/docs/
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-23 15:05:25.320999 ecosystem-notebooks-0.1.9/docs/images/
+-rw-r--r--   0 ericnewby   (501) staff       (20)    62723 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/docs/images/jupyter_landing_page.png
+-rw-r--r--   0 ericnewby   (501) staff       (20)    25467 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/docs/images/login.png
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-23 15:05:25.321844 ecosystem-notebooks-0.1.9/ecosystem_notebooks.egg-info/
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3693 2024-04-23 15:05:25.000000 ecosystem-notebooks-0.1.9/ecosystem_notebooks.egg-info/PKG-INFO
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3020 2024-04-23 15:05:25.000000 ecosystem-notebooks-0.1.9/ecosystem_notebooks.egg-info/SOURCES.txt
+-rw-r--r--   0 ericnewby   (501) staff       (20)        1 2024-04-23 15:05:25.000000 ecosystem-notebooks-0.1.9/ecosystem_notebooks.egg-info/dependency_links.txt
+-rw-r--r--   0 ericnewby   (501) staff       (20)       17 2024-04-23 15:05:25.000000 ecosystem-notebooks-0.1.9/ecosystem_notebooks.egg-info/requires.txt
+-rw-r--r--   0 ericnewby   (501) staff       (20)       19 2024-04-23 15:05:25.000000 ecosystem-notebooks-0.1.9/ecosystem_notebooks.egg-info/top_level.txt
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-23 15:05:25.324059 ecosystem-notebooks-0.1.9/prediction/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/__init__.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-23 15:05:25.346450 ecosystem-notebooks-0.1.9/prediction/apis/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/apis/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)    13360 2024-04-22 14:40:22.000000 ecosystem-notebooks-0.1.9/prediction/apis/algorithm_client_pulse.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1281 2024-04-22 15:48:07.000000 ecosystem-notebooks-0.1.9/prediction/apis/auth_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3208 2024-04-23 05:45:55.000000 ecosystem-notebooks-0.1.9/prediction/apis/data_ingestion_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)    11030 2024-04-17 14:45:49.000000 ecosystem-notebooks-0.1.9/prediction/apis/data_management_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)    13059 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/apis/data_munging_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)   149673 2024-04-23 14:47:21.000000 ecosystem-notebooks-0.1.9/prediction/apis/deployment_management.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1281 2024-04-10 18:52:10.000000 ecosystem-notebooks-0.1.9/prediction/apis/ecosystem_generation_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      889 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/apis/ecosystem_home.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      408 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/apis/ecosystem_main.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1146 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/apis/ecosystem_user_profiles.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2085 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.9/prediction/apis/functions.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      263 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/prediction/apis/interactions.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)    21095 2024-04-10 03:03:23.000000 ecosystem-notebooks-0.1.9/prediction/apis/online_learning_management.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     9428 2024-04-10 18:23:18.000000 ecosystem-notebooks-0.1.9/prediction/apis/prediction_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2067 2023-12-07 07:29:59.000000 ecosystem-notebooks-0.1.9/prediction/apis/quickflat.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      246 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/apis/settings_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      811 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/apis/transaction_categorization.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1145 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/apis/user_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2601 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/prediction/apis/utilities.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2439 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/prediction/apis/worker_aws.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     4520 2024-04-10 18:26:15.000000 ecosystem-notebooks-0.1.9/prediction/apis/worker_file_service.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      520 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/apis/worker_google.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5168 2024-04-10 18:29:50.000000 ecosystem-notebooks-0.1.9/prediction/apis/worker_h2o.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      311 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/apis/worker_microsoft.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      291 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/prediction/apis/worker_open_ai.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2860 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/apis/worker_uber.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-23 15:05:25.356551 ecosystem-notebooks-0.1.9/prediction/endpoints/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3020 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/algorithm_client_pulse.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1159 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/auth_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1765 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/data_ingestion_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     6030 2024-04-17 14:50:54.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/data_management_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5350 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/data_munging_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      840 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/ecosystem_generation_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      598 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/ecosystem_home.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      335 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/ecosystem_main.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      754 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/ecosystem_user_profiles.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      155 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/interaction.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5299 2024-04-07 09:47:48.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/prediction_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      178 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/settings_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      540 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/transaction_categorization.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      471 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/user_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1806 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/utilities.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1766 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/worker_aws.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2238 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/worker_file_service.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      331 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/worker_google.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3591 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/worker_h2o.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      173 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/worker_microsoft.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      167 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/worker_open_ai.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      831 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/endpoints/worker_uber.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      324 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/prediction/export_to_notebook.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3190 2024-04-10 02:58:53.000000 ecosystem-notebooks-0.1.9/prediction/jwt_access.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1952 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/nlp_utils.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     4412 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/notebook_functions.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     1689 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/prediction_utils.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3815 2024-04-18 19:20:21.000000 ecosystem-notebooks-0.1.9/prediction/request_utils.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-23 15:05:25.356834 ecosystem-notebooks-0.1.9/prediction/utils/
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5888 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/prediction/utils/endpoint_diff.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-23 15:05:25.357948 ecosystem-notebooks-0.1.9/runtime/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/runtime/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      666 2024-04-10 03:03:23.000000 ecosystem-notebooks-0.1.9/runtime/access.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-23 15:05:25.359878 ecosystem-notebooks-0.1.9/runtime/apis/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/runtime/apis/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5011 2024-04-15 14:37:55.000000 ecosystem-notebooks-0.1.9/runtime/apis/data_management_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     9917 2024-04-16 16:08:31.000000 ecosystem-notebooks-0.1.9/runtime/apis/predictor_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      452 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/runtime/apis/restart_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      840 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/runtime/apis/runtime_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)    14076 2023-04-24 06:53:33.000000 ecosystem-notebooks-0.1.9/runtime/apis/worker_utilities.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-23 15:05:25.361204 ecosystem-notebooks-0.1.9/runtime/endpoints/
+-rw-r--r--   0 ericnewby   (501) staff       (20)        0 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/runtime/endpoints/__init__.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2431 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/runtime/endpoints/data_management_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2538 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/runtime/endpoints/predictor_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      302 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/runtime/endpoints/restart_controller.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      283 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/runtime/endpoints/runtime_engine.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     6123 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/runtime/endpoints/worker_utilities.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)      324 2023-03-30 15:23:49.000000 ecosystem-notebooks-0.1.9/runtime/export_to_notebook.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)     3632 2024-04-08 10:10:58.000000 ecosystem-notebooks-0.1.9/runtime/request_utils.py
+drwxr-xr-x   0 ericnewby   (501) staff       (20)        0 2024-04-23 15:05:25.361400 ecosystem-notebooks-0.1.9/runtime/utils/
+-rw-r--r--   0 ericnewby   (501) staff       (20)     5079 2022-12-31 01:50:44.000000 ecosystem-notebooks-0.1.9/runtime/utils/endpoint_diff.py
+-rw-r--r--   0 ericnewby   (501) staff       (20)       38 2024-04-23 15:05:25.362350 ecosystem-notebooks-0.1.9/setup.cfg
+-rw-r--r--   0 ericnewby   (501) staff       (20)     2151 2024-04-23 15:05:12.000000 ecosystem-notebooks-0.1.9/setup.py
```

### Comparing `ecosystem-notebooks-0.1.8/LICENSE` & `ecosystem-notebooks-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/PKG-INFO` & `ecosystem-notebooks-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: ecosystem-notebooks
-Version: 0.1.8
+Version: 0.1.9
 Summary: Ecosystem Notebooks is a wrapper for the Ecosystem API servers.
 Home-page: https://github.com/ecosystemai/ecosystem-notebooks
 Author: EcosystemAi
 Author-email: jay@ecosystem.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Jupyter :: JupyterLab
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: pymongo
 
 Ecosystem Notebooks
 ===================
 
 What is Ecosystem Notebooks?
 ----------------------------
```

### Comparing `ecosystem-notebooks-0.1.8/README.rst` & `ecosystem-notebooks-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/docs/images/jupyter_landing_page.png` & `ecosystem-notebooks-0.1.9/docs/images/jupyter_landing_page.png`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/docs/images/login.png` & `ecosystem-notebooks-0.1.9/docs/images/login.png`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/PKG-INFO` & `ecosystem-notebooks-0.1.9/ecosystem_notebooks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: ecosystem-notebooks
-Version: 0.1.8
+Version: 0.1.9
 Summary: Ecosystem Notebooks is a wrapper for the Ecosystem API servers.
 Home-page: https://github.com/ecosystemai/ecosystem-notebooks
 Author: EcosystemAi
 Author-email: jay@ecosystem.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Jupyter :: JupyterLab
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: pymongo
 
 Ecosystem Notebooks
 ===================
 
 What is Ecosystem Notebooks?
 ----------------------------
```

### Comparing `ecosystem-notebooks-0.1.8/ecosystem_notebooks.egg-info/SOURCES.txt` & `ecosystem-notebooks-0.1.9/ecosystem_notebooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/auth_controller.py` & `ecosystem-notebooks-0.1.9/prediction/apis/auth_controller.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/data_ingestion_engine.py` & `ecosystem-notebooks-0.1.9/prediction/apis/data_ingestion_engine.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from prediction.endpoints import data_ingestion_engine as endpoints
 from prediction import request_utils
 
 def add_metadocumemnts(auth, meta_documents, info=False):
+    """
+    Store metadata documents
+
+    :param auth: Authentication token generated by the jwt_access module
+    :param meta_documents: A dictionary specifying the metadata documents to be stored and the location in which they are to be stored. meta_documents should be in the following format: {"database": "", "collection": "", "document": {}}
+    """
     ep = endpoints.ADD_META_DOCUMENTS
     resp = request_utils.create(auth, ep, json=meta_documents, info=info)
     response = resp.json()
     return response
 
 def delete_ingestmeta(auth, ingest_meta, info=False):
     ep = endpoints.DELETE_INGEST_META
```

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/data_management_engine.py` & `ecosystem-notebooks-0.1.9/prediction/apis/data_management_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/data_munging_engine.py` & `ecosystem-notebooks-0.1.9/prediction/apis/data_munging_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/deployment_management.py` & `ecosystem-notebooks-0.1.9/prediction/apis/deployment_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,16 +89,19 @@
 def get_api_endpoint_code_default():
     return ""
 
 def get_pre_score_code(pre_score, project_details):
     pre_score_code_options = {
         "": "package com.ecosystem.plugin.customer;\n\nimport com.datastax.oss.driver.api.core.CqlSession;\nimport org.json.JSONObject;\n\npublic class PrePredictCustomer {\n\n    public PrePredictCustomer() {\n    }\n\n    /**\n     * Pre-pre predict\n     */\n    public void getPrePredict() {\n    }\n\n    /**\n     * getPostPredict\n     * @param params\n     * @param session\n     * @return\n     */\n    public static JSONObject getPrePredict(JSONObject params, CqlSession session) {\n\n        /*\n        Manipulate params that will be used by scoring and post-scoring\n         */\n\n        return params;\n    }\n\n}\n",
     }
-    version_list = [i["version"] for i in project_details["deployment_step"] if
-                    i["plugins"]["pre_score_class_text"] == pre_score]
+    if "deployment_step" in project_details:
+        version_list = [i["version"] for i in project_details["deployment_step"] if
+                        i["plugins"]["pre_score_class_text"] == pre_score]
+    else:
+        version_list = []
     if version_list:
         max_version = max(version_list)
         pre_score_logic = [i["plugins"]["pre_score_class_code"] for i in project_details["deployment_step"] if
                             (i["plugins"]["pre_score_class_text"] == pre_score and i["version"] == max_version)][0]
     elif pre_score in pre_score_code_options:
         pre_score_logic = pre_score_code_options[pre_score]
     else:
@@ -113,44 +116,403 @@
         "PlatformDynamicEngagement.java": "package com.ecosystem.plugin.customer;\n\nimport com.datastax.oss.driver.api.core.CqlSession;\nimport com.ecosystem.utils.DataTypeConversions;\nimport com.ecosystem.utils.JSONArraySort;\nimport hex.genmodel.easy.EasyPredictModelWrapper;\nimport com.ecosystem.utils.log.LogManager;\nimport com.ecosystem.utils.log.Logger;\nimport org.json.JSONArray;\nimport org.json.JSONObject;\n\n/**\n * ECOSYSTEM.AI INTERNAL PLATFORM SCORING\n * Use this class to score with dynamic sampling configurations. This class is configured to work with no model.\n */\npublic class PlatformDynamicEngagement extends PostScoreSuper {\n\tprivate static final Logger LOGGER = LogManager.getLogger(PlatformDynamicEngagement.class.getName());\n\n\tpublic PlatformDynamicEngagement() {\n\t}\n\n\t/**\n\t * Pre-post predict logic\n\t */\n\tpublic void getPostPredict () {\n\t}\n\n\t/**\n\t * getPostPredict\n\t * Example params:\n\t *    {\"contextual_variable_one\":\"Easy Income Gold|Thin|Senior\", \"contextual_variable_two\":\"\", \"batch\": true}\n\t *\n\t * @param predictModelMojoResult Result from scoring\n\t * @param params                 Params carried from input\n\t * @param session                Session variable for Cassandra\n\t * @return JSONObject result to further post-scoring logic\n\t */\n\tpublic static JSONObject getPostPredict(JSONObject predictModelMojoResult, JSONObject params, CqlSession session, EasyPredictModelWrapper[] models) {\n\t\tdouble startTimePost = System.nanoTime();\n\t\ttry {\n\t\t\t/** Setup JSON objects for specific prediction case */\n\t\t\tJSONObject featuresObj = predictModelMojoResult.getJSONObject(\"featuresObj\");\n\t\t\t//JSONObject domainsProbabilityObj = predictModelMojoResult.getJSONObject(\"domainsProbabilityObj\");\n\n\t\t\tJSONObject offerMatrixWithKey = new JSONObject();\n\t\t\tboolean om = false;\n\t\t\tif (params.has(\"offerMatrixWithKey\")) {\n\t\t\t\tofferMatrixWithKey = params.getJSONObject(\"offerMatrixWithKey\");\n\t\t\t\tom = true;\n\t\t\t}\n\n\t\t\tJSONObject work = params.getJSONObject(\"in_params\");\n\n\t\t\t/***************************************************************************************************/\n\t\t\t/** Standardized approach to access dynamic datasets in plugin.\n\t\t\t * The options array is the data set/feature_store that's keeping track of the dynamic changes.\n\t\t\t * The optionParams is the parameter set that will influence the real-time behavior through param changes.\n\t\t\t */\n\t\t\t/***************************************************************************************************/\n\t\t\tJSONArray options = (JSONArray) ((\n\t\t\t\t\t(JSONObject) params.getJSONObject(\"dynamicCorpora\")\n\t\t\t\t\t\t\t.get(\"dynamic_engagement_options\")).get(\"data\"));\n\t\t\tJSONObject optionParams = (JSONObject) ((\n\t\t\t\t\t(JSONObject) params.getJSONObject(\"dynamicCorpora\")\n\t\t\t\t\t\t\t.get(\"dynamic_engagement\")).get(\"data\"));\n\n\t\t\tJSONObject contextual_variables = optionParams.getJSONObject(\"contextual_variables\");\n\t\t\tJSONObject randomisation = optionParams.getJSONObject(\"randomisation\");\n\n\t\t\t/***************************************************************************************************/\n\t\t\t/** Test if contextual variable is coming via api or feature store: API takes preference... */\n\t\t\tif (!work.has(\"contextual_variable_one\")) {\n\t\t\t\tif (featuresObj.has(contextual_variables.getString(\"contextual_variable_one_name\")))\n\t\t\t\t\twork.put(\"contextual_variable_one\", featuresObj.get(contextual_variables.getString(\"contextual_variable_one_name\")));\n\t\t\t\telse\n\t\t\t\t\twork.put(\"contextual_variable_one\", \"\");\n\t\t\t}\n\t\t\tif (!work.has(\"contextual_variable_two\")) {\n\t\t\t\tif (featuresObj.has(contextual_variables.getString(\"contextual_variable_two_name\")))\n\t\t\t\t\twork.put(\"contextual_variable_two\", featuresObj.get(contextual_variables.getString(\"contextual_variable_two_name\")));\n\t\t\t\telse\n\t\t\t\t\twork.put(\"contextual_variable_two\", \"\");\n\t\t\t}\n\t\t\t/***************************************************************************************************/\n\n\t\t\tJSONArray finalOffers = new JSONArray();\n\t\t\tint offerIndex = 0;\n\t\t\tint explore;\n\t\t\tString contextual_variable_one = String.valueOf(work.get(\"contextual_variable_one\"));\n\t\t\tString contextual_variable_two = String.valueOf(work.get(\"contextual_variable_two\"));\n\t\t\tfor (int j = 0; j < options.length(); j++) {\n\t\t\t\tJSONObject option = options.getJSONObject(j);\n\t\t\t\tString contextual_variable_one_Option = \"\";\n\t\t\t\tif (option.has(\"contextual_variable_one\") && !contextual_variable_one.equals(\"\"))\n\t\t\t\t\tcontextual_variable_one_Option = String.valueOf(option.get(\"contextual_variable_one\"));\n\t\t\t\tString contextual_variable_two_Option = \"\";\n\t\t\t\tif (option.has(\"contextual_variable_two\") && !contextual_variable_two.equals(\"\"))\n\t\t\t\t\tcontextual_variable_two_Option = String.valueOf(option.get(\"contextual_variable_two\"));\n\n\t\t\t\tif (contextual_variable_one_Option.equals(contextual_variable_one) && contextual_variable_two_Option.equals(contextual_variable_two)) {\n\n\t\t\t\t\tdouble alpha = (double) DataTypeConversions.getDoubleFromIntLong(option.get(\"alpha\"));\n\t\t\t\t\tdouble beta = (double) DataTypeConversions.getDoubleFromIntLong(option.get(\"beta\"));\n\t\t\t\t\tdouble accuracy = 0.001;\n\t\t\t\t\tif (option.has(\"accuracy\"))\n\t\t\t\t\t\taccuracy = (double) DataTypeConversions.getDoubleFromIntLong(option.get(\"accuracy\"));\n\n\t\t\t\t\t/***************************************************************************************************/\n\t\t\t\t\t/* r IS THE RANDOMIZED SCORE VALUE */\n\t\t\t\t\tdouble p = 0.0;\n\t\t\t\t\tdouble arm_reward = 0.001;\n\t\t\t\t\tif (randomisation.getString(\"approach\").equals(\"epsilonGreedy\")) {\n\t\t\t\t\t\t// params.put(\"explore\", 0);\n\t\t\t\t\t\texplore = 0;\n\t\t\t\t\t\tp = DataTypeConversions.getDouble(option, \"arm_reward\");\n\t\t\t\t\t\tarm_reward = p;\n\t\t\t\t\t} else {\n\t\t\t\t\t\t/** REMEMBER THAT THIS IS HERE BECAUSE OF BATCH PROCESS, OTHERWISE IT REQUIRES THE TOTAL COUNTS */\n\t\t\t\t\t\t/* Phase 2: sampling - calculate the arms and rank them */\n\t\t\t\t\t\t// params.put(\"explore\", 0); // force explore to zero and use Thompson Sampling only!!\n\t\t\t\t\t\texplore = 0; // set as explore as the dynamic responder is exploration based...\n\t\t\t\t\t\tp = DataTypeConversions.getDouble(option, \"arm_reward\");\n\t\t\t\t\t\tarm_reward = p;\n\n\t\t\t\t\t}\n\t\t\t\t\t/** Check if values are correct */\n\t\t\t\t\tif (p != p) p = 0.0;\n\t\t\t\t\tif (alpha != alpha) alpha = 0.0;\n\t\t\t\t\tif (beta != beta) beta = 0.0;\n\t\t\t\t\tif (arm_reward != arm_reward) arm_reward = 0.0;\n\t\t\t\t\t/***************************************************************************************************/\n\n\t\t\t\t\tString offer = option.getString(\"optionKey\");\n\n\t\t\t\t\tJSONObject singleOffer = new JSONObject();\n\t\t\t\t\tdouble offer_value = 1.0;\n\t\t\t\t\tdouble offer_cost = 1.0;\n\t\t\t\t\tdouble modified_offer_score = p;\n\t\t\t\t\tif (om) {\n\t\t\t\t\t\tif (offerMatrixWithKey.has(offer)) {\n\n\t\t\t\t\t\t\tsingleOffer = offerMatrixWithKey.getJSONObject(offer);\n\n\t\t\t\t\t\t\tif (singleOffer.has(\"offer_price\"))\n\t\t\t\t\t\t\t\toffer_value = DataTypeConversions.getDouble(singleOffer, \"offer_price\");\n\t\t\t\t\t\t\tif (singleOffer.has(\"price\"))\n\t\t\t\t\t\t\t\toffer_value = DataTypeConversions.getDouble(singleOffer, \"price\");\n\n\t\t\t\t\t\t\tif (singleOffer.has(\"offer_cost\"))\n\t\t\t\t\t\t\t\toffer_cost = singleOffer.getDouble(\"offer_cost\");\n\t\t\t\t\t\t\tif (singleOffer.has(\"cost\"))\n\t\t\t\t\t\t\t\toffer_cost = singleOffer.getDouble(\"cost\");\n\n\t\t\t\t\t\t\tmodified_offer_score = p * ((double) offer_value - offer_cost);\n\t\t\t\t\t\t}\n\t\t\t\t\t}\n\n\t\t\t\t\tJSONObject finalOffersObject = new JSONObject();\n\n\t\t\t\t\tfinalOffersObject.put(\"offer\", offer);\n\t\t\t\t\tfinalOffersObject.put(\"offer_name\", offer);\n\t\t\t\t\tfinalOffersObject.put(\"offer_name_desc\", option.getString(\"option\"));\n\n\t\t\t\t\t/* process final */\n\t\t\t\t\tfinalOffersObject.put(\"score\", p);\n\t\t\t\t\tfinalOffersObject.put(\"final_score\", p);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", modified_offer_score);\n\t\t\t\t\tfinalOffersObject.put(\"offer_value\", offer_value);\n\t\t\t\t\tfinalOffersObject.put(\"price\", offer_value);\n\t\t\t\t\tfinalOffersObject.put(\"cost\", offer_cost);\n\n\t\t\t\t\tfinalOffersObject.put(\"p\", p);\n\t\t\t\t\tif (option.has(\"contextual_variable_one\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"contextual_variable_one\", option.getString(\"contextual_variable_one\"));\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"contextual_variable_one\", \"\");\n\n\t\t\t\t\tif (option.has(\"contextual_variable_two\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"contextual_variable_two\", option.getString(\"contextual_variable_two\"));\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"contextual_variable_two\", \"\");\n\n\t\t\t\t\tfinalOffersObject.put(\"alpha\", alpha);\n\t\t\t\t\tfinalOffersObject.put(\"beta\", beta);\n\t\t\t\t\tfinalOffersObject.put(\"weighting\", (double) DataTypeConversions.getDoubleFromIntLong(option.get(\"weighting\")));\n\t\t\t\t\tfinalOffersObject.put(\"explore\", explore);\n\t\t\t\t\tfinalOffersObject.put(\"uuid\", params.get(\"uuid\"));\n\t\t\t\t\tfinalOffersObject.put(\"arm_reward\", arm_reward);\n\n\t\t\t\t\t/* Debugging variables */\n\t\t\t\t\tif (!option.has(\"expected_takeup\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"expected_takeup\", -1.0);\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"expected_takeup\", (double) DataTypeConversions.getDoubleFromIntLong(option.get(\"expected_takeup\")));\n\n\t\t\t\t\tif (!option.has(\"propensity\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"propensity\", -1.0);\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"propensity\", (double) DataTypeConversions.getDoubleFromIntLong(option.get(\"propensity\")));\n\n\t\t\t\t\tif (!option.has(\"epsilon_nominated\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"epsilon_nominated\", -1.0);\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"epsilon_nominated\", (double) DataTypeConversions.getDoubleFromIntLong(option.get(\"epsilon_nominated\")));\n\n\t\t\t\t\tfinalOffers.put(offerIndex, finalOffersObject);\n\t\t\t\t\tofferIndex = offerIndex + 1;\n\t\t\t\t}\n\t\t\t}\n\n\t\t\tJSONArray sortJsonArray = JSONArraySort.sortArray(finalOffers, \"arm_reward\", \"double\", \"d\");\n\t\t\tpredictModelMojoResult.put(\"final_result\", sortJsonArray);\n\n\t\t\tpredictModelMojoResult = getTopScores(params, predictModelMojoResult);\n\n\t\t\tdouble endTimePost = System.nanoTime();\n\t\t\tLOGGER.info(\"PlatformDynamicEngagement:I001: time in ms: \".concat( String.valueOf((endTimePost - startTimePost) / 1000000) ));\n\n\t\t} catch (Exception e) {\n\t\t\te.printStackTrace();\n\t\t\tLOGGER.error(e);\n\t\t}\n\n\t\treturn predictModelMojoResult;\n\n\t}\n\n}\n",
         "PostScoreBasic.java": "package com.ecosystem.plugin.customer;\n\nimport com.datastax.oss.driver.api.core.CqlSession;\nimport com.ecosystem.utils.DataTypeConversions;\nimport com.ecosystem.utils.JSONArraySort;\nimport hex.genmodel.easy.EasyPredictModelWrapper;\nimport com.ecosystem.utils.log.LogManager;\nimport com.ecosystem.utils.log.Logger;\nimport org.json.JSONArray;\nimport org.json.JSONObject;\n\nimport java.util.ArrayList;\n\nimport static com.ecosystem.EcosystemResponse.obtainBudget;\n\n/**\n * This the ecosystem/Ai generic post-score template.\n * Customer plugin for specialized logic to be added to the runtime engine.\n * This class is loaded through the plugin loader system.\n */\npublic class PostScoreBasic extends PostScoreSuper {\n\tprivate static final Logger LOGGER = LogManager.getLogger(PostScoreBasic.class.getName());\n\n\tpublic PostScoreBasic() {\n\t}\n\n\t/**\n\t * Pre-post predict logic\n\t */\n\tpublic void getPostPredict () {\n\t}\n\n\t/**\n\t * getPostPredict\n\t *\n\t * @param predictModelMojoResult Result from scoring\n\t * @param params                 Params carried from input\n\t * @param session                Session variable for Cassandra\n\t * @param models \t\t\t\t Preloaded H2O Models\n\t * @return JSONObject result to further post-scoring logic\n\t */\n\tpublic static JSONObject getPostPredict(JSONObject predictModelMojoResult, JSONObject params, CqlSession session, EasyPredictModelWrapper[] models) {\n\t\tdouble startTimePost = System.nanoTime();\n\t\ttry {\n\t\t\t/* Setup JSON objects for specific prediction case */\n\t\t\tJSONObject featuresObj = predictModelMojoResult.getJSONObject(\"featuresObj\");\n\t\t\tJSONObject domainsProbabilityObj = new JSONObject();\n\t\t\tif (predictModelMojoResult.has(\"domainsProbabilityObj\"))\n\t\t\t\tdomainsProbabilityObj = predictModelMojoResult.getJSONObject(\"domainsProbabilityObj\");\n\n\t\t\t/* If whitelist settings then only allow offers on list */\n\t\t\tboolean whitelist = false;\n\t\t\tArrayList<String> offerWhiteList = new ArrayList<>();\n\t\t\tif (params.has(\"whitelist\")) {\n\t\t\t\tif (!params.getJSONObject(\"whitelist\").isEmpty()) {\n\t\t\t\t\tofferWhiteList = (ArrayList<String>) params.getJSONObject(\"whitelist\").get(\"whitelist\");\n\t\t\t\t\tparams.put(\"resultcount\", offerWhiteList.size());\n\t\t\t\t\twhitelist = DataTypeConversions.getBooleanFromString(params.getJSONObject(\"whitelist\").get(\"logicin\"));\n\t\t\t\t}\n\t\t\t}\n\n\t\t\tif (params.has(\"preloadCorpora\")) {\n\t\t\t\tif (params.getJSONObject(\"preloadCorpora\").has(\"network\")) {\n\t\t\t\t\tJSONObject a = params.getJSONObject(\"preloadCorpora\");\n\t\t\t\t\tJSONObject preloadCorpora = a.getJSONObject(\"network\");\n\t\t\t\t}\n\t\t\t}\n\n\t\t\tJSONArray finalOffers = new JSONArray();\n\t\t\tint resultcount = (int) params.get(\"resultcount\");\n\t\t\t/* For each offer in offer matrix determine eligibility */\n\t\t\t/* get selector field from properties: predictor.selector.setup */\n\t\t\t// String s = new JSONObject(settings.getSelectorSetup()).getJSONObject(\"lookup\").getString(\"fields\");\n\n\t\t\t/** This loop can be used to add number of offers/options to return result */\n\t\t\tJSONObject finalOffersObject = new JSONObject();\n\t\t\tint offerIndex = 0;\n\t\t\tfor (int i = 0; i < resultcount; i++) {\n\n\t\t\t\t/** Model type based approaches */\n\t\t\t\tString type = \"\";\n\t\t\t\tboolean explainability = false;\n\t\t\t\t// LOGGER.info(\"predictModelMojoResult: \" + predictModelMojoResult.toString());\n\t\t\t\tif (predictModelMojoResult.get(\"type\").getClass().getName().toLowerCase().contains(\"array\")) {\n\t\t\t\t\ttype = predictModelMojoResult\n\t\t\t\t\t\t\t.getJSONArray(\"type\")\n\t\t\t\t\t\t\t.get(0)\n\t\t\t\t\t\t\t.toString().toLowerCase().trim();\n\t\t\t\t\tif (predictModelMojoResult.has(\"shapley_contributions\"))\n\t\t\t\t\t\texplainability = true;\n\t\t\t\t} else {\n\t\t\t\t\ttype = ((String) predictModelMojoResult.get(\"type\")).toLowerCase().trim();\n\t\t\t\t}\n\n\t\t\t\t/** Offer name, defaults to type (replace with offer matrix etc) */\n\t\t\t\tif (featuresObj.has(\"offer_name_final\"))\n\t\t\t\t\tfinalOffersObject.put(\"offer_name\", featuresObj.get(\"offer_name_final\"));\n\t\t\t\telse\n\t\t\t\t\tfinalOffersObject.put(\"offer_name\", type);\n\n\t\t\t\tif (featuresObj.has(\"offer\"))\n\t\t\t\t\tfinalOffersObject.put(\"offer\", featuresObj.get(\"offer\"));\n\t\t\t\telse\n\t\t\t\t\tfinalOffersObject.put(\"offer\", type);\n\n\t\t\t\tif (featuresObj.has(\"offer_id\"))\n\t\t\t\t\tfinalOffersObject.put(\"offer\", featuresObj.get(\"offer_id\"));\n\t\t\t\telse\n\t\t\t\t\tfinalOffersObject.put(\"offer_id\", type);\n\n\t\t\t\tif (featuresObj.has(\"price\"))\n\t\t\t\t\tfinalOffersObject.put(\"price\", featuresObj.get(\"price\"));\n\t\t\t\telse\n\t\t\t\t\tfinalOffersObject.put(\"price\", 1.0);\n\n\t\t\t\tif (featuresObj.has(\"cost\"))\n\t\t\t\t\tfinalOffersObject.put(\"cost\", featuresObj.get(\"cost\"));\n\t\t\t\telse\n\t\t\t\t\tfinalOffersObject.put(\"cost\", 1.0);\n\n\t\t\t\t/** Score based on model type */\n\t\t\t\tif (type.contains(\"clustering\")) {\n\t\t\t\t\tfinalOffersObject.put(\"cluster\", predictModelMojoResult.getJSONArray(\"cluster\").get(0));\n\t\t\t\t\tfinalOffersObject.put(\"score\", DataTypeConversions.getDouble(domainsProbabilityObj, \"score\"));\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", DataTypeConversions.getDouble(domainsProbabilityObj, \"score\"));\n\t\t\t\t} else if (type.contains(\"anomalydetection\")) {\n\t\t\t\t\tdouble[] score = (double[]) domainsProbabilityObj.get(\"score\");\n\t\t\t\t\tfinalOffersObject.put(\"score\", score[0]);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", score[0]);\n\t\t\t\t} else if (type.contains(\"regression\")) {\n\t\t\t\t\tObject score = predictModelMojoResult.getJSONArray(\"value\").get(0);\n\t\t\t\t\tfinalOffersObject.put(\"score\", score);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", score);\n\t\t\t\t} else if (type.contains(\"multinomial\")) {\n\t\t\t\t\tObject probability = predictModelMojoResult.getJSONArray(\"probability\").get(0);\n\t\t\t\t\tObject label = null;\n\t\t\t\t\ttry {\n\t\t\t\t\t\tlabel = predictModelMojoResult.getJSONArray(\"label\").get(0);\n\t\t\t\t\t} catch (Exception e) {\n\t\t\t\t\t\tLOGGER.error(\"PostScoreBasic:getPostPredict:E001: Error relates to scoring your model. The model wasn't loaded or is not accessible.\");\n\t\t\t\t\t\te.printStackTrace();\n\t\t\t\t\t}\n\t\t\t\t\tObject response = predictModelMojoResult.getJSONArray(\"response\").get(0);\n\t\t\t\t\tfinalOffersObject.put(\"score\", probability);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", probability);\n\t\t\t\t\tfinalOffersObject.put(\"offer\", label);\n\t\t\t\t\tfinalOffersObject.put(\"offer_name\", response);\n\t\t\t\t} else if (type.contains(\"coxph\")) {\n\t\t\t\t\tObject score = predictModelMojoResult.getJSONArray(\"value\").get(0);\n\t\t\t\t\tfinalOffersObject.put(\"score\", score);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", score);\n\t\t\t\t} else if (type.contains(\"wordembedding\")) {\n\t\t\t\t\tfloat[] score = (float[]) predictModelMojoResult.getJSONArray(\"_text_word2vec\").get(0);\n\t\t\t\t\tfinalOffersObject.put(\"score\", Double.valueOf(String.valueOf(score[0])));\n\t\t\t\t\tfinalOffersObject.put(\"embedding\", score);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", 0.0);\n\t\t\t\t} else if (type.contains(\"deeplearning\")) {\n\t\t\t\t\t/** From TensorFlow or PyTorch */\n\t\t\t\t\tObject score = domainsProbabilityObj.getDouble(\"1\");\n\t\t\t\t\tfinalOffersObject.put(\"score\", score);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", score);\n\t\t\t\t\tObject response = predictModelMojoResult.getJSONArray(\"response\").get(0);\n\t\t\t\t\tfinalOffersObject.put(\"offer_name\", response);\n\t\t\t\t} else if (type.contains(\"empty score\")) {\n\t\t\t\t\t/** This is typically used for data lookup only, obtain values from feature store! */\n\t\t\t\t\tif (featuresObj.has(\"offer_name\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"offer_name\", featuresObj.get(\"offer_name\"));\n\n\t\t\t\t\tif (featuresObj.has(\"offer\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"offer\", featuresObj.get(\"offer\"));\n\n\t\t\t\t\tif (featuresObj.has(\"score\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"score\", Double.valueOf(String.valueOf(featuresObj.get(\"score\"))));\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"score\", 1.0);\n\n\t\t\t\t\tif (featuresObj.has(\"modified_offer_score\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", Double.valueOf(String.valueOf(featuresObj.get(\"modified_offer_score\"))));\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", 1.0);\n\n\t\t\t\t\tif (featuresObj.has(\"cost\"))\n\t\t\t\t\t\tfinalOffersObject.put(\"cost\", Double.valueOf(String.valueOf(featuresObj.get(\"cost\"))));\n\t\t\t\t\telse\n\t\t\t\t\t\tfinalOffersObject.put(\"cost\", 0.0);\n\n\t\t\t\t} else {\n\t\t\t\t\tfinalOffersObject.put(\"score\", 1.0);\n\t\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", 1.0);\n\t\t\t\t}\n\n\t\t\t\tfinalOffersObject.put(\"offer_details\", domainsProbabilityObj);\n\t\t\t\tif (explainability) {\n\t\t\t\t\tfinalOffersObject.put(\"shapley_contributions\", predictModelMojoResult.get(\"shapley_contributions\"));\n\t\t\t\t\tfinalOffersObject.put(\"shapley_contributions_names\", predictModelMojoResult.get(\"shapley_contributions_names\"));\n\t\t\t\t}\n\n\t\t\t\t/** Default value, could be replaced by offer matrix or feature store */\n\t\t\t\tdouble offer_value = 1.0;\n\t\t\t\tfinalOffersObject.put(\"offer_value\", offer_value);\n\t\t\t\tfinalOffersObject.put(\"uuid\", params.get(\"uuid\"));\n\n\t\t\t\t/** Add other structures to the final result */\n\t\t\t\tfinalOffersObject.put(\"offer_matrix\", featuresObj);\n\n\t\t\t\t/** Budget processing option, if it's set in the properties */\n\t\t\t\tif (settings.getPredictorOfferBudget() != null) {\n\t\t\t\t\tJSONObject budgetItem = obtainBudget(featuresObj, params.getJSONObject(\"featuresObj\"), offer_value);\n\t\t\t\t\tdouble budgetSpendLimit = budgetItem.getDouble(\"spend_limit\");\n\t\t\t\t\tfinalOffersObject.put(\"spend_limit\", budgetSpendLimit);\n\t\t\t\t}\n\n\t\t\t\t/** Prepare offer array before final sorting */\n\t\t\t\tfinalOffers.put(offerIndex, finalOffersObject);\n\t\t\t\tofferIndex = offerIndex + 1;\n\t\t\t}\n\n\t\t\t/** Sort final offer list based on score */\n\t\t\tJSONArray sortJsonArray = JSONArraySort.sortArray(finalOffers, \"score\", \"double\", \"d\");\n\t\t\tpredictModelMojoResult.put(\"final_result\", sortJsonArray);\n\n\t\t} catch (Exception e) {\n\t\t\tLOGGER.error(e);\n\t\t}\n\n\t\t/** Get top scores and test for explore/exploit randomization */\n\t\tpredictModelMojoResult = getTopScores(params, predictModelMojoResult);\n\n\t\tdouble endTimePost = System.nanoTime();\n\t\tLOGGER.info(\"getPostPredict:I001: execution time in ms: \".concat( String.valueOf((endTimePost - startTimePost) / 1000000) ));\n\t\treturn predictModelMojoResult;\n\t}\n\n}\n",
         "PostScoreRecommender.java": "package com.ecosystem.plugin.customer;\n\nimport com.datastax.oss.driver.api.core.CqlSession;\nimport com.ecosystem.utils.GlobalSettings;\nimport com.ecosystem.utils.JSONArraySort;\nimport com.ecosystem.utils.MathRandomizer;\nimport hex.genmodel.easy.EasyPredictModelWrapper;\nimport com.ecosystem.utils.log.LogManager;\nimport com.ecosystem.utils.log.Logger;\nimport org.json.JSONArray;\nimport org.json.JSONObject;\n\nimport java.io.IOException;\n\n/**\n * ECOSYSTEM.AI INTERNAL PLATFORM SCORING\n * Use this class to perform generic scoring based on model and generic settings with label from scoring.\n */\npublic class PostScoreRecommender {\n\tprivate static final Logger LOGGER = LogManager.getLogger(PostScoreRecommender.class.getName());\n\n\tstatic GlobalSettings settings;\n\tstatic {\n\t\ttry {\n\t\t\tsettings = new GlobalSettings();\n\t\t} catch (IOException e) {\n\t\t\te.printStackTrace();\n\t\t} catch (Exception e) {\n\t\t\te.printStackTrace();\n\t\t}\n\t}\n\n\tpublic PostScoreRecommender() {\n\t}\n\n\t/**\n\t * Pre-post predict logic\n\t */\n\tpublic void getPostPredict () {\n\t}\n\n\t/**\n\t * getPostPredict\n\t * Example params:\n\t *    {\"contextual_variable_one\":\"Easy Income Gold|Thin|Senior\", \"contextual_variable_two\":\"\", \"batch\": true}\n\t *\n\t * @param predictModelMojoResult Result from scoring\n\t * @param params                 Params carried from input\n\t * @param session                Session variable for Cassandra\n\t * @return JSONObject result to further post-scoring logic\n\t */\n\tpublic static JSONObject getPostPredict(JSONObject predictModelMojoResult, JSONObject params, CqlSession session, EasyPredictModelWrapper[] models) {\n\t\tdouble startTimePost = System.nanoTime();\n\t\ttry {\n\t\t\t/* Setup JSON objects for specific prediction case */\n\t\t\tJSONObject featuresObj = predictModelMojoResult.getJSONObject(\"featuresObj\");\n\t\t\tif (predictModelMojoResult.has(\"ErrorMessage\")) {\n\t\t\t\tLOGGER.error(\"getPostPredict:E001a:\" + predictModelMojoResult.get(\"ErrorMessage\"));\n\t\t\t\treturn null;\n\t\t\t}\n\n\t\t\tJSONArray offerMatrix = new JSONArray();\n\t\t\tif (params.has(\"offerMatrix\"))\n\t\t\t\tofferMatrix = params.getJSONArray(\"offerMatrix\");\n\n\t\t\tJSONObject work = params.getJSONObject(\"in_params\");\n\n\t\t\tJSONObject domainsProbabilityObj = predictModelMojoResult.getJSONObject(\"domainsProbabilityObj\");\n\t\t\tString label = predictModelMojoResult.getJSONArray(\"label\").getString(0);\n\n\t\t\tJSONArray probabilities = new JSONArray();\n\t\t\tif (predictModelMojoResult.has(\"probability\"))\n\t\t\t\tprobabilities = predictModelMojoResult.getJSONArray(\"probability\");\n\t\t\telse\n\t\t\t\tprobabilities = predictModelMojoResult.getJSONArray(\"probabilities\");\n\n\t\t\tJSONArray domains = predictModelMojoResult.getJSONArray(\"domains\");\n\n\t\t\tJSONArray finalOffers = new JSONArray();\n\t\t\tint resultcount = (int) params.get(\"resultcount\");\n\t\t\tint offerIndex = 0;\n\n\t\t\t/** Select top items based on number of offers to present */\n\t\t\tfor (int i = 0; i < resultcount; i++) {\n\t\t\t\tint explore = (int) params.get(\"explore\");\n\t\t\t\tJSONObject finalOffersObject = new JSONObject();\n\n\t\t\t\tfinalOffersObject.put(\"offer\", label);\n\t\t\t\tfinalOffersObject.put(\"offer_name\", label);\n\t\t\t\tfinalOffersObject.put(\"offer_name_desc\", label + \" - \" + i);\n\n\t\t\t\t/** process final */\n\t\t\t\tdouble p = domainsProbabilityObj.getDouble(label);\n\t\t\t\tfinalOffersObject.put(\"score\", p);\n\t\t\t\tfinalOffersObject.put(\"final_score\", p);\n\t\t\t\tfinalOffersObject.put(\"modified_offer_score\", p);\n\t\t\t\tfinalOffersObject.put(\"offer_value\", 1.0); // use value from offer matrix\n\t\t\t\tfinalOffersObject.put(\"price\", 1.0);\n\t\t\t\tfinalOffersObject.put(\"cost\", 1.0);\n\n\t\t\t\tfinalOffersObject.put(\"p\", p);\n\t\t\t\tfinalOffersObject.put(\"explore\", explore);\n\n\t\t\t\t/** Prepare array before final sort */\n\t\t\t\tfinalOffers.put(offerIndex, finalOffersObject);\n\t\t\t\tofferIndex = offerIndex + 1;\n\t\t\t}\n\n\t\t\tJSONArray sortJsonArray = JSONArraySort.sortArray(finalOffers, \"score\", \"double\", \"d\");\n\t\t\tpredictModelMojoResult.put(\"final_result\", sortJsonArray);\n\n\t\t} catch (Exception e) {\n\t\t\te.printStackTrace();\n\t\t\tLOGGER.error(e);\n\t\t}\n\n\t\tpredictModelMojoResult = getTopScores(params, predictModelMojoResult);\n\n\t\tdouble endTimePost = System.nanoTime();\n\t\tLOGGER.info(\"PlatformDynamicEngagement:I001: time in ms: \".concat( String.valueOf((endTimePost - startTimePost) / 1000000) ));\n\n\t\treturn predictModelMojoResult;\n\n\t}\n\n\tprivate static JSONObject getExplore(JSONObject params, double epsilonIn, String name) {\n\t\tdouble rand = MathRandomizer.getRandomDoubleBetweenRange(0, 1);\n\t\tdouble epsilon = epsilonIn;\n\t\tparams.put(name + \"_epsilon\", epsilon);\n\t\tif (rand <= epsilon) {\n\t\t\tparams.put(name, 1);\n\t\t} else {\n\t\t\tparams.put(name, 0);\n\t\t}\n\t\treturn params;\n\t}\n\n\t/**\n\t * Get random results for MAB\n\t * @param predictResult\n\t * @param numberOffers\n\t * @return\n\t */\n\tpublic static JSONArray getSelectedPredictResultRandom(JSONObject predictResult, int numberOffers) {\n\t\treturn getSelectedPredictResultExploreExploit(predictResult, numberOffers, 1);\n\t}\n\n\t/**\n\t * Get result based on score\n\t * @param predictResult\n\t * @param numberOffers\n\t * @return\n\t */\n\tpublic static JSONArray getSelectedPredictResult(JSONObject predictResult, int numberOffers) {\n\t\treturn getSelectedPredictResultExploreExploit(predictResult, numberOffers, 0);\n\t}\n\n\tprivate static JSONObject setValues(JSONObject work) {\n\t\tJSONObject result = new JSONObject();\n\t\tresult.put(\"score\", work.get(\"score\"));\n\t\tif (work.has(\"price\"))\n\t\t\tresult.put(\"price\", work.get(\"price\"));\n\t\tif (work.has(\"cost\"))\n\t\t\tresult.put(\"cost\", work.get(\"cost\"));\n\t\tresult.put(\"final_score\", work.get(\"score\"));\n\t\tresult.put(\"offer\", work.get(\"offer\"));\n\t\tresult.put(\"offer_name\", work.get(\"offer_name\"));\n\t\tresult.put(\"modified_offer_score\", work.get(\"modified_offer_score\"));\n\t\tresult.put(\"offer_value\", work.get(\"offer_value\"));\n\t\treturn result;\n\t}\n\n\t/**\n\t * Set values JSONObject that will be used in final\n\t * @param work\n\t * @param rank\n\t * @return\n\t */\n\tprivate static JSONObject setValuesFinal(JSONObject work, int rank) {\n\t\tJSONObject offer = new JSONObject();\n\n\t\toffer.put(\"rank\", rank);\n\t\toffer.put(\"result\", setValues(work));\n\t\toffer.put(\"result_full\", work);\n\n\t\treturn offer;\n\t}\n\n\t/**\n\t * Review this: Master version in EcosystemMaster class. {offer_treatment_code: {$regex:\"_A\"}}\n\t *\n\t * @param predictResult\n\t * @param numberOffers\n\t * @return\n\t */\n\tpublic static JSONArray getSelectedPredictResultExploreExploit(JSONObject predictResult, int numberOffers, int explore) {\n\t\tJSONArray offers = new JSONArray();\n\t\tint resultLength = predictResult.getJSONArray(\"final_result\").length();\n\n\t\tfor (int j = 0, k = 0; j < resultLength; j++) {\n\t\t\tJSONObject work = new JSONObject();\n\t\t\tif (explore == 1) {\n\t\t\t\tint rand = MathRandomizer.getRandomIntBetweenRange(0, resultLength - 1);\n\t\t\t\twork = predictResult.getJSONArray(\"final_result\").getJSONObject(rand);\n\t\t\t} else {\n\t\t\t\twork = predictResult.getJSONArray(\"final_result\").getJSONObject(j);\n\t\t\t}\n\n\t\t\t/* test if budget is enabled && spend_limit is greater than 0, if budget is disabled, then this will be 1.0 */\n\t\t\tif (settings.getPredictorOfferBudget() != null) {\n\t\t\t\t/* if budget setting and there is budget to spend */\n\t\t\t\tif (work.has(\"spend_limit\")) {\n\t\t\t\t\tif ((work.getDouble(\"spend_limit\") > 0.0) | work.getDouble(\"spend_limit\") == -1) {\n\t\t\t\t\t\toffers.put(k, setValuesFinal(work, k + 1));\n\t\t\t\t\t\tif ((k + 1) == numberOffers) break;\n\t\t\t\t\t\tk = k + 1;\n\t\t\t\t\t}\n\t\t\t\t} else {\n\t\t\t\t\tbreak;\n\t\t\t\t}\n\t\t\t} else {\n\t\t\t\t/* no budget setting present */\n\t\t\t\toffers.put(k, setValuesFinal(work, k + 1));\n\t\t\t\tif ((k + 1) == numberOffers) break;\n\t\t\t\tk = k + 1;\n\t\t\t}\n\t\t}\n\n\t\treturn offers;\n\t}\n\n\t/**\n\t * @param params\n\t * @param predictResult\n\t * @return\n\t */\n\tprivate static JSONObject getTopScores(JSONObject params, JSONObject predictResult) {\n\t\tint resultCount = 1;\n\t\tif (params.has(\"resultcount\")) resultCount = params.getInt(\"resultcount\");\n\t\tif (predictResult.getJSONArray(\"final_result\").length() <= resultCount)\n\t\t\tresultCount = predictResult.getJSONArray(\"final_result\").length();\n\n\t\t/* depending on epsilon and mab settings */\n\t\tif (params.getInt(\"explore\") == 0) {\n\t\t\tpredictResult.put(\"final_result\", getSelectedPredictResult(predictResult, resultCount));\n\t\t\tpredictResult.put(\"explore\", 0);\n\t\t} else {\n\t\t\tpredictResult.put(\"final_result\", getSelectedPredictResultRandom(predictResult, resultCount));\n\t\t\tpredictResult.put(\"explore\", 1);\n\t\t}\n\t\treturn predictResult;\n\t}\n\n}\n",
         "PostScoreRecommenderOffers.java": "package com.ecosystem.plugin.customer;\n\nimport com.datastax.oss.driver.api.core.CqlSession;\nimport com.ecosystem.utils.DataTypeConversions;\nimport com.ecosystem.utils.JSONArraySort;\nimport hex.genmodel.easy.EasyPredictModelWrapper;\nimport com.ecosystem.utils.log.LogManager;\nimport com.ecosystem.utils.log.Logger;\nimport org.json.JSONArray;\nimport org.json.JSONObject;\n\n/**\n * recommender_smp - Single model for all products with Offermatrix\n * Multiclass classifier trained on offer_name response column, offer matrix need to have all the offers loaded with offer_price.\n */\npublic class PostScoreRecommenderOffers extends PostScoreSuper {\n    private static final Logger LOGGER = LogManager.getLogger(PostScoreRecommenderOffers.class.getName());\n\n    public PostScoreRecommenderOffers() {\n    }\n\n    /**\n     * Pre-post predict logic\n     */\n    public void getPostPredict () {\n    }\n\n    /**\n     * getPostPredict\n     *\n     * @param predictModelMojoResult Result from scoring\n     * @param params                 Params carried from input\n     * @param session                Session variable for Cassandra\n     * @return JSONObject result to further post-scoring logic\n     */\n    public static JSONObject getPostPredict(JSONObject predictModelMojoResult, JSONObject params, CqlSession session, EasyPredictModelWrapper[] models) {\n        double startTimePost = System.nanoTime();\n        try {\n            /** Value obtained via API params */\n            JSONObject work = params.getJSONObject(\"in_params\");\n            double in_balance = 1000.0;\n            if (work.has(\"in_balance\"))\n                in_balance = DataTypeConversions.getDouble(work, \"in_balance\");\n            else\n                LOGGER.info(\"getPostPredict:I001aa: No in_balance specified, default used. (1000.00)\");\n\n            JSONArray sortJsonArray = new JSONArray();\n            JSONArray finalOffers = new JSONArray();\n\n            /* Setup JSON objects for specific prediction case */\n            JSONObject featuresObj = predictModelMojoResult.getJSONObject(\"featuresObj\");\n            if (predictModelMojoResult.has(\"ErrorMessage\")) {\n                LOGGER.error(\"getPostPredict:E001a:\" + predictModelMojoResult.get(\"ErrorMessage\"));\n                return null;\n            }\n\n            JSONArray offerMatrix = new JSONArray();\n            if (params.has(\"offerMatrix\"))\n                offerMatrix = params.getJSONArray(\"offerMatrix\");\n\n            JSONObject domainsProbabilityObj = predictModelMojoResult.getJSONObject(\"domainsProbabilityObj\");\n            String label = predictModelMojoResult.getJSONArray(\"label\").getString(0);\n            JSONArray domains = predictModelMojoResult.getJSONArray(\"domains\");\n\n            int resultcount = (int) params.get(\"resultcount\");\n            int offerIndex = 0;\n\n            /** Select top items based on number of offers to present */\n            for (int i = 0; i < offerMatrix.length(); i++) {\n                JSONObject singleOffer = offerMatrix.getJSONObject(i);\n\n                int explore = (int) params.get(\"explore\");\n                JSONObject finalOffersObject = new JSONObject();\n\n                double offer_value = 1.0;\n                if (singleOffer.has(\"offer_price\"))\n                    offer_value = DataTypeConversions.getDouble(singleOffer, \"offer_price\");\n                if (singleOffer.has(\"price\"))\n                    offer_value = DataTypeConversions.getDouble(singleOffer, \"price\");\n\n                double offer_cost = 1.0;\n                if (singleOffer.has(\"offer_cost\"))\n                    offer_cost = singleOffer.getDouble(\"offer_cost\");\n                if (singleOffer.has(\"cost\"))\n                    offer_cost = singleOffer.getDouble(\"cost\");\n\n                double p = 0.0;\n                String offer_id = \"\";\n                if (domainsProbabilityObj.has(singleOffer.getString(\"offer_id\"))) {\n                    offer_id = singleOffer.getString(\"offer_id\");\n                    p = domainsProbabilityObj.getDouble(offer_id);\n                } else {\n                    LOGGER.error(\"offerRecommender:E002-1: \" + params.get(\"uuid\") + \" - Not available: \" + singleOffer.getString(\"offer_name\"));\n                }\n\n                double modified_offer_score = 1.0;\n                modified_offer_score = p * ((double) offer_value - offer_cost);\n\n                finalOffersObject.put(\"offer\", offer_id);\n                finalOffersObject.put(\"offer_name\", singleOffer.get(\"offer_name\"));\n                finalOffersObject.put(\"offer_name_desc\", singleOffer.get(\"offer_name\") + \" - \" + i);\n\n                /** process final */\n                // double p = domainsProbabilityObj.getDouble(label);\n                finalOffersObject.put(\"score\", p);\n                finalOffersObject.put(\"final_score\", p);\n                finalOffersObject.put(\"modified_offer_score\", modified_offer_score);\n                finalOffersObject.put(\"offer_value\", offer_value); // use value from offer matrix\n                finalOffersObject.put(\"price\", offer_value);\n                finalOffersObject.put(\"cost\", offer_cost);\n                finalOffersObject.put(\"uuid\", params.get(\"uuid\"));\n\n                finalOffersObject.put(\"p\", p);\n                finalOffersObject.put(\"explore\", explore);\n\n                /** Prepare array before final sort */\n                finalOffers.put(offerIndex, finalOffersObject);\n                offerIndex = offerIndex + 1;\n            }\n\n            sortJsonArray = JSONArraySort.sortArray(finalOffers, \"modified_offer_score\", \"double\", \"d\");\n            predictModelMojoResult.put(\"final_result\", sortJsonArray);\n\n            /** Select the correct number of offers */\n            predictModelMojoResult = getTopScores(params, predictModelMojoResult);\n\n        } catch (Exception e) {\n            e.printStackTrace();\n            LOGGER.error(e);\n        }\n\n        /** Top scores from final_result */\n        predictModelMojoResult = getTopScores(params, predictModelMojoResult);\n\n        double endTimePost = System.nanoTime();\n        LOGGER.info(\"PostScoreRecommenderOffers:I001: time in ms: \".concat( String.valueOf((endTimePost - startTimePost) / 1000000) ));\n\n        return predictModelMojoResult;\n\n    }\n\n}\n",
         "PostScoreRecommenderMulti.java": "package com.ecosystem.plugin.customer;\n\nimport com.datastax.oss.driver.api.core.CqlSession;\nimport com.ecosystem.plugin.lib.ScoreAsyncItems;\nimport com.ecosystem.utils.DataTypeConversions;\nimport com.ecosystem.utils.GlobalSettings;\nimport com.ecosystem.utils.JSONArraySort;\nimport com.ecosystem.utils.MathRandomizer;\nimport com.ecosystem.worker.h2o.ModelPredictWorkerH2O;\nimport hex.genmodel.easy.EasyPredictModelWrapper;\nimport hex.genmodel.easy.RowData;\nimport com.ecosystem.utils.log.LogManager;\nimport com.ecosystem.utils.log.Logger;\nimport org.json.JSONArray;\nimport org.json.JSONObject;\n\nimport java.io.IOException;\nimport java.util.concurrent.ExecutionException;\n\n/**\n * recommender_smp - Multiple models for per product with Offermatrix\n * Binomial model per product, all loaded into memory, scoring per offerMatrix line item.\n */\npublic class PostScoreRecommenderMulti {\n\n    private static final Logger LOGGER = LogManager.getLogger(PostScoreRecommenderMulti.class.getName());\n\n    ModelPredictWorkerH2O modelPredictWorkerH2O;\n    ScoreAsyncItems scoreAsyncItems;\n\n    static GlobalSettings settings;\n    static {\n        try {\n            settings = new GlobalSettings();\n        } catch (IOException e) {\n            e.printStackTrace();\n        } catch (Exception e) {\n            e.printStackTrace();\n        }\n    }\n\n    public PostScoreRecommenderMulti() {\n        modelPredictWorkerH2O = new ModelPredictWorkerH2O();\n        scoreAsyncItems = new ScoreAsyncItems(modelPredictWorkerH2O);\n    }\n\n    /**\n     * Pre-post predict logic\n     */\n    public void getPostPredict () {\n    }\n\n    /**\n     * getPostPredict\n     *\n     * @param predictModelMojoResult Result from scoring\n     * @param params                 Params carried from input\n     * @param session                Session variable for Cassandra\n     * @return JSONObject result to further post-scoring logic\n     */\n    public JSONObject getPostPredict(JSONObject predictModelMojoResult, JSONObject params, CqlSession session, EasyPredictModelWrapper[] models) {\n\n        double startTimePost = System.nanoTime();\n\n        /** Value obtained via API params */\n        JSONObject work = params.getJSONObject(\"in_params\");\n        double in_balance = 100.0;\n        if (work.has(\"in_balance\"))\n            in_balance = DataTypeConversions.getDouble(work, \"in_balance\");\n        else\n            LOGGER.info(\"getPostPredict:I001aa: No in_balance specified, default used. (1000.00)\");\n\n        JSONArray finalOffers = new JSONArray();\n\n        /* Setup JSON objects for specific prediction case */\n        JSONObject featuresObj = predictModelMojoResult.getJSONObject(\"featuresObj\");\n        if (predictModelMojoResult.has(\"ErrorMessage\")) {\n            LOGGER.error(\"getPostPredict:E001a:\" + predictModelMojoResult.get(\"ErrorMessage\"));\n            return null;\n        }\n\n        JSONArray offerMatrix = new JSONArray();\n        if (params.has(\"offerMatrix\"))\n            offerMatrix = params.getJSONArray(\"offerMatrix\");\n\n        // JSONObject domainsProbabilityObj = predictModelMojoResult.getJSONObject(\"domainsProbabilityObj\");\n        // String label = predictModelMojoResult.getJSONArray(\"label\").getString(0);\n        // JSONArray domains = predictModelMojoResult.getJSONArray(\"domains\");\n\n        int resultcount = (int) params.get(\"resultcount\");\n        int offerIndex = 0;\n\n        /** Async processing scoring across all models loaded per offer */\n        JSONObject domainsProbabilityObj = new JSONObject();\n        if (predictModelMojoResult.has(\"domainsProbabilityObj\"))\n            domainsProbabilityObj = predictModelMojoResult.getJSONObject(\"domainsProbabilityObj\");\n\n        JSONObject resultScore = new JSONObject();\n        try {\n            double startTimePost1 = System.nanoTime();\n\n            RowData row = modelPredictWorkerH2O.toRowData((JSONObject) predictModelMojoResult.get(\"features\"));\n            resultScore = scoreAsyncItems.allOfAsyncScoring(offerMatrix, params, models, row, domainsProbabilityObj);\n\n            double endTimePost1 = System.nanoTime();\n            LOGGER.info(\"scoreAsyncItems.allOfAsyncScoring:I0001a: Async process time in ms: \".concat( String.valueOf((double) ((endTimePost1 - startTimePost1) / 1000000)) ));\n        } catch (ExecutionException e) {\n            e.printStackTrace();\n        } catch (InterruptedException e) {\n            e.printStackTrace();\n        }\n\n        /** All items are excluded that are not active and no scores */\n        offerMatrix = resultScore.getJSONArray(\"newOfferMatrix\");\n\n        /** Select top items based on number of offers to present */\n        for (int i = 0; i < offerMatrix.length(); i++) {\n            JSONObject singleOffer = offerMatrix.getJSONObject(i);\n            String offer_id = String.valueOf(singleOffer.get(\"offer_id\"));\n\n            LOGGER.debug(\"singleOffer:D001-1: \" + singleOffer.toString());\n            LOGGER.debug(\"singleOffer:offer_id:D001-2: \" + offer_id);\n\n            /** Offer matrix needs item \"price\" for aggregator to work! */\n            double offer_price = 1.0;\n            if (singleOffer.has(\"offer_price\"))\n                offer_price = DataTypeConversions.getDouble(singleOffer, \"offer_price\");\n            else if (singleOffer.has(\"price\"))\n                offer_price = DataTypeConversions.getDouble(singleOffer, \"price\");\n            else\n                LOGGER.error(\"PostScoreRecommenderMultiSafaricom:E0011: price not in offerMatrix, value set to 1\");\n\n            double offer_cost = 1.0;\n            if (singleOffer.has(\"offer_cost\"))\n                offer_cost = singleOffer.getDouble(\"offer_cost\");\n            if (singleOffer.has(\"cost\"))\n                offer_cost = singleOffer.getDouble(\"cost\");\n\n            int explore = (int) params.get(\"explore\");\n            JSONObject finalOffersObject = new JSONObject();\n\n            offer_id = DataTypeConversions.getString(singleOffer.getString(\"offer_id\"));\n\n            /*******************************************************************************/\n\n            double p = resultScore.getDouble(offer_id);\n\n            /*******************************************************************************/\n\n            /** Multi-model needs to store the model for logging - DO NOT REMOVE THIS!*/\n            finalOffersObject.put(\"model_name\", offer_id + \".zip\");\n            finalOffersObject.put(\"model_index\", resultScore.get(offer_id + \"_model_index\"));\n\n            finalOffersObject.put(\"offer\", singleOffer.get(\"offer_id\"));\n            finalOffersObject.put(\"offer_name\", singleOffer.get(\"offer_name\"));\n            // finalOffersObject.put(\"offer_name_desc\", offer_name + \" - \" + i);\n\n            /** process final */\n            // double p = domainsProbabilityObj.getDouble(label);\n            finalOffersObject.put(\"score\", p);\n            finalOffersObject.put(\"final_score\", p);\n            finalOffersObject.put(\"modified_offer_score\", p);\n            finalOffersObject.put(\"offer_value\", offer_price); // use value from offer matrix\n            // finalOffersObject.put(\"offer_profit_probability\", offer_profit * p);\n            finalOffersObject.put(\"price\", offer_price);\n            finalOffersObject.put(\"cost\", offer_cost);\n\n            finalOffersObject.put(\"p\", p);\n            finalOffersObject.put(\"explore\", explore);\n\n            /** Prepare array before final sort */\n            finalOffers.put(offerIndex, finalOffersObject);\n            offerIndex = offerIndex + 1;\n        }\n\n        JSONArray sortJsonArray = JSONArraySort.sortArray(finalOffers, \"score\", \"double\", \"d\");\n        predictModelMojoResult.put(\"final_result\", sortJsonArray);\n\n        predictModelMojoResult = getTopScores(params, predictModelMojoResult);\n\n        /** Multi-model needs to store the model for logging! - DO NOT REMOVE THIS! */\n        if (sortJsonArray.length() > 0) {\n            if (sortJsonArray.getJSONObject(0).has(\"model_index\")) {\n                String model_name = (String) sortJsonArray.getJSONObject(0).get(\"model_name\");\n                params.put(\"model_selected\", model_name);\n            }\n        } else {\n            LOGGER.error(\"PostScoreRecommenderMulti:E999: No result \");\n        }\n\n        double endTimePost = System.nanoTime();\n        LOGGER.info(\"PostScoreRecommenderMulti:I001: time in ms: \".concat( String.valueOf((endTimePost - startTimePost) / 1000000) ));\n\n        return predictModelMojoResult;\n\n    }\n\n    private static JSONObject getExplore(JSONObject params, double epsilonIn, String name) {\n        double rand = MathRandomizer.getRandomDoubleBetweenRange(0, 1);\n        double epsilon = epsilonIn;\n        params.put(name + \"_epsilon\", epsilon);\n        if (rand <= epsilon) {\n            params.put(name, 1);\n        } else {\n            params.put(name, 0);\n        }\n        return params;\n    }\n\n\n    /**\n     * Get random results for MAB\n     * @param predictResult\n     * @param numberOffers\n     * @return\n     */\n    public static JSONArray getSelectedPredictResultRandom(JSONObject predictResult, int numberOffers) {\n        return getSelectedPredictResultExploreExploit(predictResult, numberOffers, 1);\n    }\n\n    /**\n     * Get result based on score\n     * @param predictResult\n     * @param numberOffers\n     * @return\n     */\n    public static JSONArray getSelectedPredictResult(JSONObject predictResult, int numberOffers) {\n        return getSelectedPredictResultExploreExploit(predictResult, numberOffers, 0);\n    }\n\n    private static JSONObject setValues(JSONObject work) {\n        JSONObject result = new JSONObject();\n        result.put(\"score\", work.get(\"score\"));\n        if (work.has(\"price\"))\n            result.put(\"price\", work.get(\"price\"));\n        if (work.has(\"cost\"))\n            result.put(\"cost\", work.get(\"cost\"));\n        result.put(\"final_score\", work.get(\"score\"));\n        result.put(\"offer\", work.get(\"offer\"));\n        result.put(\"offer_name\", work.get(\"offer_name\"));\n        result.put(\"modified_offer_score\", work.get(\"modified_offer_score\"));\n        result.put(\"offer_value\", work.get(\"offer_value\"));\n        return result;\n    }\n\n    /**\n     * Set values JSONObject that will be used in final\n     * @param work\n     * @param rank\n     * @return\n     */\n    private static JSONObject setValuesFinal(JSONObject work, int rank) {\n        JSONObject offer = new JSONObject();\n\n        offer.put(\"rank\", rank);\n        offer.put(\"result\", setValues(work));\n        offer.put(\"result_full\", work);\n\n        return offer;\n    }\n\n\n    /**\n     * Review this: Master version in EcosystemMaster class. {offer_treatment_code: {$regex:\"_A\"}}\n     *\n     * @param predictResult\n     * @param numberOffers\n     * @return\n     */\n    public static JSONArray getSelectedPredictResultExploreExploit(JSONObject predictResult, int numberOffers, int explore) {\n        JSONArray offers = new JSONArray();\n        int resultLength = predictResult.getJSONArray(\"final_result\").length();\n\n        for (int j = 0, k = 0; j < resultLength; j++) {\n            JSONObject work = new JSONObject();\n            if (explore == 1) {\n                int rand = MathRandomizer.getRandomIntBetweenRange(0, resultLength - 1);\n                work = predictResult.getJSONArray(\"final_result\").getJSONObject(rand);\n            } else {\n                work = predictResult.getJSONArray(\"final_result\").getJSONObject(j);\n            }\n\n            /* test if budget is enabled && spend_limit is greater than 0, if budget is disabled, then this will be 1.0 */\n            if (settings.getPredictorOfferBudget() != null) {\n                /* if budget setting and there is budget to spend */\n                if (work.has(\"spend_limit\")) {\n                    if ((work.getDouble(\"spend_limit\") > 0.0) | work.getDouble(\"spend_limit\") == -1) {\n                        offers.put(k, setValuesFinal(work, k + 1));\n                        if ((k + 1) == numberOffers) break;\n                        k = k + 1;\n                    }\n                } else {\n                    break;\n                }\n            } else {\n                /* no budget setting present */\n                offers.put(k, setValuesFinal(work, k + 1));\n                if ((k + 1) == numberOffers) break;\n                k = k + 1;\n            }\n        }\n\n        return offers;\n    }\n\n    /**\n     * @param params\n     * @param predictResult\n     * @return\n     */\n    private static JSONObject getTopScores(JSONObject params, JSONObject predictResult) {\n        int resultCount = 1;\n        if (params.has(\"resultcount\")) resultCount = params.getInt(\"resultcount\");\n        if (predictResult.getJSONArray(\"final_result\").length() <= resultCount)\n            resultCount = predictResult.getJSONArray(\"final_result\").length();\n\n        /* depending on epsilon and mab settings */\n        if (params.getInt(\"explore\") == 0) {\n            predictResult.put(\"final_result\", getSelectedPredictResult(predictResult, resultCount));\n            predictResult.put(\"explore\", 0);\n        } else {\n            predictResult.put(\"final_result\", getSelectedPredictResultRandom(predictResult, resultCount));\n            predictResult.put(\"explore\", 1);\n        }\n        return predictResult;\n    }\n\n}\n",
         "PostScoreNetwork.java": "package com.ecosystem.plugin.customer;\n\nimport com.datastax.oss.driver.api.core.CqlSession;\nimport hex.genmodel.easy.EasyPredictModelWrapper;\nimport com.ecosystem.utils.log.LogManager;\nimport com.ecosystem.utils.log.Logger;\nimport org.json.JSONArray;\nimport org.json.JSONObject;\n\n/**\n */\npublic class PostScoreNetwork extends PostScoreNetworkSuper {\n\n    private static final Logger LOGGER = LogManager.getLogger(PostScoreNetwork.class.getName());\n\n    public PostScoreNetwork() {\n    }\n\n    /**\n     * Pre-post predict logic\n     */\n    public void getPostPredict () {\n    }\n\n    /**\n     * getPostPredict\n     *\n     * @param predictModelMojoResult Result from scoring\n     * @param params                 Params carried from input\n     * @param session                Session variable for Cassandra\n     * @param models                  Preloaded H2O Models\n     * @return JSONObject result to further post-scoring logic\n     */\n    public static JSONObject getPostPredict(JSONObject predictModelMojoResult, JSONObject params, CqlSession session, EasyPredictModelWrapper[] models) {\n        double startTimePost = System.nanoTime();\n        try {\n            /* Setup JSON objects for specific prediction case */\n            JSONObject featuresObj = predictModelMojoResult.getJSONObject(\"featuresObj\");\n\n            /** Final offer list based on score */\n            JSONArray sortJsonArray = new JSONArray();\n\n            /** Execute network based on settings in corpora */\n            /**\n             * Configure a network of client pulse responders bu changing configuration based on lookup, scoring and\n             * other criteria. Ensure that the lookup settings coordinate and that default have been set or removed.\n             * Example, if there's a customer, or other settings in the __network collection, it will use those.\n             * If you want customer to go straight through, then remove that default.\n             *\n             * Additional corpora settings in project:\n             * [\n             * {name:'network',database:'mongodb',db:'master',table:'bank_full_1__network', type:'static', key:'value' },\n             * {name:'network_config',database:'mongodb',db:'master',table:'bank_full_1__network_config', type:'static', key:'name' }\n             * ]\n             * Add this line to \"Additional Corpora\" in your project:\n             * [{name:'network',database:'mongodb',db:'master',table:'bank_full_1__network', type:'static', key:'value' },{name:'network_config',database:'mongodb',db:'master',table:'bank_full_1__network_config', type:'static', key:'name' }]\n             *\n             * bank_full_1__network_config, ensure that this document contains this: \"name\": \"network_config\":\n             * {\n             *   \"switch_key\": \"marital\",\n             *   \"name\": \"network_config\"\n             * }\n             *\n             *\n             * bank_full_1__network, all options will be setup here. Ensure that \"value\": \"\" contains a valid value as per switch_key:\n             * {\n             *   \"numberoffers\": 4,\n             *   \"subcampaign\": \"recommender_dynamic_bayes\",\n             *   \"channel\": \"app\",\n             *   \"campaign\": \"recommender_dynamic_bayes\",\n             *   \"params\": \"{}\",\n             *   \"value\": \"married\",\n             *   \"userid\": \"ecosystem_network\",\n             *   \"url\": \"http://customer.ecosystem.ai:8091\",\n             *   \"customer\": \"281db655-d667-4671-a715-8402c29d7d11\"\n             * }\n             */\n            sortJsonArray = handlePreloadCorpora(params, featuresObj);\n\n            predictModelMojoResult.put(\"final_result\", sortJsonArray);\n\n        } catch (Exception e) {\n            LOGGER.error(\"PostScoreNetwork:E001: \" + e);\n        }\n\n        /** Get top scores and test for explore/exploit randomization */\n        predictModelMojoResult = getTopScores(params, predictModelMojoResult);\n\n        double endTimePost = System.nanoTime();\n        LOGGER.info(\"PostScoreNetwork:I001: execution time in ms: \".concat( String.valueOf((endTimePost - startTimePost) / 1000000) ));\n        return predictModelMojoResult;\n    }\n\n}\n",
     }
-    version_list = [i["version"] for i in project_details["deployment_step"] if i["plugins"]["post_score_class_text"] == post_score]
+    if "deployment_step" in project_details:
+        version_list = [i["version"] for i in project_details["deployment_step"] if i["plugins"]["post_score_class_text"] == post_score]
+    else:
+        version_list = []
     if version_list:
         max_version = max(version_list)
         post_score_logic = [i["plugins"]["post_score_class_code"] for i in project_details["deployment_step"] if
                         (i["plugins"]["post_score_class_text"] == post_score and i["version"] == max_version)][0]
+        print(f"WARNING: Using post score class from version {max_version}")
     elif post_score in post_score_code_options:
         post_score_logic = post_score_code_options[post_score]
     else:
         print(
             "WARNING: post_score_class not found in default options or existing deployments in project. Empty class "
             "saved to the deployment. To edit the class use the ecosystem.Ai plugin for IntelliJ or the ecosystem.Ai "
             "workbench")
         post_score_logic = ""
     return post_score_logic
 
+def define_deployment_virtual_variable(name,original_variable,default,variable_type,variables="",buckets=""):
+    """
+    Define a virtual variable to be used in a parameter access structure in a deployment step. Virtual variables definitions should be stored in a list that is added to the parameter access structure.
+
+    :param name: The name of the virtual variable
+    :param original_variable: The name of the original variable that the virtual variable is based on
+    :param default: The default value of the virtual variable
+    :param variable_type: The type of the virtual variable. Allowed values are discretize and concatenate
+    :param variables: A list of variables to be concatenated. Required if variable_type is concatenate
+    :param buckets: A list of buckets to be used for discretization. Should be a list of dictionaries or the form [{"from":0,"to":15,"label":"bucket_1"}] Required if variable_type is discretize
+    """
+    if not isinstance(name,str):
+        raise ValueError("name must be a string")
+    if not isinstance(original_variable,str):
+        raise ValueError("original_variable must be a string")
+    if not isinstance(default,str):
+        raise ValueError("default must be a string")
+    if variable_type not in ["discretize","concatenate"]:
+        raise ValueError("variable_type must be discretize or concatenate")
+    if variable_type == "concatenate":
+        if not isinstance(variables,list):
+            raise ValueError("variables must be a list")
+        if not all(isinstance(i,str) for i in variables):
+            raise ValueError("variables must be a list of strings")
+    if variable_type == "discretize":
+        if not isinstance(buckets,list):
+            raise ValueError("buckets must be a list of dictionaries")
+        if not all(isinstance(i,dict) for i in buckets):
+            raise ValueError("buckets must be a list of dictionaries")
+        if not all(i.keys() == ["from","to","label"] for i in buckets):
+            raise ValueError("buckets must be a list of dictionaries with keys from, to and label")
+        if not all(isinstance(i["from"],(int,float)) for i in buckets):
+            raise ValueError("from in buckets must be a number")
+        if not all(isinstance(i["to"],(int,float)) for i in buckets):
+            raise ValueError("to in buckets must be a number")
+        if not all(isinstance(i["label"],str) for i in buckets):
+            raise ValueError("label in buckets must be a string")
+
+    if variables == "":
+        variables = []
+    if buckets == "":
+        buckets = []
+
+    try:
+        virtual_variable = {
+            "name": name,
+            "default": default,
+            "type": variable_type,
+            "original_variable": original_variable,
+            "fields": variables,
+            "buckets": buckets
+        }
+    except Exception as e:
+        raise ValueError(f"Error creating virtual variable: {e}")
+
+    return virtual_variable
+
+
+def define_deployment_parameter_access(lookup_key,lookup_type,database,table_collection,lookup_fields,datasource,lookup_default="",defaults="",virtual_variables=""):
+    """
+    Define the parameter access structure for a deployment step
+
+    :param lookup_key: The key field to be used for lookup in the parameter access structure
+    :param lookup_type: The type of lookup key in the lookup data set. Allowed values are string and int
+    :param database: The database to be used for lookup
+    :param table_collection: The table or collection to be used for lookup
+    :param lookup_fields: A list of fields to be returned from the lookup
+    :param datasource: The type of datasource to be used for lookup. Allowed values are mongodb, cassandra and presto
+    :param lookup_default: The default value for the lookup key
+    :param defaults: A list of default values for fields in the lookup data set
+    :param virtual_variables: A list of virtual variables to be used in the parameter access structure. Virtual variables can be defined using the define_deployment_virtual_variable function.
+    """
+    if not isinstance(lookup_key, str):
+        raise ValueError("lookup_key must be a string")
+    if lookup_type not in ["string","int","float"]:
+        raise ValueError("lookup_type must be string or int")
+    if not isinstance(database, str):
+        raise ValueError("database must be a string")
+    if not isinstance(table_collection, str):
+        raise ValueError("table_collection must be a string")
+    if not isinstance(lookup_fields,list):
+        raise ValueError("lookup_fields must be a list")
+    if not all(isinstance(i, str) for i in lookup_fields):
+        raise ValueError("lookup_fields must be a list of strings")
+    if datasource not in ["mongodb", "cassandra", "presto"]:
+        raise ValueError("datasource must be mongodb, cassandra or presto")
+    if defaults != "":
+        if not isinstance(defaults, list):
+            raise ValueError("defaults must be a list")
+        if not all(isinstance(i, str) for i in defaults):
+            raise ValueError("defaults must be a list of strings")
+    if virtual_variables != "":
+        if not isinstance(virtual_variables, list):
+            raise ValueError("virtual_variables must be a list")
+        if not all(isinstance(i, dict) for i in virtual_variables):
+            raise ValueError("virtual_variables must be a list of dictionaries")
+
+    try:
+        if lookup_default == "":
+            if lookup_type == "string":
+                lookup_value = "123"
+            else:
+                lookup_value = 123
+        else:
+            if lookup_type == "string":
+                lookup_value = str(lookup_default)
+            else:
+                lookup_value = int(lookup_default)
+        lookup = {"key": lookup_key, "value": lookup_value}
+
+        create_virtual_variables = False
+        if virtual_variables != "":
+            create_virtual_variables = True
+        else:
+            virtual_variables = []
+
+        parameter_access = {
+            "lookup": lookup,
+            "create_virtual_variables": create_virtual_variables,
+            "database": database,
+            "table_collection": table_collection,
+            "lookup_fields": lookup_fields,
+            "datasource": datasource,
+            "lookup_defaults": defaults,
+            "virtual_variables": virtual_variables
+        }
+    except Exception as e:
+        raise ValueError(f"Error creating parameter access structure: {e}")
+
+    return parameter_access
+
+
+def define_deployment_model_configuration(models_to_load,models_note="",models_outline="Recommender"):
+    """
+    Define the model configuration structure for a deployment step
+
+    :param models_to_load: A list of model names to be loaded
+    :param models_note: A note to store with the model
+    :param models_outline: The structure of the models
+    """
+    if not isinstance(models_to_load, list):
+        raise ValueError("models_to_load must be a list")
+    if not all(isinstance(i, str) for i in models_to_load):
+        raise ValueError("models_to_load must be a list of strings")
+    if not isinstance(models_note, str):
+        raise ValueError("models_note must be a string")
+    if not isinstance(models_outline, str):
+        raise ValueError("models_outline must be a string")
+
+    try:
+        models_load= ",".join(models_to_load)
+        model_configuration = {
+            "models_load": models_load,
+            "models_note": models_note,
+            "models_outline": models_outline
+        }
+    except Exception as e:
+        raise ValueError(f"Error creating model configuration structure: {e}")
+
+    return model_configuration
+
+
+def define_deployment_model_selector(database, table_collection, datasource, lookup_key, lookup_type, selector_column, selector, model_configuration, lookup_default=""):
+    """
+    Define the model selector structure for a deployment step
+
+    :param database: The database to be used for lookup
+    :param table_collection: The table or collection to be used for lookup
+    :param datasource: The type of datasource to be used for lookup. Allowed values are mongodb, cassandra and presto
+    :param lookup_key: The key field to be used for lookup in the model selector structure
+    :param lookup_type: The type of lookup key in the model selector data set. Allowed values are string and int
+    :param selector_column: The column in the lookup database to be used for selection
+    :param selector: A dictionary specifying the model to use for each value of the selector column. The keys are the values of the selector column and the values a list of the model names.
+    :param model_configuration: The model configuration structure to be used for the deployment step
+    :param lookup_default: The default value for the lookup key
+    """
+    if not isinstance(database, str):
+        raise ValueError("database must be a string")
+    if not isinstance(table_collection, str):
+        raise ValueError("table_collection must be a string")
+    if datasource not in ["mongodb", "cassandra", "presto"]:
+        raise ValueError("datasource must be mongodb, cassandra or presto")
+    if not (isinstance(lookup_key, str) or isinstance(lookup_key, int)):
+        raise ValueError("lookup_key must be a string or an integer")
+    if lookup_type not in ["string", "int"]:
+        raise ValueError("lookup_type must be string or int")
+    if not isinstance(selector_column, str):
+        raise ValueError("selector_column must be a string")
+    if not isinstance(selector, dict):
+        raise ValueError("selector must be a dictionary")
+    if not isinstance(model_configuration, dict):
+        raise ValueError("model_configuration must be a dictionary")
+    if not "models_load" in model_configuration:
+        raise ValueError("model_configuration must contain a models_load key")
+
+    try:
+        if lookup_default == "":
+            if lookup_type == "string":
+                lookup_value = "123"
+            else:
+                lookup_value = 123
+        else:
+            if lookup_type == "string":
+                lookup_value = str(lookup_default)
+            else:
+                lookup_value = int(lookup_default)
+        lookup = {"key": lookup_key, "value": lookup_value}
+
+        selector_int = {}
+        models_list = model_configuration["models_load"].split(",")
+        for selector_iter in selector:
+            list_iter = selector[selector_iter]
+            for model_iter in list_iter:
+                if model_iter not in models_list:
+                    raise ValueError(f"Model {model_iter} in selector not in model configuration")
+                else:
+                    if selector_iter not in selector_int:
+                        selector_int[selector_iter] = [models_list.index(model_iter)]
+                    else:
+                        selector_int[selector_iter].append(models_list.index(model_iter))
+
+        model_selector = {
+            "database": database,
+            "table_collection": table_collection,
+            "datasource": datasource,
+            "lookup": lookup,
+            "selector_column": selector_column,
+            "selector": selector
+        }
+    except Exception as e:
+        raise ValueError(f"Error creating model selector structure: {e}")
+
+    return model_selector
+
+
+def define_deployment_setup_offer_matrix(database, collection, datasource, offer_lookup_id):
+    """
+    Define the setup offer matrix structure for a deployment step
+
+    :param database: The database containing the offer matrix
+    :param collection: The collection containing the offer matrix
+    :param datasource: The type of datasource containing the offer matrix. Allowed values are mongodb, cassandra and presto
+    :param offer_lookup_id: The name of the column containing the unique identifier for the offers. Allowed values are offer, offer_id and offer_name
+    """
+    if not isinstance(database, str):
+        raise ValueError("database must be a string")
+    if not isinstance(collection, str):
+        raise ValueError("collection must be a string")
+    if datasource not in ["mongodb", "cassandra", "presto"]:
+        raise ValueError("datasource must be mongodb, cassandra or presto")
+    if offer_lookup_id not in ["offer", "offer_id", "offer_name"]:
+        raise ValueError("offer_lookup_id must be offer, offer_id or offer_name")
+
+    try:
+        setup_offer_matrix = {
+            "database": database,
+            "collection": collection,
+            "datasource": datasource,
+            "offer_lookup_id": offer_lookup_id
+        }
+    except Exception as e:
+        raise ValueError(f"Error creating setup offer matrix structure: {e}")
+
+    return setup_offer_matrix
+
+
+def define_deployment_multi_armed_bandit(epsilon, duration=0, dynamic_interaction_uuid=""):
+    """
+    Define the multi armed bandit structure for a deployment step
+
+    :param epsilon: The epsilon value for the deployment
+    :param duration: The cache duration for the deployment
+    :param dynamic_interaction_uuid: The uuid of the dynamic interaction configuration to be used for the deployment
+    """
+    if not isinstance(epsilon, (int, float)):
+        raise ValueError("epsilon must be a number")
+    if not isinstance(duration, int):
+        raise ValueError("duration must be an integer")
+    if not isinstance(dynamic_interaction_uuid, str):
+        raise ValueError("pulse_responder_uuid must be a string")
+
+    try:
+        multi_armed_bandit = {
+            "epsilon": epsilon,
+            "duration": duration,
+            "pulse_responder_uuid": dynamic_interaction_uuid
+        }
+    except Exception as e:
+        raise ValueError(f"Error creating multi armed bandit structure: {e}")
+
+    return multi_armed_bandit
+
+
+def define_deployment_whitelist(database, table_collection, datasource):
+    """
+    Define the whitelist structure for a deployment step. The whitelist dataset must contain a customer_key column and a whitelist column which is a comma separated list of eligible offer names
+
+    :param database: The database containing the whitelist
+    :param table_collection: The table or collection containing the whitelist
+    :param datasource: The type of datasource containing the whitelist. Allowed values are mongodb, cassandra and presto
+    """
+    if not isinstance(database, str):
+        raise ValueError("database must be a string")
+    if not isinstance(table_collection, str):
+        raise ValueError("table_collection must be a string")
+    if datasource not in ["mongodb", "cassandra", "presto"]:
+        raise ValueError("datasource must be mongodb, cassandra or presto")
+
+    try:
+        whitelist = {
+            "database": database,
+            "collection": table_collection,
+            "datasource": datasource
+        }
+    except Exception as e:
+        raise ValueError(f"Error creating whitelist structure: {e}")
+
+    return whitelist
+
+
+def get_column_list(auth, database, table_collection, datasource):
+    """
+    Get a list of columns in a table or collection in a database.
+
+    :param auth: Token for accessing the ecosystem-server. Created using the jwt_access package.
+    :param database: The name of the database to get the columns from
+    :param table_collection: The name of the table or collection to get the columns from
+    :param datasource: The type of datasource to get the columns from. Allowed values are mongodb and cassandra
+    """
+    if not isinstance(database, str):
+        raise ValueError("database must be a string")
+    if not isinstance(table_collection, str):
+        raise ValueError("table_collection must be a string")
+    if datasource not in ["mongodb", "cassandra"]:
+        raise ValueError("datasource must be mongodb or cassandra")
+
+    columns = []
+    try:
+        if datasource == "mongodb":
+            data_check = dme.get_data(auth, database, table_collection, {}, 1, {}, 0)
+            if data_check == []:
+                print("WARNING: It looks like collection {} in database {} is empty or does not exist".format(table_collection,database))
+            else:
+                columns = list(data_check[0].keys())
+        elif datasource == "cassandra":
+            data_check = dme.get_cassandra_sql(auth, "SELECT * FROM {}.{} LIMIT 1".format(database, table_collection))
+            if data_check["data"] == []:
+                print("WARNING: It looks like {}.{} is empty or does not exist".format(database, table_collection))
+            else:
+                columns = list(data_check["data"][0].keys())
+    except Exception as e:
+        raise ValueError(f"Error getting column list: {e}")
+
+    return columns
+
 
 def create_deployment(
         auth,
         project_id,
         deployment_id,
         description,
         plugin_pre_score_class,
         plugin_post_score_class,
         version,
-        project_status,
         mongo_connect,
         mongo_server_port,
         mongo_ecosystem_password,
         mongo_ecosystem_user,
         budget_tracker="default",
+        project_status="experiment",
         complexity="Low",
         performance_expectation="High",
         model_configuration="default",
         setup_offer_matrix="default",
         multi_armed_bandit="default",
         whitelist="default",
         model_selector="default",
@@ -1184,32 +1546,35 @@
     if not distribution_tests:
         print("Error in distribution_tests")
         return "Testing Failed"
 
     return "Testing Passed"
 
 
-def create_network_configuration(auth, database, collection, name, type, switch_key="", selector_splits=[],selector_groups=[]):
+def create_network_configuration(auth, database, collection, network_collection, name, type, switch_key="", selector_splits=[],selector_groups=[]):
     """
     Create a new network configuration and store it in mongo. Existing configurations stored in the same location will be overwritten.
 
     :param auth: Token for accessing the ecosystem-server. Created using jwt_access.
     :param database: The database to store the configuration in.
     :param collection: The collection to store the configuration in.
+    :param network_collection: The collection to store the network in.
     :param name: The name of the network configuration.
     :param type: The type of the network configuration. Allowed values are lookup, lookup_passthrough, experiment_selector and no logging router.
     :param switch_key: The key to switch on for the lookup, lookup_passthrough and no_logging_router types.
     :param selector_splits: The distribution splits for the experiment_selector type. Should be a list of numbers that define the allocation of customers to an experiment group. For example selector_splits=[0.2,0.8] would have a 20% probability of assigning customers to group 1 a 60% chance of assinging customers to group 2 and and 20% chance of assigning customers to group 3.
     :param selector_groups: The groups to allocate customers to for the experiment_selector type. Should be a list of the runtime campaign names for the network nodes.
     """
 
     if not isinstance(database, str):
         raise TypeError("database should be a string")
     if not isinstance(collection, str):
         raise TypeError("collection should be a string")
+    if not isinstance(network_collection, str):
+        raise TypeError("network_collection should be a string")
     if not isinstance(name, str):
         raise TypeError("name should be a string")
     if not isinstance(type, str):
         raise TypeError("type should be a string")
     if not isinstance(switch_key, str):
         raise TypeError("switch_key should be a string")
     if not isinstance(selector_splits, list):
@@ -1256,15 +1621,25 @@
     try:
         dme.drop_document_collection(auth, database, collection)
         dme.add_documents(auth, {"database": database, "collection": collection, "document": network_configuration, "update": "name"})
     except Exception as e:
         print("Error saving network configuration: {0}".format(e))
         return "Network configuration save failed"
 
-    return "Network configuration created"
+    try:
+        network_corpora = [{"name": "network", "database": "mongodb", "db": database, "table": network_collection,
+          "type": "static", "key": "value"},
+         {"name": "network_config", "database": "mongodb", "db": database, "table": collection,
+          "type": "static"}]
+    except Exception as e:
+        print("Error creating network corpora: {0}".format(e))
+        return "Network corpora creation failed"
+
+    print("MESSAGE: Network configuration created")
+    return network_corpora
 
 def add_network_node(auth, database, collection, node_value, node_api_params):
     """
     Add a new network node to a network runtime configuration. Will replace existing network nodes with the same value.
 
     :param auth: Token for accessing the ecosystem-server. Created using jwt_access.
     :param database: The database to store the configuration in.
@@ -1293,14 +1668,15 @@
         dme.add_documents(auth, {"database": database, "collection": collection, "document": network_node, "update": "value"})
     except Exception as e:
         print("Error saving network node: {0}".format(e))
         return "Network node save failed"
 
     return "Network node added"
 
+
 def remove_network_node(auth, database, collection, node_value):
     """
     Remove a network node from a network runtime configuration.
 
     :param auth: Token for accessing the ecosystem-server. Created using jwt_access.
     :param database: The database to store the configuration in.
     :param collection: The collection to store the configuration in.
@@ -1311,14 +1687,13 @@
         raise TypeError("database should be a string")
     if not isinstance(collection, str):
         raise TypeError("collection should be a string")
     if not isinstance(node_value, str):
         raise TypeError("node_value should be a string")
 
     try:
-        {'database': 'mydb', 'collection': 'mycollection', 'key': 'KEY_NAME', 'value': 'KEY_VALUE_TO_DELETE'}
         dme.delete_documents(auth, {"database": database, "collection": collection, "key":"value", "value": node_value})
     except Exception as e:
         print("Error removing network node: {0}".format(e))
         return "Network node removal failed"
 
     return "Network node removed"
```

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/ecosystem_generation_engine.py` & `ecosystem-notebooks-0.1.9/prediction/apis/ecosystem_generation_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/ecosystem_home.py` & `ecosystem-notebooks-0.1.9/prediction/apis/ecosystem_home.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/ecosystem_user_profiles.py` & `ecosystem-notebooks-0.1.9/prediction/apis/ecosystem_user_profiles.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/functions.py` & `ecosystem-notebooks-0.1.9/prediction/apis/functions.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/online_learning_management.py` & `ecosystem-notebooks-0.1.9/prediction/apis/online_learning_management.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/prediction_engine.py` & `ecosystem-notebooks-0.1.9/prediction/apis/prediction_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/quickflat.py` & `ecosystem-notebooks-0.1.9/prediction/apis/quickflat.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/transaction_categorization.py` & `ecosystem-notebooks-0.1.9/prediction/apis/transaction_categorization.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/user_controller.py` & `ecosystem-notebooks-0.1.9/prediction/apis/user_controller.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/utilities.py` & `ecosystem-notebooks-0.1.9/prediction/apis/utilities.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/worker_aws.py` & `ecosystem-notebooks-0.1.9/prediction/apis/worker_aws.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/worker_file_service.py` & `ecosystem-notebooks-0.1.9/prediction/apis/worker_file_service.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/worker_google.py` & `ecosystem-notebooks-0.1.9/prediction/apis/worker_google.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/worker_h2o.py` & `ecosystem-notebooks-0.1.9/prediction/apis/worker_h2o.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/apis/worker_uber.py` & `ecosystem-notebooks-0.1.9/prediction/apis/worker_uber.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/algorithm_client_pulse.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/algorithm_client_pulse.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/auth_controller.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/auth_controller.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/data_ingestion_engine.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/data_ingestion_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/data_management_engine.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/data_management_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/data_munging_engine.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/data_munging_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/ecosystem_generation_engine.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/ecosystem_generation_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/ecosystem_home.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/ecosystem_home.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/ecosystem_user_profiles.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/ecosystem_user_profiles.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/prediction_engine.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/prediction_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/transaction_categorization.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/transaction_categorization.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/utilities.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/utilities.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/worker_aws.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/worker_aws.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/worker_file_service.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/worker_file_service.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/worker_h2o.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/worker_h2o.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/endpoints/worker_uber.py` & `ecosystem-notebooks-0.1.9/prediction/endpoints/worker_uber.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/jwt_access.py` & `ecosystem-notebooks-0.1.9/prediction/jwt_access.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/nlp_utils.py` & `ecosystem-notebooks-0.1.9/prediction/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/notebook_functions.py` & `ecosystem-notebooks-0.1.9/prediction/notebook_functions.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/prediction_utils.py` & `ecosystem-notebooks-0.1.9/prediction/prediction_utils.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/request_utils.py` & `ecosystem-notebooks-0.1.9/prediction/request_utils.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/prediction/utils/endpoint_diff.py` & `ecosystem-notebooks-0.1.9/prediction/utils/endpoint_diff.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/runtime/access.py` & `ecosystem-notebooks-0.1.9/runtime/access.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/runtime/apis/data_management_engine.py` & `ecosystem-notebooks-0.1.9/runtime/apis/data_management_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/runtime/apis/predictor_engine.py` & `ecosystem-notebooks-0.1.9/runtime/apis/predictor_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/runtime/apis/runtime_engine.py` & `ecosystem-notebooks-0.1.9/runtime/apis/runtime_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/runtime/apis/worker_utilities.py` & `ecosystem-notebooks-0.1.9/runtime/apis/worker_utilities.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/runtime/endpoints/data_management_engine.py` & `ecosystem-notebooks-0.1.9/runtime/endpoints/data_management_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/runtime/endpoints/predictor_engine.py` & `ecosystem-notebooks-0.1.9/runtime/endpoints/predictor_engine.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/runtime/endpoints/worker_utilities.py` & `ecosystem-notebooks-0.1.9/runtime/endpoints/worker_utilities.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/runtime/request_utils.py` & `ecosystem-notebooks-0.1.9/runtime/request_utils.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/runtime/utils/endpoint_diff.py` & `ecosystem-notebooks-0.1.9/runtime/utils/endpoint_diff.py`

 * *Files identical despite different names*

### Comparing `ecosystem-notebooks-0.1.8/setup.py` & `ecosystem-notebooks-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from pathlib import Path
 
 setup(
     name='ecosystem-notebooks',
-    version='0.1.8',
+    version='0.1.9',
     description='Ecosystem Notebooks is a wrapper for the Ecosystem API servers.',
     long_description=Path("README.rst").read_text(encoding="utf-8"),
     url='https://github.com/ecosystemai/ecosystem-notebooks',
     author='EcosystemAi',
     author_email='jay@ecosystem.ai',
     license='MIT',
     packages=['runtime', 'runtime.apis', 'runtime.endpoints', 'runtime.utils', 'prediction', 'prediction.apis', 'prediction.endpoints', 'prediction.utils'],
```

