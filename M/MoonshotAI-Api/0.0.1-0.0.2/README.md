# Comparing `tmp/MoonshotAI_Api-0.0.1.tar.gz` & `tmp/MoonshotAI_Api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MoonshotAI_Api-0.0.1.tar", last modified: Wed Apr 24 12:32:27 2024, max compression
+gzip compressed data, was "MoonshotAI_Api-0.0.2.tar", last modified: Thu May  2 13:13:13 2024, max compression
```

## Comparing `MoonshotAI_Api-0.0.1.tar` & `MoonshotAI_Api-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tomerefroni   (501) staff       (20)        0 2024-04-24 12:32:27.384457 MoonshotAI_Api-0.0.1/
-drwxr-xr-x   0 tomerefroni   (501) staff       (20)        0 2024-04-24 12:32:27.381184 MoonshotAI_Api-0.0.1/MoonshotAI_Api/
--rw-r--r--   0 tomerefroni   (501) staff       (20)     1066 2024-04-22 09:05:33.000000 MoonshotAI_Api-0.0.1/MoonshotAI_Api/LICENSE
--rw-r--r--   0 tomerefroni   (501) staff       (20)       13 2024-04-08 13:04:59.000000 MoonshotAI_Api-0.0.1/MoonshotAI_Api/README.md
--rw-r--r--   0 tomerefroni   (501) staff       (20)        0 2022-07-04 11:50:12.000000 MoonshotAI_Api-0.0.1/MoonshotAI_Api/__init__.py
--rw-r--r--   0 tomerefroni   (501) staff       (20)     5352 2024-04-24 12:26:17.000000 MoonshotAI_Api-0.0.1/MoonshotAI_Api/ltv_client.py
-drwxr-xr-x   0 tomerefroni   (501) staff       (20)        0 2024-04-24 12:32:27.383823 MoonshotAI_Api-0.0.1/MoonshotAI_Api/utils/
--rw-r--r--   0 tomerefroni   (501) staff       (20)      751 2024-04-21 08:46:30.000000 MoonshotAI_Api-0.0.1/MoonshotAI_Api/utils/consts.py
--rw-r--r--   0 tomerefroni   (501) staff       (20)       88 2024-04-21 08:43:57.000000 MoonshotAI_Api-0.0.1/MoonshotAI_Api/utils/output_enum.py
--rw-r--r--   0 tomerefroni   (501) staff       (20)     1032 2024-04-21 09:33:40.000000 MoonshotAI_Api-0.0.1/MoonshotAI_Api/utils/utils.py
-drwxr-xr-x   0 tomerefroni   (501) staff       (20)        0 2024-04-24 12:32:27.382803 MoonshotAI_Api-0.0.1/MoonshotAI_Api.egg-info/
--rw-r--r--   0 tomerefroni   (501) staff       (20)      190 2024-04-24 12:32:27.000000 MoonshotAI_Api-0.0.1/MoonshotAI_Api.egg-info/PKG-INFO
--rw-r--r--   0 tomerefroni   (501) staff       (20)      445 2024-04-24 12:32:27.000000 MoonshotAI_Api-0.0.1/MoonshotAI_Api.egg-info/SOURCES.txt
--rw-r--r--   0 tomerefroni   (501) staff       (20)        1 2024-04-24 12:32:27.000000 MoonshotAI_Api-0.0.1/MoonshotAI_Api.egg-info/dependency_links.txt
--rw-r--r--   0 tomerefroni   (501) staff       (20)        1 2024-04-24 12:32:27.000000 MoonshotAI_Api-0.0.1/MoonshotAI_Api.egg-info/not-zip-safe
--rw-r--r--   0 tomerefroni   (501) staff       (20)       17 2024-04-24 12:32:27.000000 MoonshotAI_Api-0.0.1/MoonshotAI_Api.egg-info/requires.txt
--rw-r--r--   0 tomerefroni   (501) staff       (20)       15 2024-04-24 12:32:27.000000 MoonshotAI_Api-0.0.1/MoonshotAI_Api.egg-info/top_level.txt
--rw-r--r--   0 tomerefroni   (501) staff       (20)      190 2024-04-24 12:32:27.384193 MoonshotAI_Api-0.0.1/PKG-INFO
--rw-r--r--   0 tomerefroni   (501) staff       (20)       13 2024-04-08 13:04:59.000000 MoonshotAI_Api-0.0.1/README.md
--rw-r--r--   0 tomerefroni   (501) staff       (20)       38 2024-04-24 12:32:27.384651 MoonshotAI_Api-0.0.1/setup.cfg
--rw-r--r--   0 tomerefroni   (501) staff       (20)      385 2024-04-24 09:55:28.000000 MoonshotAI_Api-0.0.1/setup.py
+drwxr-xr-x   0 tomerefroni   (501) staff       (20)        0 2024-05-02 13:13:13.494614 MoonshotAI_Api-0.0.2/
+drwxr-xr-x   0 tomerefroni   (501) staff       (20)        0 2024-05-02 13:13:13.488815 MoonshotAI_Api-0.0.2/MoonshotAI_Api/
+-rw-r--r--   0 tomerefroni   (501) staff       (20)     1066 2024-04-22 09:05:33.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api/LICENSE
+-rw-r--r--   0 tomerefroni   (501) staff       (20)       13 2024-04-08 13:04:59.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api/README.md
+-rw-r--r--   0 tomerefroni   (501) staff       (20)        0 2022-07-04 11:50:12.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api/__init__.py
+-rw-r--r--   0 tomerefroni   (501) staff       (20)     5352 2024-04-24 12:26:17.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api/ltv_client.py
+drwxr-xr-x   0 tomerefroni   (501) staff       (20)        0 2024-05-02 13:13:13.493091 MoonshotAI_Api-0.0.2/MoonshotAI_Api/utils/
+-rw-r--r--   0 tomerefroni   (501) staff       (20)      652 2024-05-02 10:52:05.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api/utils/consts.py
+-rw-r--r--   0 tomerefroni   (501) staff       (20)       88 2024-04-21 08:43:57.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api/utils/output_enum.py
+-rw-r--r--   0 tomerefroni   (501) staff       (20)     1032 2024-04-21 09:33:40.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api/utils/utils.py
+drwxr-xr-x   0 tomerefroni   (501) staff       (20)        0 2024-05-02 13:13:13.491562 MoonshotAI_Api-0.0.2/MoonshotAI_Api.egg-info/
+-rw-r--r--   0 tomerefroni   (501) staff       (20)      190 2024-05-02 13:13:13.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api.egg-info/PKG-INFO
+-rw-r--r--   0 tomerefroni   (501) staff       (20)      445 2024-05-02 13:13:13.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api.egg-info/SOURCES.txt
+-rw-r--r--   0 tomerefroni   (501) staff       (20)        1 2024-05-02 13:13:13.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api.egg-info/dependency_links.txt
+-rw-r--r--   0 tomerefroni   (501) staff       (20)        1 2024-04-24 12:32:27.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api.egg-info/not-zip-safe
+-rw-r--r--   0 tomerefroni   (501) staff       (20)       17 2024-05-02 13:13:13.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api.egg-info/requires.txt
+-rw-r--r--   0 tomerefroni   (501) staff       (20)       15 2024-05-02 13:13:13.000000 MoonshotAI_Api-0.0.2/MoonshotAI_Api.egg-info/top_level.txt
+-rw-r--r--   0 tomerefroni   (501) staff       (20)      190 2024-05-02 13:13:13.494195 MoonshotAI_Api-0.0.2/PKG-INFO
+-rw-r--r--   0 tomerefroni   (501) staff       (20)       13 2024-04-08 13:04:59.000000 MoonshotAI_Api-0.0.2/README.md
+-rw-r--r--   0 tomerefroni   (501) staff       (20)       38 2024-05-02 13:13:13.494733 MoonshotAI_Api-0.0.2/setup.cfg
+-rw-r--r--   0 tomerefroni   (501) staff       (20)      385 2024-05-02 13:11:16.000000 MoonshotAI_Api-0.0.2/setup.py
```

### Comparing `MoonshotAI_Api-0.0.1/MoonshotAI_Api/LICENSE` & `MoonshotAI_Api-0.0.2/MoonshotAI_Api/LICENSE`

 * *Files identical despite different names*

### Comparing `MoonshotAI_Api-0.0.1/MoonshotAI_Api/ltv_client.py` & `MoonshotAI_Api-0.0.2/MoonshotAI_Api/ltv_client.py`

 * *Files identical despite different names*

### Comparing `MoonshotAI_Api-0.0.1/MoonshotAI_Api/utils/consts.py` & `MoonshotAI_Api-0.0.2/MoonshotAI_Api/utils/consts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-QUERY_DATA_URL = 'https://sulbfowah3.execute-api.eu-west-2.amazonaws.com/prod/api/{account_name}/querydata/?job=inference&kpi={' \
+QUERY_DATA_URL = 'https://api.moonshot-ai.io/api/{account_name}/querydata/?job=inference&kpi={' \
                  'kpi}&predtime={pred_time}&startdate={start_date}&enddate={end_date}&datetype={date_type}'
 
-GET_DATA_URL = 'https://sulbfowah3.execute-api.eu-west-2.amazonaws.com/prod/api/{account_name}/getdata/?queryid={query_id}'
-GET_STATUS_URL = 'https://sulbfowah3.execute-api.eu-west-2.amazonaws.com/prod/api/{account_name}/getdata/?queryid={query_id}&job={job}'
+GET_DATA_URL = 'https://api.moonshot-ai.io/api/{account_name}/getdata/?queryid={query_id}'
+GET_STATUS_URL = 'https://api.moonshot-ai.io/api/{account_name}/getdata/?queryid={query_id}&job={job}'
 
 DEFAULT = 'default'
 QUERY_ID = 'query_id'
 URL = 'URL'
 SUCCESS = 'SUCCEEDED'
 FAILED = 'FAILED'
 RUNNING = 'RUNNING'
```

### Comparing `MoonshotAI_Api-0.0.1/MoonshotAI_Api/utils/utils.py` & `MoonshotAI_Api-0.0.2/MoonshotAI_Api/utils/utils.py`

 * *Files identical despite different names*

