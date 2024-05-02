# Comparing `tmp/wrapper_b2p-0.1.0.tar.gz` & `tmp/wrapper_b2p-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrapper_b2p-0.1.0.tar", max compression
+gzip compressed data, was "wrapper_b2p-0.2.0.tar", max compression
```

## Comparing `wrapper_b2p-0.1.0.tar` & `wrapper_b2p-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0     1075 2021-10-11 02:46:08.789790 wrapper_b2p-0.1.0/LICENSE.rst
--rw-r--r--   0        0        0      472 2021-10-11 05:08:52.528325 wrapper_b2p-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      729 2022-01-14 05:58:04.392943 wrapper_b2p-0.1.0/src/wrapper_b2p/__init__.py
--rw-r--r--   0        0        0       38 2021-10-06 04:26:55.418313 wrapper_b2p-0.1.0/src/wrapper_b2p/constant.py
--rw-r--r--   0        0        0      597 2021-10-10 03:01:48.018813 wrapper_b2p-0.1.0/src/wrapper_b2p/exception.py
--rw-r--r--   0        0        0      103 2021-10-06 04:55:10.860337 wrapper_b2p-0.1.0/src/wrapper_b2p/settings.py
--rw-r--r--   0        0        0        0 2021-10-05 03:36:40.936746 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/__init__.py
--rw-r--r--   0        0        0      750 2022-01-14 05:58:04.396943 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/authorize.py
--rw-r--r--   0        0        0      133 2022-01-14 05:58:04.396943 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/authorize_by_token.py
--rw-r--r--   0        0        0     1213 2021-10-11 05:22:30.542808 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/authorize_inc.py
--rw-r--r--   0        0        0      163 2021-10-10 13:53:02.198665 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/class_abs/__init__.py
--rw-r--r--   0        0        0      253 2021-10-11 05:23:01.239272 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/class_abs/b2p_abc.py
--rw-r--r--   0        0        0      770 2022-01-14 05:58:04.396943 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/class_abs/redirect_b2p_abc.py
--rw-r--r--   0        0        0      139 2021-10-10 13:49:17.402108 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/class_abs/request_b2p_abc.py
--rw-r--r--   0        0        0     1017 2021-10-11 05:22:30.558808 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/complete.py
--rw-r--r--   0        0        0      194 2021-10-10 05:26:27.520988 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/mixin/__init__.py
--rw-r--r--   0        0        0      506 2021-10-10 05:26:27.528987 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/mixin/create_signature.py
--rw-r--r--   0        0        0      230 2021-10-11 05:22:30.594809 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/mixin/get_url_stand_b2p.py
--rw-r--r--   0        0        0     1117 2021-10-11 05:22:30.598809 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/mixin/request_post_b2p.py
--rw-r--r--   0        0        0      947 2021-10-11 05:20:33.812895 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/operation.py
--rw-r--r--   0        0        0     1694 2021-10-11 05:22:30.570809 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/order.py
--rw-r--r--   0        0        0      747 2022-01-14 05:58:04.396943 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/purchase.py
--rw-r--r--   0        0        0      897 2022-01-14 05:58:04.396943 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/purchase_by_token.py
--rw-r--r--   0        0        0     1022 2021-10-11 05:22:30.578809 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/register.py
--rw-r--r--   0        0        0      997 2021-10-11 05:22:30.586809 wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/reverse.py
--rw-r--r--   0        0        0      832 2022-01-14 06:16:23.962053 wrapper_b2p-0.1.0/setup.py
--rw-r--r--   0        0        0      488 2022-01-14 06:16:23.962440 wrapper_b2p-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2021-10-11 02:46:08.789790 wrapper_b2p-0.2.0/LICENSE.rst
+-rw-r--r--   0        0        0      472 2024-05-02 08:46:42.143001 wrapper_b2p-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      729 2024-05-02 08:10:22.479031 wrapper_b2p-0.2.0/src/wrapper_b2p/__init__.py
+-rw-r--r--   0        0        0       38 2021-10-06 04:26:55.418313 wrapper_b2p-0.2.0/src/wrapper_b2p/constant.py
+-rw-r--r--   0        0        0      597 2021-10-10 03:01:48.018813 wrapper_b2p-0.2.0/src/wrapper_b2p/exception.py
+-rw-r--r--   0        0        0      103 2021-10-06 04:55:10.860337 wrapper_b2p-0.2.0/src/wrapper_b2p/settings.py
+-rw-r--r--   0        0        0        0 2021-10-05 03:36:40.936746 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/__init__.py
+-rw-r--r--   0        0        0      778 2024-05-02 08:10:04.399031 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/authorize.py
+-rw-r--r--   0        0        0      133 2022-01-14 05:58:04.396943 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/authorize_by_token.py
+-rw-r--r--   0        0        0     1241 2024-05-02 08:10:04.399031 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/authorize_inc.py
+-rw-r--r--   0        0        0      163 2021-10-10 13:53:02.198665 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/class_abs/__init__.py
+-rw-r--r--   0        0        0      253 2021-10-11 05:23:01.239272 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/class_abs/b2p_abc.py
+-rw-r--r--   0        0        0      770 2022-01-14 05:58:04.396943 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/class_abs/redirect_b2p_abc.py
+-rw-r--r--   0        0        0      139 2021-10-10 13:49:17.402108 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/class_abs/request_b2p_abc.py
+-rw-r--r--   0        0        0     1045 2024-05-02 08:10:04.399031 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/complete.py
+-rw-r--r--   0        0        0      194 2021-10-10 05:26:27.520988 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/mixin/__init__.py
+-rw-r--r--   0        0        0      506 2021-10-10 05:26:27.528987 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/mixin/create_signature.py
+-rw-r--r--   0        0        0      312 2024-05-02 08:10:04.399031 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/mixin/get_url_stand_b2p.py
+-rw-r--r--   0        0        0     1147 2024-05-02 08:10:04.403031 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/mixin/request_post_b2p.py
+-rw-r--r--   0        0        0      975 2024-05-02 08:10:04.403031 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/operation.py
+-rw-r--r--   0        0        0     1722 2024-05-02 08:10:04.403031 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/order.py
+-rw-r--r--   0        0        0      775 2024-05-02 08:10:04.403031 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/purchase.py
+-rw-r--r--   0        0        0      925 2024-05-02 08:10:04.403031 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/purchase_by_token.py
+-rw-r--r--   0        0        0     1050 2024-05-02 08:10:04.403031 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/register.py
+-rw-r--r--   0        0        0     1025 2024-05-02 08:10:04.403031 wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/reverse.py
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 wrapper_b2p-0.2.0/PKG-INFO
```

### Comparing `wrapper_b2p-0.1.0/LICENSE.rst` & `wrapper_b2p-0.2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `wrapper_b2p-0.1.0/src/wrapper_b2p/__init__.py` & `wrapper_b2p-0.2.0/src/wrapper_b2p/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.0'
+__version__ = '0.2.0'
 
 from .wrapper_class.authorize import Authorize  # noqa: F401
 from .wrapper_class.authorize_by_token import AuthorizeByToken  # noqa: F401
 from .wrapper_class.authorize_by_token import AuthorizeByToken  # noqa: F401
 from .wrapper_class.authorize_inc import AuthorizeInc  # noqa: F401
 from .wrapper_class.complete import Complete  # noqa: F401
 from .wrapper_class.operation import Operation  # noqa: F401
```

### Comparing `wrapper_b2p-0.1.0/src/wrapper_b2p/exception.py` & `wrapper_b2p-0.2.0/src/wrapper_b2p/exception.py`

 * *Files identical despite different names*

### Comparing `wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/authorize.py` & `wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/purchase.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Union, Optional, Any
+from typing import Optional, Any, Union
 
 from .class_abs import RedirectB2PABC
 
 
-class Authorize(RedirectB2PABC):
-    path_to_point_api = 'Authorize'
-
+class Purchase(RedirectB2PABC):
+    path_to_point_api = 'Purchase'
     allowed_field_with_default_value_to_b2p = {
         'get_token': 0,
         'token': False,
         'payer_id': False,
         'save_card': False,
-        'is_prod_stand': False
+        'is_prod_stand': False,
+        'stand_url': None,
     }
 
     def __init__(self, sector: str, id_: Union[str, int], b2p_token: str, **kwargs: Optional[Any]):
         self.sector = sector
         self.id = id_
         self.b2p_token = b2p_token
         for item in self.allowed_field_with_default_value_to_b2p:
```

### Comparing `wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/authorize_inc.py` & `wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/complete.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from typing import Union, Optional, Any
 
 from ..constant import RUB
 from .class_abs import RequestB2PABC
 
 
-class AuthorizeInc(RequestB2PABC):
-    path_to_point_api = 'AuthorizeInc'
+class Complete(RequestB2PABC):
+    path_to_point_api = 'Complete'
     allowed_field_with_default_value_to_b2p = {
         'fee': 0,
-        'is_prod_stand': False
+        'is_prod_stand': False,
+        'stand_url': None,
     }
 
-    def __init__(self, sector: int, id_: Union[str, int], amount: int, b2p_token: str,
+    def __init__(self, sector: Union[int, str], id_: Union[str, int], amount: int, b2p_token: str,
                  currency: str = RUB, **kwargs: Optional[Any]):
         self.sector = sector
         self.id = id_
         self.amount = amount
         self.currency = currency
         self.b2p_token = b2p_token
         for item in self.allowed_field_with_default_value_to_b2p:
             setattr(self, item, kwargs.get(item) or self.allowed_field_with_default_value_to_b2p.get(item))
         self.signature = self._create_signature()
 
-    def do(self) -> dict:
+    def do(self):
         return self._request_best2pay()
 
     def _get_raw_signature(self) -> str:
-        if hasattr(self, 'fee') and self.fee:
-            return (str(self.sector) + str(self.id) + str(self.amount) +
-                    str(self.fee) + str(self.currency) + self.b2p_token)
         return str(self.sector) + str(self.id) + str(self.amount) + str(self.currency) + self.b2p_token
```

### Comparing `wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/class_abs/redirect_b2p_abc.py` & `wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/class_abs/redirect_b2p_abc.py`

 * *Files identical despite different names*

### Comparing `wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/complete.py` & `wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/reverse.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Union, Optional, Any
 
 from ..constant import RUB
 from .class_abs import RequestB2PABC
 
 
-class Complete(RequestB2PABC):
-    path_to_point_api = 'Complete'
+class Reverse(RequestB2PABC):
+    path_to_point_api = 'Reverse'
     allowed_field_with_default_value_to_b2p = {
-        'fee': 0,
-        'is_prod_stand': False
+        'is_prod_stand': False,
+        'stand_url': None,
     }
 
     def __init__(self, sector: Union[int, str], id_: Union[str, int], amount: int, b2p_token: str,
                  currency: str = RUB, **kwargs: Optional[Any]):
         self.sector = sector
         self.id = id_
         self.amount = amount
```

### Comparing `wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/mixin/request_post_b2p.py` & `wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/mixin/request_post_b2p.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,8 +29,9 @@
         res_dict = xmltodict.parse(text, process_namespaces=True)
         return res_dict
 
     def _get_date_by_send_b2p(self) -> dict:
         data = copy(self.__dict__)
         data.pop('is_prod_stand')
         data.pop('b2p_token')
+        data.pop('stand_url')
         return data
```

### Comparing `wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/operation.py` & `wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/purchase_by_token.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import Union, Any, Optional
+from typing import Union, Optional, Any
 
 from .class_abs import RequestB2PABC
 
 
-class Operation(RequestB2PABC):
-    path_to_point_api = 'Operation'
+class PurchaseByToken(RequestB2PABC):
+    path_to_point_api = 'PurchaseByToken'
     allowed_field_with_default_value_to_b2p = {
-        'get_token': 0,
-        'is_prod_stand': False
+        'cvc': '',
+        'is_prod_stand': False,
+        'stand_url': None,
     }
 
-    def __init__(self, sector: Union[int, str], id_: Union[str, int], operation: Union[int, str], b2p_token: str,
-                 **kwargs: Optional[Any]):
+    def __init__(self, sector: str, id_: Union[str, int], token: str, b2p_token: str, **kwargs: Optional[Any]):
         self.sector = sector
         self.id = id_
-        self.operation = operation
+        self.token = token
         self.b2p_token = b2p_token
         for item in self.allowed_field_with_default_value_to_b2p:
             setattr(self, item, kwargs.get(item) or self.allowed_field_with_default_value_to_b2p.get(item))
         self.signature = self._create_signature()
 
+    def _get_raw_signature(self) -> str:
+        return str(self.sector) + str(self.id) + str(self.token) + self.b2p_token
+
     def do(self):
         return self._request_best2pay()
-
-    def _get_raw_signature(self) -> str:
-        return str(self.sector) + str(self.id) + str(self.operation) + self.b2p_token
```

### Comparing `wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/order.py` & `wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/order.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import base64
 import hashlib
 from typing import Union, Optional, Any
 
-from ..exception import ErrorDefined
 from .class_abs import RequestB2PABC
+from ..exception import ErrorDefined
 
 
 class Order(RequestB2PABC):
     path_to_point_api = 'Order'
     allowed_field_with_default_value_to_b2p = {
         'mode': 0,
         'get_token': 0,
-        'is_prod_stand': False
+        'is_prod_stand': False,
+        'stand_url': None,
     }
 
     def __init__(self, sector: Union[str, int], b2p_token: str, id_: Union[str, int] = None,
                  reference: Union[str, int] = None, **kwargs: Optional[Any]):
         self.sector = sector
         self.id = id_
         self.reference = reference
```

### Comparing `wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/purchase.py` & `wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/authorize.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from typing import Optional, Any, Union
+from typing import Union, Optional, Any
 
 from .class_abs import RedirectB2PABC
 
 
-class Purchase(RedirectB2PABC):
-    path_to_point_api = 'Purchase'
+class Authorize(RedirectB2PABC):
+    path_to_point_api = 'Authorize'
+
     allowed_field_with_default_value_to_b2p = {
         'get_token': 0,
         'token': False,
         'payer_id': False,
         'save_card': False,
-        'is_prod_stand': False
+        'is_prod_stand': False,
+        'stand_url': None,
     }
 
     def __init__(self, sector: str, id_: Union[str, int], b2p_token: str, **kwargs: Optional[Any]):
         self.sector = sector
         self.id = id_
         self.b2p_token = b2p_token
         for item in self.allowed_field_with_default_value_to_b2p:
```

### Comparing `wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/register.py` & `wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/register.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     path_to_point_api = 'Register'
     allowed_field_with_default_value_to_b2p = {
         'fee': 0,
         'url': '',
         'failurl': '',
         'currency': RUB,
         'lang': 'RU',
-        'is_prod_stand': False
+        'is_prod_stand': False,
+        'stand_url': None,
     }
 
     def __init__(self, sector: str, amount: int, description: str, b2p_token: str, **kwargs: Optional[Any]):
         self.sector = sector
         self.amount = amount
         self.description = description
         self.b2p_token = b2p_token
```

### Comparing `wrapper_b2p-0.1.0/src/wrapper_b2p/wrapper_class/reverse.py` & `wrapper_b2p-0.2.0/src/wrapper_b2p/wrapper_class/authorize_inc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from typing import Union, Optional, Any
 
 from ..constant import RUB
 from .class_abs import RequestB2PABC
 
 
-class Reverse(RequestB2PABC):
-    path_to_point_api = 'Reverse'
+class AuthorizeInc(RequestB2PABC):
+    path_to_point_api = 'AuthorizeInc'
     allowed_field_with_default_value_to_b2p = {
-        'is_prod_stand': False
+        'fee': 0,
+        'is_prod_stand': False,
+        'stand_url': None,
     }
 
-    def __init__(self, sector: Union[int, str], id_: Union[str, int], amount: int, b2p_token: str,
+    def __init__(self, sector: int, id_: Union[str, int], amount: int, b2p_token: str,
                  currency: str = RUB, **kwargs: Optional[Any]):
         self.sector = sector
         self.id = id_
         self.amount = amount
         self.currency = currency
         self.b2p_token = b2p_token
         for item in self.allowed_field_with_default_value_to_b2p:
             setattr(self, item, kwargs.get(item) or self.allowed_field_with_default_value_to_b2p.get(item))
         self.signature = self._create_signature()
 
-    def do(self):
+    def do(self) -> dict:
         return self._request_best2pay()
 
     def _get_raw_signature(self) -> str:
+        if hasattr(self, 'fee') and self.fee:
+            return (str(self.sector) + str(self.id) + str(self.amount) +
+                    str(self.fee) + str(self.currency) + self.b2p_token)
         return str(self.sector) + str(self.id) + str(self.amount) + str(self.currency) + self.b2p_token
```

