# Comparing `tmp/rulebricks-0.1.1.tar.gz` & `tmp/rulebricks-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rulebricks-0.1.1.tar", max compression
+gzip compressed data, was "rulebricks-0.1.2.tar", max compression
```

## Comparing `rulebricks-0.1.1.tar` & `rulebricks-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     2526 2024-05-02 03:28:43.536439 rulebricks-0.1.1/README.md
--rw-r--r--   0        0        0      428 2024-05-02 03:28:43.536439 rulebricks-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2759 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/__init__.py
--rw-r--r--   0        0        0     1485 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/client.py
--rw-r--r--   0        0        0      519 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/core/api_error.py
--rw-r--r--   0        0        0      968 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      221 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/errors/bad_request_error.py
--rw-r--r--   0        0        0      252 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/errors/internal_server_error.py
--rw-r--r--   0        0        0      404 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/flows/__init__.py
--rw-r--r--   0        0        0     4115 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/flows/client.py
--rw-r--r--   0        0        0      351 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/rules/__init__.py
--rw-r--r--   0        0        0    15996 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/rules/client.py
--rw-r--r--   0        0        0      473 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/rules/types/__init__.py
--rw-r--r--   0        0        0     1700 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/rules/types/list_response_item.py
--rw-r--r--   0        0        0     1870 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py
--rw-r--r--   0        0        0     1878 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py
--rw-r--r--   0        0        0     1675 2024-05-02 03:28:43.536439 rulebricks-0.1.1/src/rulebricks/resources/rules/types/usage_response.py
--rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 rulebricks-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2535 2024-05-02 03:51:49.144162 rulebricks-0.1.2/README.md
+-rw-r--r--   0        0        0      428 2024-05-02 03:51:49.144162 rulebricks-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3150 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/client.py
+-rw-r--r--   0        0        0      519 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/core/api_error.py
+-rw-r--r--   0        0        0      968 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      221 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/errors/bad_request_error.py
+-rw-r--r--   0        0        0      252 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/errors/internal_server_error.py
+-rw-r--r--   0        0        0      404 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/flows/__init__.py
+-rw-r--r--   0        0        0     4115 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/flows/client.py
+-rw-r--r--   0        0        0      351 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/rules/__init__.py
+-rw-r--r--   0        0        0    15996 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/rules/client.py
+-rw-r--r--   0        0        0      473 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/rules/types/__init__.py
+-rw-r--r--   0        0        0     1700 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/rules/types/list_response_item.py
+-rw-r--r--   0        0        0     1870 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py
+-rw-r--r--   0        0        0     1878 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py
+-rw-r--r--   0        0        0     1675 2024-05-02 03:51:49.144162 rulebricks-0.1.2/src/rulebricks/resources/rules/types/usage_response.py
+-rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 rulebricks-0.1.2/PKG-INFO
```

### Comparing `rulebricks-0.1.1/README.md` & `rulebricks-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Rulebricks – Python SDK
-[![pypi](https://img.shields.io/pypi/v/flatfile.svg)](https://pypi.python.org/pypi/rulebricks)
 
+[![pypi](https://img.shields.io/pypi/v/flatfile.svg)](https://pypi.python.org/pypi/rulebricks)
 
 ## Documentation
 
 API reference documentation is available [here](https://rulebricks.com/docs).
 
 ## Installation
 
@@ -35,15 +35,15 @@
 
 ```python
 import rulebricks as rb
 
 # Set the API key
 rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
 
-result = rb.rules.solve(
+result = rb.sync_api.rules.solve(
     slug="tJOCd8XXXX",
     request={
         "customer_id": "anc39as3",
         "purchase_history": ["t-shirt", "mug"],
         "account_age_days": 4,
         "last_purchase_days_ago": 3,
         "email_subscription": False
```

### Comparing `rulebricks-0.1.1/src/rulebricks/client.py` & `rulebricks-0.1.2/src/rulebricks/client.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.1/src/rulebricks/core/__init__.py` & `rulebricks-0.1.2/src/rulebricks/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.1/src/rulebricks/core/client_wrapper.py` & `rulebricks-0.1.2/src/rulebricks/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.1/src/rulebricks/core/datetime_utils.py` & `rulebricks-0.1.2/src/rulebricks/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.1/src/rulebricks/core/jsonable_encoder.py` & `rulebricks-0.1.2/src/rulebricks/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.1/src/rulebricks/resources/flows/client.py` & `rulebricks-0.1.2/src/rulebricks/resources/flows/client.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.1/src/rulebricks/resources/rules/client.py` & `rulebricks-0.1.2/src/rulebricks/resources/rules/client.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.1/src/rulebricks/resources/rules/types/list_response_item.py` & `rulebricks-0.1.2/src/rulebricks/resources/rules/types/list_response_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.1/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py` & `rulebricks-0.1.2/src/rulebricks/resources/rules/types/list_response_item_request_schema_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.1/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py` & `rulebricks-0.1.2/src/rulebricks/resources/rules/types/list_response_item_response_schema_item.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.1/src/rulebricks/resources/rules/types/usage_response.py` & `rulebricks-0.1.2/src/rulebricks/resources/rules/types/usage_response.py`

 * *Files identical despite different names*

### Comparing `rulebricks-0.1.1/PKG-INFO` & `rulebricks-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: rulebricks
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.21.2)
 Requires-Dist: pydantic (>=1.9.2)
 Requires-Dist: typing_extensions (>=4.0.0)
 Description-Content-Type: text/markdown
 
 # Rulebricks – Python SDK
-[![pypi](https://img.shields.io/pypi/v/flatfile.svg)](https://pypi.python.org/pypi/rulebricks)
 
+[![pypi](https://img.shields.io/pypi/v/flatfile.svg)](https://pypi.python.org/pypi/rulebricks)
 
 ## Documentation
 
 API reference documentation is available [here](https://rulebricks.com/docs).
 
 ## Installation
 
@@ -50,15 +50,15 @@
 
 ```python
 import rulebricks as rb
 
 # Set the API key
 rb.set_api_key("XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX")
 
-result = rb.rules.solve(
+result = rb.sync_api.rules.solve(
     slug="tJOCd8XXXX",
     request={
         "customer_id": "anc39as3",
         "purchase_history": ["t-shirt", "mug"],
         "account_age_days": 4,
         "last_purchase_days_ago": 3,
         "email_subscription": False
```

