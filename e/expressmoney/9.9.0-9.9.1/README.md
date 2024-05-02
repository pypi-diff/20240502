# Comparing `tmp/expressmoney-9.9.0.tar.gz` & `tmp/expressmoney-9.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expressmoney-9.9.0.tar", last modified: Fri May 20 14:12:30 2022, max compression
+gzip compressed data, was "expressmoney-9.9.1.tar", last modified: Thu May 26 08:57:20 2022, max compression
```

## Comparing `expressmoney-9.9.0.tar` & `expressmoney-9.9.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-05-20 14:12:30.825698 expressmoney-9.9.0/
--rw-rw-rw-   0        0        0      242 2022-05-20 14:12:30.825698 expressmoney-9.9.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-05-20 14:12:30.810062 expressmoney-9.9.0/expressmoney/
--rw-rw-rw-   0        0        0        0 2022-04-19 16:02:16.000000 expressmoney-9.9.0/expressmoney/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-20 14:12:30.825698 expressmoney-9.9.0/expressmoney/api/
--rw-rw-rw-   0        0        0      169 2022-03-08 14:19:04.000000 expressmoney-9.9.0/expressmoney/api/__init__.py
--rw-rw-rw-   0        0        0     4583 2022-05-20 14:06:03.000000 expressmoney-9.9.0/expressmoney/api/cache.py
--rw-rw-rw-   0        0        0    10315 2022-04-20 08:08:11.000000 expressmoney-9.9.0/expressmoney/api/client.py
--rw-rw-rw-   0        0        0      524 2022-04-06 09:00:06.000000 expressmoney-9.9.0/expressmoney/api/contract.py
--rw-rw-rw-   0        0        0     1334 2022-03-08 14:19:04.000000 expressmoney-9.9.0/expressmoney/api/filter.py
--rw-rw-rw-   0        0        0      929 2022-04-20 08:05:22.000000 expressmoney-9.9.0/expressmoney/api/id.py
--rw-rw-rw-   0        0        0    12257 2022-05-20 13:57:12.000000 expressmoney-9.9.0/expressmoney/api/point.py
--rw-rw-rw-   0        0        0      506 2022-04-25 14:00:42.000000 expressmoney-9.9.0/expressmoney/api/utils.py
-drwxrwxrwx   0        0        0        0 2022-05-20 14:12:30.825698 expressmoney-9.9.0/expressmoney/django/
--rw-rw-rw-   0        0        0        0 2022-03-08 14:19:04.000000 expressmoney-9.9.0/expressmoney/django/__init__.py
--rw-rw-rw-   0        0        0     1079 2022-04-28 12:27:19.000000 expressmoney-9.9.0/expressmoney/django/admin.py
--rw-rw-rw-   0        0        0     1885 2022-04-10 16:21:51.000000 expressmoney-9.9.0/expressmoney/django/authentication.py
--rw-rw-rw-   0        0        0     1893 2022-04-26 14:07:07.000000 expressmoney-9.9.0/expressmoney/django/db_router.py
--rw-rw-rw-   0        0        0     1284 2022-03-08 14:19:04.000000 expressmoney-9.9.0/expressmoney/django/mixins.py
--rw-rw-rw-   0        0        0      239 2022-03-08 14:19:04.000000 expressmoney-9.9.0/expressmoney/django/serializers.py
--rw-rw-rw-   0        0        0       19 2022-04-08 09:26:06.000000 expressmoney-9.9.0/expressmoney/django/settings.py
-drwxrwxrwx   0        0        0        0 2022-05-20 14:12:30.825698 expressmoney-9.9.0/expressmoney/utils/
--rw-rw-rw-   0        0        0       40 2022-04-20 08:08:11.000000 expressmoney-9.9.0/expressmoney/utils/__init__.py
--rw-rw-rw-   0        0        0     2600 2022-04-25 13:53:41.000000 expressmoney-9.9.0/expressmoney/utils/adapters.py
--rw-rw-rw-   0        0        0     2587 2022-04-20 08:08:11.000000 expressmoney-9.9.0/expressmoney/utils/status.py
--rw-rw-rw-   0        0        0     2304 2022-04-20 08:08:11.000000 expressmoney-9.9.0/expressmoney/utils/utils.py
-drwxrwxrwx   0        0        0        0 2022-05-20 14:12:30.825698 expressmoney-9.9.0/expressmoney/viewflow/
--rw-rw-rw-   0        0        0        0 2022-04-25 13:53:41.000000 expressmoney-9.9.0/expressmoney/viewflow/__init__.py
--rw-rw-rw-   0        0        0      298 2022-04-25 13:53:41.000000 expressmoney-9.9.0/expressmoney/viewflow/result.py
--rw-rw-rw-   0        0        0      594 2022-04-25 14:00:51.000000 expressmoney-9.9.0/expressmoney/viewflow/utils.py
-drwxrwxrwx   0        0        0        0 2022-05-20 14:12:30.810062 expressmoney-9.9.0/expressmoney.egg-info/
--rw-rw-rw-   0        0        0      242 2022-05-20 14:12:30.000000 expressmoney-9.9.0/expressmoney.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      870 2022-05-20 14:12:30.000000 expressmoney-9.9.0/expressmoney.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-20 14:12:30.000000 expressmoney-9.9.0/expressmoney.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2022-05-20 14:12:30.000000 expressmoney-9.9.0/expressmoney.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-05-20 14:12:30.000000 expressmoney-9.9.0/expressmoney.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-20 14:12:30.825698 expressmoney-9.9.0/setup.cfg
--rw-rw-rw-   0        0        0      469 2022-05-20 14:11:56.000000 expressmoney-9.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-26 08:57:20.102755 expressmoney-9.9.1/
+-rw-rw-rw-   0        0        0      242 2022-05-26 08:57:20.102755 expressmoney-9.9.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-05-26 08:57:20.102755 expressmoney-9.9.1/expressmoney/
+-rw-rw-rw-   0        0        0        0 2022-04-19 16:02:16.000000 expressmoney-9.9.1/expressmoney/__init__.py
+drwxrwxrwx   0        0        0        0 2022-05-26 08:57:20.102755 expressmoney-9.9.1/expressmoney/api/
+-rw-rw-rw-   0        0        0      169 2022-03-08 14:19:04.000000 expressmoney-9.9.1/expressmoney/api/__init__.py
+-rw-rw-rw-   0        0        0     4583 2022-05-20 14:06:03.000000 expressmoney-9.9.1/expressmoney/api/cache.py
+-rw-rw-rw-   0        0        0    10315 2022-04-20 08:08:11.000000 expressmoney-9.9.1/expressmoney/api/client.py
+-rw-rw-rw-   0        0        0      524 2022-04-06 09:00:06.000000 expressmoney-9.9.1/expressmoney/api/contract.py
+-rw-rw-rw-   0        0        0     1334 2022-03-08 14:19:04.000000 expressmoney-9.9.1/expressmoney/api/filter.py
+-rw-rw-rw-   0        0        0      929 2022-04-20 08:05:22.000000 expressmoney-9.9.1/expressmoney/api/id.py
+-rw-rw-rw-   0        0        0    12257 2022-05-20 13:57:12.000000 expressmoney-9.9.1/expressmoney/api/point.py
+-rw-rw-rw-   0        0        0      506 2022-04-25 14:00:42.000000 expressmoney-9.9.1/expressmoney/api/utils.py
+drwxrwxrwx   0        0        0        0 2022-05-26 08:57:20.102755 expressmoney-9.9.1/expressmoney/django/
+-rw-rw-rw-   0        0        0        0 2022-03-08 14:19:04.000000 expressmoney-9.9.1/expressmoney/django/__init__.py
+-rw-rw-rw-   0        0        0     1079 2022-04-28 12:27:19.000000 expressmoney-9.9.1/expressmoney/django/admin.py
+-rw-rw-rw-   0        0        0     1885 2022-04-10 16:21:51.000000 expressmoney-9.9.1/expressmoney/django/authentication.py
+-rw-rw-rw-   0        0        0     1893 2022-04-26 14:07:07.000000 expressmoney-9.9.1/expressmoney/django/db_router.py
+-rw-rw-rw-   0        0        0     1284 2022-03-08 14:19:04.000000 expressmoney-9.9.1/expressmoney/django/mixins.py
+-rw-rw-rw-   0        0        0      239 2022-03-08 14:19:04.000000 expressmoney-9.9.1/expressmoney/django/serializers.py
+-rw-rw-rw-   0        0        0       19 2022-04-08 09:26:06.000000 expressmoney-9.9.1/expressmoney/django/settings.py
+drwxrwxrwx   0        0        0        0 2022-05-26 08:57:20.102755 expressmoney-9.9.1/expressmoney/utils/
+-rw-rw-rw-   0        0        0       40 2022-04-20 08:08:11.000000 expressmoney-9.9.1/expressmoney/utils/__init__.py
+-rw-rw-rw-   0        0        0     2600 2022-04-25 13:53:41.000000 expressmoney-9.9.1/expressmoney/utils/adapters.py
+-rw-rw-rw-   0        0        0     2587 2022-04-20 08:08:11.000000 expressmoney-9.9.1/expressmoney/utils/status.py
+-rw-rw-rw-   0        0        0     1875 2022-05-26 08:57:17.000000 expressmoney-9.9.1/expressmoney/utils/utils.py
+drwxrwxrwx   0        0        0        0 2022-05-26 08:57:20.102755 expressmoney-9.9.1/expressmoney/viewflow/
+-rw-rw-rw-   0        0        0        0 2022-04-25 13:53:41.000000 expressmoney-9.9.1/expressmoney/viewflow/__init__.py
+-rw-rw-rw-   0        0        0      298 2022-04-25 13:53:41.000000 expressmoney-9.9.1/expressmoney/viewflow/result.py
+-rw-rw-rw-   0        0        0      594 2022-04-25 14:00:51.000000 expressmoney-9.9.1/expressmoney/viewflow/utils.py
+drwxrwxrwx   0        0        0        0 2022-05-26 08:57:20.102755 expressmoney-9.9.1/expressmoney.egg-info/
+-rw-rw-rw-   0        0        0      242 2022-05-26 08:57:20.000000 expressmoney-9.9.1/expressmoney.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      870 2022-05-26 08:57:20.000000 expressmoney-9.9.1/expressmoney.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-26 08:57:20.000000 expressmoney-9.9.1/expressmoney.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2022-05-26 08:57:20.000000 expressmoney-9.9.1/expressmoney.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2022-05-26 08:57:20.000000 expressmoney-9.9.1/expressmoney.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-05-26 08:57:20.118377 expressmoney-9.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      469 2022-05-26 08:57:17.000000 expressmoney-9.9.1/setup.py
```

### Comparing `expressmoney-9.9.0/expressmoney/api/cache.py` & `expressmoney-9.9.1/expressmoney/api/cache.py`

 * *Files identical despite different names*

### Comparing `expressmoney-9.9.0/expressmoney/api/client.py` & `expressmoney-9.9.1/expressmoney/api/client.py`

 * *Files identical despite different names*

### Comparing `expressmoney-9.9.0/expressmoney/api/contract.py` & `expressmoney-9.9.1/expressmoney/api/contract.py`

 * *Files identical despite different names*

### Comparing `expressmoney-9.9.0/expressmoney/api/filter.py` & `expressmoney-9.9.1/expressmoney/api/filter.py`

 * *Files identical despite different names*

### Comparing `expressmoney-9.9.0/expressmoney/api/id.py` & `expressmoney-9.9.1/expressmoney/api/id.py`

 * *Files identical despite different names*

### Comparing `expressmoney-9.9.0/expressmoney/api/point.py` & `expressmoney-9.9.1/expressmoney/api/point.py`

 * *Files identical despite different names*

### Comparing `expressmoney-9.9.0/expressmoney/django/admin.py` & `expressmoney-9.9.1/expressmoney/django/admin.py`

 * *Files identical despite different names*

### Comparing `expressmoney-9.9.0/expressmoney/django/authentication.py` & `expressmoney-9.9.1/expressmoney/django/authentication.py`

 * *Files identical despite different names*

### Comparing `expressmoney-9.9.0/expressmoney/django/db_router.py` & `expressmoney-9.9.1/expressmoney/django/db_router.py`

 * *Files identical despite different names*

### Comparing `expressmoney-9.9.0/expressmoney/django/mixins.py` & `expressmoney-9.9.1/expressmoney/django/mixins.py`

 * *Files identical despite different names*

### Comparing `expressmoney-9.9.0/expressmoney/utils/adapters.py` & `expressmoney-9.9.1/expressmoney/utils/adapters.py`

 * *Files identical despite different names*

### Comparing `expressmoney-9.9.0/expressmoney/utils/status.py` & `expressmoney-9.9.1/expressmoney/utils/status.py`

 * *Files identical despite different names*

### Comparing `expressmoney-9.9.0/expressmoney/viewflow/utils.py` & `expressmoney-9.9.1/expressmoney/viewflow/utils.py`

 * *Files identical despite different names*

### Comparing `expressmoney-9.9.0/expressmoney.egg-info/SOURCES.txt` & `expressmoney-9.9.1/expressmoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

