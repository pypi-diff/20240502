# Comparing `tmp/fibrous_limit_order-0.1.4.tar.gz` & `tmp/fibrous_limit_order-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fibrous_limit_order-0.1.4.tar", max compression
+gzip compressed data, was "fibrous_limit_order-0.1.5.tar", max compression
```

## Comparing `fibrous_limit_order-0.1.4.tar` & `fibrous_limit_order-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1071 2024-03-25 23:02:23.244995 fibrous_limit_order-0.1.4/LICENCE
--rw-r--r--   0        0        0     1765 2024-03-25 23:03:28.782327 fibrous_limit_order-0.1.4/README.md
--rw-r--r--   0        0        0       19 2024-05-02 18:35:46.519133 fibrous_limit_order-0.1.4/fibrous_limit_order/__init__.py
--rw-r--r--   0        0        0       54 2024-05-02 18:35:36.408716 fibrous_limit_order-0.1.4/fibrous_limit_order/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 22:21:34.556066 fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/__init__.py
--rw-r--r--   0        0        0      800 2024-03-25 22:23:22.696052 fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/cancel_order.py
--rw-r--r--   0        0        0      497 2024-03-25 22:23:29.311493 fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/fill_order.py
--rw-r--r--   0        0        0     1484 2024-03-25 22:23:10.441772 fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/full_create_order.py
--rw-r--r--   0        0        0     1713 2024-03-25 22:23:34.844548 fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/full_fill_order.py
--rw-r--r--   0        0        0      683 2024-03-25 22:23:39.512516 fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/get_nonce.py
--rw-r--r--   0        0        0     1162 2024-05-02 18:32:10.602766 fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/get_orders.py
--rw-r--r--   0        0        0      517 2024-03-25 22:23:51.165342 fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/get_remaining_amount.py
--rw-r--r--   0        0        0     1204 2024-03-25 22:23:58.045887 fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/place_order.py
--rw-r--r--   0        0        0      693 2024-03-25 22:24:02.564619 fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/sign_message.py
--rw-r--r--   0        0        0      141 2024-03-25 23:09:35.149518 fibrous_limit_order-0.1.4/fibrous_limit_order/src/limit_order/__init__.py
--rw-r--r--   0        0        0      472 2024-03-25 20:51:35.300016 fibrous_limit_order-0.1.4/fibrous_limit_order/src/limit_order/accounts.py
--rw-r--r--   0        0        0      170 2024-03-25 22:07:33.034637 fibrous_limit_order-0.1.4/fibrous_limit_order/src/limit_order/constants.py
--rw-r--r--   0        0        0     4280 2024-03-25 21:46:41.880609 fibrous_limit_order-0.1.4/fibrous_limit_order/src/limit_order/limit_order.py
--rw-r--r--   0        0        0      964 2024-03-25 22:07:28.943698 fibrous_limit_order-0.1.4/fibrous_limit_order/src/limit_order/mock_data.py
--rw-r--r--   0        0        0       19 2024-03-25 20:51:35.300593 fibrous_limit_order-0.1.4/fibrous_limit_order/src/limit_order/personal_data.py
--rw-r--r--   0        0        0     3225 2024-03-25 20:51:35.300732 fibrous_limit_order-0.1.4/fibrous_limit_order/src/limit_order/sign_message.py
--rw-r--r--   0        0        0     2079 2024-03-25 20:51:35.300861 fibrous_limit_order-0.1.4/fibrous_limit_order/src/limit_order/types.py
--rw-r--r--   0        0        0     1772 2024-03-25 20:51:35.300993 fibrous_limit_order-0.1.4/fibrous_limit_order/src/limit_order/utils.py
--rw-r--r--   0        0        0       21 2024-05-02 18:33:40.324597 fibrous_limit_order-0.1.4/fibrous_limit_order/src/return_types/__init__.py
--rw-r--r--   0        0        0     3445 2024-03-25 20:51:35.299069 fibrous_limit_order-0.1.4/fibrous_limit_order/src/return_types/orders.py
--rw-r--r--   0        0        0   120332 2024-03-25 20:51:35.299642 fibrous_limit_order-0.1.4/fibrous_limit_order/src/tokens.json
--rw-r--r--   0        0        0      449 2024-05-02 18:36:12.031021 fibrous_limit_order-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 fibrous_limit_order-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-25 23:02:23.244995 fibrous_limit_order-0.1.5/LICENCE
+-rw-r--r--   0        0        0     1765 2024-03-25 23:03:28.782327 fibrous_limit_order-0.1.5/README.md
+-rw-r--r--   0        0        0       19 2024-05-02 18:35:46.519133 fibrous_limit_order-0.1.5/fibrous_limit_order/__init__.py
+-rw-r--r--   0        0        0       54 2024-05-02 18:35:36.408716 fibrous_limit_order-0.1.5/fibrous_limit_order/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 22:21:34.556066 fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/__init__.py
+-rw-r--r--   0        0        0      800 2024-03-25 22:23:22.696052 fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/cancel_order.py
+-rw-r--r--   0        0        0      497 2024-03-25 22:23:29.311493 fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/fill_order.py
+-rw-r--r--   0        0        0     1484 2024-03-25 22:23:10.441772 fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/full_create_order.py
+-rw-r--r--   0        0        0     1713 2024-03-25 22:23:34.844548 fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/full_fill_order.py
+-rw-r--r--   0        0        0      683 2024-03-25 22:23:39.512516 fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/get_nonce.py
+-rw-r--r--   0        0        0     1138 2024-05-02 18:38:29.270300 fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/get_orders.py
+-rw-r--r--   0        0        0      517 2024-03-25 22:23:51.165342 fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/get_remaining_amount.py
+-rw-r--r--   0        0        0     1204 2024-03-25 22:23:58.045887 fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/place_order.py
+-rw-r--r--   0        0        0      693 2024-03-25 22:24:02.564619 fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/sign_message.py
+-rw-r--r--   0        0        0      169 2024-05-02 18:39:18.389430 fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/__init__.py
+-rw-r--r--   0        0        0      472 2024-03-25 20:51:35.300016 fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/accounts.py
+-rw-r--r--   0        0        0      170 2024-03-25 22:07:33.034637 fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/constants.py
+-rw-r--r--   0        0        0     4280 2024-03-25 21:46:41.880609 fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/limit_order.py
+-rw-r--r--   0        0        0      964 2024-03-25 22:07:28.943698 fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/mock_data.py
+-rw-r--r--   0        0        0       19 2024-03-25 20:51:35.300593 fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/personal_data.py
+-rw-r--r--   0        0        0       21 2024-05-02 18:33:40.324597 fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/return_types/__init__.py
+-rw-r--r--   0        0        0     3445 2024-03-25 20:51:35.299069 fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/return_types/orders.py
+-rw-r--r--   0        0        0     3225 2024-03-25 20:51:35.300732 fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/sign_message.py
+-rw-r--r--   0        0        0     2079 2024-03-25 20:51:35.300861 fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/types.py
+-rw-r--r--   0        0        0     1772 2024-03-25 20:51:35.300993 fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/utils.py
+-rw-r--r--   0        0        0   120332 2024-03-25 20:51:35.299642 fibrous_limit_order-0.1.5/fibrous_limit_order/src/tokens.json
+-rw-r--r--   0        0        0      449 2024-05-02 18:39:24.033412 fibrous_limit_order-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 fibrous_limit_order-0.1.5/PKG-INFO
```

### Comparing `fibrous_limit_order-0.1.4/LICENCE` & `fibrous_limit_order-0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/README.md` & `fibrous_limit_order-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/cancel_order.py` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/cancel_order.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/full_create_order.py` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/full_create_order.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/full_fill_order.py` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/full_fill_order.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/get_nonce.py` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/get_nonce.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/get_orders.py` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/get_orders.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import sys
 import os
 
 
 import asyncio
 import aiohttp
 
-from fibrous_limit_order.src.limit_order import LimitOrder
+from fibrous_limit_order import *
+
 # from fibrous_limit_order.src.return_types import GetOrdersResponse, OrdersFilter
 # from limit_order import utils
 
 # async def get_orders() -> GetOrdersResponse:
 #     limit_order = LimitOrder()
 #     filters: OrdersFilter = {
 #         'wallet_address': '',
```

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/get_remaining_amount.py` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/get_remaining_amount.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/place_order.py` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/place_order.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/examples/sign_message.py` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/examples/sign_message.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/limit_order/limit_order.py` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/limit_order.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/limit_order/mock_data.py` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/mock_data.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/limit_order/sign_message.py` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/sign_message.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/limit_order/types.py` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/types.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/limit_order/utils.py` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/utils.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/return_types/orders.py` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/limit_order/return_types/orders.py`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/fibrous_limit_order/src/tokens.json` & `fibrous_limit_order-0.1.5/fibrous_limit_order/src/tokens.json`

 * *Files identical despite different names*

### Comparing `fibrous_limit_order-0.1.4/PKG-INFO` & `fibrous_limit_order-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fibrous_limit_order
-Version: 0.1.4
+Version: 0.1.5
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
-Metadata-Version: 2.1 Name: fibrous_limit_order Version: 0.1.4 Summary: A
+Metadata-Version: 2.1 Name: fibrous_limit_order Version: 0.1.5 Summary: A
 Python SDK for Fibrous Finance Limit Order License: MIT Author: zeroonesymphony
 Author-email: kermo@fibrous.finance Requires-Python: >=3.9,<3.13 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Description-
 Content-Type: text/markdown
```

