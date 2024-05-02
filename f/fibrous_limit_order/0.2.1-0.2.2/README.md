# Comparing `tmp/fibrous_limit_order-0.2.1.tar.gz` & `tmp/fibrous_limit_order-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fibrous_limit_order-0.2.1.tar", max compression
+gzip compressed data, was "fibrous_limit_order-0.2.2.tar", max compression
```

## Comparing `fibrous_limit_order-0.2.1.tar` & `fibrous_limit_order-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1071 2024-03-25 23:02:23.244995 fibrous_limit_order-0.2.1/LICENCE
--rw-r--r--   0        0        0     1765 2024-03-25 23:03:28.782327 fibrous_limit_order-0.2.1/README.md
--rw-r--r--   0        0        0       19 2024-05-02 18:35:46.519133 fibrous_limit_order-0.2.1/fibrous_limit_order/__init__.py
--rw-r--r--   0        0        0       26 2024-05-02 18:40:14.804233 fibrous_limit_order-0.2.1/fibrous_limit_order/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 22:21:34.556066 fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/__init__.py
--rw-r--r--   0        0        0      800 2024-03-25 22:23:22.696052 fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/cancel_order.py
--rw-r--r--   0        0        0      497 2024-03-25 22:23:29.311493 fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/fill_order.py
--rw-r--r--   0        0        0     1484 2024-03-25 22:23:10.441772 fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/full_create_order.py
--rw-r--r--   0        0        0     1713 2024-03-25 22:23:34.844548 fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/full_fill_order.py
--rw-r--r--   0        0        0      683 2024-03-25 22:23:39.512516 fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/get_nonce.py
--rw-r--r--   0        0        0     1138 2024-05-02 18:38:29.270300 fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/get_orders.py
--rw-r--r--   0        0        0      517 2024-03-25 22:23:51.165342 fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/get_remaining_amount.py
--rw-r--r--   0        0        0     1204 2024-03-25 22:23:58.045887 fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/place_order.py
--rw-r--r--   0        0        0      693 2024-03-25 22:24:02.564619 fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/sign_message.py
--rw-r--r--   0        0        0      172 2024-05-02 18:59:02.233263 fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/__init__.py
--rw-r--r--   0        0        0      472 2024-03-25 20:51:35.300016 fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/accounts.py
--rw-r--r--   0        0        0      170 2024-03-25 22:07:33.034637 fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/constants.py
--rw-r--r--   0        0        0     4308 2024-05-02 18:43:04.152146 fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/limit_order.py
--rw-r--r--   0        0        0      992 2024-05-02 18:43:08.824974 fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/mock_data.py
--rw-r--r--   0        0        0     3445 2024-03-25 20:51:35.299069 fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/order_types.py
--rw-r--r--   0        0        0       19 2024-03-25 20:51:35.300593 fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/personal_data.py
--rw-r--r--   0        0        0     3253 2024-05-02 18:43:07.923911 fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/sign_message.py
--rw-r--r--   0        0        0     2079 2024-03-25 20:51:35.300861 fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/types.py
--rw-r--r--   0        0        0     1772 2024-03-25 20:51:35.300993 fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/utils.py
--rw-r--r--   0        0        0   120332 2024-03-25 20:51:35.299642 fibrous_limit_order-0.2.1/fibrous_limit_order/src/tokens.json
--rw-r--r--   0        0        0      449 2024-05-02 19:00:55.001603 fibrous_limit_order-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 fibrous_limit_order-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-25 23:02:23.244995 fibrous_limit_order-0.2.2/LICENCE
+-rw-r--r--   0        0        0     1765 2024-03-25 23:03:28.782327 fibrous_limit_order-0.2.2/README.md
+-rw-r--r--   0        0        0       19 2024-05-02 18:35:46.519133 fibrous_limit_order-0.2.2/fibrous_limit_order/__init__.py
+-rw-r--r--   0        0        0       26 2024-05-02 18:40:14.804233 fibrous_limit_order-0.2.2/fibrous_limit_order/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 22:21:34.556066 fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/__init__.py
+-rw-r--r--   0        0        0      800 2024-03-25 22:23:22.696052 fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/cancel_order.py
+-rw-r--r--   0        0        0      497 2024-03-25 22:23:29.311493 fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/fill_order.py
+-rw-r--r--   0        0        0     1484 2024-03-25 22:23:10.441772 fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/full_create_order.py
+-rw-r--r--   0        0        0     1713 2024-03-25 22:23:34.844548 fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/full_fill_order.py
+-rw-r--r--   0        0        0      683 2024-03-25 22:23:39.512516 fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/get_nonce.py
+-rw-r--r--   0        0        0     1138 2024-05-02 18:38:29.270300 fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/get_orders.py
+-rw-r--r--   0        0        0      517 2024-03-25 22:23:51.165342 fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/get_remaining_amount.py
+-rw-r--r--   0        0        0     1204 2024-03-25 22:23:58.045887 fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/place_order.py
+-rw-r--r--   0        0        0      693 2024-03-25 22:24:02.564619 fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/sign_message.py
+-rw-r--r--   0        0        0      231 2024-05-02 19:03:15.975890 fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/__init__.py
+-rw-r--r--   0        0        0      472 2024-03-25 20:51:35.300016 fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/accounts.py
+-rw-r--r--   0        0        0      170 2024-03-25 22:07:33.034637 fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/constants.py
+-rw-r--r--   0        0        0     4308 2024-05-02 18:43:04.152146 fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/limit_order.py
+-rw-r--r--   0        0        0      992 2024-05-02 18:43:08.824974 fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/mock_data.py
+-rw-r--r--   0        0        0     3445 2024-03-25 20:51:35.299069 fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/order_types.py
+-rw-r--r--   0        0        0       19 2024-03-25 20:51:35.300593 fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/personal_data.py
+-rw-r--r--   0        0        0     3253 2024-05-02 18:43:07.923911 fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/sign_message.py
+-rw-r--r--   0        0        0     2079 2024-03-25 20:51:35.300861 fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/types.py
+-rw-r--r--   0        0        0     1772 2024-03-25 20:51:35.300993 fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/utils.py
+-rw-r--r--   0        0        0   120332 2024-03-25 20:51:35.299642 fibrous_limit_order-0.2.2/fibrous_limit_order/src/tokens.json
+-rw-r--r--   0        0        0      449 2024-05-02 19:03:25.002768 fibrous_limit_order-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 fibrous_limit_order-0.2.2/PKG-INFO
```

### Comparing `fibrous_limit_order-0.2.1/LICENCE` & `fibrous_limit_order-0.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/README.md` & `fibrous_limit_order-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/cancel_order.py` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/cancel_order.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/full_create_order.py` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/full_create_order.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/full_fill_order.py` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/full_fill_order.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/get_nonce.py` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/get_nonce.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/get_orders.py` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/get_orders.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/get_remaining_amount.py` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/get_remaining_amount.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/place_order.py` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/place_order.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/examples/sign_message.py` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/examples/sign_message.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/limit_order.py` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/limit_order.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/mock_data.py` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/mock_data.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/order_types.py` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/order_types.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/sign_message.py` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/sign_message.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/types.py` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/types.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/limit_order/utils.py` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/limit_order/utils.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/fibrous_limit_order/src/tokens.json` & `fibrous_limit_order-0.2.2/fibrous_limit_order/src/tokens.json`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.2.1/PKG-INFO` & `fibrous_limit_order-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fibrous_limit_order
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python SDK for Fibrous Finance Limit Order
 License: MIT
 Author: zeroonesymphony
 Author-email: kermo@fibrous.finance
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fibrous_limit_order Version: 0.2.1 Summary: A
+Metadata-Version: 2.1 Name: fibrous_limit_order Version: 0.2.2 Summary: A
 Python SDK for Fibrous Finance Limit Order License: MIT Author: zeroonesymphony
 Author-email: kermo@fibrous.finance Requires-Python: >=3.9,<3.13 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Description-
 Content-Type: text/markdown
```

