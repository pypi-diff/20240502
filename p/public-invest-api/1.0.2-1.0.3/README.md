# Comparing `tmp/public_invest_api-1.0.2.tar.gz` & `tmp/public_invest_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "public_invest_api-1.0.2.tar", last modified: Sat Mar 23 16:55:57 2024, max compression
+gzip compressed data, was "public_invest_api-1.0.3.tar", last modified: Wed May  1 23:45:35 2024, max compression
```

## Comparing `public_invest_api-1.0.2.tar` & `public_invest_api-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:55:57.566690 public_invest_api-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-03-23 16:55:57.566690 public_invest_api-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-03-23 16:55:53.000000 public_invest_api-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:55:57.562690 public_invest_api-1.0.2/public_invest_api/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-23 16:55:53.000000 public_invest_api-1.0.2/public_invest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-03-23 16:55:53.000000 public_invest_api-1.0.2/public_invest_api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-03-23 16:55:53.000000 public_invest_api-1.0.2/public_invest_api/public.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 16:55:57.562690 public_invest_api-1.0.2/public_invest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-03-23 16:55:57.000000 public_invest_api-1.0.2/public_invest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-23 16:55:57.000000 public_invest_api-1.0.2/public_invest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 16:55:57.000000 public_invest_api-1.0.2/public_invest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-23 16:55:57.000000 public_invest_api-1.0.2/public_invest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-23 16:55:57.000000 public_invest_api-1.0.2/public_invest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 16:55:57.566690 public_invest_api-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-23 16:55:53.000000 public_invest_api-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:45:35.374617 public_invest_api-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-01 23:45:35.374617 public_invest_api-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-01 23:45:31.000000 public_invest_api-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:45:35.374617 public_invest_api-1.0.3/public_invest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-01 23:45:31.000000 public_invest_api-1.0.3/public_invest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-01 23:45:31.000000 public_invest_api-1.0.3/public_invest_api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-01 23:45:31.000000 public_invest_api-1.0.3/public_invest_api/public.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:45:35.374617 public_invest_api-1.0.3/public_invest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-01 23:45:35.000000 public_invest_api-1.0.3/public_invest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-01 23:45:35.000000 public_invest_api-1.0.3/public_invest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 23:45:35.000000 public_invest_api-1.0.3/public_invest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 23:45:35.000000 public_invest_api-1.0.3/public_invest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 23:45:35.000000 public_invest_api-1.0.3/public_invest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 23:45:35.374617 public_invest_api-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-01 23:45:31.000000 public_invest_api-1.0.3/setup.py
```

### Comparing `public_invest_api-1.0.2/PKG-INFO` & `public_invest_api-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: public_invest_api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Unofficial Public.com Invest API written in Python Requests
 Home-page: https://github.com/NelsonDane/public-invest-api
 Author: Nelson Dane
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: python-dotenv
 
@@ -24,15 +24,15 @@
 
 ```python
 from public_invest_api import Public
 
 public = Public()
 public.login(
     username='your_email',
-    password='your_password'
+    password='your_password',
     wait_for_2fa=True # When logging in for the first time, you need to wait for the SMS code
 )
 ```
 
 If you'd like to handle the 2FA code yourself, set `wait_for_2fa=False` and it will throw an Exception relating to 2FA. Catch this, then when you get the 2FA code, call it again with the code:
 
 ```python
@@ -48,24 +48,25 @@
 
 ```python
 positions = public.get_positions()
 for position in positions:
     print(position)
 ```
 
-## Place Order
+## Usage: Placing Orders
 
 ```python
 order = public.place_order(
     symbol='AAPL',
     quantity=1,
     side='BUY', # or 'SELL'
     order_type='MARKET', # or 'LIMIT' or 'STOP'
-    time_in_force='DAY' # or 'GTC' or 'IOC' or 'FOK'
-    is_dry_run=False # If True, it will not actually place the order
+    limit_price=None # pass float if using 'LIMIT' order_type
+    time_in_force='DAY', # or 'GTC' or 'IOC' or 'FOK'
+    is_dry_run=False, # If True, it will not actually place the order
     tip=0 # The amount to tip Public.com
 )
 print(order)
 ```
 
 ## Contributing
 Found or fixed a bug? Have a feature request? Feel free to open an issue or pull request!
```

### Comparing `public_invest_api-1.0.2/README.md` & `public_invest_api-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ```python
 from public_invest_api import Public
 
 public = Public()
 public.login(
     username='your_email',
-    password='your_password'
+    password='your_password',
     wait_for_2fa=True # When logging in for the first time, you need to wait for the SMS code
 )
 ```
 
 If you'd like to handle the 2FA code yourself, set `wait_for_2fa=False` and it will throw an Exception relating to 2FA. Catch this, then when you get the 2FA code, call it again with the code:
 
 ```python
@@ -38,24 +38,25 @@
 
 ```python
 positions = public.get_positions()
 for position in positions:
     print(position)
 ```
 
-## Place Order
+## Usage: Placing Orders
 
 ```python
 order = public.place_order(
     symbol='AAPL',
     quantity=1,
     side='BUY', # or 'SELL'
     order_type='MARKET', # or 'LIMIT' or 'STOP'
-    time_in_force='DAY' # or 'GTC' or 'IOC' or 'FOK'
-    is_dry_run=False # If True, it will not actually place the order
+    limit_price=None # pass float if using 'LIMIT' order_type
+    time_in_force='DAY', # or 'GTC' or 'IOC' or 'FOK'
+    is_dry_run=False, # If True, it will not actually place the order
     tip=0 # The amount to tip Public.com
 )
 print(order)
 ```
 
 ## Contributing
 Found or fixed a bug? Have a feature request? Feel free to open an issue or pull request!
@@ -63,8 +64,8 @@
 Enjoying the project? Feel free to Sponsor me on GitHub or Ko-fi!
 
 [![Sponsor](https://img.shields.io/badge/sponsor-30363D?style=for-the-badge&logo=GitHub-Sponsors&logoColor=#white)](https://github.com/sponsors/NelsonDane)
 [![ko-fi](https://img.shields.io/badge/Ko--fi-F16061?style=for-the-badge&logo=ko-fi&logoColor=white
 )](https://ko-fi.com/X8X6LFCI0)
 
 ## DISCLAIMER
-DISCLAIMER: I am not a financial advisor and not affiliated with Public.com. Use this tool at your own risk. I am not responsible for any losses or damages you may incur by using this project. This tool is provided as-is with no warranty.
+DISCLAIMER: I am not a financial advisor and not affiliated with Public.com. Use this tool at your own risk. I am not responsible for any losses or damages you may incur by using this project. This tool is provided as-is with no warranty.
```

### Comparing `public_invest_api-1.0.2/public_invest_api/endpoints.py` & `public_invest_api-1.0.3/public_invest_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `public_invest_api-1.0.2/public_invest_api/public.py` & `public_invest_api-1.0.3/public_invest_api/public.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,16 +132,15 @@
         headers = self.endpoints.build_headers(self.access_token)
         portfolio = self.session.get(
             self.endpoints.portfolio_url(self.account_uuid),
             headers=headers,
             timeout=self.timeout,
         )
         if portfolio.status_code != 200:
-            print("Portfolio request failed")
-            print(portfolio.text)
+            print(f"Portfolio request failed: {portfolio.text}")
             return None
         return portfolio.json()
 
     @login_required
     def get_account_number(self):
         return self.account_number
 
@@ -190,14 +189,15 @@
     def place_order(
         self,
         symbol,
         quantity,
         side,
         order_type,
         time_in_force,
+        limit_price=None,
         is_dry_run=False,
         tip=None,
     ):
         headers = self.endpoints.build_headers(self.access_token, prodApi=True)
         symbol = symbol.upper()
         time_in_force = time_in_force.upper()
         order_type = order_type.upper()
@@ -219,53 +219,53 @@
             "orderSide": side,
             "type": order_type,
             "timeInForce": time_in_force,
             "quote": quote,
             "quantity": quantity,
             "tipAmount": tip,
         }
+        if order_type == "LIMIT":
+            if limit_price is None:
+                raise Exception("Limit price required for limit orders")
+            payload["limitPrice"] = float(limit_price)
         # Preflight order endpoint
         preflight = self.session.post(
             self.endpoints.preflight_order_url(self.account_uuid),
             headers=headers,
             json=payload,
             timeout=self.timeout,
         )
         if preflight.status_code != 200:
-            print(preflight.text)
-            raise Exception("Preflight failed")
+            raise Exception(f"Preflight failed: {preflight.text}")
         preflight = preflight.json()
         # Build order endpoint
         build_response = self.session.post(
             self.endpoints.build_order_url(self.account_uuid),
             headers=headers,
             json=payload,
             timeout=self.timeout,
         )
         if build_response.status_code != 200:
-            print(build_response.text)
-            raise Exception("Build order failed")
+            raise Exception(f"Build order failed: {build_response.text}")
         build_response = build_response.json()
         if build_response.get("orderId") is None:
             raise Exception(f"No order ID: {build_response}")
         order_id = build_response["orderId"]
         # Submit order with put
         if not is_dry_run:
             submit_response = self.session.put(
                 self.endpoints.submit_put_order_url(self.account_uuid, order_id),
                 headers=headers,
                 timeout=self.timeout,
             )
             if submit_response.status_code != 200:
-                print(submit_response.text)
-                raise Exception("Submit order failed")
+                raise Exception(f"Submit order failed: {submit_response.text}")
             submit_response = submit_response.json()
             # Empty dict is success
             if submit_response != {}:
-                print(f"Submit response: {submit_response}")
                 raise Exception(f"Order failed: {submit_response}")
             sleep(1)
         # Check if order was rejected
         check_response = self.session.get(
             self.endpoints.submit_get_order_url(self.account_uuid, order_id),
             headers=headers,
             timeout=self.timeout,
```

### Comparing `public_invest_api-1.0.2/public_invest_api.egg-info/PKG-INFO` & `public_invest_api-1.0.3/public_invest_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: public_invest_api
-Version: 1.0.2
+Version: 1.0.3
 Summary: Unofficial Public.com Invest API written in Python Requests
 Home-page: https://github.com/NelsonDane/public-invest-api
 Author: Nelson Dane
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: python-dotenv
 
@@ -24,15 +24,15 @@
 
 ```python
 from public_invest_api import Public
 
 public = Public()
 public.login(
     username='your_email',
-    password='your_password'
+    password='your_password',
     wait_for_2fa=True # When logging in for the first time, you need to wait for the SMS code
 )
 ```
 
 If you'd like to handle the 2FA code yourself, set `wait_for_2fa=False` and it will throw an Exception relating to 2FA. Catch this, then when you get the 2FA code, call it again with the code:
 
 ```python
@@ -48,24 +48,25 @@
 
 ```python
 positions = public.get_positions()
 for position in positions:
     print(position)
 ```
 
-## Place Order
+## Usage: Placing Orders
 
 ```python
 order = public.place_order(
     symbol='AAPL',
     quantity=1,
     side='BUY', # or 'SELL'
     order_type='MARKET', # or 'LIMIT' or 'STOP'
-    time_in_force='DAY' # or 'GTC' or 'IOC' or 'FOK'
-    is_dry_run=False # If True, it will not actually place the order
+    limit_price=None # pass float if using 'LIMIT' order_type
+    time_in_force='DAY', # or 'GTC' or 'IOC' or 'FOK'
+    is_dry_run=False, # If True, it will not actually place the order
     tip=0 # The amount to tip Public.com
 )
 print(order)
 ```
 
 ## Contributing
 Found or fixed a bug? Have a feature request? Feel free to open an issue or pull request!
```

