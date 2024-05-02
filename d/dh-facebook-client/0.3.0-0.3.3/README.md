# Comparing `tmp/dh-facebook-client-0.3.0.tar.gz` & `tmp/dh-facebook-client-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dh-facebook-client-0.3.0.tar", max compression
+gzip compressed data, was "dh-facebook-client-0.3.3.tar", max compression
```

## Comparing `dh-facebook-client-0.3.0.tar` & `dh-facebook-client-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       21 2024-03-13 19:44:08.967932 dh-facebook-client-0.3.0/PYPI_README.md
--rw-r--r--   0        0        0      801 2024-03-13 19:44:08.967932 dh-facebook-client-0.3.0/dh_facebook_client/__init__.py
--rw-r--r--   0        0        0    11531 2024-03-13 19:44:08.967932 dh-facebook-client-0.3.0/dh_facebook_client/client.py
--rw-r--r--   0        0        0      296 2024-03-13 19:44:08.967932 dh-facebook-client-0.3.0/dh_facebook_client/constants.py
--rw-r--r--   0        0        0     2582 2024-03-13 19:44:08.967932 dh-facebook-client-0.3.0/dh_facebook_client/dataclasses.py
--rw-r--r--   0        0        0      521 2024-03-13 19:44:08.967932 dh-facebook-client-0.3.0/dh_facebook_client/error_code.py
--rw-r--r--   0        0        0     4643 2024-03-13 19:44:08.967932 dh-facebook-client-0.3.0/dh_facebook_client/exceptions.py
--rw-r--r--   0        0        0     2946 2024-03-13 19:44:08.967932 dh-facebook-client-0.3.0/dh_facebook_client/helpers.py
--rw-r--r--   0        0        0      435 2024-03-13 19:44:08.967932 dh-facebook-client-0.3.0/dh_facebook_client/typings.py
--rw-r--r--   0        0        0      731 2024-03-13 19:44:08.967932 dh-facebook-client-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      709 2024-03-13 19:45:12.240558 dh-facebook-client-0.3.0/setup.py
--rw-r--r--   0        0        0      454 2024-03-13 19:45:12.240831 dh-facebook-client-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       21 2024-05-02 20:34:24.962705 dh-facebook-client-0.3.3/PYPI_README.md
+-rw-r--r--   0        0        0      801 2024-05-02 20:34:24.962705 dh-facebook-client-0.3.3/dh_facebook_client/__init__.py
+-rw-r--r--   0        0        0    12270 2024-05-02 20:34:24.962705 dh-facebook-client-0.3.3/dh_facebook_client/client.py
+-rw-r--r--   0        0        0      296 2024-05-02 20:34:24.962705 dh-facebook-client-0.3.3/dh_facebook_client/constants.py
+-rw-r--r--   0        0        0     2707 2024-05-02 20:34:24.962705 dh-facebook-client-0.3.3/dh_facebook_client/dataclasses.py
+-rw-r--r--   0        0        0      521 2024-05-02 20:34:24.962705 dh-facebook-client-0.3.3/dh_facebook_client/error_code.py
+-rw-r--r--   0        0        0     4643 2024-05-02 20:34:24.962705 dh-facebook-client-0.3.3/dh_facebook_client/exceptions.py
+-rw-r--r--   0        0        0     2946 2024-05-02 20:34:24.962705 dh-facebook-client-0.3.3/dh_facebook_client/helpers.py
+-rw-r--r--   0        0        0      435 2024-05-02 20:34:24.966705 dh-facebook-client-0.3.3/dh_facebook_client/typings.py
+-rw-r--r--   0        0        0      731 2024-05-02 20:34:24.966705 dh-facebook-client-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      709 2024-05-02 20:34:57.717665 dh-facebook-client-0.3.3/setup.py
+-rw-r--r--   0        0        0      454 2024-05-02 20:34:57.717890 dh-facebook-client-0.3.3/PKG-INFO
```

### Comparing `dh-facebook-client-0.3.0/dh_facebook_client/__init__.py` & `dh-facebook-client-0.3.3/dh_facebook_client/__init__.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.3.0/dh_facebook_client/client.py` & `dh-facebook-client-0.3.3/dh_facebook_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 from copy import copy
 from types import TracebackType
-from typing import Any, Final, Iterator, Optional, Type
+from typing import Any, Final, Generator, Optional, Type
 
 import backoff
 from requests import Response, Session
 from requests.exceptions import JSONDecodeError
 
 from .constants import GRAPH_API_URL, GRAPH_API_VERSIONS
 from .dataclasses import AppUsageDetails, GraphAPIResponse, MarketingAPIThrottleInsights
@@ -132,15 +132,15 @@
 
     def get_all_pages(
         self,
         path: str,
         params: Optional[dict] = None,
         timeout: Optional[int] = None,
         retry_params: Optional[dict] = None,
-    ) -> Iterator[GraphAPIResponse]:
+    ) -> Generator[GraphAPIResponse, None, None]:
         """
         :param path: A path pointing to an edge or node
             (ex: /<page_id>/conversations)
         Performs a GET request to the Graph API
         :param params: Query parameters to be included with the request
         :param timeout: A custom timeout for the request (seconds)
         :param retry_params: Retry params override
@@ -157,14 +157,30 @@
                 retry_params=retry_params,
             )
             yield res
             if not res.after_cursor:
                 break
             params['after'] = res.after_cursor
 
+    def get_all_pages_from_next_url(
+        self, next_url: str, timeout: Optional[int] = None, retry_params: Optional[dict] = None
+    ) -> Generator[GraphAPIResponse, None, None]:
+        _next_url = next_url
+        while True:
+            res = self._do_request(
+                method='GET',
+                full_url=_next_url,
+                timeout=timeout,
+                retry_params=retry_params,
+            )
+            yield res
+            if not res.next_page_url:
+                break
+            _next_url = res.next_page_url
+
     def post(
         self,
         path: str,
         data: Any,
         params: Optional[Any] = None,
         timeout: Optional[int] = None,
         retry_params: Optional[dict] = None,
@@ -211,15 +227,16 @@
             timeout=timeout,
             retry_params=retry_params,
         )
 
     def _do_request(
         self,
         method: str,
-        path: str,
+        path: str = '',
+        full_url: str = '',
         params: Optional[Any] = None,
         data: Optional[Any] = None,
         timeout: Optional[int] = None,
         retry_params: Optional[dict] = None,
     ) -> GraphAPIResponse:
         """
         Handle Graph API requests. Raise if error body detected and lets ambiguous network
@@ -231,17 +248,20 @@
         :param timeout: A custom timeout for the request (seconds)
         :param retry_params: Retry params override
         :return: An instance of GraphAPIResponse
         """
 
         @backoff.on_exception(backoff.expo, **(retry_params or self.retry_params))
         def _retry_parameterizer() -> GraphAPIResponse:
+            if not path and not full_url:
+                raise ValueError('either path or full_url must be specified')
+
             response = self._session.request(
                 method=method,
-                url=f'{GRAPH_API_URL}/{self.version}/{path}',
+                url=f'{GRAPH_API_URL}/{self.version}/{path}' if path else full_url,
                 params=params,
                 data=data,
                 timeout=timeout or self.global_timeout,
             )
             result, paging = self._parse_response_body_or_raise(response)
 
             return GraphAPIResponse(
```

### Comparing `dh-facebook-client-0.3.0/dh_facebook_client/dataclasses.py` & `dh-facebook-client-0.3.3/dh_facebook_client/dataclasses.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,9 +81,13 @@
         return self.cursors.get('before')
 
     @property
     def after_cursor(self) -> Optional[str]:
         return self.cursors.get('after')
 
     @property
+    def next_page_url(self) -> Optional[str]:
+        return self.paging.get('next') if self.paging else None
+
+    @property
     def cursors(self) -> JSONTypeSimple:
         return self.paging.get('cursors', {}) if self.paging else {}
```

### Comparing `dh-facebook-client-0.3.0/dh_facebook_client/error_code.py` & `dh-facebook-client-0.3.3/dh_facebook_client/error_code.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.3.0/dh_facebook_client/exceptions.py` & `dh-facebook-client-0.3.3/dh_facebook_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.3.0/dh_facebook_client/helpers.py` & `dh-facebook-client-0.3.3/dh_facebook_client/helpers.py`

 * *Files identical despite different names*

### Comparing `dh-facebook-client-0.3.0/pyproject.toml` & `dh-facebook-client-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dh-facebook-client"
-version = "0.3.0"
+version = "0.3.3"
 description = "Simple client for interacting with the Facebook Graph API"
 authors = ["pchisholm <chisholm.p@gmail.com>"]
 readme = "PYPI_README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.26.0"
```

### Comparing `dh-facebook-client-0.3.0/setup.py` & `dh-facebook-client-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['backoff>=1.11.1,<2.0.0', 'requests>=2.26.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'dh-facebook-client',
-    'version': '0.3.0',
+    'version': '0.3.3',
     'description': 'Simple client for interacting with the Facebook Graph API',
     'long_description': '# dh-facebook-client\n',
     'author': 'pchisholm',
     'author_email': 'chisholm.p@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

