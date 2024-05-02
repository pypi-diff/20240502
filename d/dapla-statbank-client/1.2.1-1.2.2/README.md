# Comparing `tmp/dapla_statbank_client-1.2.1.tar.gz` & `tmp/dapla_statbank_client-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_statbank_client-1.2.1.tar", max compression
+gzip compressed data, was "dapla_statbank_client-1.2.2.tar", max compression
```

## Comparing `dapla_statbank_client-1.2.1.tar` & `dapla_statbank_client-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2024-04-22 14:02:41.891219 dapla_statbank_client-1.2.1/LICENSE
--rw-r--r--   0        0        0    13494 2024-04-22 14:02:41.891219 dapla_statbank_client-1.2.1/README.md
--rw-r--r--   0        0        0     4224 2024-04-22 14:02:51.511252 dapla_statbank_client-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1581 2024-04-22 14:02:41.895219 dapla_statbank_client-1.2.1/src/statbank/__init__.py
--rw-r--r--   0        0        0     4105 2024-04-22 14:02:41.895219 dapla_statbank_client-1.2.1/src/statbank/api_types.py
--rw-r--r--   0        0        0     5776 2024-04-22 14:02:41.895219 dapla_statbank_client-1.2.1/src/statbank/apidata.py
--rw-r--r--   0        0        0     4007 2024-04-22 14:02:41.895219 dapla_statbank_client-1.2.1/src/statbank/auth.py
--rw-r--r--   0        0        0    18978 2024-04-22 14:02:41.895219 dapla_statbank_client-1.2.1/src/statbank/client.py
--rw-r--r--   0        0        0     1136 2024-04-22 14:02:41.895219 dapla_statbank_client-1.2.1/src/statbank/globals.py
--rw-r--r--   0        0        0        0 2024-04-22 14:02:41.895219 dapla_statbank_client-1.2.1/src/statbank/py.typed
--rw-r--r--   0        0        0     1304 2024-04-22 14:02:41.895219 dapla_statbank_client-1.2.1/src/statbank/statbank_logger.py
--rw-r--r--   0        0        0    14268 2024-04-22 14:02:41.895219 dapla_statbank_client-1.2.1/src/statbank/transfer.py
--rw-r--r--   0        0        0    17765 2024-04-22 14:02:51.511252 dapla_statbank_client-1.2.1/src/statbank/uttrekk.py
--rw-r--r--   0        0        0    26391 2024-04-22 14:02:41.895219 dapla_statbank_client-1.2.1/src/statbank/uttrekk_validations.py
--rw-r--r--   0        0        0    14882 1970-01-01 00:00:00.000000 dapla_statbank_client-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-02 11:59:16.170213 dapla_statbank_client-1.2.2/LICENSE
+-rw-r--r--   0        0        0    12373 2024-05-02 11:59:26.766121 dapla_statbank_client-1.2.2/README.md
+-rw-r--r--   0        0        0     4224 2024-05-02 11:59:26.770120 dapla_statbank_client-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1720 2024-05-02 11:59:26.770120 dapla_statbank_client-1.2.2/src/statbank/__init__.py
+-rw-r--r--   0        0        0     4105 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/api_types.py
+-rw-r--r--   0        0        0     7555 2024-05-02 11:59:26.770120 dapla_statbank_client-1.2.2/src/statbank/apidata.py
+-rw-r--r--   0        0        0     4007 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/auth.py
+-rw-r--r--   0        0        0    20311 2024-05-02 11:59:26.770120 dapla_statbank_client-1.2.2/src/statbank/client.py
+-rw-r--r--   0        0        0     1136 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/globals.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/py.typed
+-rw-r--r--   0        0        0     1304 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/statbank_logger.py
+-rw-r--r--   0        0        0    14268 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/transfer.py
+-rw-r--r--   0        0        0    17765 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/uttrekk.py
+-rw-r--r--   0        0        0    26391 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/uttrekk_validations.py
+-rw-r--r--   0        0        0    13761 1970-01-01 00:00:00.000000 dapla_statbank_client-1.2.2/PKG-INFO
```

### Comparing `dapla_statbank_client-1.2.1/LICENSE` & `dapla_statbank_client-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.1/README.md` & `dapla_statbank_client-1.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -122,14 +122,26 @@
 
 df_folkemengde = apidata("https://i.ssb.no/pxwebi/api/v0/no/prod_24v_intern/START/be/be01/folkemengde/Rd0002Aa",
                                      query,
                                      include_id = True
                                     )
 ```
 
+`apimetadata` gets metadata from the *public* api, like apidata does.
+```python
+meta = apimetadata("05300")
+```
+
+`apicodelist` gets a specific codelist out of the metadata, or all the codelists.
+```python
+all_codelists = apimetadata("05300")
+avstand_codelist = apimetadata("05300", "Avstand1")
+```
+
+
 `apidata_rotate` is a thin wrapper around pivot_table. Stolen from: https://github.com/sehyoun/SSB_API_helper/blob/master/src/ssb_api_helper.py
 ```python
 df_folkemengde_rotert = apidata_rotate(df_folkemengde, 'tidskolonne', "verdikolonne")
 ```
 
 
 ## Using a date-widget for publish day
@@ -169,30 +181,14 @@
 If you *dont* want to see the info-parts of the validate-method, you can change the loggers level before calling validate, like this:
 ```python
 import statbank
 import logging
 statbank.logger.setLevel(logging.WARNING)
 ```
 
-## Version history
-- 1.1.0 Migrating to "new template" for Pypi-packages at SSB, with full typing support, a reference website, logging instead of print etc.
-- 1.0.6 fixing new functionality on "IRkodelister"
-- 1.0.5 Making transferdata_template smarter, were it can take a bunch of dataframes and incorporate them in the returned dict. Trying to support columntype "internasjonal rapportering".
-- 1.0.4 Fixing bug where empty codelists stops description initialization, Updating pyjstat to 2.4.0, changing imports to absolute from package root
-- 1.0.2 Doc-string style cleanup, a check on username and password on client init, changes to time and display of time, demo notebooks cleaned
-- 1.0.0 Finished going through initial issues, less complaining from verify on floats
-- 0.0.11 Statbank people wanted a user-agent-requesst-header to differentiate test from prod
-- 0.0.9 After further user-testing and requests
-- 0.0.5 Still some parameter issues
-- 0.0.4 More test coverage, some bugs fixed in rounding checks and parameter-passing
-- 0.0.3 Removed batches, stripping uttrekk from transfer, rounding function on uttrekk, data required in as a dict of dataframes, with "deltabell-navn". Tableid now works to transfer to instead of only "hovedtabellnavn"
-- 0.0.2 Starting alpha, fine-tuning release to Pypi on github-release
-- 0.0.1 Client, transfer, description, apidata. Quite a lot of work done already. Pre-alpha.
-
-
 ## License
 
 Distributed under the terms of the [MIT license][license],
 _Dapla Statbank Client_ is free and open source software.
 
 ## Issues
```

### Comparing `dapla_statbank_client-1.2.1/pyproject.toml` & `dapla_statbank_client-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-statbank-client"
-version = "1.2.1"
+version = "1.2.2"
 description = "Handles data transfer Statbank <-> Dapla for Statistics Norway"
 authors = ["Statistics Norway", "Carl F. Corneil <cfc@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-statbank-client"
 repository = "https://github.com/statisticsnorway/dapla-statbank-client"
 documentation = "https://statisticsnorway.github.io/dapla-statbank-client"
```

### Comparing `dapla_statbank_client-1.2.1/src/statbank/__init__.py` & `dapla_statbank_client-1.2.2/src/statbank/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,30 @@
 
 import datetime as dt
 import importlib
 import importlib.metadata  # Needed even with whole import over
 
 import toml
 
+from statbank.apidata import apicodelist
 from statbank.apidata import apidata
 from statbank.apidata import apidata_all
 from statbank.apidata import apidata_rotate
+from statbank.apidata import apimetadata
 from statbank.client import StatbankClient
 from statbank.statbank_logger import logger
 
-__all__ = ["StatbankClient", "apidata", "apidata_all", "apidata_rotate"]
+__all__ = [
+    "StatbankClient",
+    "apidata",
+    "apidata_all",
+    "apidata_rotate",
+    "apimetadata",
+    "apicodelist",
+]
 
 
 # Split into function for testing
 def _try_getting_pyproject_toml(e: Exception | None = None) -> str:
     if e is None:
         passed_excep: Exception = Exception("")
     else:
```

### Comparing `dapla_statbank_client-1.2.1/src/statbank/api_types.py` & `dapla_statbank_client-1.2.2/src/statbank/api_types.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.1/src/statbank/apidata.py` & `dapla_statbank_client-1.2.2/src/statbank/apidata.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import urllib
 from typing import TYPE_CHECKING
+from typing import Any
 
 import requests as r
 from pyjstat import pyjstat
 
 if TYPE_CHECKING:
     import pandas as pd
 
@@ -93,39 +94,84 @@
 
     Returns:
         pd.DataFrame: Table-content
     """
     return apidata(id_or_url, apidata_query_all(id_or_url), include_id=include_id)
 
 
-def apidata_query_all(id_or_url: str = "") -> QueryWholeType:
-    """Builds a query for ALL THE DATA in a table based on a request for metadata on the table.
+def apimetadata(id_or_url: str = "") -> dict[str, Any]:
+    """Get the metadata of a published statbank-table as a dict.
 
     Args:
         id_or_url (str): The id of the STATBANK-table to get the total query for, or supply the total url, if the table is "internal".
 
     Returns:
-        QueryWholeType: The prepared query based on all the codes in the table.
+        dict[str, Any]: The metadata of the table as the json returned from the API-get-request.
 
     Raises:
-        ValueError: If the parameter is not a valid statbank ID or a direct url.
+        ValueError: If the first parameter is not recognized as a statbank ID or a direct url.
     """
     if len(id_or_url) == STATBANK_TABLE_ID_LENGTH and id_or_url.isdigit():
         url = f"https://data.ssb.no/api/v0/no/table/{id_or_url}/"
     else:
         test_url = urllib.parse.urlparse(id_or_url)
         if not all([test_url.scheme, test_url.netloc]):
             error_msg = (
                 "First parameter not recognized as a statbank ID or a direct url"
             )
             raise ValueError(error_msg)
         url = id_or_url
     res = r.get(url, timeout=5)
     res.raise_for_status()
-    meta = res.json()["variables"]
+    meta: dict[str, Any] = res.json()
+    return meta
+
+
+def apicodelist(
+    id_or_url: str = "",
+    codelist_name: str = "",
+) -> dict[str, str] | dict[str, dict[str, str]]:
+    """Get one specific or all the codelists of a published statbank-table as a dict or nested dicts.
+
+    Args:
+        id_or_url (str): The id of the STATBANK-table to get the total query for, or supply the total url, if the table is "internal".
+        codelist_name (str): The name of the specific codelist to get.
+
+    Returns:
+        dict[str, str] | dict[str, dict[str, str]]: The codelist of the table as a dict or a nested dict.
+
+    Raises:
+        ValueError: If the specified codelist_name is not in the returned metadata.
+    """
+    metadata = apimetadata(id_or_url)
+    results = {}
+    for col in metadata["variables"]:
+        results[col["code"]] = dict(zip(col["values"], col["valueTexts"]))
+    if codelist_name == "":
+        return results
+    if codelist_name in results:
+        return results[codelist_name]
+    for col in metadata["variables"]:
+        if codelist_name == col["text"]:
+            return dict(zip(col["values"], col["valueTexts"]))
+    col_names = ", ".join([col["code"] for col in metadata["variables"]])
+    error_msg = f"Cant find {codelist_name} among the available names: {col_names}"
+    raise ValueError(error_msg)
+
+
+def apidata_query_all(id_or_url: str = "") -> QueryWholeType:
+    """Builds a query for ALL THE DATA in a table based on a request for metadata on the table.
+
+    Args:
+        id_or_url (str): The id of the STATBANK-table to get the total query for, or supply the total url, if the table is "internal".
+
+    Returns:
+        QueryWholeType: The prepared query based on all the codes in the table.
+    """
+    meta = apimetadata(id_or_url)["variables"]
     code_list: list[QueryPartType] = []
     for code in meta:
         tmp: QueryPartType = {"code": "", "selection": {"filter": "", "values": []}}
         for k, v in code.items():
             if k == "code":
                 tmp["code"] = v
             if k == "values":
```

### Comparing `dapla_statbank_client-1.2.1/src/statbank/auth.py` & `dapla_statbank_client-1.2.2/src/statbank/auth.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.1/src/statbank/client.py` & `dapla_statbank_client-1.2.2/src/statbank/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
+from typing import Any
 
 if TYPE_CHECKING:
     import pandas as pd
 
 import datetime as dt
 import json
 import os
@@ -12,17 +13,19 @@
 from typing import TYPE_CHECKING
 
 import ipywidgets as widgets
 from IPython.display import display
 
 if TYPE_CHECKING:
     from statbank.api_types import QueryWholeType
+from statbank.apidata import apicodelist
 from statbank.apidata import apidata
 from statbank.apidata import apidata_all
 from statbank.apidata import apidata_rotate
+from statbank.apidata import apimetadata
 from statbank.auth import StatbankAuth
 from statbank.globals import APPROVE_DEFAULT_JIT
 from statbank.globals import OSLO_TIMEZONE
 from statbank.globals import STATBANK_TABLE_ID_LEN
 from statbank.globals import TOMORROW
 from statbank.globals import Approve
 from statbank.globals import _approve_type_check
@@ -130,27 +133,28 @@
             self.log,
         )
 
     def __repr__(self) -> str:
         """Represent the class with the necessary argument to replicate."""
         result = "StatbankClient("
         if self.date != TOMORROW:
-            result += f', date = "{self.date.isoformat("T", "seconds")}")'
+            result += f'date = "{self.date.isoformat("T", "seconds")}", '
         if self.shortuser:
-            result += f', shortuser = "{self.shortuser}")'
+            result += f'shortuser = "{self.shortuser}", '
         if self.cc:
-            result += f', cc = "{self.cc}")'
+            result += f'cc = "{self.cc}", '
         if self.bcc:
-            result += f', bcc = "{self.bcc}")'
+            result += f', bcc = "{self.bcc}", '
         if not self.overwrite:
-            result += f", overwrite = {self.overwrite})"
+            result += f"overwrite = {self.overwrite}), "
         if self.approve != APPROVE_DEFAULT_JIT:
-            result += f", approve = {self.approve})"
+            result += f"approve = {self.approve}, "
         if self.check_username_password:
-            result += f", check_username_password = {self.check_username_password})"
+            result += f"check_username_password = {self.check_username_password}"
+        result = result.strip(" ").strip(",")
         result += ")"
         return result
 
     # Publishing date handeling
     def date_picker(self) -> widgets.DatePicker:
         """Display a datapicker-widget.
 
@@ -389,14 +393,42 @@
 
         Returns:
             pd.DataFrame: A pandas dataframe with the table-content
         """
         return apidata_all(id_or_url=id_or_url, include_id=include_id)
 
     @staticmethod
+    def apimetadata(id_or_url: str = "") -> dict[str, Any]:
+        """Get the metadata of a published statbank-table as a dict.
+
+        Args:
+            id_or_url (str): The id of the STATBANK-table to get the total query for, or supply the total url, if the table is "internal".
+
+        Returns:
+            dict[str, Any]: The metadata of the table as the json returned from the API-get-request.
+        """
+        return apimetadata(id_or_url=id_or_url)
+
+    @staticmethod
+    def apicodelist(
+        id_or_url: str = "",
+        codelist_name: str = "",
+    ) -> dict[str, str] | dict[str, dict[str, str]]:
+        """Get one specific or all the codelists of a published statbank-table as a dict or nested dicts.
+
+        Args:
+            id_or_url (str): The id of the STATBANK-table to get the total query for, or supply the total url, if the table is "internal".
+            codelist_name (str): The name of the specific codelist to get.
+
+        Returns:
+            dict[str, str] | dict[str, dict[str, str]]: The codelist of the table as a dict or a nested dict.
+        """
+        return apicodelist(id_or_url=id_or_url, codelist_name=codelist_name)
+
+    @staticmethod
     def apidata_rotate(
         df: pd.DataFrame,
         ind: str = "year",
         val: str = "value",
     ) -> pd.DataFrame:
         """Rotate the dataframe so that time is used as the index.
```

### Comparing `dapla_statbank_client-1.2.1/src/statbank/globals.py` & `dapla_statbank_client-1.2.2/src/statbank/globals.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.1/src/statbank/statbank_logger.py` & `dapla_statbank_client-1.2.2/src/statbank/statbank_logger.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.1/src/statbank/transfer.py` & `dapla_statbank_client-1.2.2/src/statbank/transfer.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.1/src/statbank/uttrekk.py` & `dapla_statbank_client-1.2.2/src/statbank/uttrekk.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.1/src/statbank/uttrekk_validations.py` & `dapla_statbank_client-1.2.2/src/statbank/uttrekk_validations.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.1/PKG-INFO` & `dapla_statbank_client-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-statbank-client
-Version: 1.2.1
+Version: 1.2.2
 Summary: Handles data transfer Statbank <-> Dapla for Statistics Norway
 Home-page: https://github.com/statisticsnorway/dapla-statbank-client
 License: MIT
 Author: Statistics Norway
 Requires-Python: >=3.10,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -154,14 +154,26 @@
 
 df_folkemengde = apidata("https://i.ssb.no/pxwebi/api/v0/no/prod_24v_intern/START/be/be01/folkemengde/Rd0002Aa",
                                      query,
                                      include_id = True
                                     )
 ```
 
+`apimetadata` gets metadata from the *public* api, like apidata does.
+```python
+meta = apimetadata("05300")
+```
+
+`apicodelist` gets a specific codelist out of the metadata, or all the codelists.
+```python
+all_codelists = apimetadata("05300")
+avstand_codelist = apimetadata("05300", "Avstand1")
+```
+
+
 `apidata_rotate` is a thin wrapper around pivot_table. Stolen from: https://github.com/sehyoun/SSB_API_helper/blob/master/src/ssb_api_helper.py
 ```python
 df_folkemengde_rotert = apidata_rotate(df_folkemengde, 'tidskolonne', "verdikolonne")
 ```
 
 
 ## Using a date-widget for publish day
@@ -201,30 +213,14 @@
 If you *dont* want to see the info-parts of the validate-method, you can change the loggers level before calling validate, like this:
 ```python
 import statbank
 import logging
 statbank.logger.setLevel(logging.WARNING)
 ```
 
-## Version history
-- 1.1.0 Migrating to "new template" for Pypi-packages at SSB, with full typing support, a reference website, logging instead of print etc.
-- 1.0.6 fixing new functionality on "IRkodelister"
-- 1.0.5 Making transferdata_template smarter, were it can take a bunch of dataframes and incorporate them in the returned dict. Trying to support columntype "internasjonal rapportering".
-- 1.0.4 Fixing bug where empty codelists stops description initialization, Updating pyjstat to 2.4.0, changing imports to absolute from package root
-- 1.0.2 Doc-string style cleanup, a check on username and password on client init, changes to time and display of time, demo notebooks cleaned
-- 1.0.0 Finished going through initial issues, less complaining from verify on floats
-- 0.0.11 Statbank people wanted a user-agent-requesst-header to differentiate test from prod
-- 0.0.9 After further user-testing and requests
-- 0.0.5 Still some parameter issues
-- 0.0.4 More test coverage, some bugs fixed in rounding checks and parameter-passing
-- 0.0.3 Removed batches, stripping uttrekk from transfer, rounding function on uttrekk, data required in as a dict of dataframes, with "deltabell-navn". Tableid now works to transfer to instead of only "hovedtabellnavn"
-- 0.0.2 Starting alpha, fine-tuning release to Pypi on github-release
-- 0.0.1 Client, transfer, description, apidata. Quite a lot of work done already. Pre-alpha.
-
-
 ## License
 
 Distributed under the terms of the [MIT license][license],
 _Dapla Statbank Client_ is free and open source software.
 
 ## Issues
```

