# Comparing `tmp/eidolon_ai_client-0.1.8.tar.gz` & `tmp/eidolon_ai_client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_client-0.1.8.tar", max compression
+gzip compressed data, was "eidolon_ai_client-0.1.9.tar", max compression
```

## Comparing `eidolon_ai_client-0.1.8.tar` & `eidolon_ai_client-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2024-04-25 15:57:51.667374 eidolon_ai_client-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-04-25 15:57:51.667374 eidolon_ai_client-0.1.8/eidolon_ai_client/__init__.py
--rw-r--r--   0        0        0     7297 2024-04-25 15:57:51.667374 eidolon_ai_client-0.1.8/eidolon_ai_client/client.py
--rw-r--r--   0        0        0     5157 2024-04-25 15:57:51.667374 eidolon_ai_client-0.1.8/eidolon_ai_client/events.py
--rw-r--r--   0        0        0     2387 2024-04-25 15:57:51.667374 eidolon_ai_client-0.1.8/eidolon_ai_client/group_conversation.py
--rw-r--r--   0        0        0        0 2024-04-25 15:57:51.667374 eidolon_ai_client-0.1.8/eidolon_ai_client/util/__init__.py
--rw-r--r--   0        0        0     3728 2024-04-25 15:57:51.667374 eidolon_ai_client-0.1.8/eidolon_ai_client/util/aiohttp.py
--rw-r--r--   0        0        0      448 2024-04-25 15:57:51.667374 eidolon_ai_client-0.1.8/eidolon_ai_client/util/logger.py
--rw-r--r--   0        0        0     2361 2024-04-25 15:57:51.667374 eidolon_ai_client-0.1.8/eidolon_ai_client/util/request_context.py
--rw-r--r--   0        0        0      424 2024-04-25 15:57:51.667374 eidolon_ai_client-0.1.8/eidolon_ai_client/util/stream_collector.py
--rw-r--r--   0        0        0      645 2024-04-25 15:58:49.679842 eidolon_ai_client-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 eidolon_ai_client-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-25 16:01:55.262192 eidolon_ai_client-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 16:01:55.262192 eidolon_ai_client-0.1.9/eidolon_ai_client/__init__.py
+-rw-r--r--   0        0        0     7297 2024-04-25 16:01:55.262192 eidolon_ai_client-0.1.9/eidolon_ai_client/client.py
+-rw-r--r--   0        0        0     5157 2024-04-25 16:01:55.262192 eidolon_ai_client-0.1.9/eidolon_ai_client/events.py
+-rw-r--r--   0        0        0     2387 2024-04-25 16:01:55.262192 eidolon_ai_client-0.1.9/eidolon_ai_client/group_conversation.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:01:55.262192 eidolon_ai_client-0.1.9/eidolon_ai_client/util/__init__.py
+-rw-r--r--   0        0        0     3728 2024-04-25 16:01:55.262192 eidolon_ai_client-0.1.9/eidolon_ai_client/util/aiohttp.py
+-rw-r--r--   0        0        0      448 2024-04-25 16:01:55.262192 eidolon_ai_client-0.1.9/eidolon_ai_client/util/logger.py
+-rw-r--r--   0        0        0     2361 2024-04-25 16:01:55.262192 eidolon_ai_client-0.1.9/eidolon_ai_client/util/request_context.py
+-rw-r--r--   0        0        0      424 2024-04-25 16:01:55.262192 eidolon_ai_client-0.1.9/eidolon_ai_client/util/stream_collector.py
+-rw-r--r--   0        0        0      645 2024-04-25 16:03:03.670686 eidolon_ai_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 eidolon_ai_client-0.1.9/PKG-INFO
```

### Comparing `eidolon_ai_client-0.1.8/eidolon_ai_client/client.py` & `eidolon_ai_client-0.1.9/eidolon_ai_client/client.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.8/eidolon_ai_client/events.py` & `eidolon_ai_client-0.1.9/eidolon_ai_client/events.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.8/eidolon_ai_client/group_conversation.py` & `eidolon_ai_client-0.1.9/eidolon_ai_client/group_conversation.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.8/eidolon_ai_client/util/aiohttp.py` & `eidolon_ai_client-0.1.9/eidolon_ai_client/util/aiohttp.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.8/eidolon_ai_client/util/request_context.py` & `eidolon_ai_client-0.1.9/eidolon_ai_client/util/request_context.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.8/PKG-INFO` & `eidolon_ai_client-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eidolon_ai_client
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiostream (>=0.5.2,<0.6.0)
```

