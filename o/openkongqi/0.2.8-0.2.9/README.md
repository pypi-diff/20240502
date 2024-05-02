# Comparing `tmp/openkongqi-0.2.8.tar.gz` & `tmp/openkongqi-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openkongqi-0.2.8.tar", last modified: Thu Jan  6 07:16:36 2022, max compression
+gzip compressed data, was "openkongqi-0.2.9.tar", last modified: Sun Dec  3 05:08:27 2023, max compression
```

## Comparing `openkongqi-0.2.8.tar` & `openkongqi-0.2.9.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 hr        (1000) hr        (1000)        0 2022-01-06 07:16:36.882022 openkongqi-0.2.8/
--rw-r--r--   0 hr        (1000) hr        (1000)    11369 2016-04-28 02:04:17.000000 openkongqi-0.2.8/LICENSE
--rw-r--r--   0 hr        (1000) hr        (1000)       36 2016-04-28 02:04:17.000000 openkongqi-0.2.8/MANIFEST.in
--rw-r--r--   0 hr        (1000) hr        (1000)     4481 2022-01-06 07:16:36.882022 openkongqi-0.2.8/PKG-INFO
--rw-r--r--   0 hr        (1000) hr        (1000)     3631 2019-12-23 09:03:20.000000 openkongqi-0.2.8/README.rst
-drwxr-xr-x   0 hr        (1000) hr        (1000)        0 2022-01-06 07:16:36.882022 openkongqi-0.2.8/openkongqi/
--rw-r--r--   0 hr        (1000) hr        (1000)      120 2022-01-06 07:14:46.000000 openkongqi-0.2.8/openkongqi/__init__.py
--rw-r--r--   0 hr        (1000) hr        (1000)      435 2018-09-21 08:43:53.000000 openkongqi-0.2.8/openkongqi/apikeys.py
--rw-r--r--   0 hr        (1000) hr        (1000)     2363 2022-01-04 07:22:45.000000 openkongqi-0.2.8/openkongqi/bin.py
-drwxr-xr-x   0 hr        (1000) hr        (1000)        0 2022-01-06 07:16:36.882022 openkongqi-0.2.8/openkongqi/cache/
--rw-r--r--   0 hr        (1000) hr        (1000)       24 2017-06-28 08:56:59.000000 openkongqi-0.2.8/openkongqi/cache/__init__.py
--rw-r--r--   0 hr        (1000) hr        (1000)      689 2017-06-28 08:56:59.000000 openkongqi-0.2.8/openkongqi/cache/base.py
--rw-r--r--   0 hr        (1000) hr        (1000)      612 2019-12-20 00:18:35.000000 openkongqi-0.2.8/openkongqi/cache/redisdb.py
--rw-r--r--   0 hr        (1000) hr        (1000)     3061 2022-01-06 07:14:46.000000 openkongqi-0.2.8/openkongqi/conf.py
-drwxr-xr-x   0 hr        (1000) hr        (1000)        0 2022-01-06 07:16:36.882022 openkongqi-0.2.8/openkongqi/data/
-drwxr-xr-x   0 hr        (1000) hr        (1000)        0 2022-01-06 07:16:36.882022 openkongqi-0.2.8/openkongqi/data/sources/
--rw-r--r--   0 hr        (1000) hr        (1000)      181 2016-09-06 10:26:25.000000 openkongqi-0.2.8/openkongqi/data/sources/pm25.in.json
-drwxr-xr-x   0 hr        (1000) hr        (1000)        0 2022-01-06 07:16:36.878022 openkongqi-0.2.8/openkongqi/data/stations/
-drwxr-xr-x   0 hr        (1000) hr        (1000)        0 2022-01-06 07:16:36.882022 openkongqi-0.2.8/openkongqi/data/stations/cn/
--rw-r--r--   0 hr        (1000) hr        (1000)      535 2021-01-19 09:53:49.000000 openkongqi-0.2.8/openkongqi/data/stations/cn/shanghai.json
--rw-r--r--   0 hr        (1000) hr        (1000)     1609 2016-04-28 02:04:17.000000 openkongqi-0.2.8/openkongqi/data/user_agent_strings.json
--rw-r--r--   0 hr        (1000) hr        (1000)      309 2021-01-19 09:53:49.000000 openkongqi-0.2.8/openkongqi/exceptions.py
--rw-r--r--   0 hr        (1000) hr        (1000)     1345 2022-01-06 07:14:46.000000 openkongqi-0.2.8/openkongqi/fetch.py
--rw-r--r--   0 hr        (1000) hr        (1000)     2185 2022-01-06 07:14:46.000000 openkongqi-0.2.8/openkongqi/filecache.py
-drwxr-xr-x   0 hr        (1000) hr        (1000)        0 2022-01-06 07:16:36.882022 openkongqi-0.2.8/openkongqi/records/
--rw-r--r--   0 hr        (1000) hr        (1000)       24 2016-09-06 12:49:01.000000 openkongqi-0.2.8/openkongqi/records/__init__.py
--rw-r--r--   0 hr        (1000) hr        (1000)     4298 2017-06-28 08:56:59.000000 openkongqi-0.2.8/openkongqi/records/base.py
--rw-r--r--   0 hr        (1000) hr        (1000)      776 2016-04-28 02:04:17.000000 openkongqi-0.2.8/openkongqi/records/mysql.py
--rw-r--r--   0 hr        (1000) hr        (1000)      789 2016-04-28 02:04:17.000000 openkongqi-0.2.8/openkongqi/records/pgsql.py
--rw-r--r--   0 hr        (1000) hr        (1000)     5485 2017-06-28 08:56:59.000000 openkongqi-0.2.8/openkongqi/records/sqlalch.py
--rw-r--r--   0 hr        (1000) hr        (1000)      582 2017-06-28 08:56:59.000000 openkongqi-0.2.8/openkongqi/records/sqlite3.py
--rw-r--r--   0 hr        (1000) hr        (1000)      919 2021-01-19 09:53:49.000000 openkongqi-0.2.8/openkongqi/routes.py
--rw-r--r--   0 hr        (1000) hr        (1000)      405 2017-07-03 04:07:29.000000 openkongqi-0.2.8/openkongqi/sched.py
-drwxr-xr-x   0 hr        (1000) hr        (1000)        0 2022-01-06 07:16:36.882022 openkongqi-0.2.8/openkongqi/source/
--rw-r--r--   0 hr        (1000) hr        (1000)      572 2016-04-28 02:04:17.000000 openkongqi-0.2.8/openkongqi/source/__init__.py
--rw-r--r--   0 hr        (1000) hr        (1000)    10942 2022-01-06 07:14:46.000000 openkongqi-0.2.8/openkongqi/source/base.py
--rw-r--r--   0 hr        (1000) hr        (1000)     2386 2022-01-06 07:14:46.000000 openkongqi-0.2.8/openkongqi/source/pm25in.py
--rw-r--r--   0 hr        (1000) hr        (1000)     2028 2021-02-05 09:32:22.000000 openkongqi-0.2.8/openkongqi/stations.py
-drwxr-xr-x   0 hr        (1000) hr        (1000)        0 2022-01-06 07:16:36.882022 openkongqi-0.2.8/openkongqi/status/
--rw-r--r--   0 hr        (1000) hr        (1000)       24 2016-04-28 02:04:17.000000 openkongqi-0.2.8/openkongqi/status/__init__.py
--rw-r--r--   0 hr        (1000) hr        (1000)     1568 2017-06-28 08:56:59.000000 openkongqi-0.2.8/openkongqi/status/base.py
--rw-r--r--   0 hr        (1000) hr        (1000)     1074 2019-12-20 00:18:35.000000 openkongqi-0.2.8/openkongqi/status/redisdb.py
--rw-r--r--   0 hr        (1000) hr        (1000)      297 2017-06-28 08:56:59.000000 openkongqi-0.2.8/openkongqi/tasks.py
--rw-r--r--   0 hr        (1000) hr        (1000)     3365 2022-01-06 07:14:46.000000 openkongqi-0.2.8/openkongqi/utils.py
-drwxr-xr-x   0 hr        (1000) hr        (1000)        0 2022-01-06 07:16:36.882022 openkongqi-0.2.8/openkongqi.egg-info/
--rw-r--r--   0 hr        (1000) hr        (1000)     4481 2022-01-06 07:16:36.000000 openkongqi-0.2.8/openkongqi.egg-info/PKG-INFO
--rw-r--r--   0 hr        (1000) hr        (1000)     1125 2022-01-06 07:16:36.000000 openkongqi-0.2.8/openkongqi.egg-info/SOURCES.txt
--rw-r--r--   0 hr        (1000) hr        (1000)        1 2022-01-06 07:16:36.000000 openkongqi-0.2.8/openkongqi.egg-info/dependency_links.txt
--rw-r--r--   0 hr        (1000) hr        (1000)      134 2022-01-06 07:16:36.000000 openkongqi-0.2.8/openkongqi.egg-info/entry_points.txt
--rw-r--r--   0 hr        (1000) hr        (1000)      139 2022-01-06 07:16:36.000000 openkongqi-0.2.8/openkongqi.egg-info/requires.txt
--rw-r--r--   0 hr        (1000) hr        (1000)       17 2022-01-06 07:16:36.000000 openkongqi-0.2.8/openkongqi.egg-info/top_level.txt
--rw-r--r--   0 hr        (1000) hr        (1000)       67 2022-01-06 07:16:36.882022 openkongqi-0.2.8/setup.cfg
--rw-r--r--   0 hr        (1000) hr        (1000)     1978 2022-01-06 07:14:46.000000 openkongqi-0.2.8/setup.py
-drwxr-xr-x   0 hr        (1000) hr        (1000)        0 2022-01-06 07:16:36.882022 openkongqi-0.2.8/utils/
--rw-r--r--   0 hr        (1000) hr        (1000)       24 2017-06-28 08:56:59.000000 openkongqi-0.2.8/utils/__init__.py
--rw-r--r--   0 hr        (1000) hr        (1000)     3005 2019-12-20 00:18:35.000000 openkongqi-0.2.8/utils/get_user_agent_strings.py
--rwxr-xr-x   0 hr        (1000) hr        (1000)     4374 2017-06-28 08:56:59.000000 openkongqi-0.2.8/utils/source_test.py
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2023-12-03 05:08:27.453957 openkongqi-0.2.9/
+-rw-r--r--   0 hr        (1000) hr        (1000)       36 2016-04-28 02:04:17.000000 openkongqi-0.2.9/MANIFEST.in
+-rw-rw-r--   0 hr        (1000) hr        (1000)     5694 2023-12-03 05:08:27.453957 openkongqi-0.2.9/PKG-INFO
+-rw-r--r--   0 hr        (1000) hr        (1000)     3631 2019-12-23 09:03:20.000000 openkongqi-0.2.9/README.rst
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2023-12-03 05:08:27.453957 openkongqi-0.2.9/openkongqi/
+-rw-rw-r--   0 hr        (1000) hr        (1000)      120 2023-12-03 05:08:02.000000 openkongqi-0.2.9/openkongqi/__init__.py
+-rw-r--r--   0 hr        (1000) hr        (1000)      435 2018-09-21 08:43:53.000000 openkongqi-0.2.9/openkongqi/apikeys.py
+-rw-r--r--   0 hr        (1000) hr        (1000)     2363 2022-01-04 07:22:45.000000 openkongqi-0.2.9/openkongqi/bin.py
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2023-12-03 05:08:27.453957 openkongqi-0.2.9/openkongqi/cache/
+-rw-r--r--   0 hr        (1000) hr        (1000)       24 2017-06-28 08:56:59.000000 openkongqi-0.2.9/openkongqi/cache/__init__.py
+-rw-r--r--   0 hr        (1000) hr        (1000)      689 2017-06-28 08:56:59.000000 openkongqi-0.2.9/openkongqi/cache/base.py
+-rw-r--r--   0 hr        (1000) hr        (1000)      612 2019-12-20 00:18:35.000000 openkongqi-0.2.9/openkongqi/cache/redisdb.py
+-rw-r--r--   0 hr        (1000) hr        (1000)     3061 2022-01-06 07:14:46.000000 openkongqi-0.2.9/openkongqi/conf.py
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2023-12-03 05:08:27.453957 openkongqi-0.2.9/openkongqi/data/
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2023-12-03 05:08:27.453957 openkongqi-0.2.9/openkongqi/data/sources/
+-rw-r--r--   0 hr        (1000) hr        (1000)      181 2016-09-06 10:26:25.000000 openkongqi-0.2.9/openkongqi/data/sources/pm25.in.json
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2023-12-03 05:08:27.453957 openkongqi-0.2.9/openkongqi/data/stations/
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2023-12-03 05:08:27.453957 openkongqi-0.2.9/openkongqi/data/stations/cn/
+-rw-r--r--   0 hr        (1000) hr        (1000)      535 2021-01-19 09:53:49.000000 openkongqi-0.2.9/openkongqi/data/stations/cn/shanghai.json
+-rw-r--r--   0 hr        (1000) hr        (1000)     1609 2016-04-28 02:04:17.000000 openkongqi-0.2.9/openkongqi/data/user_agent_strings.json
+-rw-r--r--   0 hr        (1000) hr        (1000)      309 2021-01-19 09:53:49.000000 openkongqi-0.2.9/openkongqi/exceptions.py
+-rw-r--r--   0 hr        (1000) hr        (1000)     1345 2022-01-06 07:14:46.000000 openkongqi-0.2.9/openkongqi/fetch.py
+-rw-r--r--   0 hr        (1000) hr        (1000)     2185 2022-01-06 07:14:46.000000 openkongqi-0.2.9/openkongqi/filecache.py
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2023-12-03 05:08:27.453957 openkongqi-0.2.9/openkongqi/records/
+-rw-r--r--   0 hr        (1000) hr        (1000)       24 2016-09-06 12:49:01.000000 openkongqi-0.2.9/openkongqi/records/__init__.py
+-rw-r--r--   0 hr        (1000) hr        (1000)     4298 2017-06-28 08:56:59.000000 openkongqi-0.2.9/openkongqi/records/base.py
+-rw-r--r--   0 hr        (1000) hr        (1000)      776 2016-04-28 02:04:17.000000 openkongqi-0.2.9/openkongqi/records/mysql.py
+-rw-r--r--   0 hr        (1000) hr        (1000)      789 2016-04-28 02:04:17.000000 openkongqi-0.2.9/openkongqi/records/pgsql.py
+-rw-r--r--   0 hr        (1000) hr        (1000)     5485 2017-06-28 08:56:59.000000 openkongqi-0.2.9/openkongqi/records/sqlalch.py
+-rw-r--r--   0 hr        (1000) hr        (1000)      582 2017-06-28 08:56:59.000000 openkongqi-0.2.9/openkongqi/records/sqlite3.py
+-rw-r--r--   0 hr        (1000) hr        (1000)      919 2021-01-19 09:53:49.000000 openkongqi-0.2.9/openkongqi/routes.py
+-rw-r--r--   0 hr        (1000) hr        (1000)      405 2017-07-03 04:07:29.000000 openkongqi-0.2.9/openkongqi/sched.py
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2023-12-03 05:08:27.453957 openkongqi-0.2.9/openkongqi/source/
+-rw-r--r--   0 hr        (1000) hr        (1000)      572 2016-04-28 02:04:17.000000 openkongqi-0.2.9/openkongqi/source/__init__.py
+-rw-rw-r--   0 hr        (1000) hr        (1000)    11159 2023-12-03 05:08:02.000000 openkongqi-0.2.9/openkongqi/source/base.py
+-rw-r--r--   0 hr        (1000) hr        (1000)     2386 2022-01-06 07:14:46.000000 openkongqi-0.2.9/openkongqi/source/pm25in.py
+-rw-r--r--   0 hr        (1000) hr        (1000)     2028 2021-02-05 09:32:22.000000 openkongqi-0.2.9/openkongqi/stations.py
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2023-12-03 05:08:27.453957 openkongqi-0.2.9/openkongqi/status/
+-rw-r--r--   0 hr        (1000) hr        (1000)       24 2016-04-28 02:04:17.000000 openkongqi-0.2.9/openkongqi/status/__init__.py
+-rw-r--r--   0 hr        (1000) hr        (1000)     1568 2017-06-28 08:56:59.000000 openkongqi-0.2.9/openkongqi/status/base.py
+-rw-r--r--   0 hr        (1000) hr        (1000)     1074 2019-12-20 00:18:35.000000 openkongqi-0.2.9/openkongqi/status/redisdb.py
+-rw-r--r--   0 hr        (1000) hr        (1000)      297 2017-06-28 08:56:59.000000 openkongqi-0.2.9/openkongqi/tasks.py
+-rw-r--r--   0 hr        (1000) hr        (1000)     3365 2022-01-06 07:14:46.000000 openkongqi-0.2.9/openkongqi/utils.py
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2023-12-03 05:08:27.453957 openkongqi-0.2.9/openkongqi.egg-info/
+-rw-rw-r--   0 hr        (1000) hr        (1000)     5694 2023-12-03 05:08:27.000000 openkongqi-0.2.9/openkongqi.egg-info/PKG-INFO
+-rw-rw-r--   0 hr        (1000) hr        (1000)     1117 2023-12-03 05:08:27.000000 openkongqi-0.2.9/openkongqi.egg-info/SOURCES.txt
+-rw-rw-r--   0 hr        (1000) hr        (1000)        1 2023-12-03 05:08:27.000000 openkongqi-0.2.9/openkongqi.egg-info/dependency_links.txt
+-rw-rw-r--   0 hr        (1000) hr        (1000)      134 2023-12-03 05:08:27.000000 openkongqi-0.2.9/openkongqi.egg-info/entry_points.txt
+-rw-rw-r--   0 hr        (1000) hr        (1000)      139 2023-12-03 05:08:27.000000 openkongqi-0.2.9/openkongqi.egg-info/requires.txt
+-rw-rw-r--   0 hr        (1000) hr        (1000)       17 2023-12-03 05:08:27.000000 openkongqi-0.2.9/openkongqi.egg-info/top_level.txt
+-rw-r--r--   0 hr        (1000) hr        (1000)       67 2023-12-03 05:08:27.453957 openkongqi-0.2.9/setup.cfg
+-rw-r--r--   0 hr        (1000) hr        (1000)     1978 2022-01-06 07:14:46.000000 openkongqi-0.2.9/setup.py
+drwxrwxr-x   0 hr        (1000) hr        (1000)        0 2023-12-03 05:08:27.453957 openkongqi-0.2.9/utils/
+-rw-r--r--   0 hr        (1000) hr        (1000)       24 2017-06-28 08:56:59.000000 openkongqi-0.2.9/utils/__init__.py
+-rw-r--r--   0 hr        (1000) hr        (1000)     3005 2019-12-20 00:18:35.000000 openkongqi-0.2.9/utils/get_user_agent_strings.py
+-rwxr-xr-x   0 hr        (1000) hr        (1000)     4374 2017-06-28 08:56:59.000000 openkongqi-0.2.9/utils/source_test.py
```

### Comparing `openkongqi-0.2.8/README.rst` & `openkongqi-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/bin.py` & `openkongqi-0.2.9/openkongqi/bin.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/cache/base.py` & `openkongqi-0.2.9/openkongqi/cache/base.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/cache/redisdb.py` & `openkongqi-0.2.9/openkongqi/cache/redisdb.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/conf.py` & `openkongqi-0.2.9/openkongqi/conf.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/data/stations/cn/shanghai.json` & `openkongqi-0.2.9/openkongqi/data/stations/cn/shanghai.json`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/data/user_agent_strings.json` & `openkongqi-0.2.9/openkongqi/data/user_agent_strings.json`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/fetch.py` & `openkongqi-0.2.9/openkongqi/fetch.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/filecache.py` & `openkongqi-0.2.9/openkongqi/filecache.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/records/base.py` & `openkongqi-0.2.9/openkongqi/records/base.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/records/mysql.py` & `openkongqi-0.2.9/openkongqi/records/mysql.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/records/pgsql.py` & `openkongqi-0.2.9/openkongqi/records/pgsql.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/records/sqlalch.py` & `openkongqi-0.2.9/openkongqi/records/sqlalch.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/records/sqlite3.py` & `openkongqi-0.2.9/openkongqi/records/sqlite3.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/routes.py` & `openkongqi-0.2.9/openkongqi/routes.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/source/__init__.py` & `openkongqi-0.2.9/openkongqi/source/__init__.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/source/base.py` & `openkongqi-0.2.9/openkongqi/source/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,25 +137,28 @@
     def pythonify(self, text, is_num=False):
         if text is None:
             return None
 
         if self.null_re is not None:
             if self.null_re.match(text) is None:
                 if is_num:  # remove everything but nums and dots
-                    return float(re.sub(r'[^\d.]+', '', text))
+                    try:
+                        return float(re.sub(r'[^\d.]+', '', text))
+                    except ValueError:
+                        self.log_error(f"{self.name} - Could not convert value: {text}")
                 else:
                     return text
             else:
                 return None
         else:
             if is_num:  # remove everything but nums and dots
                 try:
                     return float(re.sub(r'[^\d.]+', '', text))
                 except ValueError:
-                    pass
+                    self.log_error(f"{self.name} - Could not convert value: {text}")
             else:
                 return text
 
     def extract(self, content):
         """Extract data from the content
         """
         raise NotImplementedError
```

### Comparing `openkongqi-0.2.8/openkongqi/source/pm25in.py` & `openkongqi-0.2.9/openkongqi/source/pm25in.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/stations.py` & `openkongqi-0.2.9/openkongqi/stations.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/status/base.py` & `openkongqi-0.2.9/openkongqi/status/base.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/status/redisdb.py` & `openkongqi-0.2.9/openkongqi/status/redisdb.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi/utils.py` & `openkongqi-0.2.9/openkongqi/utils.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/openkongqi.egg-info/SOURCES.txt` & `openkongqi-0.2.9/openkongqi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 openkongqi/__init__.py
 openkongqi/apikeys.py
 openkongqi/bin.py
```

### Comparing `openkongqi-0.2.8/setup.py` & `openkongqi-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/utils/get_user_agent_strings.py` & `openkongqi-0.2.9/utils/get_user_agent_strings.py`

 * *Files identical despite different names*

### Comparing `openkongqi-0.2.8/utils/source_test.py` & `openkongqi-0.2.9/utils/source_test.py`

 * *Files identical despite different names*

