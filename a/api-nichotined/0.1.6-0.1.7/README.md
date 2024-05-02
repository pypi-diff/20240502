# Comparing `tmp/api-nichotined-0.1.6.tar.gz` & `tmp/api-nichotined-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api-nichotined-0.1.6.tar", last modified: Wed May  1 15:40:59 2024, max compression
+gzip compressed data, was "api-nichotined-0.1.7.tar", last modified: Thu May  2 18:15:55 2024, max compression
```

## Comparing `api-nichotined-0.1.6.tar` & `api-nichotined-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-01 15:40:59.328382 api-nichotined-0.1.6/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1378 2024-05-01 15:40:59.328137 api-nichotined-0.1.6/PKG-INFO
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      877 2024-05-01 15:39:36.000000 api-nichotined-0.1.6/README.md
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-01 15:40:59.324844 api-nichotined-0.1.6/api_nichotined/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      206 2024-05-01 15:37:42.000000 api-nichotined-0.1.6/api_nichotined/__init__.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-01 15:40:59.326315 api-nichotined-0.1.6/api_nichotined/core/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 04:53:46.000000 api-nichotined-0.1.6/api_nichotined/core/__init__.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     2065 2024-04-26 18:28:12.000000 api-nichotined-0.1.6/api_nichotined/core/core.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       92 2024-04-26 18:28:45.000000 api-nichotined-0.1.6/api_nichotined/core/hook.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-01 15:40:59.327091 api-nichotined-0.1.6/api_nichotined/utillity/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-27 13:10:31.000000 api-nichotined-0.1.6/api_nichotined/utillity/__init__.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1375 2024-05-01 12:24:28.000000 api-nichotined-0.1.6/api_nichotined/utillity/bq.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       53 2024-04-27 13:11:27.000000 api-nichotined-0.1.6/api_nichotined/utillity/pq.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-01 15:40:59.327855 api-nichotined-0.1.6/api_nichotined.egg-info/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1378 2024-05-01 15:40:59.000000 api-nichotined-0.1.6/api_nichotined.egg-info/PKG-INFO
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      448 2024-05-01 15:40:59.000000 api-nichotined-0.1.6/api_nichotined.egg-info/SOURCES.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        1 2024-05-01 15:40:59.000000 api-nichotined-0.1.6/api_nichotined.egg-info/dependency_links.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       39 2024-05-01 15:40:59.000000 api-nichotined-0.1.6/api_nichotined.egg-info/requires.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       20 2024-05-01 15:40:59.000000 api-nichotined-0.1.6/api_nichotined.egg-info/top_level.txt
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       38 2024-05-01 15:40:59.328441 api-nichotined-0.1.6/setup.cfg
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      750 2024-05-01 15:40:31.000000 api-nichotined-0.1.6/setup.py
-drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-01 15:40:59.327511 api-nichotined-0.1.6/test/
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 05:21:55.000000 api-nichotined-0.1.6/test/__init__.py
--rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      685 2024-05-01 15:39:33.000000 api-nichotined-0.1.6/test/main.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-02 18:15:55.432044 api-nichotined-0.1.7/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1378 2024-05-02 18:15:55.431794 api-nichotined-0.1.7/PKG-INFO
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      877 2024-05-01 15:39:36.000000 api-nichotined-0.1.7/README.md
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-02 18:15:55.428541 api-nichotined-0.1.7/api_nichotined/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      130 2024-05-01 16:18:29.000000 api-nichotined-0.1.7/api_nichotined/__init__.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-02 18:15:55.429954 api-nichotined-0.1.7/api_nichotined/core/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 04:53:46.000000 api-nichotined-0.1.7/api_nichotined/core/__init__.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     2198 2024-05-01 16:14:45.000000 api-nichotined-0.1.7/api_nichotined/core/core.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      995 2024-05-01 16:27:20.000000 api-nichotined-0.1.7/api_nichotined/core/response.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-02 18:15:55.430795 api-nichotined-0.1.7/api_nichotined/utillity/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-27 13:10:31.000000 api-nichotined-0.1.7/api_nichotined/utillity/__init__.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1375 2024-05-01 12:24:28.000000 api-nichotined-0.1.7/api_nichotined/utillity/bq.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       53 2024-04-27 13:11:27.000000 api-nichotined-0.1.7/api_nichotined/utillity/pq.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-02 18:15:55.431549 api-nichotined-0.1.7/api_nichotined.egg-info/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)     1378 2024-05-02 18:15:55.000000 api-nichotined-0.1.7/api_nichotined.egg-info/PKG-INFO
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      452 2024-05-02 18:15:55.000000 api-nichotined-0.1.7/api_nichotined.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        1 2024-05-02 18:15:55.000000 api-nichotined-0.1.7/api_nichotined.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       39 2024-05-02 18:15:55.000000 api-nichotined-0.1.7/api_nichotined.egg-info/requires.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       20 2024-05-02 18:15:55.000000 api-nichotined-0.1.7/api_nichotined.egg-info/top_level.txt
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)       38 2024-05-02 18:15:55.432098 api-nichotined-0.1.7/setup.cfg
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      750 2024-05-02 17:28:35.000000 api-nichotined-0.1.7/setup.py
+drwxr-xr-x   0 nicholaslagaunne   (501) staff       (20)        0 2024-05-02 18:15:55.431191 api-nichotined-0.1.7/test/
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)        0 2024-04-19 05:21:55.000000 api-nichotined-0.1.7/test/__init__.py
+-rw-r--r--   0 nicholaslagaunne   (501) staff       (20)      768 2024-05-01 16:31:04.000000 api-nichotined-0.1.7/test/main.py
```

### Comparing `api-nichotined-0.1.6/PKG-INFO` & `api-nichotined-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-nichotined
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simple lib for testing rest API
 Home-page: https://github.com/nichotined/simple-api
 Author: Nicholas Frederich
 Author-email: nicholas.frederich.lagaunne@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `api-nichotined-0.1.6/README.md` & `api-nichotined-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `api-nichotined-0.1.6/api_nichotined/core/core.py` & `api-nichotined-0.1.7/api_nichotined/core/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 import logging
 
 import curlify
 from requests import Response, Session
 
+from api_nichotined.core.response import ResponseWrapper
+
 
 class Api:
     def __init__(self, base_url):
         self.base_url = base_url
         self.session = Session()
         self.logger = logging.getLogger(__name__)
 
     def close_session(self):
         if self.session:
             self.session.close()
 
-    def _make_request(self, method, path, params=None, data=None, json_data=None, headers=None, auth=None) -> Response:
+    def _make_request(self, method, path, params=None, data=None, json_data=None, headers=None,
+                      auth=None) -> ResponseWrapper:
         url = self.base_url + path
         self.logger.info(f"Making {method} request to {url}")
 
         response = self.session.request(method, url, params=params, data=data, json=json_data, headers=headers,
                                         auth=auth)
+
         self.log_response(response)
-        return response
+        return ResponseWrapper(response)
 
     def log_response(self, response: Response):
         curl = curlify.to_curl(response.request)
         self.logger.info(curl)
         self.logger.info(f"Response received with status code {response.status_code}")
         self.logger.info(response.json())
 
-    def get(self, path, params=None, data=None, json_data=None, headers=None, auth=None) -> Response:
+    def get(self, path, params=None, data=None, json_data=None, headers=None, auth=None) -> ResponseWrapper:
         return self._make_request("GET", path, params=params, data=data, headers=headers, json_data=json_data,
                                   auth=auth)
 
-    def post(self, path, params=None, data=None, json_data=None, headers=None, auth=None) -> Response:
+    def post(self, path, params=None, data=None, json_data=None, headers=None, auth=None) -> ResponseWrapper:
         return self._make_request("POST", path, params=params, data=data, headers=headers, json_data=json_data,
                                   auth=auth)
 
-    def put(self, path, params=None, data=None, json_data=None, headers=None, auth=None) -> Response:
+    def put(self, path, params=None, data=None, json_data=None, headers=None, auth=None) -> ResponseWrapper:
         return self._make_request("PUT", path, params=params, data=data, headers=headers, json_data=json_data,
                                   auth=auth)
 
-    def delete(self, path, params=None, data=None, json_data=None, headers=None, auth=None) -> Response:
+    def delete(self, path, params=None, data=None, json_data=None, headers=None, auth=None) -> ResponseWrapper:
         return self._make_request("DELETE", path, params=params, data=data, headers=headers, json_data=json_data,
                                   auth=auth)
```

### Comparing `api-nichotined-0.1.6/api_nichotined/utillity/bq.py` & `api-nichotined-0.1.7/api_nichotined/utillity/bq.py`

 * *Files identical despite different names*

### Comparing `api-nichotined-0.1.6/api_nichotined.egg-info/PKG-INFO` & `api-nichotined-0.1.7/api_nichotined.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-nichotined
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simple lib for testing rest API
 Home-page: https://github.com/nichotined/simple-api
 Author: Nicholas Frederich
 Author-email: nicholas.frederich.lagaunne@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `api-nichotined-0.1.6/setup.py` & `api-nichotined-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="api-nichotined",
-    version="0.1.6",
+    version="0.1.7",
     author="Nicholas Frederich",
     author_email="nicholas.frederich.lagaunne@gmail.com",
     description="Simple lib for testing rest API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nichotined/simple-api",
     packages=setuptools.find_packages(),
```

