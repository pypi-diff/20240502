# Comparing `tmp/parcllabs-0.1.8.tar.gz` & `tmp/parcllabs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parcllabs-0.1.8.tar", last modified: Mon Apr 29 00:09:16 2024, max compression
+gzip compressed data, was "parcllabs-0.1.9.tar", last modified: Wed May  1 11:35:03 2024, max compression
```

## Comparing `parcllabs-0.1.8.tar` & `parcllabs-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 00:09:16.425693 parcllabs-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 00:08:33.000000 parcllabs-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-29 00:09:16.425693 parcllabs-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-29 00:08:33.000000 parcllabs-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 00:09:16.417693 parcllabs-0.1.8/parcllabs/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-29 00:09:12.000000 parcllabs-0.1.8/parcllabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-29 00:09:13.000000 parcllabs-0.1.8/parcllabs/plabs_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 00:09:16.421693 parcllabs-0.1.8/parcllabs/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/search/metros.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/search/top_markets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 00:09:16.421693 parcllabs-0.1.8/parcllabs/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-29 00:09:13.000000 parcllabs-0.1.8/parcllabs/services/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/services/for_sale_market_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/services/investor_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/services/market_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/services/portfolio_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/services/rental_market_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-29 00:09:13.000000 parcllabs-0.1.8/parcllabs/services/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 00:09:16.421693 parcllabs-0.1.8/parcllabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-29 00:09:16.000000 parcllabs-0.1.8/parcllabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-29 00:09:16.000000 parcllabs-0.1.8/parcllabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 00:09:16.000000 parcllabs-0.1.8/parcllabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-29 00:09:16.000000 parcllabs-0.1.8/parcllabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 00:09:16.000000 parcllabs-0.1.8/parcllabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 00:09:16.425693 parcllabs-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-29 00:08:33.000000 parcllabs-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 00:09:16.421693 parcllabs-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-29 00:08:33.000000 parcllabs-0.1.8/tests/test_for_sale_market_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-29 00:08:33.000000 parcllabs-0.1.8/tests/test_parcl_labs_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-29 00:08:33.000000 parcllabs-0.1.8/tests/test_parcl_labs_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:03.201737 parcllabs-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 11:34:28.000000 parcllabs-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-01 11:35:03.201737 parcllabs-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-05-01 11:34:28.000000 parcllabs-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:03.197737 parcllabs-0.1.9/parcllabs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/plabs_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:03.197737 parcllabs-0.1.9/parcllabs/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/search/metros.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/search/top_markets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:03.201737 parcllabs-0.1.9/parcllabs/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-01 11:35:00.000000 parcllabs-0.1.9/parcllabs/services/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/services/for_sale_market_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/services/investor_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/services/market_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/services/portfolio_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/services/rental_market_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-01 11:34:28.000000 parcllabs-0.1.9/parcllabs/services/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:03.201737 parcllabs-0.1.9/parcllabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-01 11:35:03.000000 parcllabs-0.1.9/parcllabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-01 11:35:03.000000 parcllabs-0.1.9/parcllabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 11:35:03.000000 parcllabs-0.1.9/parcllabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-01 11:35:03.000000 parcllabs-0.1.9/parcllabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 11:35:03.000000 parcllabs-0.1.9/parcllabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 11:35:03.201737 parcllabs-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-01 11:34:28.000000 parcllabs-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 11:35:03.201737 parcllabs-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-01 11:34:28.000000 parcllabs-0.1.9/tests/test_for_sale_market_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-01 11:34:28.000000 parcllabs-0.1.9/tests/test_parcl_labs_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 11:34:28.000000 parcllabs-0.1.9/tests/test_parcl_labs_service.py
```

### Comparing `parcllabs-0.1.8/LICENSE` & `parcllabs-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.8/PKG-INFO` & `parcllabs-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parcllabs
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SDK for ParclLabs API
 Home-page: https://github.com/ParclLabs/parcllabs-python
 Author: ParclLabs
 Author-email: team@parcllabs.com
 Keywords: parcllabs api real estate analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `parcllabs-0.1.8/README.md` & `parcllabs-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 ![Logo](img/labs.jpg)
 # parcllabs-python
 
 ## Sign Up for an API Key
 
 To use the Parcl Labs API, you need an API key. To get an API key, sign up at [ParclLabs](https://dashboard.parcllabs.com/signup).
 
+## Examples
+
+We maintain a repository of examples that demonstrate how to use the Parcl Labs API for analysis. You can find the examples in the [ParclLabs Examples](https://github.com/parcllabs/parcllabs-examples)
+
 ## Installation
 
 You can install the package via pip:
 
 ```bash
 pip install parcllabs
 ```
```

### Comparing `parcllabs-0.1.8/parcllabs/__init__.py` & `parcllabs-0.1.9/parcllabs/__init__.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.8/parcllabs/plabs_client.py` & `parcllabs-0.1.9/parcllabs/plabs_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+import json
 import requests
-from typing import Dict, Union
+from typing import Dict
 from requests.exceptions import RequestException
 
-import pandas as pd
-
 from parcllabs import api_base
 
 from parcllabs.services.investor_metrics import (
     InvestorMetricsHousingStockOwnership,
     InvesetorMetricsNewListingsForSaleRollingCounts,
     InvestorMetricsPurchaseToSaleRatio,
     InvestorMetricsHousingEventCounts,
@@ -31,15 +30,17 @@
 from parcllabs.services.portfolio_metrics import PortfolioMetricsSFHousingStockOwnership
 from parcllabs.services.search import SearchMarkets
 
 
 class ParclLabsClient:
     def __init__(self, api_key: str):
         if api_key is None:
-            raise ValueError("api_key is required")
+            raise ValueError(
+                "API Key is required. Please visit https://dashboard.parcllabs.com/signup to get an API key."
+            )
         self.api_key = api_key
         self.api_url = api_base
 
         # top-level services: The client is responsible for creating instances of these services
         self.investor_metrics_housing_stock_ownership = (
             InvestorMetricsHousingStockOwnership(client=self)
         )
@@ -81,21 +82,35 @@
             url (str): The URL endpoint to request.
             params (dict, optional): The parameters to send in the query string.
 
         Returns:
             dict: The JSON response as a dictionary.
         """
         try:
-            url = self.api_url + url
+            full_url = self.api_url + url
             headers = self._get_headers()
-            response = requests.get(url, headers=headers, params=params)
-            response.raise_for_status()  # Raises a HTTPError for bad responses
+            response = requests.get(full_url, headers=headers, params=params)
+            response.raise_for_status()
             return response.json()
-        except RequestException as e:
-            print(f"Request failed: {e}")
-            return None
+        except requests.exceptions.HTTPError:
+            try:
+                error_details = response.json()
+                error_message = error_details.get("detail", "No detail provided by API")
+            except json.JSONDecodeError:
+                error_message = "Failed to decode JSON error response"
+            type_of_error = ""
+            if 400 <= response.status_code < 500:
+                type_of_error = "Client"
+            elif 500 <= response.status_code < 600:
+                type_of_error = "Server"
+            msg = f"{response.status_code} {type_of_error} Error: {error_message}. Visit https://dashboard.parcllabs.com for more information or reach out to team@parcllabs.com."
+            raise RequestException(msg)
+        except requests.exceptions.RequestException as err:
+            raise RequestException(f"Request failed: {str(err)}")
+        except Exception as e:
+            raise RequestException(f"An unexpected error occurred: {str(e)}")
 
     def _get_headers(self) -> Dict[str, str]:
         return {
             "Authorization": f"{self.api_key}",
             "Content-Type": "application/json",
         }
```

### Comparing `parcllabs-0.1.8/parcllabs/search/metros.py` & `parcllabs-0.1.9/parcllabs/search/metros.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.8/parcllabs/services/base_service.py` & `parcllabs-0.1.9/parcllabs/services/base_service.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.8/parcllabs/services/for_sale_market_metrics.py` & `parcllabs-0.1.9/parcllabs/services/for_sale_market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.8/parcllabs/services/investor_metrics.py` & `parcllabs-0.1.9/parcllabs/services/investor_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.8/parcllabs/services/market_metrics.py` & `parcllabs-0.1.9/parcllabs/services/market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.8/parcllabs/services/portfolio_metrics.py` & `parcllabs-0.1.9/parcllabs/services/portfolio_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.8/parcllabs/services/rental_market_metrics.py` & `parcllabs-0.1.9/parcllabs/services/rental_market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.8/parcllabs/services/search.py` & `parcllabs-0.1.9/parcllabs/services/search.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.8/parcllabs.egg-info/PKG-INFO` & `parcllabs-0.1.9/parcllabs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parcllabs
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SDK for ParclLabs API
 Home-page: https://github.com/ParclLabs/parcllabs-python
 Author: ParclLabs
 Author-email: team@parcllabs.com
 Keywords: parcllabs api real estate analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `parcllabs-0.1.8/parcllabs.egg-info/SOURCES.txt` & `parcllabs-0.1.9/parcllabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.8/setup.py` & `parcllabs-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.8/tests/test_for_sale_market_metrics.py` & `parcllabs-0.1.9/tests/test_for_sale_market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.8/tests/test_parcl_labs_clients.py` & `parcllabs-0.1.9/tests/test_parcl_labs_clients.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 import requests
+from requests.exceptions import RequestException
 import requests_mock
 from parcllabs import ParclLabsClient
 
 
 def test_initialization(api_key):
     client = ParclLabsClient(api_key)
     assert client.api_key == api_key
@@ -20,20 +21,28 @@
         client.api_url = "https://example.com/api"
         response = client.get("/data")
         assert response == {"data": "value"}
 
 
 def test_get_with_failed_request(client):
     with requests_mock.Mocker() as m:
-        m.get("https://example.com/api/data", status_code=400)
+        m.get(
+            "https://example.com/api/data",
+            status_code=400,
+            json={"detail": "Client Error"},
+        )
         client.api_url = "https://example.com/api"
-        response = client.get("/data")
-        assert (
-            response is None
-        )  # Since we're returning None on exception in the client code
+
+        # Use pytest.raises to check for the RequestException
+        with pytest.raises(RequestException) as excinfo:
+            response = client.get("/data")
+
+        # Assert that the exception message contains '400 Client Error'
+        assert "400 Client Error" in str(excinfo.value)
+        assert "Client Error" in str(excinfo.value)
 
 
 def test_get_headers(client):
     with requests_mock.Mocker() as m:
         m.get(
             "https://example.com/api/data",
             json={},
@@ -45,24 +54,14 @@
         client.api_url = "https://example.com/api"
         client.get("/data")
         history = m.request_history[0]
         assert history.headers["Authorization"] == "fake_api_key"
         assert history.headers["Content-Type"] == "application/json"
 
 
-def test_get_request_exception(client, capsys):
-    with requests_mock.Mocker() as m:
-        m.get("https://example.com/api/data", exc=requests.exceptions.ConnectTimeout)
-        client.api_url = "https://example.com/api"
-        response = client.get("/data")
-        assert response is None
-        captured = capsys.readouterr()
-        assert "Request failed:" in captured.out
-
-
 def test_service_initialization(client):
     assert client.investor_metrics_housing_stock_ownership.client is client
     assert client.investor_metrics_new_listings_for_sale_rolling_counts.client is client
     assert client.investor_metrics_purchase_to_sale_ratio.client is client
     assert client.investor_metrics_housing_event_counts.client is client
     assert client.market_metrics_housing_event_prices.client is client
     assert client.market_metrics_housing_stock.client is client
```

### Comparing `parcllabs-0.1.8/tests/test_parcl_labs_service.py` & `parcllabs-0.1.9/tests/test_parcl_labs_service.py`

 * *Files identical despite different names*

