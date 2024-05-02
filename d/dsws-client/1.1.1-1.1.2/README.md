# Comparing `tmp/dsws_client-1.1.1.tar.gz` & `tmp/dsws_client-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsws_client-1.1.1.tar", last modified: Tue Apr 30 13:55:26 2024, max compression
+gzip compressed data, was "dsws_client-1.1.2.tar", last modified: Thu May  2 11:32:28 2024, max compression
```

## Comparing `dsws_client-1.1.1.tar` & `dsws_client-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      753 2024-04-30 13:55:07.989594 dsws_client-1.1.1/README.md
--rw-r--r--   0        0        0      319 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/__init__.py
--rw-r--r--   0        0        0    13127 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/client.py
--rw-r--r--   0        0        0     1589 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/config.py
--rw-r--r--   0        0        0      757 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/converters.py
--rw-r--r--   0        0        0     9523 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/ds_request.py
--rw-r--r--   0        0        0     5417 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/ds_response.py
--rw-r--r--   0        0        0      510 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/exceptions.py
--rw-r--r--   0        0        0     5907 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/parse.py
--rw-r--r--   0        0        0        0 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/py.typed
--rw-r--r--   0        0        0      508 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/value_objects/__init__.py
--rw-r--r--   0        0        0     1603 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/value_objects/enums.py
--rw-r--r--   0        0        0      563 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/value_objects/types.py
--rw-r--r--   0        0        0       77 2024-04-30 13:55:07.989594 dsws_client-1.1.1/dsws_client/version.py
--rw-r--r--   0        0        0     3206 2024-04-30 13:55:26.597586 dsws_client-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       18 2024-04-30 13:55:07.989594 dsws_client-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2940 2024-04-30 13:55:07.989594 dsws_client-1.1.1/tests/conftest.py
--rw-r--r--   0        0        0     2567 2024-04-30 13:55:07.989594 dsws_client-1.1.1/tests/test_client.py
--rw-r--r--   0        0        0     1248 2024-04-30 13:55:07.989594 dsws_client-1.1.1/tests/test_parsing.py
--rw-r--r--   0        0        0     4935 2024-04-30 13:55:07.989594 dsws_client-1.1.1/tests/test_requests.py
--rw-r--r--   0        0        0     1784 2024-04-30 13:55:07.989594 dsws_client-1.1.1/tests/test_responses.py
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 dsws_client-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      753 2024-05-02 11:32:10.876467 dsws_client-1.1.2/README.md
+-rw-r--r--   0        0        0      319 2024-05-02 11:32:10.876467 dsws_client-1.1.2/dsws_client/__init__.py
+-rw-r--r--   0        0        0    13127 2024-05-02 11:32:10.876467 dsws_client-1.1.2/dsws_client/client.py
+-rw-r--r--   0        0        0     1589 2024-05-02 11:32:10.876467 dsws_client-1.1.2/dsws_client/config.py
+-rw-r--r--   0        0        0      757 2024-05-02 11:32:10.876467 dsws_client-1.1.2/dsws_client/converters.py
+-rw-r--r--   0        0        0     9523 2024-05-02 11:32:10.876467 dsws_client-1.1.2/dsws_client/ds_request.py
+-rw-r--r--   0        0        0     5417 2024-05-02 11:32:10.876467 dsws_client-1.1.2/dsws_client/ds_response.py
+-rw-r--r--   0        0        0      510 2024-05-02 11:32:10.876467 dsws_client-1.1.2/dsws_client/exceptions.py
+-rw-r--r--   0        0        0     5994 2024-05-02 11:32:10.876467 dsws_client-1.1.2/dsws_client/parse.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:32:10.876467 dsws_client-1.1.2/dsws_client/py.typed
+-rw-r--r--   0        0        0      508 2024-05-02 11:32:10.876467 dsws_client-1.1.2/dsws_client/value_objects/__init__.py
+-rw-r--r--   0        0        0     1603 2024-05-02 11:32:10.876467 dsws_client-1.1.2/dsws_client/value_objects/enums.py
+-rw-r--r--   0        0        0      583 2024-05-02 11:32:10.876467 dsws_client-1.1.2/dsws_client/value_objects/types.py
+-rw-r--r--   0        0        0       77 2024-05-02 11:32:10.876467 dsws_client-1.1.2/dsws_client/version.py
+-rw-r--r--   0        0        0     3206 2024-05-02 11:32:28.856493 dsws_client-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0       18 2024-05-02 11:32:10.876467 dsws_client-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     2940 2024-05-02 11:32:10.876467 dsws_client-1.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     2567 2024-05-02 11:32:10.876467 dsws_client-1.1.2/tests/test_client.py
+-rw-r--r--   0        0        0     1248 2024-05-02 11:32:10.880467 dsws_client-1.1.2/tests/test_parsing.py
+-rw-r--r--   0        0        0     4935 2024-05-02 11:32:10.880467 dsws_client-1.1.2/tests/test_requests.py
+-rw-r--r--   0        0        0     1784 2024-05-02 11:32:10.880467 dsws_client-1.1.2/tests/test_responses.py
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 dsws_client-1.1.2/PKG-INFO
```

### Comparing `dsws_client-1.1.1/README.md` & `dsws_client-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.1/dsws_client/client.py` & `dsws_client-1.1.2/dsws_client/client.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.1/dsws_client/config.py` & `dsws_client-1.1.2/dsws_client/config.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.1/dsws_client/converters.py` & `dsws_client-1.1.2/dsws_client/converters.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.1/dsws_client/ds_request.py` & `dsws_client-1.1.2/dsws_client/ds_request.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.1/dsws_client/ds_response.py` & `dsws_client-1.1.2/dsws_client/ds_response.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.1/dsws_client/parse.py` & `dsws_client-1.1.2/dsws_client/parse.py`

 * *Files 10% similar despite different names*

```diff
@@ -149,23 +149,26 @@
 
 
 def parse_meta(response: DSDataResponse) -> Meta:
     """Parse meta information from a response."""
     meta = Meta()
     if response.data_type_names:
         meta.data_type_names = {
-            kv_pair.key: kv_pair.value for kv_pair in response.data_type_names
+            kv_pair.key or kv_pair.value: kv_pair.value
+            for kv_pair in response.data_type_names
         }
     if response.symbol_names:
         meta.symbol_names = {
-            kv_pair.key: kv_pair.value for kv_pair in response.symbol_names
+            kv_pair.key or kv_pair.value: kv_pair.value
+            for kv_pair in response.symbol_names
         }
     if response.additional_responses:
         meta.additional_responses = {
-            kv_pair.key: kv_pair.value for kv_pair in response.additional_responses
+            kv_pair.key or kv_pair.value: kv_pair.value
+            for kv_pair in response.additional_responses
         }
     if response.tag:
         meta.tags.append(response.tag)
     return meta
 
 
 def process_string_value(value: str) -> Optional[Union[str, bool]]:
```

### Comparing `dsws_client-1.1.1/dsws_client/value_objects/enums.py` & `dsws_client-1.1.2/dsws_client/value_objects/enums.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.1/pyproject.toml` & `dsws_client-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dsws-client"
-version = "1.1.1"
+version = "1.1.2"
 description = "Python client for the Datastream Web Service API (DSWS)"
 readme = "README.md"
 authors = [
     { name = "ljnsn", email = "info@ljnsn.com" },
 ]
 requires-python = ">=3.8,<4.0"
 dependencies = [
```

### Comparing `dsws_client-1.1.1/tests/conftest.py` & `dsws_client-1.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.1/tests/test_client.py` & `dsws_client-1.1.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.1/tests/test_parsing.py` & `dsws_client-1.1.2/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.1/tests/test_requests.py` & `dsws_client-1.1.2/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.1/tests/test_responses.py` & `dsws_client-1.1.2/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `dsws_client-1.1.1/PKG-INFO` & `dsws_client-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsws-client
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python client for the Datastream Web Service API (DSWS)
 Author-Email: ljnsn <info@ljnsn.com>
 License: MIT
 Requires-Python: <4.0,>=3.8
 Requires-Dist: attrs>=23.1.0
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: msgspec>=0.18.6
```

